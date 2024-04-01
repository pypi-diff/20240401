# Comparing `tmp/pjrmi-1.13.0.tar.gz` & `tmp/pjrmi-1.13.8.tar.gz`

## Comparing `pjrmi-1.13.0.tar` & `pjrmi-1.13.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0   315062 2020-02-02 00:00:00.000000 pjrmi-1.13.0/pjrmi/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pjrmi-1.13.0/pjrmi/_config.py
--rw-r--r--   0        0        0     8098 2020-02-02 00:00:00.000000 pjrmi-1.13.0/pjrmi/_util.py
--rw-r--r--   0        0        0  1159434 2020-02-02 00:00:00.000000 pjrmi-1.13.0/pjrmi/lib/pjrmi.jar
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pjrmi-1.13.0/.gitignore
--rw-r--r--   0        0        0    27528 2020-02-02 00:00:00.000000 pjrmi-1.13.0/README.md
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pjrmi-1.13.0/pyproject.toml
--rw-r--r--   0        0        0    28776 2020-02-02 00:00:00.000000 pjrmi-1.13.0/PKG-INFO
+-rw-r--r--   0        0        0   318187 2020-02-02 00:00:00.000000 pjrmi-1.13.8/pjrmi/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pjrmi-1.13.8/pjrmi/_config.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 pjrmi-1.13.8/pjrmi/_util.py
+-rw-r--r--   0        0        0  1169816 2020-02-02 00:00:00.000000 pjrmi-1.13.8/pjrmi/lib/pjrmi.jar
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pjrmi-1.13.8/.gitignore
+-rw-r--r--   0        0        0    29349 2020-02-02 00:00:00.000000 pjrmi-1.13.8/README.md
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 pjrmi-1.13.8/pyproject.toml
+-rw-r--r--   0        0        0    30604 2020-02-02 00:00:00.000000 pjrmi-1.13.8/PKG-INFO
```

### Comparing `pjrmi-1.13.0/pjrmi/__init__.py` & `pjrmi-1.13.8/pjrmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     _INJECT_CLASS          = b'N' # Client to server
     _GET_VALUE_OF          = b'O' # Client to server
     _GET_CALLBACK_HANDLE   = b'P' # Client to server
     _CALLBACK_RESPONSE     = b'Q' # Client to server
     _GET_PROXY             = b'R' # Client to server
     _INVOKE_AND_GET_OBJECT = b'S' # Client to server
     _INJECT_SOURCE         = b'T' # Client to server
+    _REPLACE_CLASS         = b'U' # Client to server
     _OBJECT_REFERENCE      = b'a' # Server to client
     _TYPE_DESCRIPTION      = b'b' # Server to client
     _ARBITRARY_ITEM        = b'c' # Server to client
     _EXCEPTION             = b'd' # Server to client
     _ASCII_VALUE           = b'e' # Server to client
     _EMPTY_ACK             = b'f' # Server to client
     _ARRAY_LENGTH          = b'g' # Server to client
@@ -840,14 +841,19 @@
 
         This method is a mechanism to do a bulk data transfer from the Java side
         to the Python side, thus making purely pythonic operations to be done
         efficiently. For example, copying a Java ``double[]`` into a Numpy
         ``ndarray`` makes for vastly more efficient array access patterns on the
         Python side.
 
+        If this method is called in a static context, with ``self`` being
+        explicitly passed as ``None``::
+            PJRmi.value_of(None, java_object)
+        then it will infer the `PJRmi` instance to use from the object.
+
         By default the Java object must be wholly converted to its Python
         equivalent, otherwise an ``UnsupportedOperationException`` will be
         thrown. However, setting the ``best_effort`` kwarg to ``True`` will mean
         that unconvertable Java objects will remain untouched. This can be
         useful if, say, one has a ``List<Object>`` on the Java side with
         thousands of elements; iterating over this on the Python side will
         require a callback for each iteration step. Turning it into a Python
@@ -868,18 +874,32 @@
                             fully converted.
         """
 
         # Null breeds null
         if obj is None:
             return None
 
-        # Sanity
+        # Check user inputs
         if not issubclass(obj.__class__, _JavaObject):
             raise TypeError("Given a non-JavaObject %s (%s)" %
                             (str(obj), str(obj.__class__)))
+        if self is not None:
+            if obj._pjrmi_inst is not self:
+                raise KeyError(
+                    "Attempt to use Java object (%s: %s) from connection %s with %s" %
+                    (str(obj.__class__), str(obj),
+                     obj._pjrmi_inst._transport, self._transport)
+                )
+        elif obj._pjrmi_inst is None:
+            raise ValueError("Object has no associated PJRmi instance")
+        else:
+            # We are being called in a static context, as opposed to from the
+            # PJRmi instance. We can use the object's instance as self for the
+            # call.
+            self = obj._pjrmi_inst
 
         if compress:
             if best_effort:
                 value_format = self._VALUE_FORMAT_BESTEFFORT_SNAPPY_PICKLE
             else:
                 value_format = self._VALUE_FORMAT_SNAPPY_PICKLE
         else:
@@ -972,39 +992,46 @@
 
 
     def inject_class(self, filename):
         """
         Read some Java bytecode from a file and inject it into the running Java
         instance as a ``Class``.
 
+        :param filename: The path of the Java class file containing the class
+                         bytecode.
+
         :return: The Python class shim of the injected Java class.
         """
 
         if filename is None:
             return ValueError('Given a null filename')
 
         # Read in and send over the bytecode from the file
-        fh = open(filename, 'rb')
-        req_id = self._send(self._INJECT_CLASS, fh.read())
+        with open(filename, 'rb') as fh:
+            req_id = self._send(self._INJECT_CLASS, fh.read())
 
         # Read the result
         type_dict = self._read_result(req_id)
         if type_dict is None:
             raise TypeError("Could not read type information back from server")
         else:
-            return self._create_class(type_dict)
+            klass = self._create_class(type_dict)
+            self._classes_by_id  [klass._type_id]   = klass
+            self._classes_by_name[klass._classname] = klass
+
+            return klass
 
 
     def inject_source(self, class_name, source):
         """
         Compile the Java class source-code with the given class name.
 
-        :param str class_name: The name of the class in the source given.
+        :param class_name: The name of the class in the source given.
 
-        :param str source: The source code for the class to compile and inject,
+        :param source: The source code for the class to compile and inject,
                            e.g.:
 public class TestInjectSource {
     public static int foo(int i) {
         return i+1;
     }
 }
 
@@ -1030,14 +1057,54 @@
             klass = self._create_class(type_dict)
             self._classes_by_id  [klass._type_id]   = klass
             self._classes_by_name[klass._classname] = klass
 
             return klass
 
 
+    def replace_class(self, klass, filename):
+        """
+        Read some Java bytecode from a file and use it to replace the implementation
+        of an existing class in the JVM.
+
+        For this to function the ``PJRmiAgent`` must be loaded into the JVM.
+
+        :param klass:    The Python shim class of the Java class which we are
+                         replacing.
+        :param filename: The path of the Java class file containing the new
+                         bytecode.
+
+        :return: The Python class shim of the replaced Java class.
+        """
+
+        if filename is None:
+            return ValueError('Given a null filename')
+
+        # Read in and send over the bytecode from the file
+        with open(filename, 'rb') as fh:
+            bytecode = fh.read()
+
+        # And send it off
+        payload  = self._format_int32(klass._type_id)
+        payload += self._format_int32(len(bytecode))
+        payload += bytecode
+        req_id   = self._send(self._REPLACE_CLASS, payload)
+
+        # Read the result
+        type_dict = self._read_result(req_id)
+        if type_dict is None:
+            raise TypeError("Could not read type information back from server")
+        else:
+            new_klass = self._create_class(type_dict)
+            self._classes_by_id  [new_klass._type_id]   = new_klass
+            self._classes_by_name[new_klass._classname] = new_klass
+
+            return new_klass
+
+
     def get_constructor(self, klass, arg_types=None):
         """
         Get a handle on the Java version of the constructor for the given class,
         potentially using any given argument types to disambiguate overloaded
         instances.
 
         Once obtained this can be used as an argument to Java methods which use
@@ -2969,25 +3036,25 @@
                             self._format_int32(len(value)) +
                             b''.join(self._format_by_class(self._java_lang_String,
                                                            el,
                                                            strict_types=strict_types)
                                           for el in value))
 
                 elif isinstance(value, int):
-                    if numpy.int8(value) == value:
+                    if numpy.can_cast(value, numpy.int8):
                         return (self._ARGUMENT_VALUE +
                                 self._format_int32(self._java_lang_Byte._type_id) +
                                 self._format_int8(strict_number(numpy.int8, value)))
 
-                    elif numpy.int16(value) == value:
+                    elif numpy.can_cast(value, numpy.int16):
                         return (self._ARGUMENT_VALUE +
                                 self._format_int32(self._java_lang_Short._type_id) +
                                 self._format_int16(strict_number(numpy.int16, value)))
 
-                    elif numpy.int32(value) == value:
+                    elif numpy.can_cast(value, numpy.int32):
                         return (self._ARGUMENT_VALUE +
                                 self._format_int32(self._java_lang_Integer._type_id) +
                                 self._format_int32(strict_number(numpy.int32, value)))
 
                     else:
                         return (self._ARGUMENT_VALUE +
                                 self._format_int32(self._java_lang_Long._type_id) +
@@ -3391,15 +3458,16 @@
                         b''.join(self._format_by_class(ok,
                                                        el,
                                                        strict_types=strict_types)
                                      for el in value))
 
             elif (hasattr(value, '__iter__') and
                   not isinstance(value, str) and
-                  klass._type_id in (self._java_util_Collection._type_id,
+                  klass._type_id in (self._java_lang_Iterable.  _type_id,
+                                     self._java_util_Collection._type_id,
                                      self._java_util_List.      _type_id)):
                 ok = self._java_lang_Object
                 return (self._ARGUMENT_VALUE +
                         self._format_int32(klass._type_id) +
                         self._format_int32(len(value)) +
                         b''.join(self._format_by_class(ok,
                                                        el,
@@ -3627,22 +3695,22 @@
 
 
     def _read_int8_array(self, bytes, index):
         """
         Reads an array of 8 bit integers array from some data looking like
         [int32:size][byte[]:data] from a byte buffer.
 
-        :return: An array of int8s, the new offset into the byte buffer.
+        :return: An array-like of int8s, the new offset into the byte buffer.
         """
 
         # Hand off to the version which reads the values as a string
         (byte_array, index) = self._read_byte_array(bytes, index)
 
         # Convert to an array of int8s
-        int8_array = [numpy.int8(b) for b in bytearray(byte_array)]
+        int8_array = numpy.array(bytearray(byte_array)).astype(numpy.int8)
 
         return (int8_array, index)
 
 
     def _read_argument(self, bytes, idx):
         """
         Reads a function call argument from the stream. This might be by reference
@@ -5669,14 +5737,15 @@
 
 
 def connect_to_child_jvm(main_class='com.deshaw.pjrmi.UnixFifoProvider',
                          environment=None, java_executable=None,
                          classpath=(), java_args=(), application_args=(), timeout=60,
                          stdin='/dev/stdin', stdout='/dev/stdout', stderr='/dev/stderr',
                          interactive_mode=True, use_shm_arg_passing=False,
+                         use_pjrmi_agent=False,
                          impl=PJRmi):
     """
     Create a child JVM instance and connect to it.
 
     The stdin, stdout and stderr arguments below may be file handles, file
     numbers or strings that will act as the standard input, standard output, and
     standard error for the child JVM process, respectively. If None is passed
@@ -5705,17 +5774,28 @@
     :param stdin:               the stdin file, or None to delete the handle.
     :param stdout:              The stdout file, or None to delete the handle.
     :param stderr:              The stderr file, or None to delete the handle.
     :param interactive_mode:    Whether the session is interactive, if so then we try to
                                 make it more friendly to that.
     :param use_shm_arg_passing: Whether to enable passing of some values by SHM
                                 copying. This requires the C extension to function.
+    :param use_pjrmi_agent:     Whether to include the directive to load the
+                                ``PJRmiAgent`` class on the command line.
     :param impl:                The `PJRmi` implementation to use.
     """
 
+    # If we have been told to load the agent then we should include that as part
+    # of the command line arguments
+    if use_pjrmi_agent:
+        if java_args is None:
+            java_args = []
+        else:
+            java_args = list(java_args)
+        java_args.append(f'-javaagent:{_PJRMI_FATJAR}')
+
     # Create and connect
     c = impl(UnixFifoTransport(main_class,
                                environment=environment,
                                java_executable=java_executable,
                                classpath=classpath,
                                java_args=java_args,
                                application_args=application_args,
@@ -6042,28 +6122,24 @@
         :param host:
             The host to connect to.
         :param port:
             The port to connect to.
         """
 
         self._host   = host
-        self._port   = port
+        self._port   = int(port)
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
 
     def __str__(self):
         """
         A brief description of the transport.
         """
 
-        if self._server_name is None:
-            details = "%s:%d" % (self._host, self._port)
-        else:
-            details = "%s@%s:%d" % (self._server_name, self._host, self._port)
-        return "Socket[%s]" % details
+        return "%s[%s:%d]" % (self.__class__.__name__, self._host, self._port)
 
 
     def connect(self):
         """
         Connect to the server.
         """
```

### Comparing `pjrmi-1.13.0/pjrmi/_util.py` & `pjrmi-1.13.8/pjrmi/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     :raise ValueError:
       Got an integer value other than 0 or 1.
     :rtype:
       ``bool``
     """
     if isinstance(arg, bool):
         return arg
-    if not isinstance(arg, (int, numpy.integer, numpy.bool8)):
+    if not isinstance(arg, (int, numpy.integer, numpy.bool_)):
         raise TypeError(
             "Expected a bool, but got a %s with value %r" %
                 (type(arg).__name__, arg))
     b = bool(arg)
     if b != arg:
         raise ValueError(
             "Expected False or True, but got %r" % (arg,))
@@ -122,19 +122,19 @@
     # Strings can be "cast" to numbers so explicitly handle them. We have to
     # do this since the value constructors will take strings and turn them
     # into numbers.
     if isinstance(value, str):
         raise TypeError("String may not be cast to %s" % typ)
 
     # Do the cast, this may throw
-    casted = typ(value)
+    casted = numpy.array(value).astype(typ)
 
     # NaNs are easy to check
     if numpy.isnan(casted) and numpy.isnan(value):
-        return casted
+        return value
 
     # Make sure they look the same, in a somewhat simplistic way
     if casted == value:
         # Handle the corner-case in float casting, since you have things
         # like:
         #   >>> np.float64(9007199254740993)
         #   9007199254740992.0
@@ -142,15 +142,15 @@
         #   True
         # To catch this we cast the result back to the original type and
         # check that it still matches.
         if (typ not in (numpy.float32, numpy.float64) or
             type(value)(casted) == value):
             # Either it wasn't being cast to a float, or it matched when we
             # cast it back. Either way, it's safe to hand back.
-            return casted
+            return value
 
     # If we got here then we failed
     raise ImpreciseRepresentationError(
         "Value %s could not be represented as a %s" % (value, typ)
     )
```

### Comparing `pjrmi-1.13.0/pjrmi/lib/pjrmi.jar` & `pjrmi-1.13.8/pjrmi/lib/pjrmi.jar`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,323 +1,325 @@
-Zip file size: 1159434 bytes, number of entries: 374
-drwxr-xr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Nov-03 18:59 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/
--rw-rw-r--  2.0 unx     3922 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Boolean1dWrappingHypercube.class
--rw-rw-r--  2.0 unx     4464 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Boolean2dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5022 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Boolean3dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5614 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Boolean4dWrappingHypercube.class
--rw-rw-r--  2.0 unx     6206 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Boolean5dWrappingHypercube.class
--rw-rw-r--  2.0 unx     9498 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanAxisRolledHypercube.class
--rw-rw-r--  2.0 unx     9077 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanBitSetHypercube.class
--rw-rw-r--  2.0 unx     7636 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanFlatRolledHypercube.class
--rw-rw-r--  2.0 unx     3187 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanFromDoubleHypercube.class
--rw-rw-r--  2.0 unx     3177 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanFromFloatHypercube.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanFromIntegerHypercube.class
--rw-rw-r--  2.0 unx     3167 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanFromLongHypercube.class
--rw-rw-r--  2.0 unx     9089 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanSlicedHypercube.class
--rw-rw-r--  2.0 unx     8421 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanTransposedHypercube.class
--rw-rw-r--  2.0 unx     5411 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanWrappingHypercube.class
--rw-rw-r--  2.0 unx     8298 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractBooleanHypercube.class
--rw-rw-r--  2.0 unx    24977 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/BooleanHypercube.class
--rw-rw-r--  2.0 unx   236862 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath.class
--rw-rw-r--  2.0 unx     3437 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$1.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$ReductiveLogicOp.class
--rw-rw-r--  2.0 unx     1413 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$ComparisonOp.class
--rw-rw-r--  2.0 unx     1336 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$AssociativeOp.class
--rw-rw-r--  2.0 unx     1842 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$UnaryOp.class
--rw-rw-r--  2.0 unx     1638 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$BinaryOp.class
--rw-rw-r--  2.0 unx     2369 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube.class
--rw-rw-r--  2.0 unx     2360 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$FloatSingleValueHypercube.class
--rw-rw-r--  2.0 unx     2320 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$LongSingleValueHypercube.class
--rw-rw-r--  2.0 unx     2374 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube.class
--rw-rw-r--  2.0 unx     2378 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube.class
--rw-rw-r--  2.0 unx     3991 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Double1dWrappingHypercube.class
--rw-rw-r--  2.0 unx     4537 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Double2dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5099 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Double3dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5695 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Double4dWrappingHypercube.class
--rw-rw-r--  2.0 unx     6291 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Double5dWrappingHypercube.class
--rw-rw-r--  2.0 unx     9375 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleArrayHypercube.class
--rw-rw-r--  2.0 unx     9504 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleAxisRolledHypercube.class
--rw-rw-r--  2.0 unx     7636 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleFlatRolledHypercube.class
--rw-rw-r--  2.0 unx     3037 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleFromFloatHypercube.class
--rw-rw-r--  2.0 unx     3053 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleFromIntegerHypercube.class
--rw-rw-r--  2.0 unx     3027 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleFromLongHypercube.class
--rw-rw-r--  2.0 unx     8302 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractDoubleHypercube.class
--rw-rw-r--  2.0 unx     9958 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleMappedHypercube.class
--rw-rw-r--  2.0 unx     9095 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleSlicedHypercube.class
--rw-rw-r--  2.0 unx     8440 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleTransposedHypercube.class
--rw-rw-r--  2.0 unx     5397 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleWrappingHypercube.class
--rw-rw-r--  2.0 unx     3968 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Float1dWrappingHypercube.class
--rw-rw-r--  2.0 unx     4512 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Float2dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5072 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Float3dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5666 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Float4dWrappingHypercube.class
--rw-rw-r--  2.0 unx     6260 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Float5dWrappingHypercube.class
--rw-rw-r--  2.0 unx     9345 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatArrayHypercube.class
--rw-rw-r--  2.0 unx     9483 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatAxisRolledHypercube.class
--rw-rw-r--  2.0 unx     7613 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatFlatRolledHypercube.class
--rw-rw-r--  2.0 unx     3036 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatFromDoubleHypercube.class
--rw-rw-r--  2.0 unx     3042 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatFromIntegerHypercube.class
--rw-rw-r--  2.0 unx     3016 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatFromLongHypercube.class
--rw-rw-r--  2.0 unx     8277 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractFloatHypercube.class
--rw-rw-r--  2.0 unx     9927 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatMappedHypercube.class
--rw-rw-r--  2.0 unx     9074 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatSlicedHypercube.class
--rw-rw-r--  2.0 unx     8408 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatTransposedHypercube.class
--rw-rw-r--  2.0 unx     5370 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatWrappingHypercube.class
--rw-rw-r--  2.0 unx     6972 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/GenericArrayHypercube.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/GenericHypercube.class
--rw-rw-r--  2.0 unx     6656 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/GenericWrappingHypercube.class
--rw-rw-r--  2.0 unx     2431 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/GenericWrappingHypercube$FlattenedList.class
--rw-rw-r--  2.0 unx     3976 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Integer1dWrappingHypercube.class
--rw-rw-r--  2.0 unx     4518 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Integer2dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5076 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Integer3dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5668 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Integer4dWrappingHypercube.class
--rw-rw-r--  2.0 unx     6260 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Integer5dWrappingHypercube.class
--rw-rw-r--  2.0 unx     9351 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerArrayHypercube.class
--rw-rw-r--  2.0 unx     9498 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerAxisRolledHypercube.class
--rw-rw-r--  2.0 unx     7655 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerFlatRolledHypercube.class
--rw-rw-r--  2.0 unx     3054 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerFromDoubleHypercube.class
--rw-rw-r--  2.0 unx     3044 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerFromFloatHypercube.class
--rw-rw-r--  2.0 unx     3034 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerFromLongHypercube.class
--rw-rw-r--  2.0 unx     8317 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractIntegerHypercube.class
--rw-rw-r--  2.0 unx     9918 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerMappedHypercube.class
--rw-rw-r--  2.0 unx     9089 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerSlicedHypercube.class
--rw-rw-r--  2.0 unx     8444 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerTransposedHypercube.class
--rw-rw-r--  2.0 unx     5424 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerWrappingHypercube.class
--rw-rw-r--  2.0 unx     3885 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Long1dWrappingHypercube.class
--rw-rw-r--  2.0 unx     4464 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Long2dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5022 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Long3dWrappingHypercube.class
--rw-rw-r--  2.0 unx     5614 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Long4dWrappingHypercube.class
--rw-rw-r--  2.0 unx     6206 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Long5dWrappingHypercube.class
--rw-rw-r--  2.0 unx     9275 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongArrayHypercube.class
--rw-rw-r--  2.0 unx     8480 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AxisRolledHypercube.class
--rw-rw-r--  2.0 unx     1132 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AxisRolledHypercube$2.class
--rw-rw-r--  2.0 unx     1132 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AxisRolledHypercube$1.class
--rw-rw-r--  2.0 unx     9442 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongAxisRolledHypercube.class
--rw-rw-r--  2.0 unx     5786 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FlatRolledHypercube.class
--rw-rw-r--  2.0 unx     1003 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FlatRolledHypercube$1.class
--rw-rw-r--  2.0 unx     7566 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongFlatRolledHypercube.class
--rw-rw-r--  2.0 unx    29448 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DoubleHypercube.class
--rw-rw-r--  2.0 unx     2999 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongFromDoubleHypercube.class
--rw-rw-r--  2.0 unx    29386 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/FloatHypercube.class
--rw-rw-r--  2.0 unx     2989 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongFromFloatHypercube.class
--rw-rw-r--  2.0 unx    30665 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/IntegerHypercube.class
--rw-rw-r--  2.0 unx     3005 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongFromIntegerHypercube.class
--rw-rw-r--  2.0 unx     8254 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractLongHypercube.class
--rw-rw-r--  2.0 unx     9856 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongMappedHypercube.class
--rw-rw-r--  2.0 unx     9033 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongSlicedHypercube.class
--rw-rw-r--  2.0 unx     8391 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongTransposedHypercube.class
--rw-rw-r--  2.0 unx    30470 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongHypercube.class
--rw-rw-r--  2.0 unx     5331 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/LongWrappingHypercube.class
--rw-rw-r--  2.0 unx     3311 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/MappedIndex.class
--rw-rw-r--  2.0 unx     2186 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/NaturalIndex.class
--rw-rw-r--  2.0 unx     9365 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/SlicedHypercube.class
--rw-rw-r--  2.0 unx     2292 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractIndex.class
--rw-rw-r--  2.0 unx     3558 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/SubIndex.class
--rw-rw-r--  2.0 unx     5028 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/TransposedHypercube.class
--rw-rw-r--  2.0 unx     1002 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/TransposedHypercube$1.class
--rw-rw-r--  2.0 unx     1066 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Index.class
--rw-rw-r--  2.0 unx      629 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/DimensionalityException.class
--rw-rw-r--  2.0 unx    37504 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Hypercube.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Hypercube$2.class
--rw-rw-r--  2.0 unx     1712 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Hypercube$1.class
--rw-rw-r--  2.0 unx     3781 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Hypercube$Flags.class
--rw-rw-r--  2.0 unx    17854 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/AbstractHypercube.class
--rw-rw-r--  2.0 unx     4906 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Dimension.class
--rw-rw-r--  2.0 unx     1951 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Dimension$Roll.class
--rw-rw-r--  2.0 unx     2192 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Dimension$Slice.class
--rw-rw-r--  2.0 unx     1625 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Dimension$Coordinate.class
--rw-rw-r--  2.0 unx     1024 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/Dimension$Accessor.class
--rw-rw-r--  2.0 unx     3497 b- defN 23-Nov-03 18:59 com/deshaw/hypercube/WrappingHypercube.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/io/
--rw-rw-r--  2.0 unx     2524 b- defN 23-Nov-03 18:59 com/deshaw/io/BlockingPipe.class
--rw-rw-r--  2.0 unx      792 b- defN 23-Nov-03 18:59 com/deshaw/io/BlockingPipe$Output.class
--rw-rw-r--  2.0 unx      752 b- defN 23-Nov-03 18:59 com/deshaw/io/BlockingPipe$Input.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/
--rw-rw-r--  2.0 unx     5916 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/AsType.class
--rw-rw-r--  2.0 unx      124 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/JavaProxyBase.class
--rw-rw-r--  2.0 unx    11968 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/JniPJRmi.class
--rw-rw-r--  2.0 unx      757 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/JniPJRmi$ArrayHandle.class
--rw-rw-r--  2.0 unx     4108 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/KwargUtil.class
--rw-rw-r--  2.0 unx     2344 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PipedProvider.class
--rw-rw-r--  2.0 unx     1794 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PipedProvider$BidirectionalPipe.class
--rw-rw-r--  2.0 unx     3095 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PipedProvider$PipedPJRmi.class
--rw-rw-r--  2.0 unx     1922 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PipedTransport.class
--rw-rw-r--  2.0 unx     6019 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonMinionProvider.class
--rw-rw-r--  2.0 unx     1499 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonMinionProvider$1.class
--rw-rw-r--  2.0 unx     5605 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonMinionTransport.class
--rw-rw-r--  2.0 unx     1498 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonSlice.class
--rw-rw-r--  2.0 unx     5353 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SSLSocketProvider.class
--rw-rw-r--  2.0 unx     1002 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonKwargsFunction.class
--rw-rw-r--  2.0 unx      442 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonFunction.class
--rw-rw-r--  2.0 unx     5307 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject.class
--rw-rw-r--  2.0 unx     2036 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$8.class
--rw-rw-r--  2.0 unx     1959 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$7.class
--rw-rw-r--  2.0 unx     1984 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$6.class
--rw-rw-r--  2.0 unx     1907 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$5.class
--rw-rw-r--  2.0 unx     2161 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$4.class
--rw-rw-r--  2.0 unx     2084 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$3.class
--rw-rw-r--  2.0 unx     2134 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$2.class
--rw-rw-r--  2.0 unx     1876 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonObject$1.class
--rw-rw-r--  2.0 unx      493 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonCallbackException.class
--rw-rw-r--  2.0 unx     2144 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonMinion.class
--rw-rw-r--  2.0 unx     1171 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PythonMinion$ByValue.class
--rw-rw-r--  2.0 unx     3228 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SSLSocketTransport.class
--rw-rw-r--  2.0 unx    30872 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi.class
--rw-rw-r--  2.0 unx     2986 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$3.class
--rw-rw-r--  2.0 unx     1274 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$2.class
--rw-rw-r--  2.0 unx      621 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$1.class
--rw-rw-r--  2.0 unx    69158 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection.class
--rw-rw-r--  2.0 unx     5116 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$3.class
--rw-rw-r--  2.0 unx     1730 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$2.class
--rw-rw-r--  2.0 unx     1626 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$1.class
--rw-rw-r--  2.0 unx     8176 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl.class
--rw-rw-r--  2.0 unx     7829 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler.class
--rw-rw-r--  2.0 unx     6602 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler.class
--rw-rw-r--  2.0 unx     2750 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate.class
--rw-rw-r--  2.0 unx     2646 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate.class
--rw-rw-r--  2.0 unx     2411 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer.class
--rw-rw-r--  2.0 unx     2310 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer.class
--rw-rw-r--  2.0 unx     2427 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction.class
--rw-rw-r--  2.0 unx     2326 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction.class
--rw-rw-r--  2.0 unx     2330 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator.class
--rw-rw-r--  2.0 unx     2014 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable.class
--rw-rw-r--  2.0 unx     5853 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallback.class
--rw-rw-r--  2.0 unx     1393 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult.class
--rw-rw-r--  2.0 unx     2163 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle.class
--rw-rw-r--  2.0 unx     3730 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$MethodCaller.class
--rw-rw-r--  2.0 unx     8409 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Connection$Worker.class
--rw-rw-r--  2.0 unx      234 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ThreadId.class
--rw-rw-r--  2.0 unx     1146 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream.class
--rw-rw-r--  2.0 unx      788 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.class
--rw-rw-r--  2.0 unx      995 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ClassInjector.class
--rw-rw-r--  2.0 unx     3608 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$HandleMapping.class
--rw-rw-r--  2.0 unx      697 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.class
--rw-rw-r--  2.0 unx     3891 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$TypeMapping.class
--rw-rw-r--  2.0 unx     5556 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodDescription.class
--rw-rw-r--  2.0 unx     2572 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.class
--rw-rw-r--  2.0 unx     3177 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodCallFuture.class
--rw-rw-r--  2.0 unx     2178 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$SyncMode.class
--rw-rw-r--  2.0 unx     1710 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodFlags.class
--rw-rw-r--  2.0 unx     1964 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$FieldDescription.class
--rw-rw-r--  2.0 unx      585 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ReadObjectResult.class
--rw-rw-r--  2.0 unx     1242 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodSignature.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MethodComparator.class
--rw-rw-r--  2.0 unx     5937 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class
--rw-rw-r--  2.0 unx     1484 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class
--rw-rw-r--  2.0 unx      420 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ArrayLike.class
--rw-rw-r--  2.0 unx      343 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PythonItemAssignable.class
--rw-rw-r--  2.0 unx      487 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PythonSubscriptable.class
--rw-rw-r--  2.0 unx    17971 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$TypeDescription.class
--rw-rw-r--  2.0 unx     1526 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$TypeFlags.class
--rw-rw-r--  2.0 unx     2581 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PythonValueFormat.class
--rw-rw-r--  2.0 unx     2603 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle.class
--rw-rw-r--  2.0 unx     4651 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$MessageType.class
--rw-rw-r--  2.0 unx     1191 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Flags.class
--rw-rw-r--  2.0 unx      556 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$Kwargs.class
--rw-rw-r--  2.0 unx      511 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$ExplicitBinding.class
--rw-rw-r--  2.0 unx      496 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$GenericReturnType.class
--rw-rw-r--  2.0 unx     7296 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PJRmiLockManager.class
--rw-rw-r--  2.0 unx     1240 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2.class
--rw-rw-r--  2.0 unx     1150 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class
--rw-rw-r--  2.0 unx     3589 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class
--rw-rw-r--  2.0 unx     6124 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/MethodUtil.class
--rw-rw-r--  2.0 unx     1521 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
--rw-rw-r--  2.0 unx     1273 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
--rw-rw-r--  2.0 unx     1629 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SocketProvider.class
--rw-rw-r--  2.0 unx     1626 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SocketTransport.class
--rw-rw-r--  2.0 unx     5792 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SourceInjector.class
--rw-rw-r--  2.0 unx     1144 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SourceInjector$2.class
--rw-rw-r--  2.0 unx     1709 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SourceInjector$1.class
--rw-rw-r--  2.0 unx     1781 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SourceInjector$JavaByteObject.class
--rw-rw-r--  2.0 unx     1616 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/SourceInjector$JavaStringObject.class
--rw-rw-r--  2.0 unx     3965 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/UnixFifoProvider.class
--rw-rw-r--  2.0 unx     2802 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/UnixFifoProvider$1.class
--rw-rw-r--  2.0 unx     1817 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/UnixFifoProvider$Fifo.class
--rw-rw-r--  2.0 unx      645 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/Transport.class
--rw-rw-r--  2.0 unx      486 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/Transport$Provider.class
--rw-rw-r--  2.0 unx     2873 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/Transport$Provider$Arguments.class
--rw-rw-r--  2.0 unx     1848 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/UnixFifoTransport.class
--rw-rw-r--  2.0 unx     1213 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/UnixSignals.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/
--rw-rw-r--  2.0 unx     3947 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers.class
--rw-rw-r--  2.0 unx     1068 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThrowIterator.class
--rw-rw-r--  2.0 unx     1187 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator.class
--rw-rw-r--  2.0 unx      650 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator$CustomNoSuchElementException.class
--rw-rw-r--  2.0 unx     1653 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$MorePrecedenceMethods.class
--rw-rw-r--  2.0 unx     6513 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$PrecedenceMethods.class
--rw-rw-r--  2.0 unx      455 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$C.class
--rw-rw-r--  2.0 unx      455 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$B.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$A.class
--rw-rw-r--  2.0 unx      639 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$1Result.class
--rw-rw-r--  2.0 unx      288 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$ObjectInterface.class
--rw-rw-r--  2.0 unx      770 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsDerived.class
--rw-rw-r--  2.0 unx      588 b- defN 23-Nov-03 18:59 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsBase.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/python/
--rw-rw-r--  2.0 unx     2696 b- defN 23-Nov-03 18:59 com/deshaw/python/BinString.class
--rw-rw-r--  2.0 unx     5140 b- defN 23-Nov-03 18:59 com/deshaw/python/Dict.class
--rw-rw-r--  2.0 unx      581 b- defN 23-Nov-03 18:59 com/deshaw/python/Dict$MissingKeyException.class
--rw-rw-r--  2.0 unx     4351 b- defN 23-Nov-03 18:59 com/deshaw/python/Operations.class
--rw-rw-r--  2.0 unx    15924 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonPickle.class
--rw-rw-r--  2.0 unx     1046 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonPickle$1.class
--rw-rw-r--  2.0 unx    18309 b- defN 23-Nov-03 18:59 com/deshaw/python/NumpyArray.class
--rw-rw-r--  2.0 unx      994 b- defN 23-Nov-03 18:59 com/deshaw/python/NumpyArray$1.class
--rw-rw-r--  2.0 unx      337 b- defN 23-Nov-03 18:59 com/deshaw/python/NumpyArray$ElementVisitor.class
--rw-rw-r--  2.0 unx     5048 b- defN 23-Nov-03 18:59 com/deshaw/python/DType.class
--rw-rw-r--  2.0 unx     2679 b- defN 23-Nov-03 18:59 com/deshaw/python/DType$Type.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Nov-03 18:59 com/deshaw/python/MalformedPickleException.class
--rw-rw-r--  2.0 unx    15621 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle.class
--rw-rw-r--  2.0 unx     3276 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$2.class
--rw-rw-r--  2.0 unx      528 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$1.class
--rw-rw-r--  2.0 unx     1130 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$UnpickleableDType.class
--rw-rw-r--  2.0 unx     2260 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$NumpyFrombufferArray.class
--rw-rw-r--  2.0 unx     3503 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$UnpickleableNumpyArray.class
--rw-rw-r--  2.0 unx     2079 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$BytesPlaceholder.class
--rw-rw-r--  2.0 unx     2755 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$Encoder.class
--rw-rw-r--  2.0 unx     1679 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$DTypeFactory.class
--rw-rw-r--  2.0 unx      983 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$NDArrayType.class
--rw-rw-r--  2.0 unx     2760 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayScalar.class
--rw-rw-r--  2.0 unx     1709 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$NumpyFrombuffer.class
--rw-rw-r--  2.0 unx     1032 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayReconstruct.class
--rw-rw-r--  2.0 unx      392 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$Global.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$Instance.class
--rw-rw-r--  2.0 unx     1208 b- defN 23-Nov-03 18:59 com/deshaw/python/PythonUnpickle$ShrinkableList.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/util/
--rw-rw-r--  2.0 unx     4673 b- defN 23-Nov-03 18:59 com/deshaw/util/ByteList.class
--rw-rw-r--  2.0 unx     3081 b- defN 23-Nov-03 18:59 com/deshaw/util/StringUtil.class
--rw-rw-r--  2.0 unx     3465 b- defN 23-Nov-03 18:59 com/deshaw/util/StringUtil$HashableSubSequence.class
--rw-rw-r--  2.0 unx     3312 b- defN 23-Nov-03 18:59 com/deshaw/util/SwappingPool.class
--rw-rw-r--  2.0 unx     1443 b- defN 23-Nov-03 18:59 com/deshaw/util/SwappingPool$1.class
--rw-rw-r--  2.0 unx     1591 b- defN 23-Nov-03 18:59 com/deshaw/util/SwappingPool$Stack.class
--rw-rw-r--  2.0 unx      982 b- defN 23-Nov-03 18:59 com/deshaw/util/ThreadLocalStringBuilder.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Nov-03 18:59 com/deshaw/util/Pool.class
--rw-rw-r--  2.0 unx      790 b- defN 23-Nov-03 18:59 com/deshaw/util/Instrumentor.class
--rw-rw-r--  2.0 unx      728 b- defN 23-Nov-03 18:59 com/deshaw/util/Instrumentor$2.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Nov-03 18:59 com/deshaw/util/Instrumentor$1.class
--rw-rw-r--  2.0 unx      335 b- defN 23-Nov-03 18:59 com/deshaw/util/Instrumentor$Factory.class
-drwxrwxr-x  2.0 unx        0 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/
--rw-rw-r--  2.0 unx    22212 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager.class
--rw-rw-r--  2.0 unx     1110 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$2.class
--rw-rw-r--  2.0 unx     5322 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$NamedReentrantLock.class
--rw-rw-r--  2.0 unx     1456 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$1.class
--rw-rw-r--  2.0 unx     3244 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$LockManagerLock.class
--rw-rw-r--  2.0 unx     4194 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$LockManagerLock$Locker.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$ColouredList.class
--rw-rw-r--  2.0 unx     4778 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$ThreadLockState.class
--rw-rw-r--  2.0 unx     2039 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$ThreadLockState$Details.class
--rw-rw-r--  2.0 unx     1407 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$SafeReadWriteLock.class
--rw-rw-r--  2.0 unx     3227 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$SafeLock.class
--rw-rw-r--  2.0 unx     1443 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$SafeLock$AcquireFailedException.class
--rw-rw-r--  2.0 unx      566 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/LockManager$DeadlockException.class
--rw-rw-r--  2.0 unx     6390 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/VirtualThreadLock.class
--rw-rw-r--  2.0 unx      895 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/VirtualThreadLock$1.class
--rw-rw-r--  2.0 unx     1273 b- defN 23-Nov-03 18:59 com/deshaw/util/concurrent/VirtualThreadLock$VirtualThread.class
+Zip file size: 1169816 bytes, number of entries: 376
+drwxr-xr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 META-INF/
+-rw-r--r--  2.0 unx      170 b- defN 24-Apr-01 11:53 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/io/
+-rw-rw-r--  2.0 unx     2524 b- defN 24-Apr-01 11:53 com/deshaw/io/BlockingPipe.class
+-rw-rw-r--  2.0 unx      792 b- defN 24-Apr-01 11:53 com/deshaw/io/BlockingPipe$Output.class
+-rw-rw-r--  2.0 unx      752 b- defN 24-Apr-01 11:53 com/deshaw/io/BlockingPipe$Input.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/
+-rw-rw-r--  2.0 unx     3922 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Boolean1dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     4464 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Boolean2dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5022 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Boolean3dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5614 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Boolean4dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6206 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Boolean5dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     9498 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanAxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     9077 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanBitSetHypercube.class
+-rw-rw-r--  2.0 unx     7636 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanFlatRolledHypercube.class
+-rw-rw-r--  2.0 unx     3187 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanFromDoubleHypercube.class
+-rw-rw-r--  2.0 unx     3177 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanFromFloatHypercube.class
+-rw-rw-r--  2.0 unx     3184 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanFromIntegerHypercube.class
+-rw-rw-r--  2.0 unx     3167 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanFromLongHypercube.class
+-rw-rw-r--  2.0 unx     9089 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanSlicedHypercube.class
+-rw-rw-r--  2.0 unx     8421 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanTransposedHypercube.class
+-rw-rw-r--  2.0 unx     5411 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanWrappingHypercube.class
+-rw-rw-r--  2.0 unx     8298 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractBooleanHypercube.class
+-rw-rw-r--  2.0 unx   256779 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath.class
+-rw-rw-r--  2.0 unx     3437 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$1.class
+-rw-rw-r--  2.0 unx     1262 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$ReductiveLogicOp.class
+-rw-rw-r--  2.0 unx     1413 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$ComparisonOp.class
+-rw-rw-r--  2.0 unx     1336 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$AssociativeOp.class
+-rw-rw-r--  2.0 unx     1842 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$UnaryOp.class
+-rw-rw-r--  2.0 unx     1638 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$BinaryOp.class
+-rw-rw-r--  2.0 unx     2369 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube.class
+-rw-rw-r--  2.0 unx     2360 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$FloatSingleValueHypercube.class
+-rw-rw-r--  2.0 unx     2320 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$LongSingleValueHypercube.class
+-rw-rw-r--  2.0 unx     2374 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube.class
+-rw-rw-r--  2.0 unx     2378 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube.class
+-rw-rw-r--  2.0 unx     3991 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Double1dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     4537 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Double2dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5099 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Double3dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5695 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Double4dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6291 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Double5dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     9375 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleArrayHypercube.class
+-rw-rw-r--  2.0 unx     9504 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleAxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     7636 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleFlatRolledHypercube.class
+-rw-rw-r--  2.0 unx     3037 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleFromFloatHypercube.class
+-rw-rw-r--  2.0 unx     3053 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleFromIntegerHypercube.class
+-rw-rw-r--  2.0 unx     3027 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleFromLongHypercube.class
+-rw-rw-r--  2.0 unx     8302 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractDoubleHypercube.class
+-rw-rw-r--  2.0 unx     9958 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleMappedHypercube.class
+-rw-rw-r--  2.0 unx     9095 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleSlicedHypercube.class
+-rw-rw-r--  2.0 unx     8440 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleTransposedHypercube.class
+-rw-rw-r--  2.0 unx     5397 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleWrappingHypercube.class
+-rw-rw-r--  2.0 unx     3968 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Float1dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     4512 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Float2dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5072 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Float3dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5666 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Float4dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6260 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Float5dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     9345 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatArrayHypercube.class
+-rw-rw-r--  2.0 unx     9483 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatAxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     7613 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatFlatRolledHypercube.class
+-rw-rw-r--  2.0 unx     3036 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatFromDoubleHypercube.class
+-rw-rw-r--  2.0 unx     3042 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatFromIntegerHypercube.class
+-rw-rw-r--  2.0 unx     3016 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatFromLongHypercube.class
+-rw-rw-r--  2.0 unx     8277 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractFloatHypercube.class
+-rw-rw-r--  2.0 unx     9927 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatMappedHypercube.class
+-rw-rw-r--  2.0 unx     9074 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatSlicedHypercube.class
+-rw-rw-r--  2.0 unx     8408 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatTransposedHypercube.class
+-rw-rw-r--  2.0 unx     5370 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6972 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/GenericArrayHypercube.class
+-rw-rw-r--  2.0 unx     1045 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/GenericHypercube.class
+-rw-rw-r--  2.0 unx     6656 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/GenericWrappingHypercube.class
+-rw-rw-r--  2.0 unx     2431 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/GenericWrappingHypercube$FlattenedList.class
+-rw-rw-r--  2.0 unx     3976 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Integer1dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     4518 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Integer2dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5076 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Integer3dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5668 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Integer4dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6260 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Integer5dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     9351 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerArrayHypercube.class
+-rw-rw-r--  2.0 unx     9498 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerAxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     7655 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerFlatRolledHypercube.class
+-rw-rw-r--  2.0 unx     3054 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerFromDoubleHypercube.class
+-rw-rw-r--  2.0 unx     3044 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerFromFloatHypercube.class
+-rw-rw-r--  2.0 unx     3034 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerFromLongHypercube.class
+-rw-rw-r--  2.0 unx     8317 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractIntegerHypercube.class
+-rw-rw-r--  2.0 unx     9918 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerMappedHypercube.class
+-rw-rw-r--  2.0 unx     9089 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerSlicedHypercube.class
+-rw-rw-r--  2.0 unx     8444 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerTransposedHypercube.class
+-rw-rw-r--  2.0 unx     5424 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerWrappingHypercube.class
+-rw-rw-r--  2.0 unx     3885 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Long1dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     4464 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Long2dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5022 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Long3dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     5614 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Long4dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     6206 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Long5dWrappingHypercube.class
+-rw-rw-r--  2.0 unx     9275 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongArrayHypercube.class
+-rw-rw-r--  2.0 unx     8480 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     1132 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AxisRolledHypercube$2.class
+-rw-rw-r--  2.0 unx     1132 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AxisRolledHypercube$1.class
+-rw-rw-r--  2.0 unx     9442 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongAxisRolledHypercube.class
+-rw-rw-r--  2.0 unx     5786 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FlatRolledHypercube.class
+-rw-rw-r--  2.0 unx     1003 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FlatRolledHypercube$1.class
+-rw-rw-r--  2.0 unx     7566 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongFlatRolledHypercube.class
+-rw-rw-r--  2.0 unx    29448 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DoubleHypercube.class
+-rw-rw-r--  2.0 unx     2999 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongFromDoubleHypercube.class
+-rw-rw-r--  2.0 unx    29386 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/FloatHypercube.class
+-rw-rw-r--  2.0 unx     2989 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongFromFloatHypercube.class
+-rw-rw-r--  2.0 unx    30665 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/IntegerHypercube.class
+-rw-rw-r--  2.0 unx     3005 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongFromIntegerHypercube.class
+-rw-rw-r--  2.0 unx     8254 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractLongHypercube.class
+-rw-rw-r--  2.0 unx     9856 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongMappedHypercube.class
+-rw-rw-r--  2.0 unx     9033 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongSlicedHypercube.class
+-rw-rw-r--  2.0 unx     8391 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongTransposedHypercube.class
+-rw-rw-r--  2.0 unx    30470 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongHypercube.class
+-rw-rw-r--  2.0 unx     5331 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/LongWrappingHypercube.class
+-rw-rw-r--  2.0 unx     3311 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/MappedIndex.class
+-rw-rw-r--  2.0 unx     2186 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/NaturalIndex.class
+-rw-rw-r--  2.0 unx     9365 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/SlicedHypercube.class
+-rw-rw-r--  2.0 unx     2292 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractIndex.class
+-rw-rw-r--  2.0 unx     3558 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/SubIndex.class
+-rw-rw-r--  2.0 unx     5028 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/TransposedHypercube.class
+-rw-rw-r--  2.0 unx     1002 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/TransposedHypercube$1.class
+-rw-rw-r--  2.0 unx    17854 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/AbstractHypercube.class
+-rw-rw-r--  2.0 unx     3497 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/WrappingHypercube.class
+-rw-rw-r--  2.0 unx     1066 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Index.class
+-rw-rw-r--  2.0 unx      629 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/DimensionalityException.class
+-rw-rw-r--  2.0 unx    37504 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Hypercube.class
+-rw-rw-r--  2.0 unx     1266 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Hypercube$2.class
+-rw-rw-r--  2.0 unx     1712 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Hypercube$1.class
+-rw-rw-r--  2.0 unx     3781 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Hypercube$Flags.class
+-rw-rw-r--  2.0 unx    24977 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/BooleanHypercube.class
+-rw-rw-r--  2.0 unx     4906 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Dimension.class
+-rw-rw-r--  2.0 unx     1951 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Dimension$Roll.class
+-rw-rw-r--  2.0 unx     2192 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Dimension$Slice.class
+-rw-rw-r--  2.0 unx     1625 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Dimension$Coordinate.class
+-rw-rw-r--  2.0 unx     1024 b- defN 24-Apr-01 11:53 com/deshaw/hypercube/Dimension$Accessor.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/
+-rw-rw-r--  2.0 unx     5916 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/AsType.class
+-rw-rw-r--  2.0 unx      124 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/JavaProxyBase.class
+-rw-rw-r--  2.0 unx    11968 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/JniPJRmi.class
+-rw-rw-r--  2.0 unx      757 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/JniPJRmi$ArrayHandle.class
+-rw-rw-r--  2.0 unx     6846 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/KwargUtil.class
+-rw-rw-r--  2.0 unx     1126 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmiAgent.class
+-rw-rw-r--  2.0 unx     2344 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PipedProvider.class
+-rw-rw-r--  2.0 unx     1794 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PipedProvider$BidirectionalPipe.class
+-rw-rw-r--  2.0 unx     3095 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PipedProvider$PipedPJRmi.class
+-rw-rw-r--  2.0 unx     1922 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PipedTransport.class
+-rw-rw-r--  2.0 unx     6019 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonMinionProvider.class
+-rw-rw-r--  2.0 unx     1499 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonMinionProvider$1.class
+-rw-rw-r--  2.0 unx     5605 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonMinionTransport.class
+-rw-rw-r--  2.0 unx     1498 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonSlice.class
+-rw-rw-r--  2.0 unx     5353 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SSLSocketProvider.class
+-rw-rw-r--  2.0 unx     1002 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonKwargsFunction.class
+-rw-rw-r--  2.0 unx      442 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonFunction.class
+-rw-rw-r--  2.0 unx     5307 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject.class
+-rw-rw-r--  2.0 unx     2036 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$8.class
+-rw-rw-r--  2.0 unx     1959 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$7.class
+-rw-rw-r--  2.0 unx     1984 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$6.class
+-rw-rw-r--  2.0 unx     1907 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$5.class
+-rw-rw-r--  2.0 unx     2161 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$4.class
+-rw-rw-r--  2.0 unx     2084 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$3.class
+-rw-rw-r--  2.0 unx     2134 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$2.class
+-rw-rw-r--  2.0 unx     1876 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonObject$1.class
+-rw-rw-r--  2.0 unx      493 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonCallbackException.class
+-rw-rw-r--  2.0 unx     2144 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonMinion.class
+-rw-rw-r--  2.0 unx     1171 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PythonMinion$ByValue.class
+-rw-rw-r--  2.0 unx     6854 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/MethodUtil.class
+-rw-rw-r--  2.0 unx     1521 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
+-rw-rw-r--  2.0 unx      452 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
+-rw-rw-r--  2.0 unx     3228 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SSLSocketTransport.class
+-rw-rw-r--  2.0 unx    32184 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi.class
+-rw-rw-r--  2.0 unx     3041 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$3.class
+-rw-rw-r--  2.0 unx     1274 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$2.class
+-rw-rw-r--  2.0 unx      621 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$1.class
+-rw-rw-r--  2.0 unx    70799 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection.class
+-rw-rw-r--  2.0 unx     5116 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$3.class
+-rw-rw-r--  2.0 unx     1730 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$2.class
+-rw-rw-r--  2.0 unx     1626 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$1.class
+-rw-rw-r--  2.0 unx     8176 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl.class
+-rw-rw-r--  2.0 unx     7829 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler.class
+-rw-rw-r--  2.0 unx     6602 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler.class
+-rw-rw-r--  2.0 unx     2750 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate.class
+-rw-rw-r--  2.0 unx     2646 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate.class
+-rw-rw-r--  2.0 unx     2411 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer.class
+-rw-rw-r--  2.0 unx     2310 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer.class
+-rw-rw-r--  2.0 unx     2427 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction.class
+-rw-rw-r--  2.0 unx     2326 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction.class
+-rw-rw-r--  2.0 unx     2330 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator.class
+-rw-rw-r--  2.0 unx     2014 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable.class
+-rw-rw-r--  2.0 unx     5853 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallback.class
+-rw-rw-r--  2.0 unx     1393 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult.class
+-rw-rw-r--  2.0 unx     2163 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle.class
+-rw-rw-r--  2.0 unx     3730 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$MethodCaller.class
+-rw-rw-r--  2.0 unx     8409 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Connection$Worker.class
+-rw-rw-r--  2.0 unx      234 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ThreadId.class
+-rw-rw-r--  2.0 unx     1146 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream.class
+-rw-rw-r--  2.0 unx      788 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.class
+-rw-rw-r--  2.0 unx      995 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ClassInjector.class
+-rw-rw-r--  2.0 unx     3608 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$HandleMapping.class
+-rw-rw-r--  2.0 unx      697 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.class
+-rw-rw-r--  2.0 unx     4652 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$TypeMapping.class
+-rw-rw-r--  2.0 unx     5556 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodDescription.class
+-rw-rw-r--  2.0 unx     2572 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.class
+-rw-rw-r--  2.0 unx     3177 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodCallFuture.class
+-rw-rw-r--  2.0 unx     2178 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$SyncMode.class
+-rw-rw-r--  2.0 unx     1710 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodFlags.class
+-rw-rw-r--  2.0 unx     1964 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$FieldDescription.class
+-rw-rw-r--  2.0 unx      585 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ReadObjectResult.class
+-rw-rw-r--  2.0 unx     1242 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodSignature.class
+-rw-rw-r--  2.0 unx     2758 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MethodComparator.class
+-rw-rw-r--  2.0 unx     1151 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PythonicMethodUtil.class
+-rw-rw-r--  2.0 unx     5903 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class
+-rw-rw-r--  2.0 unx     1484 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class
+-rw-rw-r--  2.0 unx      420 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ArrayLike.class
+-rw-rw-r--  2.0 unx      343 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PythonItemAssignable.class
+-rw-rw-r--  2.0 unx      487 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PythonSubscriptable.class
+-rw-rw-r--  2.0 unx    19323 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$TypeDescription.class
+-rw-rw-r--  2.0 unx     1526 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$TypeFlags.class
+-rw-rw-r--  2.0 unx     2581 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PythonValueFormat.class
+-rw-rw-r--  2.0 unx     2603 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle.class
+-rw-rw-r--  2.0 unx     4716 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$MessageType.class
+-rw-rw-r--  2.0 unx     1191 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Flags.class
+-rw-rw-r--  2.0 unx      556 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$Kwargs.class
+-rw-rw-r--  2.0 unx      511 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$ExplicitBinding.class
+-rw-rw-r--  2.0 unx      496 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$GenericReturnType.class
+-rw-rw-r--  2.0 unx     7296 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PJRmiLockManager.class
+-rw-rw-r--  2.0 unx     1240 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2.class
+-rw-rw-r--  2.0 unx     1150 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class
+-rw-rw-r--  2.0 unx     3589 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class
+-rw-rw-r--  2.0 unx     1629 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SocketProvider.class
+-rw-rw-r--  2.0 unx     1626 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SocketTransport.class
+-rw-rw-r--  2.0 unx     5761 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SourceInjector.class
+-rw-rw-r--  2.0 unx     1144 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SourceInjector$2.class
+-rw-rw-r--  2.0 unx     1709 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SourceInjector$1.class
+-rw-rw-r--  2.0 unx     1781 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SourceInjector$JavaByteObject.class
+-rw-rw-r--  2.0 unx     1616 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/SourceInjector$JavaStringObject.class
+-rw-rw-r--  2.0 unx     3965 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/UnixFifoProvider.class
+-rw-rw-r--  2.0 unx     2802 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/UnixFifoProvider$1.class
+-rw-rw-r--  2.0 unx     1817 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/UnixFifoProvider$Fifo.class
+-rw-rw-r--  2.0 unx      645 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/Transport.class
+-rw-rw-r--  2.0 unx      486 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/Transport$Provider.class
+-rw-rw-r--  2.0 unx     2873 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/Transport$Provider$Arguments.class
+-rw-rw-r--  2.0 unx     1848 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/UnixFifoTransport.class
+-rw-rw-r--  2.0 unx     1213 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/UnixSignals.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/
+-rw-rw-r--  2.0 unx     3947 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers.class
+-rw-rw-r--  2.0 unx     1068 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThrowIterator.class
+-rw-rw-r--  2.0 unx     1187 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator.class
+-rw-rw-r--  2.0 unx      650 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$OneTwoThreeIterator$CustomNoSuchElementException.class
+-rw-rw-r--  2.0 unx     1653 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$MorePrecedenceMethods.class
+-rw-rw-r--  2.0 unx     6513 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$PrecedenceMethods.class
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$C.class
+-rw-rw-r--  2.0 unx      455 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$B.class
+-rw-rw-r--  2.0 unx      419 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$A.class
+-rw-rw-r--  2.0 unx      639 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$1Result.class
+-rw-rw-r--  2.0 unx      288 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$ObjectInterface.class
+-rw-rw-r--  2.0 unx      770 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsDerived.class
+-rw-rw-r--  2.0 unx      588 b- defN 24-Apr-01 11:53 com/deshaw/pjrmi/test/PJRmiTestHelpers$OverriddenMethodsBase.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/python/
+-rw-rw-r--  2.0 unx     2696 b- defN 24-Apr-01 11:53 com/deshaw/python/BinString.class
+-rw-rw-r--  2.0 unx     5140 b- defN 24-Apr-01 11:53 com/deshaw/python/Dict.class
+-rw-rw-r--  2.0 unx      581 b- defN 24-Apr-01 11:53 com/deshaw/python/Dict$MissingKeyException.class
+-rw-rw-r--  2.0 unx     4351 b- defN 24-Apr-01 11:53 com/deshaw/python/Operations.class
+-rw-rw-r--  2.0 unx    15924 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonPickle.class
+-rw-rw-r--  2.0 unx     1046 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonPickle$1.class
+-rw-rw-r--  2.0 unx    18309 b- defN 24-Apr-01 11:53 com/deshaw/python/NumpyArray.class
+-rw-rw-r--  2.0 unx      994 b- defN 24-Apr-01 11:53 com/deshaw/python/NumpyArray$1.class
+-rw-rw-r--  2.0 unx      337 b- defN 24-Apr-01 11:53 com/deshaw/python/NumpyArray$ElementVisitor.class
+-rw-rw-r--  2.0 unx     5048 b- defN 24-Apr-01 11:53 com/deshaw/python/DType.class
+-rw-rw-r--  2.0 unx     2679 b- defN 24-Apr-01 11:53 com/deshaw/python/DType$Type.class
+-rw-rw-r--  2.0 unx      683 b- defN 24-Apr-01 11:53 com/deshaw/python/MalformedPickleException.class
+-rw-rw-r--  2.0 unx    15621 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle.class
+-rw-rw-r--  2.0 unx     3276 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$2.class
+-rw-rw-r--  2.0 unx      528 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$1.class
+-rw-rw-r--  2.0 unx     1130 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$UnpickleableDType.class
+-rw-rw-r--  2.0 unx     2260 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$NumpyFrombufferArray.class
+-rw-rw-r--  2.0 unx     3503 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$UnpickleableNumpyArray.class
+-rw-rw-r--  2.0 unx     2079 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$BytesPlaceholder.class
+-rw-rw-r--  2.0 unx     2755 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$Encoder.class
+-rw-rw-r--  2.0 unx     1679 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$DTypeFactory.class
+-rw-rw-r--  2.0 unx      983 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$NDArrayType.class
+-rw-rw-r--  2.0 unx     2760 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayScalar.class
+-rw-rw-r--  2.0 unx     1709 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$NumpyFrombuffer.class
+-rw-rw-r--  2.0 unx     1032 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$NumpyCoreMultiarrayReconstruct.class
+-rw-rw-r--  2.0 unx      392 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$Global.class
+-rw-rw-r--  2.0 unx      387 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$Instance.class
+-rw-rw-r--  2.0 unx     1208 b- defN 24-Apr-01 11:53 com/deshaw/python/PythonUnpickle$ShrinkableList.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/util/
+-rw-rw-r--  2.0 unx     4673 b- defN 24-Apr-01 11:53 com/deshaw/util/ByteList.class
+-rw-rw-r--  2.0 unx     2919 b- defN 24-Apr-01 11:53 com/deshaw/util/StringUtil.class
+-rw-rw-r--  2.0 unx     3465 b- defN 24-Apr-01 11:53 com/deshaw/util/StringUtil$HashableSubSequence.class
+-rw-rw-r--  2.0 unx     3312 b- defN 24-Apr-01 11:53 com/deshaw/util/SwappingPool.class
+-rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-01 11:53 com/deshaw/util/SwappingPool$1.class
+-rw-rw-r--  2.0 unx     1591 b- defN 24-Apr-01 11:53 com/deshaw/util/SwappingPool$Stack.class
+-rw-rw-r--  2.0 unx      982 b- defN 24-Apr-01 11:53 com/deshaw/util/ThreadLocalStringBuilder.class
+-rw-rw-r--  2.0 unx      675 b- defN 24-Apr-01 11:53 com/deshaw/util/Pool.class
+-rw-rw-r--  2.0 unx      790 b- defN 24-Apr-01 11:53 com/deshaw/util/Instrumentor.class
+-rw-rw-r--  2.0 unx      728 b- defN 24-Apr-01 11:53 com/deshaw/util/Instrumentor$2.class
+-rw-rw-r--  2.0 unx      729 b- defN 24-Apr-01 11:53 com/deshaw/util/Instrumentor$1.class
+-rw-rw-r--  2.0 unx      335 b- defN 24-Apr-01 11:53 com/deshaw/util/Instrumentor$Factory.class
+drwxrwxr-x  2.0 unx        0 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/
+-rw-rw-r--  2.0 unx    22212 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager.class
+-rw-rw-r--  2.0 unx     1110 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$2.class
+-rw-rw-r--  2.0 unx     5322 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$NamedReentrantLock.class
+-rw-rw-r--  2.0 unx     1456 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$1.class
+-rw-rw-r--  2.0 unx     3244 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$LockManagerLock.class
+-rw-rw-r--  2.0 unx     4194 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$LockManagerLock$Locker.class
+-rw-rw-r--  2.0 unx     1200 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$ColouredList.class
+-rw-rw-r--  2.0 unx     4778 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$ThreadLockState.class
+-rw-rw-r--  2.0 unx     2039 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$ThreadLockState$Details.class
+-rw-rw-r--  2.0 unx     1407 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$SafeReadWriteLock.class
+-rw-rw-r--  2.0 unx     3227 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$SafeLock.class
+-rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$SafeLock$AcquireFailedException.class
+-rw-rw-r--  2.0 unx      566 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/LockManager$DeadlockException.class
+-rw-rw-r--  2.0 unx     6390 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/VirtualThreadLock.class
+-rw-rw-r--  2.0 unx      895 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/VirtualThreadLock$1.class
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-01 11:53 com/deshaw/util/concurrent/VirtualThreadLock$VirtualThread.class
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/snappy-java/
 -rw-r--r--  2.0 unx    11560 b- defN 13-Mar-22 15:33 META-INF/maven/org.xerial.snappy/snappy-java/LICENSE
 -rw-r--r--  2.0 unx      139 b- defN 13-Nov-08 00:11 META-INF/maven/org.xerial.snappy/snappy-java/pom.properties
 -rw-r--r--  2.0 unx    11865 b- defN 13-Nov-08 00:10 META-INF/maven/org.xerial.snappy/snappy-java/pom.xml
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/
@@ -369,8 +371,8 @@
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/xerial/snappy/native/SunOS/x86_64/
 -rw-r--r--  2.0 unx    40352 b- defN 13-Nov-08 00:07 org/xerial/snappy/native/SunOS/x86_64/libsnappyjava.so
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/xerial/snappy/native/Windows/
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/xerial/snappy/native/Windows/x86/
 -rw-r--r--  2.0 unx   118784 b- defN 13-Nov-08 00:10 org/xerial/snappy/native/Windows/x86/snappyjava.dll
 drwxr-xr-x  2.0 unx        0 b- defN 13-Nov-08 00:11 org/xerial/snappy/native/Windows/x86_64/
 -rw-r--r--  2.0 unx   137216 b- defN 13-Nov-08 00:10 org/xerial/snappy/native/Windows/x86_64/snappyjava.dll
-374 files, 2680862 bytes uncompressed, 1097112 bytes compressed:  59.1%
+376 files, 2711628 bytes uncompressed, 1107182 bytes compressed:  59.2%
```

#### zipnote «TEMP»/diffoscope_9kkaekmd_/tmpavaz4p70_.zip

```diff
@@ -6,14 +6,26 @@
 
 Filename: com/
 Comment: 
 
 Filename: com/deshaw/
 Comment: 
 
+Filename: com/deshaw/io/
+Comment: 
+
+Filename: com/deshaw/io/BlockingPipe.class
+Comment: 
+
+Filename: com/deshaw/io/BlockingPipe$Output.class
+Comment: 
+
+Filename: com/deshaw/io/BlockingPipe$Input.class
+Comment: 
+
 Filename: com/deshaw/hypercube/
 Comment: 
 
 Filename: com/deshaw/hypercube/Boolean1dWrappingHypercube.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Boolean2dWrappingHypercube.class
@@ -57,17 +69,14 @@
 
 Filename: com/deshaw/hypercube/BooleanWrappingHypercube.class
 Comment: 
 
 Filename: com/deshaw/hypercube/AbstractBooleanHypercube.class
 Comment: 
 
-Filename: com/deshaw/hypercube/BooleanHypercube.class
-Comment: 
-
 Filename: com/deshaw/hypercube/CubeMath.class
 Comment: 
 
 Filename: com/deshaw/hypercube/CubeMath$1.class
 Comment: 
 
 Filename: com/deshaw/hypercube/CubeMath$ReductiveLogicOp.class
@@ -348,14 +357,20 @@
 
 Filename: com/deshaw/hypercube/TransposedHypercube.class
 Comment: 
 
 Filename: com/deshaw/hypercube/TransposedHypercube$1.class
 Comment: 
 
+Filename: com/deshaw/hypercube/AbstractHypercube.class
+Comment: 
+
+Filename: com/deshaw/hypercube/WrappingHypercube.class
+Comment: 
+
 Filename: com/deshaw/hypercube/Index.class
 Comment: 
 
 Filename: com/deshaw/hypercube/DimensionalityException.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Hypercube.class
@@ -366,15 +381,15 @@
 
 Filename: com/deshaw/hypercube/Hypercube$1.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Hypercube$Flags.class
 Comment: 
 
-Filename: com/deshaw/hypercube/AbstractHypercube.class
+Filename: com/deshaw/hypercube/BooleanHypercube.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Dimension.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Dimension$Roll.class
 Comment: 
@@ -384,29 +399,14 @@
 
 Filename: com/deshaw/hypercube/Dimension$Coordinate.class
 Comment: 
 
 Filename: com/deshaw/hypercube/Dimension$Accessor.class
 Comment: 
 
-Filename: com/deshaw/hypercube/WrappingHypercube.class
-Comment: 
-
-Filename: com/deshaw/io/
-Comment: 
-
-Filename: com/deshaw/io/BlockingPipe.class
-Comment: 
-
-Filename: com/deshaw/io/BlockingPipe$Output.class
-Comment: 
-
-Filename: com/deshaw/io/BlockingPipe$Input.class
-Comment: 
-
 Filename: com/deshaw/pjrmi/
 Comment: 
 
 Filename: com/deshaw/pjrmi/AsType.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/JavaProxyBase.class
@@ -417,14 +417,17 @@
 
 Filename: com/deshaw/pjrmi/JniPJRmi$ArrayHandle.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/KwargUtil.class
 Comment: 
 
+Filename: com/deshaw/pjrmi/PJRmiAgent.class
+Comment: 
+
 Filename: com/deshaw/pjrmi/PipedProvider.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PipedProvider$BidirectionalPipe.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PipedProvider$PipedPJRmi.class
@@ -486,14 +489,26 @@
 
 Filename: com/deshaw/pjrmi/PythonMinion.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PythonMinion$ByValue.class
 Comment: 
 
+Filename: com/deshaw/pjrmi/MethodUtil.class
+Comment: 
+
+Filename: com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
+Comment: 
+
+Filename: com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
+Comment: 
+
+Filename: com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
+Comment: 
+
 Filename: com/deshaw/pjrmi/SSLSocketTransport.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi$3.class
@@ -609,14 +624,17 @@
 
 Filename: com/deshaw/pjrmi/PJRmi$MethodSignature.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi$MethodComparator.class
 Comment: 
 
+Filename: com/deshaw/pjrmi/PJRmi$PythonicMethodUtil.class
+Comment: 
+
 Filename: com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi$ArrayLike.class
@@ -663,26 +681,14 @@
 
 Filename: com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class
 Comment: 
 
-Filename: com/deshaw/pjrmi/MethodUtil.class
-Comment: 
-
-Filename: com/deshaw/pjrmi/MethodUtil$ConstructorWrapper.class
-Comment: 
-
-Filename: com/deshaw/pjrmi/MethodUtil$MethodWrapper.class
-Comment: 
-
-Filename: com/deshaw/pjrmi/MethodUtil$CallableWrapper.class
-Comment: 
-
 Filename: com/deshaw/pjrmi/SocketProvider.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/SocketTransport.class
 Comment: 
 
 Filename: com/deshaw/pjrmi/SourceInjector.class
```

#### filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,2 +1,6 @@
 Manifest-Version: 1.0
+Agent-Class: com.deshaw.pjrmi.PJRmiAgent
+Premain-Class: com.deshaw.pjrmi.PJRmiAgent
+Can-Redefine-Classes: true
+Can-Retransform-Classes: true
```

#### com/deshaw/hypercube/CubeMath.class

##### procyon -ec {}

```diff
@@ -163,28 +163,16 @@
         Dimension<?>[] dims;
         if (shape instanceof Dimension[]) {
             dims = (Dimension<?>[])shape;
         }
         else {
             dims = (Dimension<?>[])Dimension.of(KwargUtil.toLongArray(shape));
         }
-        Object dtype = (kwargs == null) ? "float64" : kwargs.getOrDefault("dtype", "float");
-        if (dtype == null) {
-            throw new IllegalArgumentException("Specified dtype was null");
-        }
-        if (dtype.equals("float")) {
-            dtype = "float64";
-        }
-        if (!(dtype instanceof String)) {
-            dtype = dtype.toString();
-        }
-        final DType.Type type = DType.Type.byName((String)dtype);
-        if (type == null) {
-            throw new IllegalArgumentException("No dtype for '" + dtype);
-        }
+        final Object dtype = (kwargs == null) ? "float64" : kwargs.get("dtype");
+        final DType.Type type = KwargUtil.toDTypeType(dtype);
         final Class<?> klass = type.objectClass;
         if (klass.equals(Double.class)) {
             return (Hypercube<?>)new DoubleArrayHypercube((Dimension[])dims);
         }
         if (klass.equals(Float.class)) {
             return (Hypercube<?>)new FloatArrayHypercube((Dimension[])dims);
         }
@@ -209,28 +197,16 @@
         Dimension<?>[] dims;
         if (shape instanceof Dimension[]) {
             dims = (Dimension<?>[])shape;
         }
         else {
             dims = (Dimension<?>[])Dimension.of(KwargUtil.toLongArray(shape));
         }
-        Object dtype = (kwargs == null) ? "float64" : kwargs.get("dtype");
-        if (dtype == null) {
-            dtype = "float";
-        }
-        if (dtype.equals("float")) {
-            dtype = "float64";
-        }
-        if (!(dtype instanceof String)) {
-            dtype = dtype.toString();
-        }
-        final DType.Type type = DType.Type.byName((String)dtype);
-        if (type == null) {
-            throw new IllegalArgumentException("No dtype for '" + dtype);
-        }
+        final Object dtype = (kwargs == null) ? "float64" : kwargs.get("dtype");
+        final DType.Type type = KwargUtil.toDTypeType(dtype);
         final Class<?> klass = type.objectClass;
         if (klass.equals(Double.class)) {
             return full(dims, 0.0);
         }
         if (klass.equals(Float.class)) {
             return full(dims, 0.0f);
         }
@@ -255,28 +231,16 @@
         Dimension<?>[] dims;
         if (shape instanceof Dimension[]) {
             dims = (Dimension<?>[])shape;
         }
         else {
             dims = (Dimension<?>[])Dimension.of(KwargUtil.toLongArray(shape));
         }
-        Object dtype = (kwargs == null) ? "float64" : kwargs.get("dtype");
-        if (dtype == null) {
-            dtype = "float";
-        }
-        if (dtype.equals("float")) {
-            dtype = "float64";
-        }
-        if (!(dtype instanceof String)) {
-            dtype = dtype.toString();
-        }
-        final DType.Type type = DType.Type.byName((String)dtype);
-        if (type == null) {
-            throw new IllegalArgumentException("No dtype for '" + dtype);
-        }
+        final Object dtype = (kwargs == null) ? "float64" : kwargs.get("dtype");
+        final DType.Type type = KwargUtil.toDTypeType(dtype);
         final Class<?> klass = type.objectClass;
         if (klass.equals(Double.class)) {
             return full(dims, 1.0);
         }
         if (klass.equals(Float.class)) {
             return full(dims, 1.0f);
         }
@@ -394,250 +358,250 @@
     
     public static long popcount(final Hypercube<Boolean> a) throws NullPointerException {
         return popcount(a, 0L, a.getSize());
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.ADD);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.ADD);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.ADD);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.ADD);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.ADD);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> add(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.ADD);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.ADD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.SUB);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.SUB);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.SUB);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.SUB);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.SUB);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> subtract(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.SUB);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.SUB);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.MUL);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.MUL);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.MUL);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.MUL);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.MUL);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> multiply(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.MUL);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.MUL);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.DIV);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.DIV);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.DIV);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.DIV);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.DIV);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> divide(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.DIV);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.DIV);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.MOD);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.MOD);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.MOD);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.MOD);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.MOD);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> mod(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.MOD);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.MOD);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.POW);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.POW);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.POW);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.POW);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.POW);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> power(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.POW);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.POW);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.MIN);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.MIN);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.MIN);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.MIN);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.MIN);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> minimum(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.MIN);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.MIN);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.MAX);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.MAX);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.MAX);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.MAX);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.MAX);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> maximum(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.MAX);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.MAX);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> negative(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
         return unaryOp(a, CubeMath.UnaryOp.NEG);
     }
     
@@ -773,393 +737,441 @@
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> tanh(final Hypercube<T> a, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         return unaryOp(a, r, CubeMath.UnaryOp.TANH);
     }
     
     public static <T> T sum0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return associativeOp(a, CubeMath.AssociativeOp.ADD);
+        return associativeOp(a, null, (BooleanHypercube)null, CubeMath.AssociativeOp.ADD);
+    }
+    
+    public static <T> T sum0d(final Hypercube<T> a, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOp(a, initial, where, CubeMath.AssociativeOp.ADD);
     }
     
     public static <T> T min0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return associativeOp(a, CubeMath.AssociativeOp.MIN);
+        return associativeOp(a, null, (BooleanHypercube)null, CubeMath.AssociativeOp.MIN);
+    }
+    
+    public static <T> T min0d(final Hypercube<T> a, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOp(a, initial, where, CubeMath.AssociativeOp.MIN);
     }
     
     public static <T> T max0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return associativeOp(a, CubeMath.AssociativeOp.MAX);
+        return associativeOp(a, null, (BooleanHypercube)null, CubeMath.AssociativeOp.MAX);
+    }
+    
+    public static <T> T max0d(final Hypercube<T> a, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOp(a, initial, where, CubeMath.AssociativeOp.MAX);
     }
     
     public static <T> T nansum0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return associativeOp(a, CubeMath.AssociativeOp.NANADD);
+        return associativeOp(a, null, (BooleanHypercube)null, CubeMath.AssociativeOp.NANADD);
+    }
+    
+    public static <T> T nansum0d(final Hypercube<T> a, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOp(a, initial, where, CubeMath.AssociativeOp.NANADD);
     }
     
     @PJRmi.GenericReturnType
-    public static <T> Hypercube<T> sumNd(final Hypercube<T> a, final int[] axes) throws NullPointerException, UnsupportedOperationException {
-        return associativeOpByAxes(a, axes, CubeMath.AssociativeOp.ADD);
+    public static <T> Hypercube<T> sumNd(final Hypercube<T> a, final int[] axes, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.ADD);
     }
     
     @PJRmi.GenericReturnType
-    public static <T> Hypercube<T> minNd(final Hypercube<T> a, final int[] axes) throws NullPointerException, UnsupportedOperationException {
-        return associativeOpByAxes(a, axes, CubeMath.AssociativeOp.MIN);
+    public static <T> Hypercube<T> minNd(final Hypercube<T> a, final int[] axes, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.MIN);
     }
     
     @PJRmi.GenericReturnType
-    public static <T> Hypercube<T> maxNd(final Hypercube<T> a, final int[] axes) throws NullPointerException, UnsupportedOperationException {
-        return associativeOpByAxes(a, axes, CubeMath.AssociativeOp.MAX);
+    public static <T> Hypercube<T> maxNd(final Hypercube<T> a, final int[] axes, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.MAX);
     }
     
     @PJRmi.GenericReturnType
-    public static <T> Hypercube<T> nansumNd(final Hypercube<T> a, final int[] axes) throws NullPointerException, UnsupportedOperationException {
-        return associativeOpByAxes(a, axes, CubeMath.AssociativeOp.NANADD);
+    public static <T> Hypercube<T> nansumNd(final Hypercube<T> a, final int[] axes, final T initial, final BooleanHypercube where) throws NullPointerException, UnsupportedOperationException {
+        return associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.NANADD);
     }
     
     @PJRmi.Kwargs("axis,dtype,out,keepdims,initial,where")
     @PJRmi.GenericReturnType
     public static <T> Object sum(final Hypercube<T> a, final Map<String, Object> kwargs) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         int[] axes = null;
+        T initial = null;
+        BooleanHypercube where = null;
         if (kwargs != null) {
             for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
                 final String s = (String)entry.getKey();
                 int n = -1;
                 switch (s.hashCode()) {
                     case 3008417: {
                         if (s.equals("axis")) {
                             n = 0;
                             break;
                         }
                         break;
                     }
-                    case 110414: {
-                        if (s.equals("out")) {
+                    case 1948342084: {
+                        if (s.equals("initial")) {
                             n = 1;
                             break;
                         }
                         break;
                     }
-                    case 1948342084: {
-                        if (s.equals("initial")) {
+                    case 113097959: {
+                        if (s.equals("where")) {
                             n = 2;
                             break;
                         }
                         break;
                     }
-                    case 113097959: {
-                        if (s.equals("where")) {
+                    case 110414: {
+                        if (s.equals("out")) {
                             n = 3;
                             break;
                         }
                         break;
                     }
                 }
                 switch (n) {
                     case 0: {
                         axes = KwargUtil.toIntArray(entry.getValue());
                         continue;
                     }
-                    case 1:
-                    case 2:
+                    case 1: {
+                        initial = (T)KwargUtil.toClassValue(entry.getValue(), a.getElementType());
+                        continue;
+                    }
+                    case 2: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
                     case 3: {
                         if (entry.getValue() != null) {
                             throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                         }
                         continue;
                     }
                     default: {
                         throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                     }
                 }
             }
         }
         if (axes == null) {
-            return associativeOp(a, CubeMath.AssociativeOp.ADD);
+            return associativeOp(a, initial, where, CubeMath.AssociativeOp.ADD);
         }
-        final Hypercube<T> result = associativeOpByAxes(a, axes, CubeMath.AssociativeOp.ADD);
+        final Hypercube<T> result = associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.ADD);
         return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
     @PJRmi.Kwargs("axis,dtype,out,keepdims,initial,where")
     @PJRmi.GenericReturnType
     public static <T> Object min(final Hypercube<T> a, final Map<String, Object> kwargs) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         int[] axes = null;
+        T initial = null;
+        BooleanHypercube where = null;
         if (kwargs != null) {
             for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
                 final String s = (String)entry.getKey();
                 int n = -1;
                 switch (s.hashCode()) {
                     case 3008417: {
                         if (s.equals("axis")) {
                             n = 0;
                             break;
                         }
                         break;
                     }
-                    case 110414: {
-                        if (s.equals("out")) {
+                    case 1948342084: {
+                        if (s.equals("initial")) {
                             n = 1;
                             break;
                         }
                         break;
                     }
-                    case 1948342084: {
-                        if (s.equals("initial")) {
+                    case 113097959: {
+                        if (s.equals("where")) {
                             n = 2;
                             break;
                         }
                         break;
                     }
-                    case 113097959: {
-                        if (s.equals("where")) {
+                    case 110414: {
+                        if (s.equals("out")) {
                             n = 3;
                             break;
                         }
                         break;
                     }
                 }
                 switch (n) {
                     case 0: {
                         axes = KwargUtil.toIntArray(entry.getValue());
                         continue;
                     }
-                    case 1:
-                    case 2:
+                    case 1: {
+                        initial = (T)KwargUtil.toClassValue(entry.getValue(), a.getElementType());
+                        continue;
+                    }
+                    case 2: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
                     case 3: {
                         if (entry.getValue() != null) {
                             throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                         }
                         continue;
                     }
                     default: {
                         throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                     }
                 }
             }
         }
         if (axes == null) {
-            return associativeOp(a, CubeMath.AssociativeOp.MIN);
+            return associativeOp(a, initial, where, CubeMath.AssociativeOp.MIN);
         }
-        final Hypercube<T> result = associativeOpByAxes(a, axes, CubeMath.AssociativeOp.MIN);
+        final Hypercube<T> result = associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.MIN);
         return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
     @PJRmi.Kwargs("axis,dtype,out,keepdims,initial,where")
     @PJRmi.GenericReturnType
     public static <T> Object max(final Hypercube<T> a, final Map<String, Object> kwargs) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         int[] axes = null;
+        T initial = null;
+        BooleanHypercube where = null;
         if (kwargs != null) {
             for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
                 final String s = (String)entry.getKey();
                 int n = -1;
                 switch (s.hashCode()) {
                     case 3008417: {
                         if (s.equals("axis")) {
                             n = 0;
                             break;
                         }
                         break;
                     }
-                    case 110414: {
-                        if (s.equals("out")) {
+                    case 1948342084: {
+                        if (s.equals("initial")) {
                             n = 1;
                             break;
                         }
                         break;
                     }
-                    case 1948342084: {
-                        if (s.equals("initial")) {
+                    case 113097959: {
+                        if (s.equals("where")) {
                             n = 2;
                             break;
                         }
                         break;
                     }
-                    case 113097959: {
-                        if (s.equals("where")) {
+                    case 110414: {
+                        if (s.equals("out")) {
                             n = 3;
                             break;
                         }
                         break;
                     }
                 }
                 switch (n) {
                     case 0: {
                         axes = KwargUtil.toIntArray(entry.getValue());
                         continue;
                     }
-                    case 1:
-                    case 2:
+                    case 1: {
+                        initial = (T)KwargUtil.toClassValue(entry.getValue(), a.getElementType());
+                        continue;
+                    }
+                    case 2: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
                     case 3: {
                         if (entry.getValue() != null) {
                             throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                         }
                         continue;
                     }
                     default: {
                         throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                     }
                 }
             }
         }
         if (axes == null) {
-            return associativeOp(a, CubeMath.AssociativeOp.MAX);
+            return associativeOp(a, initial, where, CubeMath.AssociativeOp.MAX);
         }
-        final Hypercube<T> result = associativeOpByAxes(a, axes, CubeMath.AssociativeOp.MAX);
+        final Hypercube<T> result = associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.MAX);
         return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
     @PJRmi.Kwargs("axis,dtype,out,keepdims,initial,where")
     @PJRmi.GenericReturnType
     public static <T> Object nansum(final Hypercube<T> a, final Map<String, Object> kwargs) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         int[] axes = null;
+        T initial = null;
+        BooleanHypercube where = null;
         if (kwargs != null) {
             for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
                 final String s = (String)entry.getKey();
                 int n = -1;
                 switch (s.hashCode()) {
                     case 3008417: {
                         if (s.equals("axis")) {
                             n = 0;
                             break;
                         }
                         break;
                     }
-                    case 110414: {
-                        if (s.equals("out")) {
+                    case 1948342084: {
+                        if (s.equals("initial")) {
                             n = 1;
                             break;
                         }
                         break;
                     }
-                    case 1948342084: {
-                        if (s.equals("initial")) {
+                    case 113097959: {
+                        if (s.equals("where")) {
                             n = 2;
                             break;
                         }
                         break;
                     }
-                    case 113097959: {
-                        if (s.equals("where")) {
+                    case 110414: {
+                        if (s.equals("out")) {
                             n = 3;
                             break;
                         }
                         break;
                     }
                 }
                 switch (n) {
                     case 0: {
                         axes = KwargUtil.toIntArray(entry.getValue());
                         continue;
                     }
-                    case 1:
-                    case 2:
+                    case 1: {
+                        initial = (T)KwargUtil.toClassValue(entry.getValue(), a.getElementType());
+                        continue;
+                    }
+                    case 2: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
                     case 3: {
                         if (entry.getValue() != null) {
                             throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                         }
                         continue;
                     }
                     default: {
                         throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
                     }
                 }
             }
         }
         if (axes == null) {
-            return associativeOp(a, CubeMath.AssociativeOp.NANADD);
+            return associativeOp(a, initial, where, CubeMath.AssociativeOp.NANADD);
         }
-        final Hypercube<T> result = associativeOpByAxes(a, axes, CubeMath.AssociativeOp.NANADD);
+        final Hypercube<T> result = associativeOpByAxes(a, axes, initial, where, CubeMath.AssociativeOp.NANADD);
         return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.AND);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.AND);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.AND);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.AND);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.AND);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> and(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.AND);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.AND);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.OR);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.OR);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.OR);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.OR);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.OR);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> or(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.OR);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.OR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final Hypercube<T> a, final Hypercube<T> b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, CubeMath.BinaryOp.XOR);
+        return binaryOp(a, b, null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, b, r, CubeMath.BinaryOp.XOR);
+        return binaryOp(a, b, r, null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final Hypercube<T> a, final T b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), CubeMath.BinaryOp.XOR);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), (BooleanHypercube)null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final T a, final Hypercube<T> b) throws NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.BinaryOp.XOR);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, (BooleanHypercube)null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final Hypercube<T> a, final T b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp(a, (com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, CubeMath.BinaryOp.XOR);
+        return binaryOp(a, singleValuedCube((com.deshaw.hypercube.Hypercube<T>)a, (T)b), r, (BooleanHypercube)null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> xor(final T a, final Hypercube<T> b, final Hypercube<T> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
-        return binaryOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.BinaryOp.XOR);
+        return binaryOp(singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, (BooleanHypercube)null, CubeMath.BinaryOp.XOR);
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> not(final Hypercube<T> a) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         return unaryOp(a, CubeMath.UnaryOp.NOT);
     }
     
@@ -1308,20 +1320,156 @@
         return comparisonOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, CubeMath.ComparisonOp.GE);
     }
     
     public static <T> Hypercube<Boolean> greaterEqual(final T a, final Hypercube<T> b, final Hypercube<Boolean> r) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         return comparisonOp((com.deshaw.hypercube.Hypercube<T>)singleValuedCube((com.deshaw.hypercube.Hypercube<T>)b, (T)a), b, r, CubeMath.ComparisonOp.GE);
     }
     
-    public static <T> boolean any(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return reductiveLogicOp(a, CubeMath.ReductiveLogicOp.ANY);
+    public static <T> boolean any0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
+        return reductiveLogicOp(a, null, CubeMath.ReductiveLogicOp.ANY);
+    }
+    
+    public static <T> boolean all0d(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
+        return reductiveLogicOp(a, null, CubeMath.ReductiveLogicOp.ALL);
+    }
+    
+    @PJRmi.Kwargs("axis,out,keepdims,where")
+    @PJRmi.GenericReturnType
+    public static <T> Object any(final Hypercube<T> a, final Map<String, Object> kwargs) throws NullPointerException, UnsupportedOperationException {
+        int[] axes = null;
+        BooleanHypercube where = null;
+        if (kwargs != null) {
+            for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
+                final String s = (String)entry.getKey();
+                int n = -1;
+                switch (s.hashCode()) {
+                    case 3008417: {
+                        if (s.equals("axis")) {
+                            n = 0;
+                            break;
+                        }
+                        break;
+                    }
+                    case 113097959: {
+                        if (s.equals("where")) {
+                            n = 1;
+                            break;
+                        }
+                        break;
+                    }
+                    case 110414: {
+                        if (s.equals("out")) {
+                            n = 2;
+                            break;
+                        }
+                        break;
+                    }
+                    case 1948342084: {
+                        if (s.equals("initial")) {
+                            n = 3;
+                            break;
+                        }
+                        break;
+                    }
+                }
+                switch (n) {
+                    case 0: {
+                        axes = KwargUtil.toIntArray(entry.getValue());
+                        continue;
+                    }
+                    case 1: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
+                    case 2:
+                    case 3: {
+                        if (entry.getValue() != null) {
+                            throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
+                        }
+                        continue;
+                    }
+                    default: {
+                        throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
+                    }
+                }
+            }
+        }
+        if (axes == null) {
+            return Boolean.valueOf(reductiveLogicOp(a, (BooleanHypercube)null, CubeMath.ReductiveLogicOp.ANY));
+        }
+        final BooleanHypercube result = reductiveLogicOpByAxes(a, axes, where, CubeMath.ReductiveLogicOp.ANY);
+        return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
-    public static <T> boolean all(final Hypercube<T> a) throws NullPointerException, UnsupportedOperationException {
-        return reductiveLogicOp(a, CubeMath.ReductiveLogicOp.ALL);
+    @PJRmi.Kwargs("axis,out,keepdims,where")
+    @PJRmi.GenericReturnType
+    public static <T> Object all(final Hypercube<T> a, final Map<String, Object> kwargs) throws NullPointerException, UnsupportedOperationException {
+        int[] axes = null;
+        BooleanHypercube where = null;
+        if (kwargs != null) {
+            for (final Map.Entry<String, Object> entry : kwargs.entrySet()) {
+                final String s = (String)entry.getKey();
+                int n = -1;
+                switch (s.hashCode()) {
+                    case 3008417: {
+                        if (s.equals("axis")) {
+                            n = 0;
+                            break;
+                        }
+                        break;
+                    }
+                    case 113097959: {
+                        if (s.equals("where")) {
+                            n = 1;
+                            break;
+                        }
+                        break;
+                    }
+                    case 110414: {
+                        if (s.equals("out")) {
+                            n = 2;
+                            break;
+                        }
+                        break;
+                    }
+                    case 1948342084: {
+                        if (s.equals("initial")) {
+                            n = 3;
+                            break;
+                        }
+                        break;
+                    }
+                }
+                switch (n) {
+                    case 0: {
+                        axes = KwargUtil.toIntArray(entry.getValue());
+                        continue;
+                    }
+                    case 1: {
+                        where = KwargUtil.toBooleanHypercube(entry.getValue());
+                        continue;
+                    }
+                    case 2:
+                    case 3: {
+                        if (entry.getValue() != null) {
+                            throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
+                        }
+                        continue;
+                    }
+                    default: {
+                        throw new UnsupportedOperationException("Unhandled kwarg: " + entry);
+                    }
+                }
+            }
+        }
+        if (axes == null) {
+            return Boolean.valueOf(reductiveLogicOp(a, (BooleanHypercube)null, CubeMath.ReductiveLogicOp.ALL));
+        }
+        final BooleanHypercube result = reductiveLogicOpByAxes(a, axes, where, CubeMath.ReductiveLogicOp.ALL);
+        return result.isSingleton() ? result.getObjectAt(0L) : result;
     }
     
     @PJRmi.GenericReturnType
     public static <T> Hypercube<T> extract(final Hypercube<Boolean> c, final Hypercube<T> a) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         if (c == null) {
             throw new NullPointerException("Given a null cube, 'c'");
         }
@@ -1345,69 +1493,75 @@
         }
         if (a.getElementType().equals(Boolean.class)) {
             return (Hypercube<T>)booleanExtract(c, (Hypercube<Boolean>)a);
         }
         throw new UnsupportedOperationException("Don't know how to perform extract operation on a cube with element type " + a.getElementType().getSimpleName());
     }
     
-    private static <T> Hypercube<T> binaryOp(final Hypercube<T> a, final Hypercube<T> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static <T> Hypercube<T> binaryOp(final Hypercube<T> a, final Hypercube<T> b, final BooleanHypercube w, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Given an incompatible 'w' cube");
+        }
         if (a.getElementType().equals(Double.class)) {
-            return (Hypercube<T>)doubleBinaryOp((Hypercube<Double>)a, (Hypercube<Double>)b, op);
+            return (Hypercube<T>)doubleBinaryOp((Hypercube<Double>)a, (Hypercube<Double>)b, w, op);
         }
         if (a.getElementType().equals(Float.class)) {
-            return (Hypercube<T>)floatBinaryOp((Hypercube<Float>)a, (Hypercube<Float>)b, op);
+            return (Hypercube<T>)floatBinaryOp((Hypercube<Float>)a, (Hypercube<Float>)b, w, op);
         }
         if (a.getElementType().equals(Integer.class)) {
-            return (Hypercube<T>)intBinaryOp((Hypercube<Integer>)a, (Hypercube<Integer>)b, op);
+            return (Hypercube<T>)intBinaryOp((Hypercube<Integer>)a, (Hypercube<Integer>)b, w, op);
         }
         if (a.getElementType().equals(Long.class)) {
-            return (Hypercube<T>)longBinaryOp((Hypercube<Long>)a, (Hypercube<Long>)b, op);
+            return (Hypercube<T>)longBinaryOp((Hypercube<Long>)a, (Hypercube<Long>)b, w, op);
         }
         if (a.getElementType().equals(Boolean.class)) {
-            return (Hypercube<T>)booleanBinaryOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)b, op);
+            return (Hypercube<T>)booleanBinaryOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)b, w, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform binary " + op + " on cubes with element type " + a.getElementType().getSimpleName());
     }
     
-    private static <T> Hypercube<T> binaryOp(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static <T> Hypercube<T> binaryOp(final Hypercube<T> a, final Hypercube<T> b, final Hypercube<T> r, final BooleanHypercube w, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
             throw new NullPointerException("Given a null cube, 'r'");
         }
         if (!a.matches((Hypercube)b) || !a.matches((Hypercube)r)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Given an incompatible 'w' cube");
+        }
         if (a.getElementType().equals(Double.class)) {
-            return (Hypercube<T>)doubleBinaryOp((Hypercube<Double>)a, (Hypercube<Double>)b, (Hypercube<Double>)r, op);
+            return (Hypercube<T>)doubleBinaryOp((Hypercube<Double>)a, (Hypercube<Double>)b, (Hypercube<Double>)r, w, op);
         }
         if (a.getElementType().equals(Float.class)) {
-            return (Hypercube<T>)floatBinaryOp((Hypercube<Float>)a, (Hypercube<Float>)b, (Hypercube<Float>)r, op);
+            return (Hypercube<T>)floatBinaryOp((Hypercube<Float>)a, (Hypercube<Float>)b, (Hypercube<Float>)r, w, op);
         }
         if (a.getElementType().equals(Integer.class)) {
-            return (Hypercube<T>)intBinaryOp((Hypercube<Integer>)a, (Hypercube<Integer>)b, (Hypercube<Integer>)r, op);
+            return (Hypercube<T>)intBinaryOp((Hypercube<Integer>)a, (Hypercube<Integer>)b, (Hypercube<Integer>)r, w, op);
         }
         if (a.getElementType().equals(Long.class)) {
-            return (Hypercube<T>)longBinaryOp((Hypercube<Long>)a, (Hypercube<Long>)b, (Hypercube<Long>)r, op);
+            return (Hypercube<T>)longBinaryOp((Hypercube<Long>)a, (Hypercube<Long>)b, (Hypercube<Long>)r, w, op);
         }
         if (a.getElementType().equals(Boolean.class)) {
-            return (Hypercube<T>)booleanBinaryOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)b, (Hypercube<Boolean>)r, op);
+            return (Hypercube<T>)booleanBinaryOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)b, (Hypercube<Boolean>)r, w, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform binary " + op + " on cubes with element type " + a.getElementType().getSimpleName());
     }
     
     private static <T> Hypercube<T> unaryOp(final Hypercube<T> a, final CubeMath.UnaryOp op) throws NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
@@ -1454,50 +1608,52 @@
         }
         if (a.getElementType().equals(Boolean.class)) {
             return (Hypercube<T>)booleanUnaryOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)r, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform unary " + op + " on a cube with element type " + a.getElementType().getSimpleName());
     }
     
-    private static <T> T associativeOp(final Hypercube<T> a, final CubeMath.AssociativeOp op) throws NullPointerException, UnsupportedOperationException {
+    private static <T> T associativeOp(final Hypercube<T> a, final T i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
+        final Object o = i;
         if (a.getElementType().equals(Double.class)) {
-            return (T)doubleAssociativeOp((Hypercube<Double>)a, op);
+            return (T)doubleAssociativeOp((Hypercube<Double>)a, (Double)o, w, op);
         }
         if (a.getElementType().equals(Float.class)) {
-            return (T)floatAssociativeOp((Hypercube<Float>)a, op);
+            return (T)floatAssociativeOp((Hypercube<Float>)a, (Float)o, w, op);
         }
         if (a.getElementType().equals(Integer.class)) {
-            return (T)intAssociativeOp((Hypercube<Integer>)a, op);
+            return (T)intAssociativeOp((Hypercube<Integer>)a, (Integer)o, w, op);
         }
         if (a.getElementType().equals(Long.class)) {
-            return (T)longAssociativeOp((Hypercube<Long>)a, op);
+            return (T)longAssociativeOp((Hypercube<Long>)a, (Long)o, w, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform associative " + op + " on a cube with element type " + a.getElementType().getSimpleName());
     }
     
-    private static <T> Hypercube<T> associativeOpByAxes(final Hypercube<T> a, final int[] axes, final CubeMath.AssociativeOp op) throws NullPointerException, UnsupportedOperationException {
-        if (a == null) {
-            throw new NullPointerException("Given a null cube, 'a'");
+    private static <T> Hypercube<T> associativeOpByAxes(final Hypercube<T> c, final int[] a, final T i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException, UnsupportedOperationException {
+        if (c == null) {
+            throw new NullPointerException("Given a null cube");
         }
-        if (a.getElementType().equals(Double.class)) {
-            return (Hypercube<T>)doubleAssociativeOpByAxes((Hypercube<Double>)a, axes, op);
+        final Object o = i;
+        if (c.getElementType().equals(Double.class)) {
+            return (Hypercube<T>)doubleAssociativeOpByAxes((Hypercube<Double>)c, a, (Double)o, w, op);
         }
-        if (a.getElementType().equals(Float.class)) {
-            return (Hypercube<T>)floatAssociativeOpByAxes((Hypercube<Float>)a, axes, op);
+        if (c.getElementType().equals(Float.class)) {
+            return (Hypercube<T>)floatAssociativeOpByAxes((Hypercube<Float>)c, a, (Float)o, w, op);
         }
-        if (a.getElementType().equals(Integer.class)) {
-            return (Hypercube<T>)intAssociativeOpByAxes((Hypercube<Integer>)a, axes, op);
+        if (c.getElementType().equals(Integer.class)) {
+            return (Hypercube<T>)intAssociativeOpByAxes((Hypercube<Integer>)c, a, (Integer)o, w, op);
         }
-        if (a.getElementType().equals(Long.class)) {
-            return (Hypercube<T>)longAssociativeOpByAxes((Hypercube<Long>)a, axes, op);
+        if (c.getElementType().equals(Long.class)) {
+            return (Hypercube<T>)longAssociativeOpByAxes((Hypercube<Long>)c, a, (Long)o, w, op);
         }
-        throw new UnsupportedOperationException("Don't know how to perform associative " + op + " on a cube with element type " + a.getElementType().getSimpleName());
+        throw new UnsupportedOperationException("Don't know how to perform associative " + op + " on a cube with element type " + c.getElementType().getSimpleName());
     }
     
     private static <T> Hypercube<Boolean> comparisonOp(final Hypercube<T> a, final Hypercube<T> b, final CubeMath.ComparisonOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
@@ -1551,32 +1707,54 @@
         }
         if (a.getElementType().equals(Boolean.class)) {
             return booleanComparisonOp((Hypercube<Boolean>)a, (Hypercube<Boolean>)b, r, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform comparison " + op + " on cubes with element type " + a.getElementType().getSimpleName());
     }
     
-    private static <T> boolean reductiveLogicOp(final Hypercube<T> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException, UnsupportedOperationException {
+    private static <T> boolean reductiveLogicOp(final Hypercube<T> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException, UnsupportedOperationException {
+        if (a == null) {
+            throw new NullPointerException("Given a null cube, 'a'");
+        }
+        if (a.getElementType().equals(Double.class)) {
+            return doubleReductiveLogicOp((Hypercube<Double>)a, w, op);
+        }
+        if (a.getElementType().equals(Float.class)) {
+            return floatReductiveLogicOp((Hypercube<Float>)a, w, op);
+        }
+        if (a.getElementType().equals(Integer.class)) {
+            return intReductiveLogicOp((Hypercube<Integer>)a, w, op);
+        }
+        if (a.getElementType().equals(Long.class)) {
+            return longReductiveLogicOp((Hypercube<Long>)a, w, op);
+        }
+        if (a.getElementType().equals(Boolean.class)) {
+            return booleanReductiveLogicOp((Hypercube<Boolean>)a, w, op);
+        }
+        throw new UnsupportedOperationException("Don't know how to perform reductive logical " + op + " on a cube with element type " + a.getElementType().getSimpleName());
+    }
+    
+    private static BooleanHypercube reductiveLogicOpByAxes(final Hypercube<?> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (a.getElementType().equals(Double.class)) {
-            return doubleReductiveLogicOp((Hypercube<Double>)a, op);
+            return doubleReductiveLogicOpByAxes((Hypercube<Double>)a, axes, where, op);
         }
         if (a.getElementType().equals(Float.class)) {
-            return floatReductiveLogicOp((Hypercube<Float>)a, op);
+            return floatReductiveLogicOpByAxes((Hypercube<Float>)a, axes, where, op);
         }
         if (a.getElementType().equals(Integer.class)) {
-            return intReductiveLogicOp((Hypercube<Integer>)a, op);
+            return intReductiveLogicOpByAxes((Hypercube<Integer>)a, axes, where, op);
         }
         if (a.getElementType().equals(Long.class)) {
-            return longReductiveLogicOp((Hypercube<Long>)a, op);
+            return longReductiveLogicOpByAxes((Hypercube<Long>)a, axes, where, op);
         }
         if (a.getElementType().equals(Boolean.class)) {
-            return booleanReductiveLogicOp((Hypercube<Boolean>)a, op);
+            return booleanReductiveLogicOpByAxes((Hypercube<Boolean>)a, axes, where, op);
         }
         throw new UnsupportedOperationException("Don't know how to perform reductive logical " + op + " on a cube with element type " + a.getElementType().getSimpleName());
     }
     
     private static <T> Hypercube<T> singleValuedCube(final Hypercube<T> a, final T b) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
@@ -3654,63 +3832,82 @@
         return (Hypercube<Boolean>)a;
     }
     
     public static Hypercube<Boolean> broadcast(final long size, final boolean value) {
         return broadcast((Dimension<?>[])Dimension.of(size), value);
     }
     
-    private static void booleanBinaryOpHelper(final BooleanHypercube da, final BooleanHypercube db, final BooleanHypercube dr, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static void booleanBinaryOpHelper(final BooleanHypercube da, final BooleanHypercube db, final BooleanHypercube dr, final BooleanHypercube dw, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         final boolean[] aa = new boolean[CubeMath.STAGING_SIZE];
         final boolean[] ab = new boolean[CubeMath.STAGING_SIZE];
         final boolean[] ar = new boolean[CubeMath.STAGING_SIZE];
+        final boolean[] aw = (boolean[])((dw == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
             db.toFlattened(i, ab, 0, len);
+            if (dw != null) {
+                dw.toFlattened(i, aw, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$BinaryOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] & ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] & ab[j]);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] | ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] | ab[j]);
+                        }
                     }
                     break;
                 }
                 case 3: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] ^ ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] ^ ab[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported binary operation: " + op);
                 }
             }
-            dr.fromFlattened(ar, 0, i, len);
+            if (aw == null) {
+                dr.fromFlattened(ar, 0, i, len);
+            }
+            else {
+                for (int j = 0; j < len; ++j) {
+                    if (aw[j]) {
+                        dr.setAt(i + (long)j, ar[j]);
+                    }
+                }
+            }
         }
     }
     
-    private static Hypercube<Boolean> booleanBinaryOp(final Hypercube<Boolean> a, final Hypercube<Boolean> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Boolean> booleanBinaryOp(final Hypercube<Boolean> a, final Hypercube<Boolean> b, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
-        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Boolean>)new BooleanBitSetHypercube(a.getDimensions()), op);
+        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Boolean>)new BooleanBitSetHypercube(a.getDimensions()), dw, op);
     }
     
-    private static Hypercube<Boolean> booleanBinaryOp(final Hypercube<Boolean> a, final Hypercube<Boolean> b, final Hypercube<Boolean> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Boolean> booleanBinaryOp(final Hypercube<Boolean> a, final Hypercube<Boolean> b, final Hypercube<Boolean> r, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
@@ -3720,27 +3917,27 @@
             throw new IllegalArgumentException("Given incompatible cubes");
         }
         try {
             final BooleanHypercube da = (BooleanHypercube)a;
             final BooleanHypercube db = (BooleanHypercube)b;
             final BooleanHypercube dr = (BooleanHypercube)r;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                booleanBinaryOpHelper(da, db, dr, op, 0L, a.getSize());
+                booleanBinaryOpHelper(da, db, dr, dw, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                booleanBinaryOpHelper(da, db, dr, op, startIndex, endIndex);
+                                booleanBinaryOpHelper(da, db, dr, dw, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -4047,15 +4244,91 @@
                 }
             }
             return r;
         }
         return r;
     }
     
-    private static boolean booleanReductiveLogicOpHelper(final BooleanHypercube da, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static BooleanHypercube booleanReductiveLogicOpByAxes(final Hypercube<Boolean> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+        final BitSet axesSet = new BitSet(a.getNDim());
+        for (final int axis : axes) {
+            if (axis >= a.getNDim()) {
+                throw new IllegalArgumentException("Axis " + axis + " not in given cube");
+            }
+            if (axesSet.get(axis)) {
+                throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
+            }
+            axesSet.set(axis);
+        }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
+        final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
+        final int dstNDim = a.getNDim() - axesSet.cardinality();
+        Dimension<?>[] dstDims;
+        if (dstNDim > 0) {
+            dstDims = (Dimension<?>[])new Dimension[dstNDim];
+            int i = 0;
+            int j = 0;
+            while (i < a.getNDim()) {
+                if (!axesSet.get(i)) {
+                    dstDims[j++] = srcDims[i];
+                }
+                ++i;
+            }
+        }
+        else {
+            dstDims = (Dimension<?>[])Dimension.of(1L);
+        }
+        final BooleanHypercube dst = (BooleanHypercube)new BooleanBitSetHypercube((Dimension[])dstDims);
+        final long[] indices = new long[a.getNDim()];
+        final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
+        final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
+        for (int k = 0; k < srcAccessors.length; ++k) {
+            if (axesSet.get(k)) {
+                srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
+            }
+        }
+        boolean carry;
+        do {
+            int k = 0;
+            int l = 0;
+            while (k < a.getNDim()) {
+                if (!axesSet.get(k)) {
+                    srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
+                }
+                ++k;
+            }
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final boolean result = booleanReductiveLogicOp((Hypercube<Boolean>)a.slice((Dimension.Accessor[])srcAccessors), whereSlice, op);
+            if (dstNDim > 0) {
+                dst.setObj((Object)Boolean.valueOf(result), (Dimension.Coordinate[])dstAccessors);
+            }
+            else {
+                dst.setObjectAt(0L, (Object)Boolean.valueOf(result));
+            }
+            carry = true;
+            for (int m = 0; m < indices.length && carry; ++m) {
+                if (!axesSet.get(m)) {
+                    if (indices[m] < a.length(m) - 1L) {
+                        final long[] array = indices;
+                        final int n2 = m;
+                        ++array[n2];
+                        carry = false;
+                    }
+                    else {
+                        indices[m] = 0L;
+                    }
+                }
+            }
+        } while (!carry);
+        return dst;
+    }
+    
+    private static boolean booleanReductiveLogicOpHelper(final BooleanHypercube da, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
                 break;
             }
             case 2: {
@@ -4063,39 +4336,47 @@
                 break;
             }
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         final boolean[] aa = new boolean[CubeMath.STAGING_SIZE];
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(i, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r |= aa[j];
+                        if (ww == null || ww[j]) {
+                            r |= aa[j];
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r &= aa[j];
+                        if (ww == null || ww[j]) {
+                            r &= aa[j];
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static boolean booleanReductiveLogicOp(final Hypercube<Boolean> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
+    private static boolean booleanReductiveLogicOp(final Hypercube<Boolean> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
@@ -4108,29 +4389,29 @@
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         try {
             final BooleanHypercube da = (BooleanHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = booleanReductiveLogicOpHelper(da, op, 0L, a.getSize());
+                r = booleanReductiveLogicOpHelper(da, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final boolean[] ar = new boolean[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = booleanReductiveLogicOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = booleanReductiveLogicOpHelper(da, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -4323,25 +4604,28 @@
         final IntegerHypercube cube = (IntegerHypercube)new IntegerArrayHypercube(Dimension.of(length));
         for (long i = 0L; i < length; ++i) {
             cube.setAt(i, (int)(start + step * i));
         }
         return cube;
     }
     
-    private static IntegerHypercube intAssociativeOpByAxes(final Hypercube<Integer> a, final int[] axes, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static IntegerHypercube intAssociativeOpByAxes(final Hypercube<Integer> a, final int[] axes, final Integer initial, final BooleanHypercube where, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         final BitSet axesSet = new BitSet(a.getNDim());
         for (final int axis : axes) {
             if (axis >= a.getNDim()) {
                 throw new IllegalArgumentException("Axis " + axis + " not in given cube");
             }
             if (axesSet.get(axis)) {
                 throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
             }
             axesSet.set(axis);
         }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
         final int dstNDim = a.getNDim() - axesSet.cardinality();
         Dimension<?>[] dstDims;
         if (dstNDim > 0) {
             dstDims = (Dimension<?>[])new Dimension[Math.max(1, dstNDim)];
             int i = 0;
             int j = 0;
@@ -4355,33 +4639,31 @@
         else {
             dstDims = (Dimension<?>[])Dimension.of(1L);
         }
         final IntegerHypercube dst = (IntegerHypercube)new IntegerArrayHypercube((Dimension[])dstDims);
         final long[] indices = new long[a.getNDim()];
         final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
         final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
-        int k = 0;
-        int l = 0;
-        while (k < srcAccessors.length) {
+        for (int k = 0; k < srcAccessors.length; ++k) {
             if (axesSet.get(k)) {
                 srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
             }
-            ++k;
         }
         boolean carry;
         do {
-            k = 0;
-            l = 0;
+            int k = 0;
+            int l = 0;
             while (k < a.getNDim()) {
                 if (!axesSet.get(k)) {
                     srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
                 }
                 ++k;
             }
-            final Integer result = Integer.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Integer>)a.slice((Dimension.Accessor[])srcAccessors), op));
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final Integer result = Integer.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Integer>)a.slice((Dimension.Accessor[])srcAccessors), initial, whereSlice, op));
             if (dstNDim > 0) {
                 dst.setObj((Object)result, (Dimension.Coordinate[])dstAccessors);
             }
             else {
                 dst.setObjectAt(0L, (Object)result);
             }
             carry = true;
@@ -4398,118 +4680,143 @@
                     }
                 }
             }
         } while (!carry);
         return dst;
     }
     
-    private static int intAssociativeOpHelper(final IntegerHypercube da, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static int intAssociativeOpHelper(final IntegerHypercube da, final Integer i, final BooleanHypercube w, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         int r = 0;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0;
-                break;
-            }
-            case 2: {
-                r = 0;
-                break;
-            }
-            case 3: {
-                r = Integer.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Integer.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0;
+                    break;
+                }
+                case 2: {
+                    r = 0;
+                    break;
+                }
+                case 3: {
+                    r = Integer.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Integer.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         final int[] aa = new int[CubeMath.STAGING_SIZE];
-        for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
-            final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
-            da.toFlattened(i, aa, 0, len);
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
+        for (long ii = startIndex; ii < endIndex; ii += CubeMath.STAGING_SIZE) {
+            final int len = (int)Math.min(endIndex - ii, CubeMath.STAGING_SIZE);
+            da.toFlattened(ii, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(ii, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r += aa[j];
+                        if (ww == null || ww[j]) {
+                            r += aa[j];
+                        }
                     }
                     break;
                 }
                 case 3: {
                     for (int j = 0; j < len; ++j) {
-                        r = ((r < aa[j]) ? r : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r = ((r < aa[j]) ? r : aa[j]);
+                        }
                     }
                     break;
                 }
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        r = ((r > aa[j]) ? r : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r = ((r > aa[j]) ? r : aa[j]);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r += (Float.isNaN((float)aa[j]) ? 0 : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r += (Float.isNaN((float)aa[j]) ? 0 : aa[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static Integer intAssociativeOp(final Hypercube<Integer> a, final CubeMath.AssociativeOp op) throws NullPointerException {
+    private static Integer intAssociativeOp(final Hypercube<Integer> a, final Integer i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         int r = 0;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0;
-                break;
-            }
-            case 2: {
-                r = 0;
-                break;
-            }
-            case 3: {
-                r = Integer.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Integer.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0;
+                    break;
+                }
+                case 2: {
+                    r = 0;
+                    break;
+                }
+                case 3: {
+                    r = Integer.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Integer.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         try {
             final IntegerHypercube da = (IntegerHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = intAssociativeOpHelper(da, op, 0L, a.getSize());
+                r = intAssociativeOpHelper(da, i, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final int[] ar = new int[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = intAssociativeOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = intAssociativeOpHelper(da, null, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -4549,52 +4856,54 @@
                     default: {
                         throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                     }
                 }
             }
         }
         catch (final Exception e) {
-            for (long i = 0L, size = a.getSize(); i < size; ++i) {
-                final Integer va = (Integer)a.getObjectAt(i);
-                if (va != null) {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r += va;
-                            break;
-                        }
-                        case 3: {
-                            r = ((r < va) ? r : ((int)va));
-                            break;
-                        }
-                        case 4: {
-                            r = ((r > va) ? r : ((int)va));
-                            break;
-                        }
-                        case 2: {
-                            r += (Float.isNaN((float)(int)va) ? 0 : ((int)va));
-                            break;
-                        }
-                        default: {
-                            throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+            for (long ii = 0L, size = a.getSize(); ii < size; ++ii) {
+                if (w == null || w.getAt(ii)) {
+                    final Integer va = (Integer)a.getObjectAt(ii);
+                    if (va != null) {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r += va;
+                                break;
+                            }
+                            case 3: {
+                                r = ((r < va) ? r : ((int)va));
+                                break;
+                            }
+                            case 4: {
+                                r = ((r > va) ? r : ((int)va));
+                                break;
+                            }
+                            case 2: {
+                                r += (Float.isNaN((float)(int)va) ? 0 : ((int)va));
+                                break;
+                            }
+                            default: {
+                                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                            }
                         }
                     }
-                }
-                else {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r = Integer.valueOf(0);
-                            break;
-                        }
-                        case 3: {
-                            r = Integer.valueOf(0);
-                            break;
-                        }
-                        case 4: {
-                            r = Integer.valueOf(0);
-                            break;
+                    else {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r = Integer.valueOf(0);
+                                break;
+                            }
+                            case 3: {
+                                r = Integer.valueOf(0);
+                                break;
+                            }
+                            case 4: {
+                                r = Integer.valueOf(0);
+                                break;
+                            }
                         }
                     }
                 }
             }
             return Integer.valueOf(r);
         }
         return Integer.valueOf(r);
@@ -4610,111 +4919,146 @@
         return (Hypercube<Integer>)a;
     }
     
     public static Hypercube<Integer> broadcast(final long size, final int value) {
         return broadcast((Dimension<?>[])Dimension.of(size), value);
     }
     
-    private static void intBinaryOpHelper(final IntegerHypercube da, final IntegerHypercube db, final IntegerHypercube dr, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static void intBinaryOpHelper(final IntegerHypercube da, final IntegerHypercube db, final IntegerHypercube dr, final BooleanHypercube dw, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         final int[] aa = new int[CubeMath.STAGING_SIZE];
         final int[] ab = new int[CubeMath.STAGING_SIZE];
         final int[] ar = new int[CubeMath.STAGING_SIZE];
+        final boolean[] aw = (boolean[])((dw == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
             db.toFlattened(i, ab, 0, len);
+            if (dw != null) {
+                dw.toFlattened(i, aw, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$BinaryOp[op.ordinal()]) {
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] + ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] + ab[j];
+                        }
                     }
                     break;
                 }
                 case 5: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] - ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] - ab[j];
+                        }
                     }
                     break;
                 }
                 case 6: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] * ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] * ab[j];
+                        }
                     }
                     break;
                 }
                 case 7: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] / ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] / ab[j];
+                        }
                     }
                     break;
                 }
                 case 8: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] % ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] % ab[j];
+                        }
                     }
                     break;
                 }
                 case 9: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.min(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.min(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 10: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.max(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.max(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 11: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (int)Math.pow(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (int)Math.pow(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] & ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] & ab[j]);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] | ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] | ab[j]);
+                        }
                     }
                     break;
                 }
                 case 3: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] ^ ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] ^ ab[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported binary operation: " + op);
                 }
             }
-            dr.fromFlattened(ar, 0, i, len);
+            if (aw == null) {
+                dr.fromFlattened(ar, 0, i, len);
+            }
+            else {
+                for (int j = 0; j < len; ++j) {
+                    if (aw[j]) {
+                        dr.setAt(i + (long)j, ar[j]);
+                    }
+                }
+            }
         }
     }
     
-    private static Hypercube<Integer> intBinaryOp(final Hypercube<Integer> a, final Hypercube<Integer> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Integer> intBinaryOp(final Hypercube<Integer> a, final Hypercube<Integer> b, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
-        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Integer>)new IntegerArrayHypercube(a.getDimensions()), op);
+        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Integer>)new IntegerArrayHypercube(a.getDimensions()), dw, op);
     }
     
-    private static Hypercube<Integer> intBinaryOp(final Hypercube<Integer> a, final Hypercube<Integer> b, final Hypercube<Integer> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Integer> intBinaryOp(final Hypercube<Integer> a, final Hypercube<Integer> b, final Hypercube<Integer> r, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
@@ -4724,27 +5068,27 @@
             throw new IllegalArgumentException("Given incompatible cubes");
         }
         try {
             final IntegerHypercube da = (IntegerHypercube)a;
             final IntegerHypercube db = (IntegerHypercube)b;
             final IntegerHypercube dr = (IntegerHypercube)r;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                intBinaryOpHelper(da, db, dr, op, 0L, a.getSize());
+                intBinaryOpHelper(da, db, dr, dw, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                intBinaryOpHelper(da, db, dr, op, startIndex, endIndex);
+                                intBinaryOpHelper(da, db, dr, dw, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -5101,15 +5445,91 @@
                 }
             }
             return r;
         }
         return r;
     }
     
-    private static boolean intReductiveLogicOpHelper(final IntegerHypercube da, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static BooleanHypercube intReductiveLogicOpByAxes(final Hypercube<Integer> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+        final BitSet axesSet = new BitSet(a.getNDim());
+        for (final int axis : axes) {
+            if (axis >= a.getNDim()) {
+                throw new IllegalArgumentException("Axis " + axis + " not in given cube");
+            }
+            if (axesSet.get(axis)) {
+                throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
+            }
+            axesSet.set(axis);
+        }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
+        final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
+        final int dstNDim = a.getNDim() - axesSet.cardinality();
+        Dimension<?>[] dstDims;
+        if (dstNDim > 0) {
+            dstDims = (Dimension<?>[])new Dimension[dstNDim];
+            int i = 0;
+            int j = 0;
+            while (i < a.getNDim()) {
+                if (!axesSet.get(i)) {
+                    dstDims[j++] = srcDims[i];
+                }
+                ++i;
+            }
+        }
+        else {
+            dstDims = (Dimension<?>[])Dimension.of(1L);
+        }
+        final BooleanHypercube dst = (BooleanHypercube)new BooleanBitSetHypercube((Dimension[])dstDims);
+        final long[] indices = new long[a.getNDim()];
+        final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
+        final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
+        for (int k = 0; k < srcAccessors.length; ++k) {
+            if (axesSet.get(k)) {
+                srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
+            }
+        }
+        boolean carry;
+        do {
+            int k = 0;
+            int l = 0;
+            while (k < a.getNDim()) {
+                if (!axesSet.get(k)) {
+                    srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
+                }
+                ++k;
+            }
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final boolean result = intReductiveLogicOp((Hypercube<Integer>)a.slice((Dimension.Accessor[])srcAccessors), whereSlice, op);
+            if (dstNDim > 0) {
+                dst.setObj((Object)Boolean.valueOf(result), (Dimension.Coordinate[])dstAccessors);
+            }
+            else {
+                dst.setObjectAt(0L, (Object)Boolean.valueOf(result));
+            }
+            carry = true;
+            for (int m = 0; m < indices.length && carry; ++m) {
+                if (!axesSet.get(m)) {
+                    if (indices[m] < a.length(m) - 1L) {
+                        final long[] array = indices;
+                        final int n2 = m;
+                        ++array[n2];
+                        carry = false;
+                    }
+                    else {
+                        indices[m] = 0L;
+                    }
+                }
+            }
+        } while (!carry);
+        return dst;
+    }
+    
+    private static boolean intReductiveLogicOpHelper(final IntegerHypercube da, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
                 break;
             }
             case 2: {
@@ -5117,39 +5537,47 @@
                 break;
             }
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         final int[] aa = new int[CubeMath.STAGING_SIZE];
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(i, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r |= (aa[j] != 0);
+                        if (ww == null || ww[j]) {
+                            r |= (aa[j] != 0);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r &= (aa[j] != 0);
+                        if (ww == null || ww[j]) {
+                            r &= (aa[j] != 0);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static boolean intReductiveLogicOp(final Hypercube<Integer> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
+    private static boolean intReductiveLogicOp(final Hypercube<Integer> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
@@ -5162,29 +5590,29 @@
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         try {
             final IntegerHypercube da = (IntegerHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = intReductiveLogicOpHelper(da, op, 0L, a.getSize());
+                r = intReductiveLogicOpHelper(da, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final boolean[] ar = new boolean[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = intReductiveLogicOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = intReductiveLogicOpHelper(da, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -5377,25 +5805,28 @@
         final LongHypercube cube = (LongHypercube)new LongArrayHypercube(Dimension.of(length));
         for (long i = 0L; i < length; ++i) {
             cube.setAt(i, start + step * i);
         }
         return cube;
     }
     
-    private static LongHypercube longAssociativeOpByAxes(final Hypercube<Long> a, final int[] axes, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static LongHypercube longAssociativeOpByAxes(final Hypercube<Long> a, final int[] axes, final Long initial, final BooleanHypercube where, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         final BitSet axesSet = new BitSet(a.getNDim());
         for (final int axis : axes) {
             if (axis >= a.getNDim()) {
                 throw new IllegalArgumentException("Axis " + axis + " not in given cube");
             }
             if (axesSet.get(axis)) {
                 throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
             }
             axesSet.set(axis);
         }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
         final int dstNDim = a.getNDim() - axesSet.cardinality();
         Dimension<?>[] dstDims;
         if (dstNDim > 0) {
             dstDims = (Dimension<?>[])new Dimension[Math.max(1, dstNDim)];
             int i = 0;
             int j = 0;
@@ -5409,33 +5840,31 @@
         else {
             dstDims = (Dimension<?>[])Dimension.of(1L);
         }
         final LongHypercube dst = (LongHypercube)new LongArrayHypercube((Dimension[])dstDims);
         final long[] indices = new long[a.getNDim()];
         final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
         final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
-        int k = 0;
-        int l = 0;
-        while (k < srcAccessors.length) {
+        for (int k = 0; k < srcAccessors.length; ++k) {
             if (axesSet.get(k)) {
                 srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
             }
-            ++k;
         }
         boolean carry;
         do {
-            k = 0;
-            l = 0;
+            int k = 0;
+            int l = 0;
             while (k < a.getNDim()) {
                 if (!axesSet.get(k)) {
                     srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
                 }
                 ++k;
             }
-            final Long result = Long.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Long>)a.slice((Dimension.Accessor[])srcAccessors), op));
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final Long result = Long.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Long>)a.slice((Dimension.Accessor[])srcAccessors), initial, whereSlice, op));
             if (dstNDim > 0) {
                 dst.setObj((Object)result, (Dimension.Coordinate[])dstAccessors);
             }
             else {
                 dst.setObjectAt(0L, (Object)result);
             }
             carry = true;
@@ -5452,118 +5881,143 @@
                     }
                 }
             }
         } while (!carry);
         return dst;
     }
     
-    private static long longAssociativeOpHelper(final LongHypercube da, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static long longAssociativeOpHelper(final LongHypercube da, final Long i, final BooleanHypercube w, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         long r = 0L;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0L;
-                break;
-            }
-            case 2: {
-                r = 0L;
-                break;
-            }
-            case 3: {
-                r = Long.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Long.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0L;
+                    break;
+                }
+                case 2: {
+                    r = 0L;
+                    break;
+                }
+                case 3: {
+                    r = Long.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Long.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         final long[] aa = new long[CubeMath.STAGING_SIZE];
-        for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
-            final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
-            da.toFlattened(i, aa, 0, len);
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
+        for (long ii = startIndex; ii < endIndex; ii += CubeMath.STAGING_SIZE) {
+            final int len = (int)Math.min(endIndex - ii, CubeMath.STAGING_SIZE);
+            da.toFlattened(ii, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(ii, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r += aa[j];
+                        if (ww == null || ww[j]) {
+                            r += aa[j];
+                        }
                     }
                     break;
                 }
                 case 3: {
                     for (int j = 0; j < len; ++j) {
-                        r = ((r < aa[j]) ? r : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r = ((r < aa[j]) ? r : aa[j]);
+                        }
                     }
                     break;
                 }
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        r = ((r > aa[j]) ? r : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r = ((r > aa[j]) ? r : aa[j]);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r += (Double.isNaN((double)aa[j]) ? 0L : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r += (Double.isNaN((double)aa[j]) ? 0L : aa[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static Long longAssociativeOp(final Hypercube<Long> a, final CubeMath.AssociativeOp op) throws NullPointerException {
+    private static Long longAssociativeOp(final Hypercube<Long> a, final Long i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         long r = 0L;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0L;
-                break;
-            }
-            case 2: {
-                r = 0L;
-                break;
-            }
-            case 3: {
-                r = Long.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Long.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0L;
+                    break;
+                }
+                case 2: {
+                    r = 0L;
+                    break;
+                }
+                case 3: {
+                    r = Long.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Long.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         try {
             final LongHypercube da = (LongHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = longAssociativeOpHelper(da, op, 0L, a.getSize());
+                r = longAssociativeOpHelper(da, i, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final long[] ar = new long[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = longAssociativeOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = longAssociativeOpHelper(da, null, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -5603,52 +6057,54 @@
                     default: {
                         throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                     }
                 }
             }
         }
         catch (final Exception e) {
-            for (long i = 0L, size = a.getSize(); i < size; ++i) {
-                final Long va = (Long)a.getObjectAt(i);
-                if (va != null) {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r += va;
-                            break;
-                        }
-                        case 3: {
-                            r = ((r < va) ? r : ((long)va));
-                            break;
-                        }
-                        case 4: {
-                            r = ((r > va) ? r : ((long)va));
-                            break;
-                        }
-                        case 2: {
-                            r += (Double.isNaN((double)(long)va) ? 0L : ((long)va));
-                            break;
-                        }
-                        default: {
-                            throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+            for (long ii = 0L, size = a.getSize(); ii < size; ++ii) {
+                if (w == null || w.getAt(ii)) {
+                    final Long va = (Long)a.getObjectAt(ii);
+                    if (va != null) {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r += va;
+                                break;
+                            }
+                            case 3: {
+                                r = ((r < va) ? r : ((long)va));
+                                break;
+                            }
+                            case 4: {
+                                r = ((r > va) ? r : ((long)va));
+                                break;
+                            }
+                            case 2: {
+                                r += (Double.isNaN((double)(long)va) ? 0L : ((long)va));
+                                break;
+                            }
+                            default: {
+                                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                            }
                         }
                     }
-                }
-                else {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r = Long.valueOf(0L);
-                            break;
-                        }
-                        case 3: {
-                            r = Long.valueOf(0L);
-                            break;
-                        }
-                        case 4: {
-                            r = Long.valueOf(0L);
-                            break;
+                    else {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r = Long.valueOf(0L);
+                                break;
+                            }
+                            case 3: {
+                                r = Long.valueOf(0L);
+                                break;
+                            }
+                            case 4: {
+                                r = Long.valueOf(0L);
+                                break;
+                            }
                         }
                     }
                 }
             }
             return Long.valueOf(r);
         }
         return Long.valueOf(r);
@@ -5664,111 +6120,146 @@
         return (Hypercube<Long>)a;
     }
     
     public static Hypercube<Long> broadcast(final long size, final long value) {
         return broadcast((Dimension<?>[])Dimension.of(size), value);
     }
     
-    private static void longBinaryOpHelper(final LongHypercube da, final LongHypercube db, final LongHypercube dr, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static void longBinaryOpHelper(final LongHypercube da, final LongHypercube db, final LongHypercube dr, final BooleanHypercube dw, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         final long[] aa = new long[CubeMath.STAGING_SIZE];
         final long[] ab = new long[CubeMath.STAGING_SIZE];
         final long[] ar = new long[CubeMath.STAGING_SIZE];
+        final boolean[] aw = (boolean[])((dw == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
             db.toFlattened(i, ab, 0, len);
+            if (dw != null) {
+                dw.toFlattened(i, aw, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$BinaryOp[op.ordinal()]) {
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] + ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] + ab[j];
+                        }
                     }
                     break;
                 }
                 case 5: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] - ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] - ab[j];
+                        }
                     }
                     break;
                 }
                 case 6: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] * ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] * ab[j];
+                        }
                     }
                     break;
                 }
                 case 7: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] / ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] / ab[j];
+                        }
                     }
                     break;
                 }
                 case 8: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] % ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] % ab[j];
+                        }
                     }
                     break;
                 }
                 case 9: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.min(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.min(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 10: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.max(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.max(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 11: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (long)Math.pow((double)aa[j], (double)ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (long)Math.pow((double)aa[j], (double)ab[j]);
+                        }
                     }
                     break;
                 }
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] & ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] & ab[j]);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] | ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] | ab[j]);
+                        }
                     }
                     break;
                 }
                 case 3: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (aa[j] ^ ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (aa[j] ^ ab[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported binary operation: " + op);
                 }
             }
-            dr.fromFlattened(ar, 0, i, len);
+            if (aw == null) {
+                dr.fromFlattened(ar, 0, i, len);
+            }
+            else {
+                for (int j = 0; j < len; ++j) {
+                    if (aw[j]) {
+                        dr.setAt(i + (long)j, ar[j]);
+                    }
+                }
+            }
         }
     }
     
-    private static Hypercube<Long> longBinaryOp(final Hypercube<Long> a, final Hypercube<Long> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Long> longBinaryOp(final Hypercube<Long> a, final Hypercube<Long> b, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
-        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Long>)new LongArrayHypercube(a.getDimensions()), op);
+        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Long>)new LongArrayHypercube(a.getDimensions()), dw, op);
     }
     
-    private static Hypercube<Long> longBinaryOp(final Hypercube<Long> a, final Hypercube<Long> b, final Hypercube<Long> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Long> longBinaryOp(final Hypercube<Long> a, final Hypercube<Long> b, final Hypercube<Long> r, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
@@ -5778,27 +6269,27 @@
             throw new IllegalArgumentException("Given incompatible cubes");
         }
         try {
             final LongHypercube da = (LongHypercube)a;
             final LongHypercube db = (LongHypercube)b;
             final LongHypercube dr = (LongHypercube)r;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                longBinaryOpHelper(da, db, dr, op, 0L, a.getSize());
+                longBinaryOpHelper(da, db, dr, dw, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                longBinaryOpHelper(da, db, dr, op, startIndex, endIndex);
+                                longBinaryOpHelper(da, db, dr, dw, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -6155,15 +6646,91 @@
                 }
             }
             return r;
         }
         return r;
     }
     
-    private static boolean longReductiveLogicOpHelper(final LongHypercube da, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static BooleanHypercube longReductiveLogicOpByAxes(final Hypercube<Long> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+        final BitSet axesSet = new BitSet(a.getNDim());
+        for (final int axis : axes) {
+            if (axis >= a.getNDim()) {
+                throw new IllegalArgumentException("Axis " + axis + " not in given cube");
+            }
+            if (axesSet.get(axis)) {
+                throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
+            }
+            axesSet.set(axis);
+        }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
+        final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
+        final int dstNDim = a.getNDim() - axesSet.cardinality();
+        Dimension<?>[] dstDims;
+        if (dstNDim > 0) {
+            dstDims = (Dimension<?>[])new Dimension[dstNDim];
+            int i = 0;
+            int j = 0;
+            while (i < a.getNDim()) {
+                if (!axesSet.get(i)) {
+                    dstDims[j++] = srcDims[i];
+                }
+                ++i;
+            }
+        }
+        else {
+            dstDims = (Dimension<?>[])Dimension.of(1L);
+        }
+        final BooleanHypercube dst = (BooleanHypercube)new BooleanBitSetHypercube((Dimension[])dstDims);
+        final long[] indices = new long[a.getNDim()];
+        final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
+        final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
+        for (int k = 0; k < srcAccessors.length; ++k) {
+            if (axesSet.get(k)) {
+                srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
+            }
+        }
+        boolean carry;
+        do {
+            int k = 0;
+            int l = 0;
+            while (k < a.getNDim()) {
+                if (!axesSet.get(k)) {
+                    srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
+                }
+                ++k;
+            }
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final boolean result = longReductiveLogicOp((Hypercube<Long>)a.slice((Dimension.Accessor[])srcAccessors), whereSlice, op);
+            if (dstNDim > 0) {
+                dst.setObj((Object)Boolean.valueOf(result), (Dimension.Coordinate[])dstAccessors);
+            }
+            else {
+                dst.setObjectAt(0L, (Object)Boolean.valueOf(result));
+            }
+            carry = true;
+            for (int m = 0; m < indices.length && carry; ++m) {
+                if (!axesSet.get(m)) {
+                    if (indices[m] < a.length(m) - 1L) {
+                        final long[] array = indices;
+                        final int n2 = m;
+                        ++array[n2];
+                        carry = false;
+                    }
+                    else {
+                        indices[m] = 0L;
+                    }
+                }
+            }
+        } while (!carry);
+        return dst;
+    }
+    
+    private static boolean longReductiveLogicOpHelper(final LongHypercube da, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
                 break;
             }
             case 2: {
@@ -6171,39 +6738,47 @@
                 break;
             }
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         final long[] aa = new long[CubeMath.STAGING_SIZE];
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(i, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r |= (aa[j] != 0L);
+                        if (ww == null || ww[j]) {
+                            r |= (aa[j] != 0L);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r &= (aa[j] != 0L);
+                        if (ww == null || ww[j]) {
+                            r &= (aa[j] != 0L);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static boolean longReductiveLogicOp(final Hypercube<Long> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
+    private static boolean longReductiveLogicOp(final Hypercube<Long> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
@@ -6216,29 +6791,29 @@
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         try {
             final LongHypercube da = (LongHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = longReductiveLogicOpHelper(da, op, 0L, a.getSize());
+                r = longReductiveLogicOpHelper(da, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final boolean[] ar = new boolean[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = longReductiveLogicOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = longReductiveLogicOpHelper(da, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -6431,25 +7006,28 @@
         final FloatHypercube cube = (FloatHypercube)new FloatArrayHypercube(Dimension.of(length));
         for (long i = 0L; i < length; ++i) {
             cube.setAt(i, start + step * i);
         }
         return cube;
     }
     
-    private static FloatHypercube floatAssociativeOpByAxes(final Hypercube<Float> a, final int[] axes, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static FloatHypercube floatAssociativeOpByAxes(final Hypercube<Float> a, final int[] axes, final Float initial, final BooleanHypercube where, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         final BitSet axesSet = new BitSet(a.getNDim());
         for (final int axis : axes) {
             if (axis >= a.getNDim()) {
                 throw new IllegalArgumentException("Axis " + axis + " not in given cube");
             }
             if (axesSet.get(axis)) {
                 throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
             }
             axesSet.set(axis);
         }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
         final int dstNDim = a.getNDim() - axesSet.cardinality();
         Dimension<?>[] dstDims;
         if (dstNDim > 0) {
             dstDims = (Dimension<?>[])new Dimension[Math.max(1, dstNDim)];
             int i = 0;
             int j = 0;
@@ -6463,33 +7041,31 @@
         else {
             dstDims = (Dimension<?>[])Dimension.of(1L);
         }
         final FloatHypercube dst = (FloatHypercube)new FloatArrayHypercube((Dimension[])dstDims);
         final long[] indices = new long[a.getNDim()];
         final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
         final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
-        int k = 0;
-        int l = 0;
-        while (k < srcAccessors.length) {
+        for (int k = 0; k < srcAccessors.length; ++k) {
             if (axesSet.get(k)) {
                 srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
             }
-            ++k;
         }
         boolean carry;
         do {
-            k = 0;
-            l = 0;
+            int k = 0;
+            int l = 0;
             while (k < a.getNDim()) {
                 if (!axesSet.get(k)) {
                     srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
                 }
                 ++k;
             }
-            final Float result = Float.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Float>)a.slice((Dimension.Accessor[])srcAccessors), op));
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final Float result = Float.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Float>)a.slice((Dimension.Accessor[])srcAccessors), initial, whereSlice, op));
             if (dstNDim > 0) {
                 dst.setObj((Object)result, (Dimension.Coordinate[])dstAccessors);
             }
             else {
                 dst.setObjectAt(0L, (Object)result);
             }
             carry = true;
@@ -6506,112 +7082,143 @@
                     }
                 }
             }
         } while (!carry);
         return dst;
     }
     
-    private static float floatAssociativeOpHelper(final FloatHypercube da, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static float floatAssociativeOpHelper(final FloatHypercube da, final Float i, final BooleanHypercube w, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         float r = 0.0f;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0.0f;
-                break;
-            }
-            case 2: {
-                r = 0.0f;
-                break;
-            }
-            case 3: {
-                r = Float.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Float.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0.0f;
+                    break;
+                }
+                case 2: {
+                    r = 0.0f;
+                    break;
+                }
+                case 3: {
+                    r = Float.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Float.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         final float[] aa = new float[CubeMath.STAGING_SIZE];
-        for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
-            final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
-            da.toFlattened(i, aa, 0, len);
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
+        for (long ii = startIndex; ii < endIndex; ii += CubeMath.STAGING_SIZE) {
+            final int len = (int)Math.min(endIndex - ii, CubeMath.STAGING_SIZE);
+            da.toFlattened(ii, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(ii, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
                 case 1: {
-                    for (int j = 0; j < len && !Float.isNaN(r); r += aa[j], ++j) {}
+                    for (int j = 0; j < len && !Float.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r += aa[j];
+                        }
+                    }
                     break;
                 }
                 case 3: {
-                    for (int j = 0; j < len && !Float.isNaN(r); r = ((r < aa[j]) ? r : aa[j]), ++j) {}
+                    for (int j = 0; j < len && !Float.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r = ((r < aa[j]) ? r : aa[j]);
+                        }
+                    }
                     break;
                 }
                 case 4: {
-                    for (int j = 0; j < len && !Float.isNaN(r); r = ((r > aa[j]) ? r : aa[j]), ++j) {}
+                    for (int j = 0; j < len && !Float.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r = ((r > aa[j]) ? r : aa[j]);
+                        }
+                    }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r += (Float.isNaN(aa[j]) ? 0.0f : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r += (Float.isNaN(aa[j]) ? 0.0f : aa[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static Float floatAssociativeOp(final Hypercube<Float> a, final CubeMath.AssociativeOp op) throws NullPointerException {
+    private static Float floatAssociativeOp(final Hypercube<Float> a, final Float i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         float r = 0.0f;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0.0f;
-                break;
-            }
-            case 2: {
-                r = 0.0f;
-                break;
-            }
-            case 3: {
-                r = Float.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Float.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0.0f;
+                    break;
+                }
+                case 2: {
+                    r = 0.0f;
+                    break;
+                }
+                case 3: {
+                    r = Float.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Float.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         try {
             final FloatHypercube da = (FloatHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = floatAssociativeOpHelper(da, op, 0L, a.getSize());
+                r = floatAssociativeOpHelper(da, i, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final float[] ar = new float[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = floatAssociativeOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = floatAssociativeOpHelper(da, null, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -6645,52 +7252,54 @@
                     default: {
                         throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                     }
                 }
             }
         }
         catch (final Exception e) {
-            for (long i = 0L, size = a.getSize(); i < size && !Float.isNaN(r); ++i) {
-                final Float va = (Float)a.getObjectAt(i);
-                if (va != null) {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r += va;
-                            break;
-                        }
-                        case 3: {
-                            r = ((r < va) ? r : ((float)va));
-                            break;
-                        }
-                        case 4: {
-                            r = ((r > va) ? r : ((float)va));
-                            break;
-                        }
-                        case 2: {
-                            r += (Float.isNaN(va) ? 0.0f : ((float)va));
-                            break;
-                        }
-                        default: {
-                            throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+            for (long ii = 0L, size = a.getSize(); ii < size && !Float.isNaN(r); ++ii) {
+                if (w == null || w.getAt(ii)) {
+                    final Float va = (Float)a.getObjectAt(ii);
+                    if (va != null) {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r += va;
+                                break;
+                            }
+                            case 3: {
+                                r = ((r < va) ? r : ((float)va));
+                                break;
+                            }
+                            case 4: {
+                                r = ((r > va) ? r : ((float)va));
+                                break;
+                            }
+                            case 2: {
+                                r += (Float.isNaN(va) ? 0.0f : ((float)va));
+                                break;
+                            }
+                            default: {
+                                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                            }
                         }
                     }
-                }
-                else {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r = Float.valueOf(Float.NaN);
-                            break;
-                        }
-                        case 3: {
-                            r = Float.valueOf(Float.NaN);
-                            break;
-                        }
-                        case 4: {
-                            r = Float.valueOf(Float.NaN);
-                            break;
+                    else {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r = Float.valueOf(Float.NaN);
+                                break;
+                            }
+                            case 3: {
+                                r = Float.valueOf(Float.NaN);
+                                break;
+                            }
+                            case 4: {
+                                r = Float.valueOf(Float.NaN);
+                                break;
+                            }
                         }
                     }
                 }
             }
             return Float.valueOf(r);
         }
         return Float.valueOf(r);
@@ -6706,93 +7315,122 @@
         return (Hypercube<Float>)a;
     }
     
     public static Hypercube<Float> broadcast(final long size, final float value) {
         return broadcast((Dimension<?>[])Dimension.of(size), value);
     }
     
-    private static void floatBinaryOpHelper(final FloatHypercube da, final FloatHypercube db, final FloatHypercube dr, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static void floatBinaryOpHelper(final FloatHypercube da, final FloatHypercube db, final FloatHypercube dr, final BooleanHypercube dw, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         final float[] aa = new float[CubeMath.STAGING_SIZE];
         final float[] ab = new float[CubeMath.STAGING_SIZE];
         final float[] ar = new float[CubeMath.STAGING_SIZE];
+        final boolean[] aw = (boolean[])((dw == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
             db.toFlattened(i, ab, 0, len);
+            if (dw != null) {
+                dw.toFlattened(i, aw, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$BinaryOp[op.ordinal()]) {
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] + ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] + ab[j];
+                        }
                     }
                     break;
                 }
                 case 5: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] - ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] - ab[j];
+                        }
                     }
                     break;
                 }
                 case 6: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] * ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] * ab[j];
+                        }
                     }
                     break;
                 }
                 case 7: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] / ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] / ab[j];
+                        }
                     }
                     break;
                 }
                 case 8: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] % ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] % ab[j];
+                        }
                     }
                     break;
                 }
                 case 9: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.min(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.min(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 10: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.max(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.max(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 11: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = (float)Math.pow(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = (float)Math.pow(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported binary operation: " + op);
                 }
             }
-            dr.fromFlattened(ar, 0, i, len);
+            if (aw == null) {
+                dr.fromFlattened(ar, 0, i, len);
+            }
+            else {
+                for (int j = 0; j < len; ++j) {
+                    if (aw[j]) {
+                        dr.setAt(i + (long)j, ar[j]);
+                    }
+                }
+            }
         }
     }
     
-    private static Hypercube<Float> floatBinaryOp(final Hypercube<Float> a, final Hypercube<Float> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Float> floatBinaryOp(final Hypercube<Float> a, final Hypercube<Float> b, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
-        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Float>)new FloatArrayHypercube(a.getDimensions()), op);
+        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Float>)new FloatArrayHypercube(a.getDimensions()), dw, op);
     }
     
-    private static Hypercube<Float> floatBinaryOp(final Hypercube<Float> a, final Hypercube<Float> b, final Hypercube<Float> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Float> floatBinaryOp(final Hypercube<Float> a, final Hypercube<Float> b, final Hypercube<Float> r, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
@@ -6802,27 +7440,27 @@
             throw new IllegalArgumentException("Given incompatible cubes");
         }
         try {
             final FloatHypercube da = (FloatHypercube)a;
             final FloatHypercube db = (FloatHypercube)b;
             final FloatHypercube dr = (FloatHypercube)r;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                floatBinaryOpHelper(da, db, dr, op, 0L, a.getSize());
+                floatBinaryOpHelper(da, db, dr, dw, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                floatBinaryOpHelper(da, db, dr, op, startIndex, endIndex);
+                                floatBinaryOpHelper(da, db, dr, dw, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -7277,15 +7915,91 @@
                 }
             }
             return r;
         }
         return r;
     }
     
-    private static boolean floatReductiveLogicOpHelper(final FloatHypercube da, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static BooleanHypercube floatReductiveLogicOpByAxes(final Hypercube<Float> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+        final BitSet axesSet = new BitSet(a.getNDim());
+        for (final int axis : axes) {
+            if (axis >= a.getNDim()) {
+                throw new IllegalArgumentException("Axis " + axis + " not in given cube");
+            }
+            if (axesSet.get(axis)) {
+                throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
+            }
+            axesSet.set(axis);
+        }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
+        final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
+        final int dstNDim = a.getNDim() - axesSet.cardinality();
+        Dimension<?>[] dstDims;
+        if (dstNDim > 0) {
+            dstDims = (Dimension<?>[])new Dimension[dstNDim];
+            int i = 0;
+            int j = 0;
+            while (i < a.getNDim()) {
+                if (!axesSet.get(i)) {
+                    dstDims[j++] = srcDims[i];
+                }
+                ++i;
+            }
+        }
+        else {
+            dstDims = (Dimension<?>[])Dimension.of(1L);
+        }
+        final BooleanHypercube dst = (BooleanHypercube)new BooleanBitSetHypercube((Dimension[])dstDims);
+        final long[] indices = new long[a.getNDim()];
+        final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
+        final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
+        for (int k = 0; k < srcAccessors.length; ++k) {
+            if (axesSet.get(k)) {
+                srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
+            }
+        }
+        boolean carry;
+        do {
+            int k = 0;
+            int l = 0;
+            while (k < a.getNDim()) {
+                if (!axesSet.get(k)) {
+                    srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
+                }
+                ++k;
+            }
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final boolean result = floatReductiveLogicOp((Hypercube<Float>)a.slice((Dimension.Accessor[])srcAccessors), whereSlice, op);
+            if (dstNDim > 0) {
+                dst.setObj((Object)Boolean.valueOf(result), (Dimension.Coordinate[])dstAccessors);
+            }
+            else {
+                dst.setObjectAt(0L, (Object)Boolean.valueOf(result));
+            }
+            carry = true;
+            for (int m = 0; m < indices.length && carry; ++m) {
+                if (!axesSet.get(m)) {
+                    if (indices[m] < a.length(m) - 1L) {
+                        final long[] array = indices;
+                        final int n2 = m;
+                        ++array[n2];
+                        carry = false;
+                    }
+                    else {
+                        indices[m] = 0L;
+                    }
+                }
+            }
+        } while (!carry);
+        return dst;
+    }
+    
+    private static boolean floatReductiveLogicOpHelper(final FloatHypercube da, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
                 break;
             }
             case 2: {
@@ -7293,39 +8007,47 @@
                 break;
             }
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         final float[] aa = new float[CubeMath.STAGING_SIZE];
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(i, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r |= (aa[j] != 0.0f);
+                        if (ww == null || ww[j]) {
+                            r |= (aa[j] != 0.0f);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r &= (aa[j] != 0.0f);
+                        if (ww == null || ww[j]) {
+                            r &= (aa[j] != 0.0f);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static boolean floatReductiveLogicOp(final Hypercube<Float> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
+    private static boolean floatReductiveLogicOp(final Hypercube<Float> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
@@ -7338,29 +8060,29 @@
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         try {
             final FloatHypercube da = (FloatHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = floatReductiveLogicOpHelper(da, op, 0L, a.getSize());
+                r = floatReductiveLogicOpHelper(da, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final boolean[] ar = new boolean[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = floatReductiveLogicOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = floatReductiveLogicOpHelper(da, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -7553,25 +8275,28 @@
         final DoubleHypercube cube = (DoubleHypercube)new DoubleArrayHypercube(Dimension.of(length));
         for (long i = 0L; i < length; ++i) {
             cube.setAt(i, start + step * i);
         }
         return cube;
     }
     
-    private static DoubleHypercube doubleAssociativeOpByAxes(final Hypercube<Double> a, final int[] axes, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+    private static DoubleHypercube doubleAssociativeOpByAxes(final Hypercube<Double> a, final int[] axes, final Double initial, final BooleanHypercube where, final CubeMath.AssociativeOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
         final BitSet axesSet = new BitSet(a.getNDim());
         for (final int axis : axes) {
             if (axis >= a.getNDim()) {
                 throw new IllegalArgumentException("Axis " + axis + " not in given cube");
             }
             if (axesSet.get(axis)) {
                 throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
             }
             axesSet.set(axis);
         }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
         final int dstNDim = a.getNDim() - axesSet.cardinality();
         Dimension<?>[] dstDims;
         if (dstNDim > 0) {
             dstDims = (Dimension<?>[])new Dimension[Math.max(1, dstNDim)];
             int i = 0;
             int j = 0;
@@ -7585,33 +8310,31 @@
         else {
             dstDims = (Dimension<?>[])Dimension.of(1L);
         }
         final DoubleHypercube dst = (DoubleHypercube)new DoubleArrayHypercube((Dimension[])dstDims);
         final long[] indices = new long[a.getNDim()];
         final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
         final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
-        int k = 0;
-        int l = 0;
-        while (k < srcAccessors.length) {
+        for (int k = 0; k < srcAccessors.length; ++k) {
             if (axesSet.get(k)) {
                 srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
             }
-            ++k;
         }
         boolean carry;
         do {
-            k = 0;
-            l = 0;
+            int k = 0;
+            int l = 0;
             while (k < a.getNDim()) {
                 if (!axesSet.get(k)) {
                     srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
                 }
                 ++k;
             }
-            final Double result = Double.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Double>)a.slice((Dimension.Accessor[])srcAccessors), op));
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final Double result = Double.valueOf(associativeOp((com.deshaw.hypercube.Hypercube<Double>)a.slice((Dimension.Accessor[])srcAccessors), initial, whereSlice, op));
             if (dstNDim > 0) {
                 dst.setObj((Object)result, (Dimension.Coordinate[])dstAccessors);
             }
             else {
                 dst.setObjectAt(0L, (Object)result);
             }
             carry = true;
@@ -7628,112 +8351,143 @@
                     }
                 }
             }
         } while (!carry);
         return dst;
     }
     
-    private static double doubleAssociativeOpHelper(final DoubleHypercube da, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static double doubleAssociativeOpHelper(final DoubleHypercube da, final Double i, final BooleanHypercube w, final CubeMath.AssociativeOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         double r = 0.0;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0.0;
-                break;
-            }
-            case 2: {
-                r = 0.0;
-                break;
-            }
-            case 3: {
-                r = Double.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Double.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0.0;
+                    break;
+                }
+                case 2: {
+                    r = 0.0;
+                    break;
+                }
+                case 3: {
+                    r = Double.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Double.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         final double[] aa = new double[CubeMath.STAGING_SIZE];
-        for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
-            final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
-            da.toFlattened(i, aa, 0, len);
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
+        for (long ii = startIndex; ii < endIndex; ii += CubeMath.STAGING_SIZE) {
+            final int len = (int)Math.min(endIndex - ii, CubeMath.STAGING_SIZE);
+            da.toFlattened(ii, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(ii, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
                 case 1: {
-                    for (int j = 0; j < len && !Double.isNaN(r); r += aa[j], ++j) {}
+                    for (int j = 0; j < len && !Double.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r += aa[j];
+                        }
+                    }
                     break;
                 }
                 case 3: {
-                    for (int j = 0; j < len && !Double.isNaN(r); r = ((r < aa[j]) ? r : aa[j]), ++j) {}
+                    for (int j = 0; j < len && !Double.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r = ((r < aa[j]) ? r : aa[j]);
+                        }
+                    }
                     break;
                 }
                 case 4: {
-                    for (int j = 0; j < len && !Double.isNaN(r); r = ((r > aa[j]) ? r : aa[j]), ++j) {}
+                    for (int j = 0; j < len && !Double.isNaN(r); ++j) {
+                        if (ww == null || ww[j]) {
+                            r = ((r > aa[j]) ? r : aa[j]);
+                        }
+                    }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r += (Double.isNaN(aa[j]) ? 0.0 : aa[j]);
+                        if (ww == null || ww[j]) {
+                            r += (Double.isNaN(aa[j]) ? 0.0 : aa[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static Double doubleAssociativeOp(final Hypercube<Double> a, final CubeMath.AssociativeOp op) throws NullPointerException {
+    private static Double doubleAssociativeOp(final Hypercube<Double> a, final Double i, final BooleanHypercube w, final CubeMath.AssociativeOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
+        if (w != null && !a.matchesInShape((Hypercube)w)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
         double r = 0.0;
-        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-            case 1: {
-                r = 0.0;
-                break;
-            }
-            case 2: {
-                r = 0.0;
-                break;
-            }
-            case 3: {
-                r = Double.MAX_VALUE;
-                break;
-            }
-            case 4: {
-                r = Double.MIN_VALUE;
-                break;
-            }
-            default: {
-                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+        if (i != null) {
+            r = i;
+        }
+        else {
+            switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                case 1: {
+                    r = 0.0;
+                    break;
+                }
+                case 2: {
+                    r = 0.0;
+                    break;
+                }
+                case 3: {
+                    r = Double.MAX_VALUE;
+                    break;
+                }
+                case 4: {
+                    r = Double.MIN_VALUE;
+                    break;
+                }
+                default: {
+                    throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                }
             }
         }
         try {
             final DoubleHypercube da = (DoubleHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = doubleAssociativeOpHelper(da, op, 0L, a.getSize());
+                r = doubleAssociativeOpHelper(da, i, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final double[] ar = new double[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = doubleAssociativeOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = doubleAssociativeOpHelper(da, null, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -7767,52 +8521,54 @@
                     default: {
                         throw new UnsupportedOperationException("Unsupported associative operation: " + op);
                     }
                 }
             }
         }
         catch (final Exception e) {
-            for (long i = 0L, size = a.getSize(); i < size && !Double.isNaN(r); ++i) {
-                final Double va = (Double)a.getObjectAt(i);
-                if (va != null) {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r += va;
-                            break;
-                        }
-                        case 3: {
-                            r = ((r < va) ? r : ((double)va));
-                            break;
-                        }
-                        case 4: {
-                            r = ((r > va) ? r : ((double)va));
-                            break;
-                        }
-                        case 2: {
-                            r += (Double.isNaN(va) ? 0.0 : ((double)va));
-                            break;
-                        }
-                        default: {
-                            throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+            for (long ii = 0L, size = a.getSize(); ii < size && !Double.isNaN(r); ++ii) {
+                if (w == null || w.getAt(ii)) {
+                    final Double va = (Double)a.getObjectAt(ii);
+                    if (va != null) {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r += va;
+                                break;
+                            }
+                            case 3: {
+                                r = ((r < va) ? r : ((double)va));
+                                break;
+                            }
+                            case 4: {
+                                r = ((r > va) ? r : ((double)va));
+                                break;
+                            }
+                            case 2: {
+                                r += (Double.isNaN(va) ? 0.0 : ((double)va));
+                                break;
+                            }
+                            default: {
+                                throw new UnsupportedOperationException("Unsupported associative operation: " + op);
+                            }
                         }
                     }
-                }
-                else {
-                    switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
-                        case 1: {
-                            r = Double.valueOf(Double.NaN);
-                            break;
-                        }
-                        case 3: {
-                            r = Double.valueOf(Double.NaN);
-                            break;
-                        }
-                        case 4: {
-                            r = Double.valueOf(Double.NaN);
-                            break;
+                    else {
+                        switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$AssociativeOp[op.ordinal()]) {
+                            case 1: {
+                                r = Double.valueOf(Double.NaN);
+                                break;
+                            }
+                            case 3: {
+                                r = Double.valueOf(Double.NaN);
+                                break;
+                            }
+                            case 4: {
+                                r = Double.valueOf(Double.NaN);
+                                break;
+                            }
                         }
                     }
                 }
             }
             return Double.valueOf(r);
         }
         return Double.valueOf(r);
@@ -7828,93 +8584,122 @@
         return (Hypercube<Double>)a;
     }
     
     public static Hypercube<Double> broadcast(final long size, final double value) {
         return broadcast((Dimension<?>[])Dimension.of(size), value);
     }
     
-    private static void doubleBinaryOpHelper(final DoubleHypercube da, final DoubleHypercube db, final DoubleHypercube dr, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static void doubleBinaryOpHelper(final DoubleHypercube da, final DoubleHypercube db, final DoubleHypercube dr, final BooleanHypercube dw, final CubeMath.BinaryOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         final double[] aa = new double[CubeMath.STAGING_SIZE];
         final double[] ab = new double[CubeMath.STAGING_SIZE];
         final double[] ar = new double[CubeMath.STAGING_SIZE];
+        final boolean[] aw = (boolean[])((dw == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
             db.toFlattened(i, ab, 0, len);
+            if (dw != null) {
+                dw.toFlattened(i, aw, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$BinaryOp[op.ordinal()]) {
                 case 4: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] + ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] + ab[j];
+                        }
                     }
                     break;
                 }
                 case 5: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] - ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] - ab[j];
+                        }
                     }
                     break;
                 }
                 case 6: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] * ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] * ab[j];
+                        }
                     }
                     break;
                 }
                 case 7: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] / ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] / ab[j];
+                        }
                     }
                     break;
                 }
                 case 8: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = aa[j] % ab[j];
+                        if (aw == null || aw[j]) {
+                            ar[j] = aa[j] % ab[j];
+                        }
                     }
                     break;
                 }
                 case 9: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.min(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.min(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 10: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.max(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.max(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 case 11: {
                     for (int j = 0; j < len; ++j) {
-                        ar[j] = Math.pow(aa[j], ab[j]);
+                        if (aw == null || aw[j]) {
+                            ar[j] = Math.pow(aa[j], ab[j]);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported binary operation: " + op);
                 }
             }
-            dr.fromFlattened(ar, 0, i, len);
+            if (aw == null) {
+                dr.fromFlattened(ar, 0, i, len);
+            }
+            else {
+                for (int j = 0; j < len; ++j) {
+                    if (aw[j]) {
+                        dr.setAt(i + (long)j, ar[j]);
+                    }
+                }
+            }
         }
     }
     
-    private static Hypercube<Double> doubleBinaryOp(final Hypercube<Double> a, final Hypercube<Double> b, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Double> doubleBinaryOp(final Hypercube<Double> a, final Hypercube<Double> b, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (!a.matches((Hypercube)b)) {
             throw new IllegalArgumentException("Given incompatible cubes");
         }
-        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Double>)new DoubleArrayHypercube(a.getDimensions()), op);
+        return binaryOp(a, b, (com.deshaw.hypercube.Hypercube<Double>)new DoubleArrayHypercube(a.getDimensions()), dw, op);
     }
     
-    private static Hypercube<Double> doubleBinaryOp(final Hypercube<Double> a, final Hypercube<Double> b, final Hypercube<Double> r, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
+    private static Hypercube<Double> doubleBinaryOp(final Hypercube<Double> a, final Hypercube<Double> b, final Hypercube<Double> r, final BooleanHypercube dw, final CubeMath.BinaryOp op) throws IllegalArgumentException, NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube 'a'");
         }
         if (b == null) {
             throw new NullPointerException("Given a null cube, 'b'");
         }
         if (r == null) {
@@ -7924,27 +8709,27 @@
             throw new IllegalArgumentException("Given incompatible cubes");
         }
         try {
             final DoubleHypercube da = (DoubleHypercube)a;
             final DoubleHypercube db = (DoubleHypercube)b;
             final DoubleHypercube dr = (DoubleHypercube)r;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                doubleBinaryOpHelper(da, db, dr, op, 0L, a.getSize());
+                doubleBinaryOpHelper(da, db, dr, dw, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                doubleBinaryOpHelper(da, db, dr, op, startIndex, endIndex);
+                                doubleBinaryOpHelper(da, db, dr, dw, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
@@ -8399,15 +9184,91 @@
                 }
             }
             return r;
         }
         return r;
     }
     
-    private static boolean doubleReductiveLogicOpHelper(final DoubleHypercube da, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
+    private static BooleanHypercube doubleReductiveLogicOpByAxes(final Hypercube<Double> a, final int[] axes, final BooleanHypercube where, final CubeMath.ReductiveLogicOp op) throws IllegalArgumentException, NullPointerException, UnsupportedOperationException {
+        final BitSet axesSet = new BitSet(a.getNDim());
+        for (final int axis : axes) {
+            if (axis >= a.getNDim()) {
+                throw new IllegalArgumentException("Axis " + axis + " not in given cube");
+            }
+            if (axesSet.get(axis)) {
+                throw new IllegalArgumentException("Duplicate axis " + axis + " in " + Arrays.toString(axes));
+            }
+            axesSet.set(axis);
+        }
+        if (where != null && !a.matchesInShape((Hypercube)where)) {
+            throw new IllegalArgumentException("Source cube and where cube don't match in shape");
+        }
+        final Dimension<?>[] srcDims = (Dimension<?>[])a.getDimensions();
+        final int dstNDim = a.getNDim() - axesSet.cardinality();
+        Dimension<?>[] dstDims;
+        if (dstNDim > 0) {
+            dstDims = (Dimension<?>[])new Dimension[dstNDim];
+            int i = 0;
+            int j = 0;
+            while (i < a.getNDim()) {
+                if (!axesSet.get(i)) {
+                    dstDims[j++] = srcDims[i];
+                }
+                ++i;
+            }
+        }
+        else {
+            dstDims = (Dimension<?>[])Dimension.of(1L);
+        }
+        final BooleanHypercube dst = (BooleanHypercube)new BooleanBitSetHypercube((Dimension[])dstDims);
+        final long[] indices = new long[a.getNDim()];
+        final Dimension.Accessor<?>[] srcAccessors = (Dimension.Accessor<?>[])new Dimension.Accessor[a.getNDim()];
+        final Dimension.Coordinate<?>[] dstAccessors = (Dimension.Coordinate<?>[])new Dimension.Coordinate[dstNDim];
+        for (int k = 0; k < srcAccessors.length; ++k) {
+            if (axesSet.get(k)) {
+                srcAccessors[k] = (Dimension.Accessor<?>)a.dim(k).slice(0L, a.length(k));
+            }
+        }
+        boolean carry;
+        do {
+            int k = 0;
+            int l = 0;
+            while (k < a.getNDim()) {
+                if (!axesSet.get(k)) {
+                    srcAccessors[k] = (Dimension.Accessor<?>)(dstAccessors[l++] = (Dimension.Coordinate<?>)a.dim(k).at(indices[k]));
+                }
+                ++k;
+            }
+            final BooleanHypercube whereSlice = (where == null) ? null : where.slice((Dimension.Accessor[])srcAccessors);
+            final boolean result = doubleReductiveLogicOp((Hypercube<Double>)a.slice((Dimension.Accessor[])srcAccessors), whereSlice, op);
+            if (dstNDim > 0) {
+                dst.setObj((Object)Boolean.valueOf(result), (Dimension.Coordinate[])dstAccessors);
+            }
+            else {
+                dst.setObjectAt(0L, (Object)Boolean.valueOf(result));
+            }
+            carry = true;
+            for (int m = 0; m < indices.length && carry; ++m) {
+                if (!axesSet.get(m)) {
+                    if (indices[m] < a.length(m) - 1L) {
+                        final long[] array = indices;
+                        final int n2 = m;
+                        ++array[n2];
+                        carry = false;
+                    }
+                    else {
+                        indices[m] = 0L;
+                    }
+                }
+            }
+        } while (!carry);
+        return dst;
+    }
+    
+    private static boolean doubleReductiveLogicOpHelper(final DoubleHypercube da, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op, final long startIndex, final long endIndex) throws UnsupportedOperationException {
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
                 break;
             }
             case 2: {
@@ -8415,39 +9276,47 @@
                 break;
             }
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         final double[] aa = new double[CubeMath.STAGING_SIZE];
+        final boolean[] ww = (boolean[])((w == null) ? null : new boolean[CubeMath.STAGING_SIZE]);
         for (long i = startIndex; i < endIndex; i += CubeMath.STAGING_SIZE) {
             final int len = (int)Math.min(endIndex - i, CubeMath.STAGING_SIZE);
             da.toFlattened(i, aa, 0, len);
+            if (w != null) {
+                w.toFlattened(i, ww, 0, len);
+            }
             switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
                 case 1: {
                     for (int j = 0; j < len; ++j) {
-                        r |= (aa[j] != 0.0);
+                        if (ww == null || ww[j]) {
+                            r |= (aa[j] != 0.0);
+                        }
                     }
                     break;
                 }
                 case 2: {
                     for (int j = 0; j < len; ++j) {
-                        r &= (aa[j] != 0.0);
+                        if (ww == null || ww[j]) {
+                            r &= (aa[j] != 0.0);
+                        }
                     }
                     break;
                 }
                 default: {
                     throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
                 }
             }
         }
         return r;
     }
     
-    private static boolean doubleReductiveLogicOp(final Hypercube<Double> a, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
+    private static boolean doubleReductiveLogicOp(final Hypercube<Double> a, final BooleanHypercube w, final CubeMath.ReductiveLogicOp op) throws NullPointerException {
         if (a == null) {
             throw new NullPointerException("Given a null cube, 'a'");
         }
         boolean r = false;
         switch (CubeMath.CubeMath$1.$SwitchMap$com$deshaw$hypercube$CubeMath$ReductiveLogicOp[op.ordinal()]) {
             case 1: {
                 r = false;
@@ -8460,29 +9329,29 @@
             default: {
                 throw new UnsupportedOperationException("Unsupported reductive logic operation: " + op);
             }
         }
         try {
             final DoubleHypercube da = (DoubleHypercube)a;
             if (CubeMath.ourExecutorService == null || a.getSize() < CubeMath.THREADING_THRESHOLD) {
-                r = doubleReductiveLogicOpHelper(da, op, 0L, a.getSize());
+                r = doubleReductiveLogicOpHelper(da, w, op, 0L, a.getSize());
             }
             else {
                 final CountDownLatch latch = new CountDownLatch(CubeMath.NUM_THREADS);
                 final long bucket = (a.getSize() / CubeMath.NUM_THREADS / 32L + 1L) * 32L;
                 final boolean[] ar = new boolean[CubeMath.NUM_THREADS];
                 final AtomicReference<Exception> exception = new AtomicReference<Exception>();
                 for (int j = 0; j < CubeMath.NUM_THREADS; ++j) {
                     final long startIndex = bucket * j;
                     final long endIndex = (j == CubeMath.NUM_THREADS - 1) ? a.getSize() : Math.min(bucket * (long)(j + 1), a.getSize());
                     final int idx = j;
                     if (startIndex != endIndex) {
                         CubeMath.ourExecutorService.submit(() -> {
                             try {
-                                ar[idx] = doubleReductiveLogicOpHelper(da, op, startIndex, endIndex);
+                                ar[idx] = doubleReductiveLogicOpHelper(da, w, op, startIndex, endIndex);
                             }
                             catch (final Exception e2) {
                                 exception.set(e2);
                             }
                             finally {
                                 latch.countDown();
                             }
```

#### com/deshaw/hypercube/CubeMath$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum b7e8cd1904441ab183bfbf4e0177a93d17b9381a76a2e9045d3e67b578d8c086
+  SHA-256 checksum 3139b3f5b82f824703029a3f3451d8bf852d84e41cd77cc3f643688efb2c62ef
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$1
   minor version: 0
   major version: 55
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #55                         // com/deshaw/hypercube/CubeMath$1
   super_class: #56                        // java/lang/Object
@@ -548,19 +548,19 @@
            536   548   551   Class java/lang/NoSuchFieldError
            552   564   567   Class java/lang/NoSuchFieldError
            568   580   583   Class java/lang/NoSuchFieldError
            584   596   599   Class java/lang/NoSuchFieldError
            600   612   615   Class java/lang/NoSuchFieldError
            616   628   631   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 10131: 0
-        line 9590: 69
-        line 9406: 108
-        line 9237: 208
-        line 9052: 452
+        line 10570: 0
+        line 10005: 69
+        line 9696: 108
+        line 9527: 208
+        line 9331: 452
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 76
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### com/deshaw/hypercube/CubeMath$ReductiveLogicOp.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0b766d40c8305150498d5ec15c31ca4658e85b3093876840dd3c583a9d7da29b
+  SHA-256 checksum 0b4d2d4a379fa764bea0567a2adfe23079dc35077c7e316f595c441622be4d9d
   Compiled from "CubeMath.java"
 final class com.deshaw.hypercube.CubeMath$ReductiveLogicOp extends java.lang.Enum<com.deshaw.hypercube.CubeMath$ReductiveLogicOp>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/hypercube/CubeMath$ReductiveLogicOp
   super_class: #12                        // java/lang/Enum
@@ -82,28 +82,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;"
          9: areturn
       LineNumberTable:
-        line 601: 0
+        line 606: 0
 
   public static com.deshaw.hypercube.CubeMath$ReductiveLogicOp valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/hypercube/CubeMath$ReductiveLogicOp
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/hypercube/CubeMath$ReductiveLogicOp
          9: areturn
       LineNumberTable:
-        line 601: 0
+        line 606: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -114,15 +114,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: return
       LineNumberTable:
-        line 601: 0
+        line 606: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
       $enum$ordinal                  synthetic
@@ -154,15 +154,15 @@
         36: dup
         37: iconst_1
         38: getstatic     #11                 // Field ALL:Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;
         41: aastore
         42: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;
         45: return
       LineNumberTable:
-        line 603: 0
-        line 601: 26
+        line 608: 0
+        line 606: 26
 }
 Signature: #38                          // Ljava/lang/Enum<Lcom/deshaw/hypercube/CubeMath$ReductiveLogicOp;>;
 SourceFile: "CubeMath.java"
 NestHost: class com/deshaw/hypercube/CubeMath
 InnerClasses:
   private static final #14= #4 of #42;    // ReductiveLogicOp=class com/deshaw/hypercube/CubeMath$ReductiveLogicOp of class com/deshaw/hypercube/CubeMath
```

#### com/deshaw/hypercube/CubeMath$ComparisonOp.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 5a9be63e634472e5844ade4e211a031c0f44b02ace1dcec05af88f09e6d37f3d
+  SHA-256 checksum b60e4488ba3c64d504fbc60fa349e1305890d12f87533e190cc17eee9fc3cbda
   Compiled from "CubeMath.java"
 final class com.deshaw.hypercube.CubeMath$ComparisonOp extends java.lang.Enum<com.deshaw.hypercube.CubeMath$ComparisonOp>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/hypercube/CubeMath$ComparisonOp
   super_class: #20                        // java/lang/Enum
@@ -114,28 +114,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$ComparisonOp;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/hypercube/CubeMath$ComparisonOp;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/hypercube/CubeMath$ComparisonOp;"
          9: areturn
       LineNumberTable:
-        line 593: 0
+        line 598: 0
 
   public static com.deshaw.hypercube.CubeMath$ComparisonOp valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/hypercube/CubeMath$ComparisonOp;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/hypercube/CubeMath$ComparisonOp
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/hypercube/CubeMath$ComparisonOp
          9: areturn
       LineNumberTable:
-        line 593: 0
+        line 598: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -146,15 +146,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: return
       LineNumberTable:
-        line 593: 0
+        line 598: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/hypercube/CubeMath$ComparisonOp;
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
       $enum$ordinal                  synthetic
@@ -226,15 +226,15 @@
        113: dup
        114: iconst_5
        115: getstatic     #19                 // Field GE:Lcom/deshaw/hypercube/CubeMath$ComparisonOp;
        118: aastore
        119: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$ComparisonOp;
        122: return
       LineNumberTable:
-        line 595: 0
-        line 593: 78
+        line 600: 0
+        line 598: 78
 }
 Signature: #50                          // Ljava/lang/Enum<Lcom/deshaw/hypercube/CubeMath$ComparisonOp;>;
 SourceFile: "CubeMath.java"
 NestHost: class com/deshaw/hypercube/CubeMath
 InnerClasses:
   private static final #22= #4 of #54;    // ComparisonOp=class com/deshaw/hypercube/CubeMath$ComparisonOp of class com/deshaw/hypercube/CubeMath
```

#### com/deshaw/hypercube/CubeMath$AssociativeOp.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6040c6d6de12e8dd2a3e8d9c28831317caa6e4c9af4797ad501b3f66b4e4a63f
+  SHA-256 checksum d26069440d381e0e387df92a9223c579544b97bdc345c0edff2ac69960ce63e5
   Compiled from "CubeMath.java"
 final class com.deshaw.hypercube.CubeMath$AssociativeOp extends java.lang.Enum<com.deshaw.hypercube.CubeMath$AssociativeOp>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/hypercube/CubeMath$AssociativeOp
   super_class: #16                        // java/lang/Enum
@@ -98,28 +98,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$AssociativeOp;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/hypercube/CubeMath$AssociativeOp;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/hypercube/CubeMath$AssociativeOp;"
          9: areturn
       LineNumberTable:
-        line 585: 0
+        line 590: 0
 
   public static com.deshaw.hypercube.CubeMath$AssociativeOp valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/hypercube/CubeMath$AssociativeOp;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/hypercube/CubeMath$AssociativeOp
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/hypercube/CubeMath$AssociativeOp
          9: areturn
       LineNumberTable:
-        line 585: 0
+        line 590: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -130,15 +130,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: return
       LineNumberTable:
-        line 585: 0
+        line 590: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/hypercube/CubeMath$AssociativeOp;
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
       $enum$ordinal                  synthetic
@@ -190,15 +190,15 @@
         74: dup
         75: iconst_3
         76: getstatic     #15                 // Field NANADD:Lcom/deshaw/hypercube/CubeMath$AssociativeOp;
         79: aastore
         80: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$AssociativeOp;
         83: return
       LineNumberTable:
-        line 587: 0
-        line 585: 52
+        line 592: 0
+        line 590: 52
 }
 Signature: #44                          // Ljava/lang/Enum<Lcom/deshaw/hypercube/CubeMath$AssociativeOp;>;
 SourceFile: "CubeMath.java"
 NestHost: class com/deshaw/hypercube/CubeMath
 InnerClasses:
   private static final #18= #4 of #48;    // AssociativeOp=class com/deshaw/hypercube/CubeMath$AssociativeOp of class com/deshaw/hypercube/CubeMath
```

#### com/deshaw/hypercube/CubeMath$UnaryOp.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 15988720d45c4d24ae62852a50d8baee7bf577684fb389a6583aebdc3a2bd8f3
+  SHA-256 checksum 4df18d52eed97f7989586b8dbf34e510009caa5150e95afda2e17388300b03d1
   Compiled from "CubeMath.java"
 final class com.deshaw.hypercube.CubeMath$UnaryOp extends java.lang.Enum<com.deshaw.hypercube.CubeMath$UnaryOp>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/hypercube/CubeMath$UnaryOp
   super_class: #38                        // java/lang/Enum
@@ -186,28 +186,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$UnaryOp;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/hypercube/CubeMath$UnaryOp;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/hypercube/CubeMath$UnaryOp;"
          9: areturn
       LineNumberTable:
-        line 573: 0
+        line 578: 0
 
   public static com.deshaw.hypercube.CubeMath$UnaryOp valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/hypercube/CubeMath$UnaryOp;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/hypercube/CubeMath$UnaryOp
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/hypercube/CubeMath$UnaryOp
          9: areturn
       LineNumberTable:
-        line 573: 0
+        line 578: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -218,15 +218,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: return
       LineNumberTable:
-        line 573: 0
+        line 578: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/hypercube/CubeMath$UnaryOp;
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
       $enum$ordinal                  synthetic
@@ -388,19 +388,19 @@
        301: dup
        302: bipush        14
        304: getstatic     #37                 // Field NOT:Lcom/deshaw/hypercube/CubeMath$UnaryOp;
        307: aastore
        308: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$UnaryOp;
        311: return
       LineNumberTable:
-        line 575: 0
-        line 576: 26
-        line 577: 65
-        line 578: 148
-        line 579: 190
-        line 573: 204
+        line 580: 0
+        line 581: 26
+        line 582: 65
+        line 583: 148
+        line 584: 190
+        line 578: 204
 }
 Signature: #77                          // Ljava/lang/Enum<Lcom/deshaw/hypercube/CubeMath$UnaryOp;>;
 SourceFile: "CubeMath.java"
 NestHost: class com/deshaw/hypercube/CubeMath
 InnerClasses:
   private static final #40= #4 of #81;    // UnaryOp=class com/deshaw/hypercube/CubeMath$UnaryOp of class com/deshaw/hypercube/CubeMath
```

#### com/deshaw/hypercube/CubeMath$BinaryOp.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 662456deb15f5715f0652ebde786d8a8cb85693e6e9ef487e985f2b03a042c42
+  SHA-256 checksum 1a96cbfcad5a886dc66f37737a30cf15936b20fda97b34d0ca0af2aacbd3ff9e
   Compiled from "CubeMath.java"
 final class com.deshaw.hypercube.CubeMath$BinaryOp extends java.lang.Enum<com.deshaw.hypercube.CubeMath$BinaryOp>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/hypercube/CubeMath$BinaryOp
   super_class: #30                        // java/lang/Enum
@@ -154,28 +154,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$BinaryOp;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/hypercube/CubeMath$BinaryOp;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/hypercube/CubeMath$BinaryOp;"
          9: areturn
       LineNumberTable:
-        line 563: 0
+        line 568: 0
 
   public static com.deshaw.hypercube.CubeMath$BinaryOp valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/hypercube/CubeMath$BinaryOp;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/hypercube/CubeMath$BinaryOp
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/hypercube/CubeMath$BinaryOp
          9: areturn
       LineNumberTable:
-        line 563: 0
+        line 568: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -186,15 +186,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: return
       LineNumberTable:
-        line 563: 0
+        line 568: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/hypercube/CubeMath$BinaryOp;
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
       $enum$ordinal                  synthetic
@@ -316,17 +316,17 @@
        217: dup
        218: bipush        10
        220: getstatic     #29                 // Field XOR:Lcom/deshaw/hypercube/CubeMath$BinaryOp;
        223: aastore
        224: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/hypercube/CubeMath$BinaryOp;
        227: return
       LineNumberTable:
-        line 565: 0
-        line 566: 78
-        line 567: 106
-        line 563: 148
+        line 570: 0
+        line 571: 78
+        line 572: 106
+        line 568: 148
 }
 Signature: #65                          // Ljava/lang/Enum<Lcom/deshaw/hypercube/CubeMath$BinaryOp;>;
 SourceFile: "CubeMath.java"
 NestHost: class com/deshaw/hypercube/CubeMath
 InnerClasses:
   private static final #32= #4 of #69;    // BinaryOp=class com/deshaw/hypercube/CubeMath$BinaryOp of class com/deshaw/hypercube/CubeMath
```

#### com/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c100b8d49a356d2ecbd7d5b18114ae85584c16261171520e6ed01e02e985f6e3
+  SHA-256 checksum e421af97bcc9963aed7a5e5cbb293c4ea1c332f4ee80ea45b9c24462572e7b4d
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$DoubleSingleValueHypercube extends com.deshaw.hypercube.AbstractDoubleHypercube
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #11                         // com/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube
   super_class: #12                        // com/deshaw/hypercube/AbstractDoubleHypercube
@@ -108,17 +108,17 @@
          1: aload_1
          2: invokespecial #1                  // Method com/deshaw/hypercube/AbstractDoubleHypercube."<init>":([Lcom/deshaw/hypercube/Dimension;)V
          5: aload_0
          6: dload_2
          7: putfield      #2                  // Field singleValue:D
         10: return
       LineNumberTable:
-        line 442: 0
-        line 443: 5
-        line 444: 10
+        line 447: 0
+        line 448: 5
+        line 449: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0      11     1 dimensions   [Lcom/deshaw/hypercube/Dimension;
             0      11     2     v   D
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -140,16 +140,16 @@
          5: iload         5
          7: iadd
          8: aload_0
          9: getfield      #2                  // Field singleValue:D
         12: invokestatic  #3                  // Method java/util/Arrays.fill:([DIID)V
         15: return
       LineNumberTable:
-        line 455: 0
-        line 456: 15
+        line 460: 0
+        line 461: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0      16     1 srcPos   J
             0      16     3   dst   [D
             0      16     4 dstPos   I
             0      16     5 length   I
@@ -166,15 +166,15 @@
     Code:
       stack=2, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:D
          4: invokestatic  #4                  // Method java/lang/Double.valueOf:(D)Ljava/lang/Double;
          7: areturn
       LineNumberTable:
-        line 464: 0
+        line 469: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0       8     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -186,15 +186,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 474: 0
+        line 479: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Ljava/lang/Double;
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -208,15 +208,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:D
          4: dreturn
       LineNumberTable:
-        line 485: 0
+        line 490: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0       5     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -228,15 +228,15 @@
       stack=3, locals=5, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 495: 0
+        line 500: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   D
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -250,15 +250,15 @@
     flags: (0x0081) ACC_PUBLIC, ACC_VARARGS
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:D
          4: dreturn
       LineNumberTable:
-        line 506: 0
+        line 511: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0       5     1 indices   [J
     MethodParameters:
       Name                           Flags
       indices                        final
@@ -270,15 +270,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 516: 0
+        line 521: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
             0      10     1     v   D
             0      10     3 indices   [J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -295,15 +295,15 @@
          0: aload_0
          1: lload_1
          2: aload_3
          3: checkcast     #8                  // class java/lang/Double
          6: invokevirtual #9                  // Method setObjectAt:(JLjava/lang/Double;)V
          9: return
       LineNumberTable:
-        line 429: 0
+        line 434: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
@@ -316,15 +316,15 @@
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
          1: lload_1
          2: invokevirtual #10                 // Method getObjectAt:(J)Ljava/lang/Double;
          5: areturn
       LineNumberTable:
-        line 429: 0
+        line 434: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/hypercube/CubeMath$DoubleSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/hypercube/CubeMath$FloatSingleValueHypercube.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 46b2a0a892647437ea6c01bcf39dde8484e14c5eb17522bdb82c14bf469fe7f5
+  SHA-256 checksum 7ae0dc4768c7a42f91d9b37a3347947023817b3de4d3779780a4f51b475ecb3b
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$FloatSingleValueHypercube extends com.deshaw.hypercube.AbstractFloatHypercube
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #11                         // com/deshaw/hypercube/CubeMath$FloatSingleValueHypercube
   super_class: #12                        // com/deshaw/hypercube/AbstractFloatHypercube
@@ -108,17 +108,17 @@
          1: aload_1
          2: invokespecial #1                  // Method com/deshaw/hypercube/AbstractFloatHypercube."<init>":([Lcom/deshaw/hypercube/Dimension;)V
          5: aload_0
          6: fload_2
          7: putfield      #2                  // Field singleValue:F
         10: return
       LineNumberTable:
-        line 343: 0
-        line 344: 5
-        line 345: 10
+        line 348: 0
+        line 349: 5
+        line 350: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0      11     1 dimensions   [Lcom/deshaw/hypercube/Dimension;
             0      11     2     v   F
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -140,16 +140,16 @@
          5: iload         5
          7: iadd
          8: aload_0
          9: getfield      #2                  // Field singleValue:F
         12: invokestatic  #3                  // Method java/util/Arrays.fill:([FIIF)V
         15: return
       LineNumberTable:
-        line 356: 0
-        line 357: 15
+        line 361: 0
+        line 362: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0      16     1 srcPos   J
             0      16     3   dst   [F
             0      16     4 dstPos   I
             0      16     5 length   I
@@ -166,15 +166,15 @@
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:F
          4: invokestatic  #4                  // Method java/lang/Float.valueOf:(F)Ljava/lang/Float;
          7: areturn
       LineNumberTable:
-        line 365: 0
+        line 370: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0       8     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -186,15 +186,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 375: 0
+        line 380: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Ljava/lang/Float;
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -208,15 +208,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:F
          4: freturn
       LineNumberTable:
-        line 386: 0
+        line 391: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0       5     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -228,15 +228,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 396: 0
+        line 401: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   F
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -250,15 +250,15 @@
     flags: (0x0081) ACC_PUBLIC, ACC_VARARGS
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:F
          4: freturn
       LineNumberTable:
-        line 407: 0
+        line 412: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0       5     1 indices   [J
     MethodParameters:
       Name                           Flags
       indices                        final
@@ -270,15 +270,15 @@
       stack=3, locals=3, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 417: 0
+        line 422: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
             0      10     1     v   F
             0      10     2 indices   [J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -295,15 +295,15 @@
          0: aload_0
          1: lload_1
          2: aload_3
          3: checkcast     #8                  // class java/lang/Float
          6: invokevirtual #9                  // Method setObjectAt:(JLjava/lang/Float;)V
          9: return
       LineNumberTable:
-        line 330: 0
+        line 335: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
@@ -316,15 +316,15 @@
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
          1: lload_1
          2: invokevirtual #10                 // Method getObjectAt:(J)Ljava/lang/Float;
          5: areturn
       LineNumberTable:
-        line 330: 0
+        line 335: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/hypercube/CubeMath$FloatSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/hypercube/CubeMath$LongSingleValueHypercube.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 39ffe05d35e5f03217b17d1e991318fbec78d016f2de0d370d490fb61ab19b1d
+  SHA-256 checksum c18026efcc752c5595d4bdc6dd63e40f2ff5c1bc37e252cb53f4b0a584e73c0a
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$LongSingleValueHypercube extends com.deshaw.hypercube.AbstractLongHypercube
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #11                         // com/deshaw/hypercube/CubeMath$LongSingleValueHypercube
   super_class: #12                        // com/deshaw/hypercube/AbstractLongHypercube
@@ -105,17 +105,17 @@
          1: aload_1
          2: invokespecial #1                  // Method com/deshaw/hypercube/AbstractLongHypercube."<init>":([Lcom/deshaw/hypercube/Dimension;)V
          5: aload_0
          6: lload_2
          7: putfield      #2                  // Field singleValue:J
         10: return
       LineNumberTable:
-        line 244: 0
-        line 245: 5
-        line 246: 10
+        line 249: 0
+        line 250: 5
+        line 251: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0      11     1 dimensions   [Lcom/deshaw/hypercube/Dimension;
             0      11     2     v   J
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -137,16 +137,16 @@
          5: iload         5
          7: iadd
          8: aload_0
          9: getfield      #2                  // Field singleValue:J
         12: invokestatic  #3                  // Method java/util/Arrays.fill:([JIIJ)V
         15: return
       LineNumberTable:
-        line 257: 0
-        line 258: 15
+        line 262: 0
+        line 263: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0      16     1 srcPos   J
             0      16     3   dst   [J
             0      16     4 dstPos   I
             0      16     5 length   I
@@ -163,15 +163,15 @@
     Code:
       stack=2, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:J
          4: invokestatic  #4                  // Method java/lang/Long.valueOf:(J)Ljava/lang/Long;
          7: areturn
       LineNumberTable:
-        line 266: 0
+        line 271: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0       8     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -183,15 +183,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 276: 0
+        line 281: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Ljava/lang/Long;
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -205,15 +205,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:J
          4: lreturn
       LineNumberTable:
-        line 287: 0
+        line 292: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0       5     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -225,15 +225,15 @@
       stack=3, locals=5, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 297: 0
+        line 302: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -247,15 +247,15 @@
     flags: (0x0081) ACC_PUBLIC, ACC_VARARGS
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:J
          4: lreturn
       LineNumberTable:
-        line 308: 0
+        line 313: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0       5     1 indices   [J
     MethodParameters:
       Name                           Flags
       indices                        final
@@ -267,15 +267,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 318: 0
+        line 323: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
             0      10     1     v   J
             0      10     3 indices   [J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -292,15 +292,15 @@
          0: aload_0
          1: lload_1
          2: aload_3
          3: checkcast     #8                  // class java/lang/Long
          6: invokevirtual #9                  // Method setObjectAt:(JLjava/lang/Long;)V
          9: return
       LineNumberTable:
-        line 231: 0
+        line 236: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
@@ -313,15 +313,15 @@
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
          1: lload_1
          2: invokevirtual #10                 // Method getObjectAt:(J)Ljava/lang/Long;
          5: areturn
       LineNumberTable:
-        line 231: 0
+        line 236: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/hypercube/CubeMath$LongSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3cac7d041707cf9f0377b32e042ddea7c0079dc190a96fbc90c1c4e5358edf33
+  SHA-256 checksum c311cc9e7e2c5a4afda7ddd47085359f5f1d56e0c017a5aee13464cb10195e2c
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$IntegerSingleValueHypercube extends com.deshaw.hypercube.AbstractIntegerHypercube
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #11                         // com/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube
   super_class: #12                        // com/deshaw/hypercube/AbstractIntegerHypercube
@@ -107,17 +107,17 @@
          1: aload_1
          2: invokespecial #1                  // Method com/deshaw/hypercube/AbstractIntegerHypercube."<init>":([Lcom/deshaw/hypercube/Dimension;)V
          5: aload_0
          6: iload_2
          7: putfield      #2                  // Field singleValue:I
         10: return
       LineNumberTable:
-        line 145: 0
-        line 146: 5
-        line 147: 10
+        line 150: 0
+        line 151: 5
+        line 152: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0      11     1 dimensions   [Lcom/deshaw/hypercube/Dimension;
             0      11     2     v   I
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -139,16 +139,16 @@
          5: iload         5
          7: iadd
          8: aload_0
          9: getfield      #2                  // Field singleValue:I
         12: invokestatic  #3                  // Method java/util/Arrays.fill:([IIII)V
         15: return
       LineNumberTable:
-        line 158: 0
-        line 159: 15
+        line 163: 0
+        line 164: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0      16     1 srcPos   J
             0      16     3   dst   [I
             0      16     4 dstPos   I
             0      16     5 length   I
@@ -165,15 +165,15 @@
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:I
          4: invokestatic  #4                  // Method java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
          7: areturn
       LineNumberTable:
-        line 167: 0
+        line 172: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0       8     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -185,15 +185,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 177: 0
+        line 182: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Ljava/lang/Integer;
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -207,15 +207,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:I
          4: ireturn
       LineNumberTable:
-        line 188: 0
+        line 193: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0       5     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -227,15 +227,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 198: 0
+        line 203: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   I
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -249,15 +249,15 @@
     flags: (0x0081) ACC_PUBLIC, ACC_VARARGS
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:I
          4: ireturn
       LineNumberTable:
-        line 209: 0
+        line 214: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0       5     1 indices   [J
     MethodParameters:
       Name                           Flags
       indices                        final
@@ -269,15 +269,15 @@
       stack=3, locals=3, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 219: 0
+        line 224: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
             0      10     1     v   I
             0      10     2 indices   [J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -294,15 +294,15 @@
          0: aload_0
          1: lload_1
          2: aload_3
          3: checkcast     #8                  // class java/lang/Integer
          6: invokevirtual #9                  // Method setObjectAt:(JLjava/lang/Integer;)V
          9: return
       LineNumberTable:
-        line 132: 0
+        line 137: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
@@ -315,15 +315,15 @@
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
          1: lload_1
          2: invokevirtual #10                 // Method getObjectAt:(J)Ljava/lang/Integer;
          5: areturn
       LineNumberTable:
-        line 132: 0
+        line 137: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/hypercube/CubeMath$IntegerSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6721ec8d0b1500fcc992babc7484b068b30a590857e35ca2bd55b946a38c2cd8
+  SHA-256 checksum d6f8685b89148d430953f1d39e4bf23114714d74eec749d0f0e4a84fdd280c04
   Compiled from "CubeMath.java"
 class com.deshaw.hypercube.CubeMath$BooleanSingleValueHypercube extends com.deshaw.hypercube.AbstractBooleanHypercube
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #11                         // com/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube
   super_class: #12                        // com/deshaw/hypercube/AbstractBooleanHypercube
@@ -108,17 +108,17 @@
          1: aload_1
          2: invokespecial #1                  // Method com/deshaw/hypercube/AbstractBooleanHypercube."<init>":([Lcom/deshaw/hypercube/Dimension;)V
          5: aload_0
          6: iload_2
          7: putfield      #2                  // Field singleValue:Z
         10: return
       LineNumberTable:
-        line 46: 0
-        line 47: 5
-        line 48: 10
+        line 51: 0
+        line 52: 5
+        line 53: 10
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0      11     1 dimensions   [Lcom/deshaw/hypercube/Dimension;
             0      11     2     v   Z
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -140,16 +140,16 @@
          5: iload         5
          7: iadd
          8: aload_0
          9: getfield      #2                  // Field singleValue:Z
         12: invokestatic  #3                  // Method java/util/Arrays.fill:([ZIIZ)V
         15: return
       LineNumberTable:
-        line 59: 0
-        line 60: 15
+        line 64: 0
+        line 65: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0      16     1 srcPos   J
             0      16     3   dst   [Z
             0      16     4 dstPos   I
             0      16     5 length   I
@@ -166,15 +166,15 @@
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:Z
          4: invokestatic  #4                  // Method java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
          7: areturn
       LineNumberTable:
-        line 68: 0
+        line 73: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0       8     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -186,15 +186,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 78: 0
+        line 83: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Ljava/lang/Boolean;
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -208,15 +208,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=3, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:Z
          4: ireturn
       LineNumberTable:
-        line 89: 0
+        line 94: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0       5     1 index   J
     MethodParameters:
       Name                           Flags
       index                          final
@@ -228,15 +228,15 @@
       stack=3, locals=4, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 99: 0
+        line 104: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0      10     1 index   J
             0      10     3     v   Z
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -250,15 +250,15 @@
     flags: (0x0081) ACC_PUBLIC, ACC_VARARGS
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field singleValue:Z
          4: ireturn
       LineNumberTable:
-        line 110: 0
+        line 115: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0       5     1 indices   [J
     MethodParameters:
       Name                           Flags
       indices                        final
@@ -270,15 +270,15 @@
       stack=3, locals=3, args_size=3
          0: new           #5                  // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #6                  // String Mutator methods should never be used
          6: invokespecial #7                  // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 120: 0
+        line 125: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
             0      10     1     v   Z
             0      10     2 indices   [J
     Exceptions:
       throws java.lang.UnsupportedOperationException
@@ -295,15 +295,15 @@
          0: aload_0
          1: lload_1
          2: aload_3
          3: checkcast     #8                  // class java/lang/Boolean
          6: invokevirtual #9                  // Method setObjectAt:(JLjava/lang/Boolean;)V
          9: return
       LineNumberTable:
-        line 33: 0
+        line 38: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
@@ -316,15 +316,15 @@
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
          1: lload_1
          2: invokevirtual #10                 // Method getObjectAt:(J)Ljava/lang/Boolean;
          5: areturn
       LineNumberTable:
-        line 33: 0
+        line 38: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/hypercube/CubeMath$BooleanSingleValueHypercube;
     Exceptions:
       throws java.lang.IndexOutOfBoundsException
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/pjrmi/KwargUtil.class

##### procyon -ec {}

```diff
@@ -1,15 +1,75 @@
 
 package com.deshaw.pjrmi;
 
+import com.deshaw.hypercube.Hypercube;
+import com.deshaw.hypercube.Boolean1dWrappingHypercube;
+import com.deshaw.hypercube.BooleanHypercube;
 import java.util.List;
 import java.util.Arrays;
+import com.deshaw.python.DType;
 
 public class KwargUtil
 {
+    public static <T> T toClassValue(final Object kwarg, final Class<T> klass) throws IllegalArgumentException {
+        if (kwarg == null) {
+            return null;
+        }
+        if (klass == null) {
+            throw new IllegalArgumentException("Given a null class");
+        }
+        try {
+            return klass.cast(kwarg);
+        }
+        catch (final ClassCastException ex) {
+            if (kwarg instanceof Number) {
+                final Number number = (Number)kwarg;
+                if (klass == Byte.class) {
+                    return (T)Byte.valueOf(number.byteValue());
+                }
+                if (klass == Double.class) {
+                    return (T)Double.valueOf(number.doubleValue());
+                }
+                if (klass == Float.class) {
+                    return (T)Float.valueOf(number.floatValue());
+                }
+                if (klass == Integer.class) {
+                    return (T)Integer.valueOf(number.intValue());
+                }
+                if (klass == Short.class) {
+                    return (T)Short.valueOf(number.shortValue());
+                }
+                if (klass == Long.class) {
+                    return (T)Long.valueOf(number.longValue());
+                }
+            }
+            if (klass == String.class) {
+                return (T)kwarg.toString();
+            }
+            throw new IllegalArgumentException("Could not convert " + kwarg + " to a " + klass.getSimpleName());
+        }
+    }
+    
+    public static DType.Type toDTypeType(Object kwarg) throws IllegalArgumentException {
+        if (kwarg == null) {
+            kwarg = "float";
+        }
+        if (kwarg.equals("float")) {
+            kwarg = "float64";
+        }
+        if (!(kwarg instanceof String)) {
+            kwarg = kwarg.toString();
+        }
+        final DType.Type type = DType.Type.byName((String)kwarg);
+        if (type == null) {
+            throw new IllegalArgumentException("No kwarg for '" + kwarg);
+        }
+        return type;
+    }
+    
     public static int[] toIntArray(final Object kwarg) throws IllegalArgumentException {
         if (kwarg == null || kwarg instanceof int[]) {
             return (int[])kwarg;
         }
         long[] array;
         try {
             array = toLongArray(kwarg);
@@ -122,8 +182,29 @@
                 catch (final ClassCastException e) {
                     throw new IllegalArgumentException("Could not convert " + kwarg + " to a long[]", (Throwable)e);
                 }
             }
             throw new IllegalArgumentException("Could not convert " + kwarg + " to a long[]");
         }
     }
+    
+    public static BooleanHypercube toBooleanHypercube(final Object kwarg) throws IllegalArgumentException {
+        if (kwarg == null) {
+            return null;
+        }
+        if (kwarg instanceof Boolean) {
+            return (BooleanHypercube)new Boolean1dWrappingHypercube(new boolean[] { (boolean)kwarg });
+        }
+        if (kwarg instanceof Number) {
+            return (BooleanHypercube)new Boolean1dWrappingHypercube(new boolean[] { ((Number)kwarg).byteValue() != 0 });
+        }
+        BooleanHypercube result = null;
+        try {
+            result = BooleanHypercube.asBooleanHypercube((Hypercube)kwarg);
+        }
+        catch (final ClassCastException ex) {}
+        if (result == null) {
+            throw new IllegalArgumentException("Could not convert value to a BooleanHypercube: " + kwarg);
+        }
+        return result;
+    }
 }
```

#### com/deshaw/pjrmi/PJRmi.class

##### procyon -ec {}

```diff
@@ -3,24 +3,24 @@
 
 import java.lang.invoke.CallSite;
 import java.lang.reflect.UndeclaredThrowableException;
 import java.lang.invoke.MethodHandle;
 import java.lang.invoke.StringConcatFactory;
 import java.lang.invoke.MethodType;
 import java.lang.invoke.MethodHandles;
+import java.util.Arrays;
 import java.io.OutputStream;
 import java.io.InputStream;
 import java.net.InetAddress;
 import java.util.logging.Level;
 import java.util.Set;
 import java.util.Collections;
 import java.util.HashSet;
 import java.util.Random;
 import java.util.Objects;
-import java.util.Arrays;
 import java.io.IOException;
 import java.io.DataOutputStream;
 import com.deshaw.util.StringUtil;
 import com.deshaw.util.ByteList;
 import com.deshaw.util.Instrumentor;
 import java.util.concurrent.atomic.AtomicBoolean;
 import com.deshaw.python.PythonPickle;
@@ -41,14 +41,15 @@
     static final Logger LOG;
     private static final String HELLO = "PJRMI_1.13";
     private static final int CALLBACK_REQUEST_ID = -1;
     private static final List<Method> OBJECT_METHODS;
     private static final int MAX_CALL_DEPTH = 128;
     private final long THREAD_ID_XOR;
     private static final Object[] EMPTY_OBJECTS;
+    private static MethodUtil ourMethodUtil;
     private static final ThreadLocal<PJRmi.ByteArrayDataOutputStream> ourByteOutBuffer;
     private static final ThreadLocal<PythonPickle> ourPythonPickle;
     private final Transport.Provider myTransportProvider;
     private final String myName;
     private int myConnectionIndex;
     private final AtomicBoolean myIsClosed;
     private final PJRmi.TypeMapping myTypeMapping;
@@ -132,41 +133,14 @@
         if (buffer.length < size) {
             buffer = new byte[(int)(size * 1.1)];
             PJRmi.ourThreadLocalByteBuffer.set(buffer);
         }
         return buffer;
     }
     
-    private static void methodSort(final Method[] methods) {
-        final int length = methods.length;
-        methodSort(Arrays.copyOf(methods, length), methods, 0, length);
-    }
-    
-    private static void methodSort(final Method[] src, final Method[] dst, final int low, final int high) {
-        final int length = high - low;
-        if (length < 2) {
-            return;
-        }
-        final int mid = low + high >>> 1;
-        methodSort(dst, src, low, mid);
-        methodSort(dst, src, mid, high);
-        int i = low;
-        int j = low;
-        int k = mid;
-        while (i < high) {
-            if (k >= high || (j < mid && PJRmi.MethodComparator.INSTANCE.compare(src[j], src[k]) <= 0)) {
-                dst[i] = src[j++];
-            }
-            else {
-                dst[i] = src[k++];
-            }
-            ++i;
-        }
-    }
-    
     public PJRmi(final String name, final Transport.Provider provider) throws IOException {
         this(name, provider, false);
     }
     
     public PJRmi(final String name, final Transport.Provider provider, final boolean useGlobalLock) throws IOException {
         this(name, provider, useGlobalLock, null);
     }
@@ -214,15 +188,15 @@
                 case 1:
                 case 4:
                 case 17: {
                     instr.setIntervalMod(1);
                     break;
                 }
                 case 5:
-                case 20: {
+                case 21: {
                     instr.setIntervalMod(1000);
                     break;
                 }
                 default: {
                     instr.setIntervalMod(10);
                     break;
                 }
@@ -378,20 +352,24 @@
             }
             default: {
                 return len > 3 && className.charAt(0) == '[' && className.charAt(1) == 'L' && className.charAt(len - 1) == ';' && this.isClassPermitted(className.subSequence(2, len - 1));
             }
         }
     }
     
+    private boolean isClassPermitted(final Class<?> klass) {
+        return klass != null && this.isClassPermitted(klass.getName());
+    }
+    
     protected String getClassNotPermittedMessage() {
         return "";
     }
     
     protected boolean isClassInjectionPermitted() {
-        return this.isClassPermitted(null);
+        return this.isClassPermitted((CharSequence)null);
     }
     
     protected void connectionAccepted(final String username, final InetAddress address, final Transport transport, final String clientCommand, final Integer pid, final Long id) {
         final StringBuilder sb = new StringBuilder();
         sb.append(this.myName).append(' ').append("Allowed ");
         if (username != null) {
             sb.append("user \"").append(username).append("\"");
@@ -539,18 +517,19 @@
     }
     
     static {
         ourGlobalLockCount = new AtomicLong();
         ourByteListStringBuilder = new ThreadLocalStringBuilder(1024);
         ourByteArrayStringBuilder = new ThreadLocalStringBuilder(1024);
         ourThreadLocalByteBuffer = (ThreadLocal)new PJRmi.PJRmi$1();
-        DEFAULT_CLASS_NAME_ALLOWLIST = Collections.unmodifiableList((List<?>)Arrays.asList("boolean", "byte", "char", "double", "float", "int", "long", "short", "void", "[B", "[C", "[D", "[F", "[I", "[J", "[Ljava.lang.Object;", "[Ljava.lang.String;", "[S", "[Z", "com.deshaw.hypercube.CubeMath", "com.deshaw.hypercube.AbstractBooleanHypercube", "com.deshaw.hypercube.AbstractDoubleHypercube", "com.deshaw.hypercube.AbstractFloatHypercube", "com.deshaw.hypercube.AbstractHypercube", "com.deshaw.hypercube.AbstractIntegerHypercube", "com.deshaw.hypercube.AbstractLongHypercube", "com.deshaw.hypercube.AxisRolledHypercube", "com.deshaw.hypercube.Boolean1dWrappingHypercube", "com.deshaw.hypercube.Boolean2dWrappingHypercube", "com.deshaw.hypercube.Boolean3dWrappingHypercube", "com.deshaw.hypercube.Boolean4dWrappingHypercube", "com.deshaw.hypercube.Boolean5dWrappingHypercube", "com.deshaw.hypercube.BooleanAxisRolledHypercube", "com.deshaw.hypercube.BooleanBitSetHypercube", "com.deshaw.hypercube.BooleanFlatRolledHypercube", "com.deshaw.hypercube.BooleanHypercube", "com.deshaw.hypercube.BooleanSlicedHypercube", "com.deshaw.hypercube.BooleanWrappingHypercube", "com.deshaw.hypercube.Double1dWrappingHypercube", "com.deshaw.hypercube.Double2dWrappingHypercube", "com.deshaw.hypercube.Double3dWrappingHypercube", "com.deshaw.hypercube.Double4dWrappingHypercube", "com.deshaw.hypercube.Double5dWrappingHypercube", "com.deshaw.hypercube.DoubleArrayHypercube", "com.deshaw.hypercube.DoubleAxisRolledHypercube", "com.deshaw.hypercube.DoubleFlatRolledHypercube", "com.deshaw.hypercube.DoubleFromFloatHypercube", "com.deshaw.hypercube.DoubleFromIntegerHypercube", "com.deshaw.hypercube.DoubleFromLongHypercube", "com.deshaw.hypercube.DoubleHypercube", "com.deshaw.hypercube.DoubleMappedHypercube", "com.deshaw.hypercube.DoubleSlicedHypercube", "com.deshaw.hypercube.DoubleWrappingHypercube", "com.deshaw.hypercube.FlatRolledHypercube", "com.deshaw.hypercube.Float1dWrappingHypercube", "com.deshaw.hypercube.Float2dWrappingHypercube", "com.deshaw.hypercube.Float3dWrappingHypercube", "com.deshaw.hypercube.Float4dWrappingHypercube", "com.deshaw.hypercube.Float5dWrappingHypercube", "com.deshaw.hypercube.FloatArrayHypercube", "com.deshaw.hypercube.FloatAxisRolledHypercube", "com.deshaw.hypercube.FloatFlatRolledHypercube", "com.deshaw.hypercube.FloatFromDoubleHypercube", "com.deshaw.hypercube.FloatFromIntegerHypercube", "com.deshaw.hypercube.FloatFromLongHypercube", "com.deshaw.hypercube.FloatHypercube", "com.deshaw.hypercube.FloatMappedHypercube", "com.deshaw.hypercube.FloatSlicedHypercube", "com.deshaw.hypercube.FloatWrappingHypercube", "com.deshaw.hypercube.GenericArrayHypercube", "com.deshaw.hypercube.GenericHypercube", "com.deshaw.hypercube.GenericWrappingHypercube", "com.deshaw.hypercube.Hypercube", "com.deshaw.hypercube.Integer1dWrappingHypercube", "com.deshaw.hypercube.Integer2dWrappingHypercube", "com.deshaw.hypercube.Integer3dWrappingHypercube", "com.deshaw.hypercube.Integer4dWrappingHypercube", "com.deshaw.hypercube.Integer5dWrappingHypercube", "com.deshaw.hypercube.IntegerArrayHypercube", "com.deshaw.hypercube.IntegerAxisRolledHypercube", "com.deshaw.hypercube.IntegerFlatRolledHypercube", "com.deshaw.hypercube.IntegerFromDoubleHypercube", "com.deshaw.hypercube.IntegerFromFloatHypercube", "com.deshaw.hypercube.IntegerFromLongHypercube", "com.deshaw.hypercube.IntegerHypercube", "com.deshaw.hypercube.IntegerMappedHypercube", "com.deshaw.hypercube.IntegerSlicedHypercube", "com.deshaw.hypercube.IntegerWrappingHypercube", "com.deshaw.hypercube.Long1dWrappingHypercube", "com.deshaw.hypercube.Long2dWrappingHypercube", "com.deshaw.hypercube.Long3dWrappingHypercube", "com.deshaw.hypercube.Long4dWrappingHypercube", "com.deshaw.hypercube.Long5dWrappingHypercube", "com.deshaw.hypercube.LongArrayHypercube", "com.deshaw.hypercube.LongAxisRolledHypercube", "com.deshaw.hypercube.LongFlatRolledHypercube", "com.deshaw.hypercube.LongFromDoubleHypercube", "com.deshaw.hypercube.LongFromFloatHypercube", "com.deshaw.hypercube.LongFromIntegerHypercube", "com.deshaw.hypercube.LongHypercube", "com.deshaw.hypercube.LongMappedHypercube", "com.deshaw.hypercube.LongSlicedHypercube", "com.deshaw.hypercube.LongWrappingHypercube", "com.deshaw.hypercube.SlicedHypercube", "com.deshaw.hypercube.WrappingHypercube", "com.deshaw.pjrmi.JavaProxyBase", "com.deshaw.pjrmi.PythonFunction", "com.deshaw.pjrmi.PythonKwargsFunction", "com.deshaw.pjrmi.PythonObject", "com.deshaw.pjrmi.PythonSlice", "com.deshaw.util.StringUtil", "java.lang.AutoCloseable", "java.lang.Boolean", "java.lang.Byte", "java.lang.Character", "java.lang.ClassNotFoundException", "java.lang.Comparable", "java.lang.Double", "java.lang.Exception", "java.lang.Float", "java.lang.Integer", "java.lang.Iterable", "java.lang.Long", "java.lang.NoSuchFieldException", "java.lang.NoSuchMethodException", "java.lang.Number", "java.lang.Object", "java.lang.Short", "java.lang.String", "java.util.Collection", "java.util.Iterator", "java.util.List", "java.util.Map", "java.util.Map$Entry", "java.util.NoSuchElementException", "java.util.Set", "java.util.concurrent.Future", "java.util.function.BiFunction", "java.util.function.Function", "java.util.logging.Level", "java.util.logging.LogManager", "sun.misc.Signal"));
+        DEFAULT_CLASS_NAME_ALLOWLIST = Collections.unmodifiableList((List<?>)Arrays.asList("boolean", "byte", "char", "double", "float", "int", "long", "short", "void", "[B", "[C", "[D", "[F", "[I", "[J", "[Ljava.lang.Object;", "[Ljava.lang.String;", "[Ljava.util.Map$Entry;", "[S", "[Z", "com.deshaw.hypercube.CubeMath", "com.deshaw.hypercube.AbstractBooleanHypercube", "com.deshaw.hypercube.AbstractDoubleHypercube", "com.deshaw.hypercube.AbstractFloatHypercube", "com.deshaw.hypercube.AbstractHypercube", "com.deshaw.hypercube.AbstractIntegerHypercube", "com.deshaw.hypercube.AbstractLongHypercube", "com.deshaw.hypercube.AxisRolledHypercube", "com.deshaw.hypercube.Boolean1dWrappingHypercube", "com.deshaw.hypercube.Boolean2dWrappingHypercube", "com.deshaw.hypercube.Boolean3dWrappingHypercube", "com.deshaw.hypercube.Boolean4dWrappingHypercube", "com.deshaw.hypercube.Boolean5dWrappingHypercube", "com.deshaw.hypercube.BooleanAxisRolledHypercube", "com.deshaw.hypercube.BooleanBitSetHypercube", "com.deshaw.hypercube.BooleanFlatRolledHypercube", "com.deshaw.hypercube.BooleanHypercube", "com.deshaw.hypercube.BooleanSlicedHypercube", "com.deshaw.hypercube.BooleanWrappingHypercube", "com.deshaw.hypercube.Dimension", "com.deshaw.hypercube.Dimension$Accessor", "com.deshaw.hypercube.Dimension$Coordinate", "com.deshaw.hypercube.Dimension$Roll", "com.deshaw.hypercube.Double1dWrappingHypercube", "com.deshaw.hypercube.Double2dWrappingHypercube", "com.deshaw.hypercube.Double3dWrappingHypercube", "com.deshaw.hypercube.Double4dWrappingHypercube", "com.deshaw.hypercube.Double5dWrappingHypercube", "com.deshaw.hypercube.DoubleArrayHypercube", "com.deshaw.hypercube.DoubleAxisRolledHypercube", "com.deshaw.hypercube.DoubleFlatRolledHypercube", "com.deshaw.hypercube.DoubleFromFloatHypercube", "com.deshaw.hypercube.DoubleFromIntegerHypercube", "com.deshaw.hypercube.DoubleFromLongHypercube", "com.deshaw.hypercube.DoubleHypercube", "com.deshaw.hypercube.DoubleMappedHypercube", "com.deshaw.hypercube.DoubleSlicedHypercube", "com.deshaw.hypercube.DoubleTransposedHypercube", "com.deshaw.hypercube.DoubleWrappingHypercube", "com.deshaw.hypercube.FlatRolledHypercube", "com.deshaw.hypercube.Float1dWrappingHypercube", "com.deshaw.hypercube.Float2dWrappingHypercube", "com.deshaw.hypercube.Float3dWrappingHypercube", "com.deshaw.hypercube.Float4dWrappingHypercube", "com.deshaw.hypercube.Float5dWrappingHypercube", "com.deshaw.hypercube.FloatArrayHypercube", "com.deshaw.hypercube.FloatAxisRolledHypercube", "com.deshaw.hypercube.FloatFlatRolledHypercube", "com.deshaw.hypercube.FloatFromDoubleHypercube", "com.deshaw.hypercube.FloatFromIntegerHypercube", "com.deshaw.hypercube.FloatFromLongHypercube", "com.deshaw.hypercube.FloatHypercube", "com.deshaw.hypercube.FloatMappedHypercube", "com.deshaw.hypercube.FloatSlicedHypercube", "com.deshaw.hypercube.FloatWrappingHypercube", "com.deshaw.hypercube.GenericArrayHypercube", "com.deshaw.hypercube.GenericHypercube", "com.deshaw.hypercube.GenericWrappingHypercube", "com.deshaw.hypercube.Hypercube", "com.deshaw.hypercube.Integer1dWrappingHypercube", "com.deshaw.hypercube.Integer2dWrappingHypercube", "com.deshaw.hypercube.Integer3dWrappingHypercube", "com.deshaw.hypercube.Integer4dWrappingHypercube", "com.deshaw.hypercube.Integer5dWrappingHypercube", "com.deshaw.hypercube.IntegerArrayHypercube", "com.deshaw.hypercube.IntegerAxisRolledHypercube", "com.deshaw.hypercube.IntegerFlatRolledHypercube", "com.deshaw.hypercube.IntegerFromDoubleHypercube", "com.deshaw.hypercube.IntegerFromFloatHypercube", "com.deshaw.hypercube.IntegerFromLongHypercube", "com.deshaw.hypercube.IntegerHypercube", "com.deshaw.hypercube.IntegerMappedHypercube", "com.deshaw.hypercube.IntegerSlicedHypercube", "com.deshaw.hypercube.IntegerWrappingHypercube", "com.deshaw.hypercube.Long1dWrappingHypercube", "com.deshaw.hypercube.Long2dWrappingHypercube", "com.deshaw.hypercube.Long3dWrappingHypercube", "com.deshaw.hypercube.Long4dWrappingHypercube", "com.deshaw.hypercube.Long5dWrappingHypercube", "com.deshaw.hypercube.LongArrayHypercube", "com.deshaw.hypercube.LongAxisRolledHypercube", "com.deshaw.hypercube.LongFlatRolledHypercube", "com.deshaw.hypercube.LongFromDoubleHypercube", "com.deshaw.hypercube.LongFromFloatHypercube", "com.deshaw.hypercube.LongFromIntegerHypercube", "com.deshaw.hypercube.LongHypercube", "com.deshaw.hypercube.LongMappedHypercube", "com.deshaw.hypercube.LongSlicedHypercube", "com.deshaw.hypercube.LongWrappingHypercube", "com.deshaw.hypercube.SlicedHypercube", "com.deshaw.hypercube.TransposedHypercube", "com.deshaw.hypercube.WrappingHypercube", "com.deshaw.pjrmi.JavaProxyBase", "com.deshaw.pjrmi.PJRmi$ArrayLike", "com.deshaw.pjrmi.PJRmi$PJRmiLockManager", "com.deshaw.pjrmi.PJRmi$PythonItemAssignable", "com.deshaw.pjrmi.PJRmi$PythonSubscriptable", "com.deshaw.pjrmi.PJRmi$WrappedArrayLike", "com.deshaw.pjrmi.PythonFunction", "com.deshaw.pjrmi.PythonKwargsFunction", "com.deshaw.pjrmi.PythonObject", "com.deshaw.pjrmi.PythonSlice", "com.deshaw.python.DType", "com.deshaw.util.concurrent.LockManager", "com.deshaw.util.StringUtil", "java.io.Serializable", "java.lang.AutoCloseable", "java.lang.Boolean", "java.lang.Byte", "java.lang.Character", "java.lang.CharSequence", "java.lang.ClassNotFoundException", "java.lang.Cloneable", "java.lang.Comparable", "java.lang.Double", "java.lang.Error", "java.lang.Exception", "java.lang.Float", "java.lang.IllegalArgumentException", "java.lang.Integer", "java.lang.Iterable", "java.lang.Long", "java.lang.NoSuchFieldException", "java.lang.NoSuchMethodException", "java.lang.Number", "java.lang.Object", "java.lang.OutOfMemoryError", "java.lang.ReflectiveOperationException", "java.lang.RuntimeException", "java.lang.SecurityException", "java.lang.Short", "java.lang.String", "java.lang.Throwable", "java.lang.UnsupportedOperationException", "java.lang.VirtualMachineError", "java.lang.constant.Constable", "java.lang.constant.ConstantDesc", "java.util.AbstractMap", "java.util.AbstractSet", "java.util.Collection", "java.util.HashMap", "java.util.HashMap$Node", "java.util.HashSet", "java.util.Iterator", "java.util.List", "java.util.ListIterator", "java.util.Map", "java.util.Map$Entry", "java.util.NoSuchElementException", "java.util.RandomAccess", "java.util.Set", "java.util.concurrent.Future", "java.util.function.BiFunction", "java.util.function.Consumer", "java.util.function.Function", "java.util.function.Supplier", "java.util.logging.Level", "java.util.logging.LogManager", "java.util.stream.DoubleStream", "java.util.stream.IntStream", "java.util.stream.LongStream", "java.util.stream.Stream", "sun.misc.Signal"));
         LOG = Logger.getLogger("com.deshaw.pjrmi.PJRmi");
         OBJECT_METHODS = Collections.unmodifiableList((List<? extends Method>)Arrays.asList((T[])Object.class.getMethods()));
         EMPTY_OBJECTS = new Object[0];
+        PJRmi.ourMethodUtil = (MethodUtil)new PJRmi.PythonicMethodUtil();
         ourByteOutBuffer = (ThreadLocal)new PJRmi.ThreadLocalByteArrayDataOutputStream();
         ourPythonPickle = ThreadLocal.withInitial(() -> new PJRmi.PJRmiPythonPickle());
     }
     
     // This helper class was generated by Procyon to approximate the behavior of an
     // 'invokedynamic' instruction that it doesn't know how to interpret.
     private static final class ProcyonInvokeDynamicHelper_1
```

#### com/deshaw/pjrmi/PJRmi$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,171 +1,174 @@
-  SHA-256 checksum 130bc27d4286bf05a43d59de696e1b61be99f33af90df81dd1425c6277dac495
+  SHA-256 checksum bba5512a2e1de539f09f794b9b555c33a0d8d7882125f2e9b2d4ebdac16fa8c5
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$3
   minor version: 0
   major version: 55
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
-  this_class: #43                         // com/deshaw/pjrmi/PJRmi$3
-  super_class: #44                        // java/lang/Object
+  this_class: #44                         // com/deshaw/pjrmi/PJRmi$3
+  super_class: #45                        // java/lang/Object
   interfaces: 0, fields: 3, methods: 1, attributes: 4
 Constant pool:
-    #1 = Methodref          #60.#61       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.values:()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-    #2 = Fieldref           #43.#62       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType:[I
-    #3 = Fieldref           #60.#63       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.VALUE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-    #4 = Methodref          #60.#64       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.ordinal:()I
-    #5 = Class              #65           // java/lang/NoSuchFieldError
-    #6 = Fieldref           #60.#66       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-    #7 = Fieldref           #60.#67       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.SHMDATA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-    #8 = Fieldref           #60.#68       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.METHOD:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-    #9 = Fieldref           #60.#69       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.LAMBDA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #10 = Methodref          #70.#71       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.values:()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #11 = Fieldref           #43.#72       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat:[I
-   #12 = Fieldref           #70.#73       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #13 = Methodref          #70.#64       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.ordinal:()I
-   #14 = Fieldref           #70.#74       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.PYTHON_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #15 = Fieldref           #70.#75       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.RAW_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #16 = Fieldref           #70.#76       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #17 = Fieldref           #70.#77       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.BESTEFFORT_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #18 = Fieldref           #70.#78       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.BESTEFFORT_SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #19 = Fieldref           #70.#79       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.SHMDATA:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #20 = Methodref          #80.#81       // com/deshaw/pjrmi/PJRmi$MessageType.values:()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #21 = Fieldref           #43.#82       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
-   #22 = Fieldref           #80.#83       // com/deshaw/pjrmi/PJRmi$MessageType.INSTANCE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #23 = Methodref          #80.#64       // com/deshaw/pjrmi/PJRmi$MessageType.ordinal:()I
-   #24 = Fieldref           #80.#84       // com/deshaw/pjrmi/PJRmi$MessageType.ADD_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #25 = Fieldref           #80.#85       // com/deshaw/pjrmi/PJRmi$MessageType.DROP_REFERENCES:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #26 = Fieldref           #80.#86       // com/deshaw/pjrmi/PJRmi$MessageType.TYPE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #27 = Fieldref           #80.#87       // com/deshaw/pjrmi/PJRmi$MessageType.METHOD_CALL:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #28 = Fieldref           #80.#88       // com/deshaw/pjrmi/PJRmi$MessageType.TO_STRING:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #29 = Fieldref           #80.#89       // com/deshaw/pjrmi/PJRmi$MessageType.GET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #30 = Fieldref           #80.#90       // com/deshaw/pjrmi/PJRmi$MessageType.SET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #31 = Fieldref           #80.#91       // com/deshaw/pjrmi/PJRmi$MessageType.GET_ARRAY_LENGTH:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #32 = Fieldref           #80.#92       // com/deshaw/pjrmi/PJRmi$MessageType.NEW_ARRAY_INSTANCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #33 = Fieldref           #80.#93       // com/deshaw/pjrmi/PJRmi$MessageType.OBJECT_CAST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #34 = Fieldref           #80.#94       // com/deshaw/pjrmi/PJRmi$MessageType.LOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #35 = Fieldref           #80.#95       // com/deshaw/pjrmi/PJRmi$MessageType.UNLOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #36 = Fieldref           #80.#96       // com/deshaw/pjrmi/PJRmi$MessageType.INJECT_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #37 = Fieldref           #80.#97       // com/deshaw/pjrmi/PJRmi$MessageType.INJECT_SOURCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #38 = Fieldref           #80.#98       // com/deshaw/pjrmi/PJRmi$MessageType.GET_VALUE_OF:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #39 = Fieldref           #80.#99       // com/deshaw/pjrmi/PJRmi$MessageType.GET_CALLBACK_HANDLE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #40 = Fieldref           #80.#100      // com/deshaw/pjrmi/PJRmi$MessageType.CALLBACK_RESPONSE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #41 = Fieldref           #80.#101      // com/deshaw/pjrmi/PJRmi$MessageType.GET_PROXY:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #42 = Fieldref           #80.#102      // com/deshaw/pjrmi/PJRmi$MessageType.ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #43 = Class              #103          // com/deshaw/pjrmi/PJRmi$3
-   #44 = Class              #105          // java/lang/Object
-   #45 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType
-   #46 = Utf8               [I
-   #47 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat
-   #48 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType
-   #49 = Utf8               <clinit>
-   #50 = Utf8               ()V
-   #51 = Utf8               Code
-   #52 = Utf8               LineNumberTable
-   #53 = Utf8               LocalVariableTable
-   #54 = Utf8               StackMapTable
-   #55 = Utf8               SourceFile
-   #56 = Utf8               PJRmi.java
-   #57 = Utf8               EnclosingMethod
-   #58 = Class              #106          // com/deshaw/pjrmi/PJRmi
-   #59 = Utf8               NestHost
-   #60 = Class              #108          // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
-   #61 = NameAndType        #111:#112     // values:()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #62 = NameAndType        #48:#46       // $SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType:[I
-   #63 = NameAndType        #113:#114     // VALUE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #64 = NameAndType        #115:#116     // ordinal:()I
-   #65 = Utf8               java/lang/NoSuchFieldError
-   #66 = NameAndType        #117:#114     // REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #67 = NameAndType        #118:#114     // SHMDATA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #68 = NameAndType        #119:#114     // METHOD:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #69 = NameAndType        #120:#114     // LAMBDA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-   #70 = Class              #121          // com/deshaw/pjrmi/PJRmi$PythonValueFormat
-   #71 = NameAndType        #111:#123     // values:()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #72 = NameAndType        #47:#46       // $SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat:[I
-   #73 = NameAndType        #117:#124     // REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #74 = NameAndType        #125:#124     // PYTHON_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #75 = NameAndType        #126:#124     // RAW_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #76 = NameAndType        #127:#124     // SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #77 = NameAndType        #128:#124     // BESTEFFORT_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #78 = NameAndType        #129:#124     // BESTEFFORT_SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #79 = NameAndType        #118:#124     // SHMDATA:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-   #80 = Class              #130          // com/deshaw/pjrmi/PJRmi$MessageType
-   #81 = NameAndType        #111:#132     // values:()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #82 = NameAndType        #45:#46       // $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
-   #83 = NameAndType        #133:#134     // INSTANCE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #84 = NameAndType        #135:#134     // ADD_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #85 = NameAndType        #136:#134     // DROP_REFERENCES:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #86 = NameAndType        #137:#134     // TYPE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #87 = NameAndType        #138:#134     // METHOD_CALL:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #88 = NameAndType        #139:#134     // TO_STRING:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #89 = NameAndType        #140:#134     // GET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #90 = NameAndType        #141:#134     // SET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #91 = NameAndType        #142:#134     // GET_ARRAY_LENGTH:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #92 = NameAndType        #143:#134     // NEW_ARRAY_INSTANCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #93 = NameAndType        #144:#134     // OBJECT_CAST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #94 = NameAndType        #145:#134     // LOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #95 = NameAndType        #146:#134     // UNLOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #96 = NameAndType        #147:#134     // INJECT_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #97 = NameAndType        #148:#134     // INJECT_SOURCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #98 = NameAndType        #149:#134     // GET_VALUE_OF:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-   #99 = NameAndType        #150:#134     // GET_CALLBACK_HANDLE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #100 = NameAndType        #151:#134     // CALLBACK_RESPONSE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #101 = NameAndType        #152:#134     // GET_PROXY:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #102 = NameAndType        #153:#134     // ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #103 = Utf8               com/deshaw/pjrmi/PJRmi$3
-  #104 = Utf8               InnerClasses
-  #105 = Utf8               java/lang/Object
-  #106 = Utf8               com/deshaw/pjrmi/PJRmi
-  #107 = Class              #154          // com/deshaw/pjrmi/PJRmi$MethodDescription
-  #108 = Utf8               com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
-  #109 = Utf8               MethodDescription
-  #110 = Utf8               ArgumentType
-  #111 = Utf8               values
-  #112 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-  #113 = Utf8               VALUE
-  #114 = Utf8               Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
-  #115 = Utf8               ordinal
-  #116 = Utf8               ()I
-  #117 = Utf8               REFERENCE
-  #118 = Utf8               SHMDATA
-  #119 = Utf8               METHOD
-  #120 = Utf8               LAMBDA
-  #121 = Utf8               com/deshaw/pjrmi/PJRmi$PythonValueFormat
-  #122 = Utf8               PythonValueFormat
-  #123 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-  #124 = Utf8               Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
-  #125 = Utf8               PYTHON_REFERENCE
-  #126 = Utf8               RAW_PICKLE
-  #127 = Utf8               SNAPPY_PICKLE
-  #128 = Utf8               BESTEFFORT_PICKLE
-  #129 = Utf8               BESTEFFORT_SNAPPY_PICKLE
-  #130 = Utf8               com/deshaw/pjrmi/PJRmi$MessageType
-  #131 = Utf8               MessageType
-  #132 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #133 = Utf8               INSTANCE_REQUEST
-  #134 = Utf8               Lcom/deshaw/pjrmi/PJRmi$MessageType;
-  #135 = Utf8               ADD_REFERENCE
-  #136 = Utf8               DROP_REFERENCES
-  #137 = Utf8               TYPE_REQUEST
-  #138 = Utf8               METHOD_CALL
-  #139 = Utf8               TO_STRING
-  #140 = Utf8               GET_FIELD
-  #141 = Utf8               SET_FIELD
-  #142 = Utf8               GET_ARRAY_LENGTH
-  #143 = Utf8               NEW_ARRAY_INSTANCE
-  #144 = Utf8               OBJECT_CAST
-  #145 = Utf8               LOCK
-  #146 = Utf8               UNLOCK
-  #147 = Utf8               INJECT_CLASS
-  #148 = Utf8               INJECT_SOURCE
-  #149 = Utf8               GET_VALUE_OF
-  #150 = Utf8               GET_CALLBACK_HANDLE
-  #151 = Utf8               CALLBACK_RESPONSE
-  #152 = Utf8               GET_PROXY
-  #153 = Utf8               ARBITRARY_ITEM
-  #154 = Utf8               com/deshaw/pjrmi/PJRmi$MethodDescription
+    #1 = Methodref          #61.#62       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.values:()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+    #2 = Fieldref           #44.#63       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType:[I
+    #3 = Fieldref           #61.#64       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.VALUE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+    #4 = Methodref          #61.#65       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.ordinal:()I
+    #5 = Class              #66           // java/lang/NoSuchFieldError
+    #6 = Fieldref           #61.#67       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+    #7 = Fieldref           #61.#68       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.SHMDATA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+    #8 = Fieldref           #61.#69       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.METHOD:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+    #9 = Fieldref           #61.#70       // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.LAMBDA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #10 = Methodref          #71.#72       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.values:()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #11 = Fieldref           #44.#73       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat:[I
+   #12 = Fieldref           #71.#74       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #13 = Methodref          #71.#65       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.ordinal:()I
+   #14 = Fieldref           #71.#75       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.PYTHON_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #15 = Fieldref           #71.#76       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.RAW_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #16 = Fieldref           #71.#77       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #17 = Fieldref           #71.#78       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.BESTEFFORT_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #18 = Fieldref           #71.#79       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.BESTEFFORT_SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #19 = Fieldref           #71.#80       // com/deshaw/pjrmi/PJRmi$PythonValueFormat.SHMDATA:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #20 = Methodref          #81.#82       // com/deshaw/pjrmi/PJRmi$MessageType.values:()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #21 = Fieldref           #44.#83       // com/deshaw/pjrmi/PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
+   #22 = Fieldref           #81.#84       // com/deshaw/pjrmi/PJRmi$MessageType.INSTANCE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #23 = Methodref          #81.#65       // com/deshaw/pjrmi/PJRmi$MessageType.ordinal:()I
+   #24 = Fieldref           #81.#85       // com/deshaw/pjrmi/PJRmi$MessageType.ADD_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #25 = Fieldref           #81.#86       // com/deshaw/pjrmi/PJRmi$MessageType.DROP_REFERENCES:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #26 = Fieldref           #81.#87       // com/deshaw/pjrmi/PJRmi$MessageType.TYPE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #27 = Fieldref           #81.#88       // com/deshaw/pjrmi/PJRmi$MessageType.METHOD_CALL:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #28 = Fieldref           #81.#89       // com/deshaw/pjrmi/PJRmi$MessageType.TO_STRING:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #29 = Fieldref           #81.#90       // com/deshaw/pjrmi/PJRmi$MessageType.GET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #30 = Fieldref           #81.#91       // com/deshaw/pjrmi/PJRmi$MessageType.SET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #31 = Fieldref           #81.#92       // com/deshaw/pjrmi/PJRmi$MessageType.GET_ARRAY_LENGTH:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #32 = Fieldref           #81.#93       // com/deshaw/pjrmi/PJRmi$MessageType.NEW_ARRAY_INSTANCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #33 = Fieldref           #81.#94       // com/deshaw/pjrmi/PJRmi$MessageType.OBJECT_CAST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #34 = Fieldref           #81.#95       // com/deshaw/pjrmi/PJRmi$MessageType.LOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #35 = Fieldref           #81.#96       // com/deshaw/pjrmi/PJRmi$MessageType.UNLOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #36 = Fieldref           #81.#97       // com/deshaw/pjrmi/PJRmi$MessageType.INJECT_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #37 = Fieldref           #81.#98       // com/deshaw/pjrmi/PJRmi$MessageType.INJECT_SOURCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #38 = Fieldref           #81.#99       // com/deshaw/pjrmi/PJRmi$MessageType.GET_VALUE_OF:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #39 = Fieldref           #81.#100      // com/deshaw/pjrmi/PJRmi$MessageType.GET_CALLBACK_HANDLE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #40 = Fieldref           #81.#101      // com/deshaw/pjrmi/PJRmi$MessageType.CALLBACK_RESPONSE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #41 = Fieldref           #81.#102      // com/deshaw/pjrmi/PJRmi$MessageType.GET_PROXY:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #42 = Fieldref           #81.#103      // com/deshaw/pjrmi/PJRmi$MessageType.REPLACE_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #43 = Fieldref           #81.#104      // com/deshaw/pjrmi/PJRmi$MessageType.ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #44 = Class              #105          // com/deshaw/pjrmi/PJRmi$3
+   #45 = Class              #107          // java/lang/Object
+   #46 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType
+   #47 = Utf8               [I
+   #48 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat
+   #49 = Utf8               $SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType
+   #50 = Utf8               <clinit>
+   #51 = Utf8               ()V
+   #52 = Utf8               Code
+   #53 = Utf8               LineNumberTable
+   #54 = Utf8               LocalVariableTable
+   #55 = Utf8               StackMapTable
+   #56 = Utf8               SourceFile
+   #57 = Utf8               PJRmi.java
+   #58 = Utf8               EnclosingMethod
+   #59 = Class              #108          // com/deshaw/pjrmi/PJRmi
+   #60 = Utf8               NestHost
+   #61 = Class              #110          // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
+   #62 = NameAndType        #113:#114     // values:()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #63 = NameAndType        #49:#47       // $SwitchMap$com$deshaw$pjrmi$PJRmi$MethodDescription$ArgumentType:[I
+   #64 = NameAndType        #115:#116     // VALUE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #65 = NameAndType        #117:#118     // ordinal:()I
+   #66 = Utf8               java/lang/NoSuchFieldError
+   #67 = NameAndType        #119:#116     // REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #68 = NameAndType        #120:#116     // SHMDATA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #69 = NameAndType        #121:#116     // METHOD:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #70 = NameAndType        #122:#116     // LAMBDA:Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+   #71 = Class              #123          // com/deshaw/pjrmi/PJRmi$PythonValueFormat
+   #72 = NameAndType        #113:#125     // values:()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #73 = NameAndType        #48:#47       // $SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat:[I
+   #74 = NameAndType        #119:#126     // REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #75 = NameAndType        #127:#126     // PYTHON_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #76 = NameAndType        #128:#126     // RAW_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #77 = NameAndType        #129:#126     // SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #78 = NameAndType        #130:#126     // BESTEFFORT_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #79 = NameAndType        #131:#126     // BESTEFFORT_SNAPPY_PICKLE:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #80 = NameAndType        #120:#126     // SHMDATA:Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+   #81 = Class              #132          // com/deshaw/pjrmi/PJRmi$MessageType
+   #82 = NameAndType        #113:#134     // values:()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #83 = NameAndType        #46:#47       // $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
+   #84 = NameAndType        #135:#136     // INSTANCE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #85 = NameAndType        #137:#136     // ADD_REFERENCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #86 = NameAndType        #138:#136     // DROP_REFERENCES:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #87 = NameAndType        #139:#136     // TYPE_REQUEST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #88 = NameAndType        #140:#136     // METHOD_CALL:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #89 = NameAndType        #141:#136     // TO_STRING:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #90 = NameAndType        #142:#136     // GET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #91 = NameAndType        #143:#136     // SET_FIELD:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #92 = NameAndType        #144:#136     // GET_ARRAY_LENGTH:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #93 = NameAndType        #145:#136     // NEW_ARRAY_INSTANCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #94 = NameAndType        #146:#136     // OBJECT_CAST:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #95 = NameAndType        #147:#136     // LOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #96 = NameAndType        #148:#136     // UNLOCK:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #97 = NameAndType        #149:#136     // INJECT_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #98 = NameAndType        #150:#136     // INJECT_SOURCE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+   #99 = NameAndType        #151:#136     // GET_VALUE_OF:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #100 = NameAndType        #152:#136     // GET_CALLBACK_HANDLE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #101 = NameAndType        #153:#136     // CALLBACK_RESPONSE:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #102 = NameAndType        #154:#136     // GET_PROXY:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #103 = NameAndType        #155:#136     // REPLACE_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #104 = NameAndType        #156:#136     // ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #105 = Utf8               com/deshaw/pjrmi/PJRmi$3
+  #106 = Utf8               InnerClasses
+  #107 = Utf8               java/lang/Object
+  #108 = Utf8               com/deshaw/pjrmi/PJRmi
+  #109 = Class              #157          // com/deshaw/pjrmi/PJRmi$MethodDescription
+  #110 = Utf8               com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
+  #111 = Utf8               MethodDescription
+  #112 = Utf8               ArgumentType
+  #113 = Utf8               values
+  #114 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+  #115 = Utf8               VALUE
+  #116 = Utf8               Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
+  #117 = Utf8               ordinal
+  #118 = Utf8               ()I
+  #119 = Utf8               REFERENCE
+  #120 = Utf8               SHMDATA
+  #121 = Utf8               METHOD
+  #122 = Utf8               LAMBDA
+  #123 = Utf8               com/deshaw/pjrmi/PJRmi$PythonValueFormat
+  #124 = Utf8               PythonValueFormat
+  #125 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+  #126 = Utf8               Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
+  #127 = Utf8               PYTHON_REFERENCE
+  #128 = Utf8               RAW_PICKLE
+  #129 = Utf8               SNAPPY_PICKLE
+  #130 = Utf8               BESTEFFORT_PICKLE
+  #131 = Utf8               BESTEFFORT_SNAPPY_PICKLE
+  #132 = Utf8               com/deshaw/pjrmi/PJRmi$MessageType
+  #133 = Utf8               MessageType
+  #134 = Utf8               ()[Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #135 = Utf8               INSTANCE_REQUEST
+  #136 = Utf8               Lcom/deshaw/pjrmi/PJRmi$MessageType;
+  #137 = Utf8               ADD_REFERENCE
+  #138 = Utf8               DROP_REFERENCES
+  #139 = Utf8               TYPE_REQUEST
+  #140 = Utf8               METHOD_CALL
+  #141 = Utf8               TO_STRING
+  #142 = Utf8               GET_FIELD
+  #143 = Utf8               SET_FIELD
+  #144 = Utf8               GET_ARRAY_LENGTH
+  #145 = Utf8               NEW_ARRAY_INSTANCE
+  #146 = Utf8               OBJECT_CAST
+  #147 = Utf8               LOCK
+  #148 = Utf8               UNLOCK
+  #149 = Utf8               INJECT_CLASS
+  #150 = Utf8               INJECT_SOURCE
+  #151 = Utf8               GET_VALUE_OF
+  #152 = Utf8               GET_CALLBACK_HANDLE
+  #153 = Utf8               CALLBACK_RESPONSE
+  #154 = Utf8               GET_PROXY
+  #155 = Utf8               REPLACE_CLASS
+  #156 = Utf8               ARBITRARY_ITEM
+  #157 = Utf8               com/deshaw/pjrmi/PJRmi$MethodDescription
 {
   static final int[] $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType;
     descriptor: [I
     flags: (0x1018) ACC_STATIC, ACC_FINAL, ACC_SYNTHETIC
 
   static final int[] $SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat;
     descriptor: [I
@@ -406,21 +409,28 @@
        495: getstatic     #41                 // Field com/deshaw/pjrmi/PJRmi$MessageType.GET_PROXY:Lcom/deshaw/pjrmi/PJRmi$MessageType;
        498: invokevirtual #23                 // Method com/deshaw/pjrmi/PJRmi$MessageType.ordinal:()I
        501: bipush        19
        503: iastore
        504: goto          508
        507: astore_0
        508: getstatic     #21                 // Field $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
-       511: getstatic     #42                 // Field com/deshaw/pjrmi/PJRmi$MessageType.ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+       511: getstatic     #42                 // Field com/deshaw/pjrmi/PJRmi$MessageType.REPLACE_CLASS:Lcom/deshaw/pjrmi/PJRmi$MessageType;
        514: invokevirtual #23                 // Method com/deshaw/pjrmi/PJRmi$MessageType.ordinal:()I
        517: bipush        20
        519: iastore
        520: goto          524
        523: astore_0
-       524: return
+       524: getstatic     #21                 // Field $SwitchMap$com$deshaw$pjrmi$PJRmi$MessageType:[I
+       527: getstatic     #43                 // Field com/deshaw/pjrmi/PJRmi$MessageType.ARBITRARY_ITEM:Lcom/deshaw/pjrmi/PJRmi$MessageType;
+       530: invokevirtual #23                 // Method com/deshaw/pjrmi/PJRmi$MessageType.ordinal:()I
+       533: bipush        21
+       535: iastore
+       536: goto          540
+       539: astore_0
+       540: return
       Exception table:
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             54    65    68   Class java/lang/NoSuchFieldError
             69    80    83   Class java/lang/NoSuchFieldError
@@ -447,21 +457,22 @@
            412   424   427   Class java/lang/NoSuchFieldError
            428   440   443   Class java/lang/NoSuchFieldError
            444   456   459   Class java/lang/NoSuchFieldError
            460   472   475   Class java/lang/NoSuchFieldError
            476   488   491   Class java/lang/NoSuchFieldError
            492   504   507   Class java/lang/NoSuchFieldError
            508   520   523   Class java/lang/NoSuchFieldError
+           524   536   539   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 6336: 0
-        line 6054: 84
-        line 5854: 200
+        line 6490: 0
+        line 6208: 84
+        line 6004: 200
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
-      StackMapTable: number_of_entries = 64
+      StackMapTable: number_of_entries = 66
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
@@ -550,17 +561,20 @@
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 78 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
+        frame_type = 78 /* same_locals_1_stack_item */
+          stack = [ class java/lang/NoSuchFieldError ]
+        frame_type = 0 /* same */
 }
 SourceFile: "PJRmi.java"
-EnclosingMethod: #58.#0                 // com.deshaw.pjrmi.PJRmi
+EnclosingMethod: #59.#0                 // com.deshaw.pjrmi.PJRmi
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
-  static #43;                             // class com/deshaw/pjrmi/PJRmi$3
-  private static #109= #107 of #58;       // MethodDescription=class com/deshaw/pjrmi/PJRmi$MethodDescription of class com/deshaw/pjrmi/PJRmi
-  private static final #110= #60 of #107; // ArgumentType=class com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType of class com/deshaw/pjrmi/PJRmi$MethodDescription
-  private static final #122= #70 of #58;  // PythonValueFormat=class com/deshaw/pjrmi/PJRmi$PythonValueFormat of class com/deshaw/pjrmi/PJRmi
-  private static final #131= #80 of #58;  // MessageType=class com/deshaw/pjrmi/PJRmi$MessageType of class com/deshaw/pjrmi/PJRmi
+  static #44;                             // class com/deshaw/pjrmi/PJRmi$3
+  private static #111= #109 of #59;       // MethodDescription=class com/deshaw/pjrmi/PJRmi$MethodDescription of class com/deshaw/pjrmi/PJRmi
+  private static final #112= #61 of #109; // ArgumentType=class com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType of class com/deshaw/pjrmi/PJRmi$MethodDescription
+  private static final #124= #71 of #59;  // PythonValueFormat=class com/deshaw/pjrmi/PJRmi$PythonValueFormat of class com/deshaw/pjrmi/PJRmi
+  private static final #133= #81 of #59;  // MessageType=class com/deshaw/pjrmi/PJRmi$MessageType of class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 603fbde744d1d4828b3e585c7eefc608e03b485ad2998cf17bc36a3ccf04a0d0
+  SHA-256 checksum 170dce3347710022a719b05ea08675fa44503d4f27580585c251714aadbfe040
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$2 extends com.deshaw.pjrmi.PJRmi
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$2
   super_class: #5                         // com/deshaw/pjrmi/PJRmi
@@ -72,15 +72,15 @@
          0: aload_0
          1: aload_1
          2: aload_2
          3: iload_3
          4: invokespecial #1                  // Method com/deshaw/pjrmi/PJRmi."<init>":(Ljava/lang/String;Lcom/deshaw/pjrmi/Transport$Provider;Z)V
          7: return
       LineNumberTable:
-        line 9895: 0
+        line 10127: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/pjrmi/PJRmi$2;
             0       8     1  name   Ljava/lang/String;
             0       8     2 provider   Lcom/deshaw/pjrmi/Transport$Provider;
             0       8     3 useGlobalLock   Z
     Exceptions:
@@ -95,15 +95,15 @@
     descriptor: (Ljava/lang/CharSequence;)Z
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=1, locals=2, args_size=2
          0: iconst_1
          1: ireturn
       LineNumberTable:
-        line 9899: 0
+        line 10131: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lcom/deshaw/pjrmi/PJRmi$2;
             0       2     1 username   Ljava/lang/CharSequence;
     MethodParameters:
       Name                           Flags
       username
@@ -112,30 +112,30 @@
     descriptor: ()I
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_2
          1: ireturn
       LineNumberTable:
-        line 9905: 0
+        line 10137: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lcom/deshaw/pjrmi/PJRmi$2;
 
   protected java.lang.Object getObjectInstance(java.lang.CharSequence);
     descriptor: (Ljava/lang/CharSequence;)Ljava/lang/Object;
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=1, locals=2, args_size=2
          0: aload_1
          1: invokeinterface #2,  1            // InterfaceMethod java/lang/CharSequence.toString:()Ljava/lang/String;
          6: invokevirtual #3                  // Method java/lang/String.intern:()Ljava/lang/String;
          9: areturn
       LineNumberTable:
-        line 9911: 0
+        line 10143: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/pjrmi/PJRmi$2;
             0      10     1  name   Ljava/lang/CharSequence;
     MethodParameters:
       Name                           Flags
       name
```

#### com/deshaw/pjrmi/PJRmi$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum a8b27a04e0fcdbaba0c91dc259dfc4c8d0851432f39e05a833d5afb6c8460576
+  SHA-256 checksum 9e30da212d7c212f2176a0f8d387cf6af7b16b06bd96a470d7e88a03c2d3f689
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$1 extends java.lang.ThreadLocal<byte[]>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$1
   super_class: #5                         // java/lang/ThreadLocal
@@ -42,43 +42,43 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/ThreadLocal."<init>":()V
          4: return
       LineNumberTable:
-        line 8749: 0
+        line 8973: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$1;
 
   protected byte[] initialValue();
     descriptor: ()[B
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=1, locals=1, args_size=1
          0: ldc           #2                  // int 1048576
          2: newarray       byte
          4: areturn
       LineNumberTable:
-        line 8754: 0
+        line 8978: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$1;
 
   protected java.lang.Object initialValue();
     descriptor: ()Ljava/lang/Object;
     flags: (0x1044) ACC_PROTECTED, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #3                  // Method initialValue:()[B
          4: areturn
       LineNumberTable:
-        line 8749: 0
+        line 8973: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$1;
 }
 Signature: #18                          // Ljava/lang/ThreadLocal<[B>;
 SourceFile: "PJRmi.java"
 EnclosingMethod: #22.#0                 // com.deshaw.pjrmi.PJRmi
```

#### com/deshaw/pjrmi/PJRmi$Connection.class

##### procyon -ec {}

```diff
@@ -7,14 +7,16 @@
 import java.lang.reflect.Proxy;
 import java.util.function.UnaryOperator;
 import java.util.function.BiPredicate;
 import java.util.function.Predicate;
 import java.util.function.BiConsumer;
 import java.util.function.Consumer;
 import java.util.function.BiFunction;
+import java.lang.instrument.Instrumentation;
+import java.lang.instrument.ClassDefinition;
 import java.util.concurrent.Future;
 import com.deshaw.hypercube.Hypercube;
 import java.util.List;
 import java.util.Set;
 import com.deshaw.hypercube.LongHypercube;
 import com.deshaw.hypercube.IntegerHypercube;
 import com.deshaw.hypercube.DoubleHypercube;
@@ -536,14 +538,18 @@
                 this.handleCallbackResponse(threadId, reqId, payload, result);
                 return;
             }
             case 19: {
                 this.handleGetProxy(threadId, reqId, payload, result, clientReceiver);
                 return;
             }
+            case 20: {
+                this.handleReplaceClass(threadId, reqId, payload, result);
+                return;
+            }
             default: {
                 throw new IllegalArgumentException("Unhandled incoming message type: " + type);
             }
         }
     }
     
     private void buildMessage(final DataOutputStream out, final PJRmi.MessageType type, final long threadId, final int reqId, final ByteArrayOutputStream payload) throws IOException {
@@ -978,15 +984,15 @@
                     for (int i = 0; i < count; ++i) {
                         final PJRmi.ReadObjectResult ror2 = this.readObject(bytes, offset);
                         offset = ror2.offset;
                         set.add(ror2.object);
                     }
                     result = set;
                 }
-                else if (typeDesc.getName().equals("java.util.Collection") || typeDesc.getName().equals("java.util.List")) {
+                else if (typeDesc.getName().equals("java.lang.Iterable") || typeDesc.getName().equals("java.util.Collection") || typeDesc.getName().equals("java.util.List")) {
                     final int count = this.readInt(bytes, offset);
                     offset += 4;
                     final List<Object> list = new ArrayList<Object>(count);
                     for (int i = 0; i < count; ++i) {
                         final PJRmi.ReadObjectResult ror2 = this.readObject(bytes, offset);
                         offset = ror2.offset;
                         list.add(ror2.object);
@@ -1228,15 +1234,17 @@
             final StringBuilder sb = new StringBuilder();
             while (sb.length() < int32) {
                 sb.append((char)payload.get(offset++));
             }
             final String className = sb.toString();
             if (!this.this$0.isClassPermitted((CharSequence)className)) {
                 final String msg = this.this$0.getClassNotPermittedMessage();
-                throw new SecurityException("Access permission denied for class \"" + className + "\"" + ((msg == null) ? "" : invokedynamic(invokestatic java/lang/invoke/StringConcatFactory.makeConcatWithConstants:(Ljava/lang/invoke/MethodHandles$Lookup;Ljava/lang/String;Ljava/lang/invoke/MethodType;Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/invoke/CallSite;, makeConcatWithConstants:(Ljava/lang/String;)Ljava/lang/String;": \u0001")(msg)));
+                final String txt = "Access permission denied for class \"" + className + "\"" + ((msg == null) ? "" : invokedynamic(invokestatic java/lang/invoke/StringConcatFactory.makeConcatWithConstants:(Ljava/lang/invoke/MethodHandles$Lookup;Ljava/lang/String;Ljava/lang/invoke/MethodType;Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/invoke/CallSite;, makeConcatWithConstants:(Ljava/lang/String;)Ljava/lang/String;": \u0001")(msg));
+                PJRmi.LOG.warning(txt);
+                throw new SecurityException(txt);
             }
             final String s = className;
             int n = -1;
             switch (s.hashCode()) {
                 case 3625364: {
                     if (s.equals("void")) {
                         n = 0;
@@ -1342,14 +1350,20 @@
                 default: {
                     klass = Class.forName(className);
                     break;
                 }
             }
             desc = this.this$0.myTypeMapping.getDescription((Class)klass);
         }
+        if (!this.this$0.isClassPermitted(desc.getRepresentedClass())) {
+            final String msg2 = this.this$0.getClassNotPermittedMessage();
+            final String txt2 = "Access permission denied for class " + desc.getRepresentedClass() + ((msg2 == null) ? "" : invokedynamic(invokestatic java/lang/invoke/StringConcatFactory.makeConcatWithConstants:(Ljava/lang/invoke/MethodHandles$Lookup;Ljava/lang/String;Ljava/lang/invoke/MethodType;Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/invoke/CallSite;, makeConcatWithConstants:(Ljava/lang/String;)Ljava/lang/String;": \u0001")(msg2));
+            PJRmi.LOG.warning(txt2);
+            throw new SecurityException(txt2);
+        }
         this.writeTypeDesc(desc, threadId, reqId, buf);
     }
     
     private void handleMethodCall(final long threadId, final VirtualThreadLock.VirtualThread virtualThread, final int reqId, final ByteList payload, final PJRmi.ByteArrayDataOutputStream buf) throws Throwable {
         if (payload.size() < 18) {
             throw new IllegalArgumentException("Got a malformed payload: " + PJRmi.toString(payload));
         }
@@ -1651,23 +1665,48 @@
         }
         final String source = sbSource.toString();
         final SourceInjector mySourceInjector = this.this$0.mySourceInjector;
         final Class<?> klass = SourceInjector.inject(className, source);
         this.writeTypeDesc(this.this$0.myTypeMapping.getDescription((Class)klass), threadId, reqId, buf);
     }
     
+    private void handleReplaceClass(final long threadId, final int reqId, final ByteList payload, final PJRmi.ByteArrayDataOutputStream buf) throws Throwable {
+        if (!this.this$0.isClassInjectionPermitted()) {
+            throw new SecurityException("Source replacement not permitted");
+        }
+        int offset = 0;
+        final int typeId = this.readInt(payload, offset);
+        offset += 4;
+        final int len = this.readInt(payload, offset);
+        offset += 4;
+        final byte[] bytecode = new byte[len];
+        for (int i = 0; i < len; ++i) {
+            bytecode[i] = payload.get(offset++);
+        }
+        final Instrumentation instr = PJRmiAgent.getInstrumentation();
+        if (instr == null) {
+            throw new UnsupportedOperationException("Classes can't be redefined since the PJRmiAgent is not loaded");
+        }
+        final PJRmi.TypeDescription desc = this.this$0.myTypeMapping.getDescription(typeId);
+        if (desc == null) {
+            throw new IllegalArgumentException("Unknown type " + typeId);
+        }
+        final Class<?> klass = desc.getRepresentedClass();
+        instr.redefineClasses(new ClassDefinition(klass, bytecode));
+        final Class<?> newKlass = Class.forName(klass.getName());
+        final PJRmi.TypeDescription newDesc = this.this$0.myTypeMapping.replaceDescription(typeId, (Class)newKlass);
+        this.writeTypeDesc(newDesc, threadId, reqId, buf);
+    }
+    
     private void handleGetValueOf(final long threadId, final int reqId, final ByteList payload, final PJRmi.ByteArrayDataOutputStream buf) throws Throwable {
         if (payload.size() != 9) {
             throw new IllegalArgumentException("Got a malformed payload: " + PJRmi.toString(payload));
         }
         final long handle = this.readLong(payload, 0);
         final PJRmi.PythonValueFormat valueFormat = PJRmi.PythonValueFormat.byId(payload.get(8));
-        if (valueFormat == null) {
-            throw new IllegalArgumentException("Unknown return format #" + payload.get(8));
-        }
         switch (PJRmi.PJRmi$3.$SwitchMap$com$deshaw$pjrmi$PJRmi$PythonValueFormat[valueFormat.ordinal()]) {
             case 3:
             case 4:
             case 5:
             case 6:
             case 7: {
                 final Object object = this.myHandleMapping.getObject(handle);
@@ -1990,27 +2029,32 @@
     }
     
     private long readLong(final ByteList bytes, int offset) {
         return Byte.toUnsignedLong(bytes.get(offset++)) << 56 | Byte.toUnsignedLong(bytes.get(offset++)) << 48 | Byte.toUnsignedLong(bytes.get(offset++)) << 40 | Byte.toUnsignedLong(bytes.get(offset++)) << 32 | Byte.toUnsignedLong(bytes.get(offset++)) << 24 | Byte.toUnsignedLong(bytes.get(offset++)) << 16 | Byte.toUnsignedLong(bytes.get(offset++)) << 8 | Byte.toUnsignedLong(bytes.get(offset++));
     }
     
     private <T> T awaitCallbackReponse(final Connection.PythonCallbackResult result) throws PythonCallbackException {
-        while (!result.isReady()) {
-            LockSupport.parkNanos(1000L);
-        }
-        final Object pythonResult = result.getResult();
-        if (PJRmi.LOG.isLoggable(Level.FINEST)) {
-            PJRmi.LOG.finest("Result was " + pythonResult + " " + ((pythonResult == null) ? "" : pythonResult.getClass()));
-        }
-        if (result.isException()) {
-            final Throwable t = (Throwable)pythonResult;
-            throw new PythonCallbackException(t.getMessage(), t);
+        while (!this.myTransport.isClosed()) {
+            if (result.isReady()) {
+                final Object pythonResult = result.getResult();
+                if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+                    PJRmi.LOG.finest("Result was " + pythonResult + " " + ((pythonResult == null) ? "" : pythonResult.getClass()));
+                }
+                if (result.isException()) {
+                    final Throwable t = (Throwable)pythonResult;
+                    throw new PythonCallbackException(t.getMessage(), t);
+                }
+                final T pr = (T)pythonResult;
+                return pr;
+            }
+            else {
+                LockSupport.parkNanos(1000L);
+            }
         }
-        final T pr = (T)pythonResult;
-        return pr;
+        throw new PythonCallbackException("Connection to Python is closed", (Throwable)new IOException("Connection to Python is closed"));
     }
     
     public Object getProxyForMethod(final Class<?> iface, final PJRmi.TypeDescription typeDesc, final PJRmi.MethodDescription methodDesc, final boolean isConstructor, final Object instance) {
         Objects.requireNonNull(iface);
         Objects.requireNonNull(typeDesc);
         Objects.requireNonNull(methodDesc);
         final InvocationHandler handler = (InvocationHandler)new Connection.PJRmi$Connection$3(this, methodDesc, isConstructor, instance, typeDesc, (Class)iface);
```

#### com/deshaw/pjrmi/PJRmi$Connection$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 1679afe7a68ce92a3bf0b44f8dbb5f3fa0c92dc541fd0f558b1637a2a8eb5b21
+  SHA-256 checksum 42c397caf088346e272baf13484e8f5417f245ec41c552397740533051103695
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$3 implements java.lang.reflect.InvocationHandler
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #41                         // com/deshaw/pjrmi/PJRmi$Connection$3
   super_class: #42                        // java/lang/Object
@@ -268,15 +268,15 @@
         27: aload_0
         28: aload         6
         30: putfield      #6                  // Field val$iface:Ljava/lang/Class;
         33: aload_0
         34: invokespecial #7                  // Method java/lang/Object."<init>":()V
         37: return
       LineNumberTable:
-        line 8485: 0
+        line 8709: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      38     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$3;
             0      38     1 this$1   Lcom/deshaw/pjrmi/PJRmi$Connection;
     MethodParameters:
       Name                           Flags
       this$1                         final mandated
@@ -458,53 +458,53 @@
        363: invokedynamic #39,  0             // InvokeDynamic #4:makeConcatWithConstants:(Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
        368: invokespecial #40                 // Method java/lang/reflect/InvocationTargetException."<init>":(Ljava/lang/Throwable;Ljava/lang/String;)V
        371: athrow
       Exception table:
          from    to  target type
            235   279   280   Class java/lang/Throwable
       LineNumberTable:
-        line 8494: 0
-        line 8499: 17
-        line 8500: 20
-        line 8502: 26
-        line 8507: 33
-        line 8508: 42
-        line 8510: 47
-        line 8513: 59
-        line 8515: 64
-        line 8516: 70
-        line 8517: 76
-        line 8524: 88
-        line 8525: 94
-        line 8535: 97
-        line 8536: 101
-        line 8537: 109
-        line 8538: 127
-        line 8541: 133
-        line 8545: 143
-        line 8553: 162
-        line 8554: 176
-        line 8555: 188
-        line 8559: 199
-        line 8561: 220
-        line 8568: 235
-        line 8569: 242
-        line 8571: 261
-        line 8568: 279
-        line 8575: 280
-        line 8578: 282
-        line 8579: 287
-        line 8582: 294
-        line 8583: 298
-        line 8587: 308
-        line 8590: 314
-        line 8592: 335
-        line 8593: 342
-        line 8595: 349
-        line 8597: 356
+        line 8718: 0
+        line 8723: 17
+        line 8724: 20
+        line 8726: 26
+        line 8731: 33
+        line 8732: 42
+        line 8734: 47
+        line 8737: 59
+        line 8739: 64
+        line 8740: 70
+        line 8741: 76
+        line 8748: 88
+        line 8749: 94
+        line 8759: 97
+        line 8760: 101
+        line 8761: 109
+        line 8762: 127
+        line 8765: 133
+        line 8769: 143
+        line 8777: 162
+        line 8778: 176
+        line 8779: 188
+        line 8783: 199
+        line 8785: 220
+        line 8792: 235
+        line 8793: 242
+        line 8795: 261
+        line 8792: 279
+        line 8799: 280
+        line 8802: 282
+        line 8803: 287
+        line 8806: 294
+        line 8807: 298
+        line 8811: 308
+        line 8814: 314
+        line 8816: 335
+        line 8817: 342
+        line 8819: 349
+        line 8821: 356
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            20       6     4 callInst   Ljava/lang/Object;
            23       3     5 callArgs   [Ljava/lang/Object;
            64      24     4 callInst   Ljava/lang/Object;
            85       3     5 callArgs   [Ljava/lang/Object;
           291       3     9  inst   Ljava/lang/String;
```

#### com/deshaw/pjrmi/PJRmi$Connection$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum de855b89b059b6f4678ae268abff790e000e9f5a199f3a2457a0de76eec89e04
+  SHA-256 checksum 44fde6e8b812c31e2345a17712640f02f7b5014ca828d3687ac271af3d793f5b
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$2 extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<com.deshaw.pjrmi.PJRmi$TypeDescription>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #7                          // com/deshaw/pjrmi/PJRmi$Connection$2
   super_class: #8                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -97,15 +97,15 @@
         11: aload_0
         12: aload_1
         13: iload_2
         14: aload_3
         15: invokespecial #3                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         18: return
       LineNumberTable:
-        line 8047: 0
+        line 8260: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$2;
             0      19     1 this$1   Lcom/deshaw/pjrmi/PJRmi$Connection;
             0      19     2 functionId   I
             0      19     3   out   Ljava/io/DataOutputStream;
     MethodParameters:
@@ -125,15 +125,15 @@
          4: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #5                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: aload_0
         11: getfield      #2                  // Field val$klass:Ljava/lang/Class;
         14: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         17: areturn
       LineNumberTable:
-        line 8050: 0
+        line 8263: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$2;
 }
 Signature: #34                          // Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback<Lcom/deshaw/pjrmi/PJRmi$TypeDescription;>;
 SourceFile: "PJRmi.java"
 EnclosingMethod: #12.#38                // com.deshaw.pjrmi.PJRmi$Connection.handleGetCallbackHandle
```

#### com/deshaw/pjrmi/PJRmi$Connection$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum eb2a40d3b828e8669d2e2ff31e3a68b6da3a842e9fa03688abd9532173bef5f5
+  SHA-256 checksum 52b393a5f0357c1d7612f9b3689a4b2ee751ed3bce5645c50510ebed8f93c4d4
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$1 extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<com.deshaw.pjrmi.PJRmi$TypeDescription>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #7                          // com/deshaw/pjrmi/PJRmi$Connection$1
   super_class: #8                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -87,15 +87,15 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 8001: 0
+        line 8214: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$1;
             0      13     1 this$1   Lcom/deshaw/pjrmi/PJRmi$Connection;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
     MethodParameters:
@@ -113,15 +113,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class com/deshaw/pjrmi/PythonKwargsFunction
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 8004: 0
+        line 8217: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$1;
 }
 Signature: #32                          // Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback<Lcom/deshaw/pjrmi/PJRmi$TypeDescription;>;
 SourceFile: "PJRmi.java"
 EnclosingMethod: #10.#36                // com.deshaw.pjrmi.PJRmi$Connection.handleGetCallbackHandle
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4b799d98a1c5f271d5fd056afd65695ed2dacc4a6bc6819df7edbf8a46d3c9d0
+  SHA-256 checksum 3010ee8d6fa0db8ab78fe0b6da23c955f7d986eb32abd2b5bd67490399dfb027
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonObjectImpl extends com.deshaw.pjrmi.PythonObject
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #67                         // com/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl
   super_class: #30                        // com/deshaw/pjrmi/PythonObject
@@ -399,22 +399,22 @@
         57: ldc2_w        #13                 // long -1l
         60: iconst_m1
         61: aload         5
         63: getfield      #15                 // Field com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.bytes:Ljava/io/ByteArrayOutputStream;
         66: invokevirtual #16                 // Method com/deshaw/pjrmi/PJRmi$Connection.sendMessage:(Ljava/io/DataOutputStream;Lcom/deshaw/pjrmi/PJRmi$MessageType;JILjava/io/ByteArrayOutputStream;)V
         69: return
       LineNumberTable:
-        line 4673: 0
-        line 4675: 9
-        line 4676: 14
-        line 4677: 19
-        line 4680: 25
-        line 4681: 36
-        line 4682: 49
-        line 4687: 69
+        line 4823: 0
+        line 4825: 9
+        line 4826: 14
+        line 4827: 19
+        line 4830: 25
+        line 4831: 36
+        line 4832: 49
+        line 4837: 69
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      70     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
             0      70     2  name   Ljava/lang/String;
             0      70     3 objectId   I
             0      70     4   out   Ljava/io/DataOutputStream;
            36      34     5 bados   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
@@ -599,51 +599,51 @@
        411: invokevirtual #16                 // Method com/deshaw/pjrmi/PJRmi$Connection.sendMessage:(Ljava/io/DataOutputStream;Lcom/deshaw/pjrmi/PJRmi$MessageType;JILjava/io/ByteArrayOutputStream;)V
        414: aload_0
        415: getfield      #2                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
        418: aload         11
        420: invokevirtual #51                 // Method com/deshaw/pjrmi/PJRmi$Connection.awaitCallbackReponse:(Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;)Ljava/lang/Object;
        423: areturn
       LineNumberTable:
-        line 4700: 0
-        line 4701: 12
-        line 4703: 19
-        line 4701: 28
-        line 4710: 31
-        line 4711: 36
-        line 4712: 44
-        line 4713: 57
-        line 4716: 62
-        line 4722: 74
-        line 4723: 84
-        line 4724: 93
-        line 4723: 94
-        line 4727: 99
-        line 4728: 110
-        line 4729: 120
-        line 4730: 132
-        line 4731: 142
-        line 4734: 151
-        line 4735: 156
-        line 4738: 168
-        line 4739: 179
-        line 4740: 205
-        line 4739: 219
-        line 4745: 225
-        line 4746: 229
-        line 4749: 241
-        line 4750: 255
-        line 4752: 290
-        line 4753: 308
-        line 4754: 327
-        line 4758: 330
-        line 4759: 345
-        line 4762: 365
-        line 4763: 377
-        line 4768: 392
-        line 4775: 414
+        line 4850: 0
+        line 4851: 12
+        line 4853: 19
+        line 4851: 28
+        line 4860: 31
+        line 4861: 36
+        line 4862: 44
+        line 4863: 57
+        line 4866: 62
+        line 4872: 74
+        line 4873: 84
+        line 4874: 93
+        line 4873: 94
+        line 4877: 99
+        line 4878: 110
+        line 4879: 120
+        line 4880: 132
+        line 4881: 142
+        line 4884: 151
+        line 4885: 156
+        line 4888: 168
+        line 4889: 179
+        line 4890: 205
+        line 4889: 219
+        line 4895: 225
+        line 4896: 229
+        line 4899: 241
+        line 4900: 255
+        line 4902: 290
+        line 4903: 308
+        line 4904: 327
+        line 4908: 330
+        line 4909: 345
+        line 4912: 365
+        line 4913: 377
+        line 4918: 392
+        line 4925: 414
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           205      14    14   arg   Ljava/lang/Object;
           290      37    12 entry   Ljava/util/Map$Entry;
             0     424     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
             0     424     1 returnType   Ljava/lang/Class;
             0     424     2 methodName   Ljava/lang/String;
@@ -807,38 +807,38 @@
        237: aload         10
        239: invokevirtual #55                 // Method com/deshaw/pjrmi/PythonCallbackException.getCause:()Ljava/lang/Throwable;
        242: athrow
       Exception table:
          from    to  target type
            225   234   235   Class com/deshaw/pjrmi/PythonCallbackException
       LineNumberTable:
-        line 4787: 0
-        line 4788: 12
-        line 4792: 25
-        line 4793: 29
-        line 4794: 36
-        line 4795: 48
-        line 4798: 53
-        line 4802: 65
-        line 4803: 75
-        line 4804: 84
-        line 4803: 85
-        line 4807: 90
-        line 4808: 101
-        line 4809: 111
-        line 4810: 123
-        line 4811: 133
-        line 4814: 142
-        line 4815: 156
-        line 4818: 176
-        line 4819: 188
-        line 4824: 203
-        line 4832: 225
-        line 4834: 235
-        line 4835: 237
+        line 4937: 0
+        line 4938: 12
+        line 4942: 25
+        line 4943: 29
+        line 4944: 36
+        line 4945: 48
+        line 4948: 53
+        line 4952: 65
+        line 4953: 75
+        line 4954: 84
+        line 4953: 85
+        line 4957: 90
+        line 4958: 101
+        line 4959: 111
+        line 4960: 123
+        line 4961: 133
+        line 4964: 142
+        line 4965: 156
+        line 4968: 176
+        line 4969: 188
+        line 4974: 203
+        line 4982: 225
+        line 4984: 235
+        line 4985: 237
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           237       6    10     e   Lcom/deshaw/pjrmi/PythonCallbackException;
             0     243     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
             0     243     1 fieldType   Ljava/lang/Class;
             0     243     2 fieldName   Ljava/lang/String;
            29     214     3 thread   Ljava/lang/Thread;
@@ -899,17 +899,17 @@
         21: getfield      #5                  // Field myObjectId:I
         24: aload_0
         25: getfield      #6                  // Field myOut:Ljava/io/DataOutputStream;
         28: invokespecial #59                 // Method com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         31: invokestatic  #60                 // Method java/lang/reflect/Proxy.newProxyInstance:(Ljava/lang/ClassLoader;[Ljava/lang/Class;Ljava/lang/reflect/InvocationHandler;)Ljava/lang/Object;
         34: areturn
       LineNumberTable:
-        line 4847: 0
-        line 4848: 1
-        line 4847: 31
+        line 4997: 0
+        line 4998: 1
+        line 4997: 31
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      35     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
             0      35     1 klass   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      35     1 klass   Ljava/lang/Class<TT;>;
@@ -937,17 +937,17 @@
         17: aload_0
         18: getfield      #4                  // Field myName:Ljava/lang/String;
         21: areturn
       Exception table:
          from    to  target type
              0    15    16   Class java/lang/Throwable
       LineNumberTable:
-        line 4862: 0
-        line 4864: 16
-        line 4866: 17
+        line 5012: 0
+        line 5014: 16
+        line 5016: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            17       5     1     t   Ljava/lang/Throwable;
             0      22     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
       StackMapTable: number_of_entries = 1
         frame_type = 80 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
@@ -957,15 +957,15 @@
     flags: (0x0004) ACC_PROTECTED
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #5                  // Field myObjectId:I
          4: ireturn
       LineNumberTable:
-        line 4875: 0
+        line 5025: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
 
   protected void finalize() throws java.lang.Throwable;
     descriptor: ()V
     flags: (0x0004) ACC_PROTECTED
@@ -1004,23 +1004,23 @@
         64: aload_2
         65: athrow
         66: return
       Exception table:
          from    to  target type
              0    52    59   any
       LineNumberTable:
-        line 4888: 0
-        line 4889: 10
-        line 4890: 18
-        line 4891: 30
-        line 4898: 52
-        line 4899: 56
-        line 4898: 59
-        line 4899: 64
-        line 4900: 66
+        line 5038: 0
+        line 5039: 10
+        line 5040: 18
+        line 5041: 30
+        line 5048: 52
+        line 5049: 56
+        line 5048: 59
+        line 5049: 64
+        line 5050: 66
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            10      42     1 bados   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
             0      67     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonObjectImpl;
       StackMapTable: number_of_entries = 2
         frame_type = 123 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bd9af27148c5e5f4f6bbf4fe3a1470cc360ac96596c0c6a3f60847bea91ebd39
+  SHA-256 checksum a12cc985c05cbcbe22b8296c36384bd8bb85f7c7b32d6120024fa8421be64564
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonProxyHandler implements java.lang.reflect.InvocationHandler
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #37                         // com/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler
   super_class: #81                        // java/lang/Object
@@ -431,21 +431,21 @@
         51: ldc2_w        #12                 // long -1l
         54: iconst_m1
         55: aload         4
         57: getfield      #14                 // Field com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.bytes:Ljava/io/ByteArrayOutputStream;
         60: invokevirtual #15                 // Method com/deshaw/pjrmi/PJRmi$Connection.sendMessage:(Ljava/io/DataOutputStream;Lcom/deshaw/pjrmi/PJRmi$MessageType;JILjava/io/ByteArrayOutputStream;)V
         63: return
       LineNumberTable:
-        line 4452: 0
-        line 4454: 9
-        line 4455: 14
-        line 4458: 19
-        line 4459: 30
-        line 4460: 43
-        line 4465: 63
+        line 4602: 0
+        line 4604: 9
+        line 4605: 14
+        line 4608: 19
+        line 4609: 30
+        line 4610: 43
+        line 4615: 63
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      64     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler;
             0      64     2 objectId   I
             0      64     3   out   Ljava/io/DataOutputStream;
            30      34     4 bados   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
     Exceptions:
@@ -728,79 +728,79 @@
        607: areturn
        608: aload         10
        610: athrow
       Exception table:
          from    to  target type
            519   528   529   Class com/deshaw/pjrmi/PythonCallbackException
       LineNumberTable:
-        line 4477: 0
-        line 4479: 12
-        line 4480: 16
-        line 4485: 23
-        line 4486: 34
-        line 4487: 44
-        line 4488: 49
-        line 4490: 57
-        line 4491: 63
-        line 4492: 68
-        line 4495: 79
-        line 4496: 91
-        line 4497: 96
-        line 4486: 100
-        line 4500: 106
-        line 4501: 114
-        line 4503: 121
-        line 4504: 126
-        line 4503: 136
-        line 4511: 139
-        line 4516: 170
-        line 4517: 178
-        line 4518: 186
-        line 4519: 193
-        line 4520: 205
-        line 4521: 210
-        line 4520: 218
-        line 4524: 221
-        line 4529: 242
-        line 4530: 247
-        line 4531: 255
-        line 4532: 268
-        line 4535: 273
-        line 4538: 285
-        line 4539: 296
-        line 4540: 306
-        line 4541: 318
-        line 4542: 343
-        line 4545: 355
-        line 4546: 359
-        line 4549: 371
-        line 4550: 381
-        line 4551: 406
-        line 4550: 420
-        line 4556: 426
-        line 4559: 435
-        line 4560: 450
-        line 4563: 470
-        line 4564: 482
-        line 4569: 497
-        line 4577: 519
-        line 4579: 529
-        line 4582: 531
-        line 4583: 543
-        line 4587: 549
-        line 4588: 555
-        line 4589: 565
-        line 4590: 569
-        line 4591: 574
-        line 4592: 580
-        line 4593: 591
-        line 4594: 600
-        line 4595: 604
-        line 4593: 607
-        line 4599: 608
+        line 4627: 0
+        line 4629: 12
+        line 4630: 16
+        line 4635: 23
+        line 4636: 34
+        line 4637: 44
+        line 4638: 49
+        line 4640: 57
+        line 4641: 63
+        line 4642: 68
+        line 4645: 79
+        line 4646: 91
+        line 4647: 96
+        line 4636: 100
+        line 4650: 106
+        line 4651: 114
+        line 4653: 121
+        line 4654: 126
+        line 4653: 136
+        line 4661: 139
+        line 4666: 170
+        line 4667: 178
+        line 4668: 186
+        line 4669: 193
+        line 4670: 205
+        line 4671: 210
+        line 4670: 218
+        line 4674: 221
+        line 4679: 242
+        line 4680: 247
+        line 4681: 255
+        line 4682: 268
+        line 4685: 273
+        line 4688: 285
+        line 4689: 296
+        line 4690: 306
+        line 4691: 318
+        line 4692: 343
+        line 4695: 355
+        line 4696: 359
+        line 4699: 371
+        line 4700: 381
+        line 4701: 406
+        line 4700: 420
+        line 4706: 426
+        line 4709: 435
+        line 4710: 450
+        line 4713: 470
+        line 4714: 482
+        line 4719: 497
+        line 4727: 519
+        line 4729: 529
+        line 4732: 531
+        line 4733: 543
+        line 4737: 549
+        line 4738: 555
+        line 4739: 565
+        line 4740: 569
+        line 4741: 574
+        line 4742: 580
+        line 4743: 591
+        line 4744: 600
+        line 4745: 604
+        line 4743: 607
+        line 4749: 608
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            20       3     4 argString   Ljava/lang/String;
            63      37     7   arg   Ljava/lang/Object;
            37      69     6     i   I
            34      87     5    sb   Ljava/lang/StringBuilder;
           121      18     4 argString   Ljava/lang/String;
@@ -917,23 +917,23 @@
         64: aload_2
         65: athrow
         66: return
       Exception table:
          from    to  target type
              0    52    59   any
       LineNumberTable:
-        line 4613: 0
-        line 4614: 10
-        line 4615: 18
-        line 4616: 30
-        line 4623: 52
-        line 4624: 56
-        line 4623: 59
-        line 4624: 64
-        line 4625: 66
+        line 4763: 0
+        line 4764: 10
+        line 4765: 18
+        line 4766: 30
+        line 4773: 52
+        line 4774: 56
+        line 4773: 59
+        line 4774: 64
+        line 4775: 66
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            10      42     1 bados   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
             0      67     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler;
       StackMapTable: number_of_entries = 2
         frame_type = 123 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
@@ -946,15 +946,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field myObjectId:I
          4: ireturn
       LineNumberTable:
-        line 4632: 0
+        line 4782: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler;
 
   private java.lang.String toLocalString();
     descriptor: ()Ljava/lang/String;
     flags: (0x0002) ACC_PRIVATE
@@ -964,15 +964,15 @@
          1: invokevirtual #25                 // Method java/lang/Object.getClass:()Ljava/lang/Class;
          4: invokevirtual #78                 // Method java/lang/Class.getSimpleName:()Ljava/lang/String;
          7: aload_0
          8: invokevirtual #79                 // Method getId:()I
         11: invokedynamic #80,  0             // InvokeDynamic #3:makeConcatWithConstants:(Ljava/lang/String;I)Ljava/lang/String;
         16: areturn
       LineNumberTable:
-        line 4640: 0
+        line 4790: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonProxyHandler;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum f7b8c689be6bc353da7debc659cbfc68a4aafaa2d30e6ca3751916c75e4a66b0
+  SHA-256 checksum ed7deb3607ff0b1f18cb4bf325d24b99e5e68c09544d795fb1b1e00090488273
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonLambdaHandler implements java.lang.reflect.InvocationHandler
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #23                         // com/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler
   super_class: #69                        // java/lang/Object
@@ -362,19 +362,19 @@
         15: iload_3
         16: putfield      #5                  // Field myFunctionId:I
         19: aload_0
         20: aload         4
         22: putfield      #6                  // Field myOut:Ljava/io/DataOutputStream;
         25: return
       LineNumberTable:
-        line 4297: 0
-        line 4298: 9
-        line 4299: 14
-        line 4300: 19
-        line 4301: 25
+        line 4447: 0
+        line 4448: 9
+        line 4449: 14
+        line 4450: 19
+        line 4451: 25
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler;
             0      26     2 methodName   Ljava/lang/String;
             0      26     3 functionId   I
             0      26     4   out   Ljava/io/DataOutputStream;
     MethodParameters:
@@ -683,67 +683,67 @@
        714: new           #66                 // class java/lang/IllegalArgumentException
        717: dup
        718: aload_2
        719: invokedynamic #67,  0             // InvokeDynamic #3:makeConcatWithConstants:(Ljava/lang/reflect/Method;)Ljava/lang/String;
        724: invokespecial #68                 // Method java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
        727: athrow
       LineNumberTable:
-        line 4313: 0
-        line 4314: 12
-        line 4315: 17
-        line 4314: 25
-        line 4319: 28
-        line 4321: 264
-        line 4322: 279
-        line 4323: 287
-        line 4324: 294
-        line 4328: 330
-        line 4333: 335
-        line 4336: 340
-        line 4339: 356
-        line 4340: 360
-        line 4343: 362
-        line 4344: 366
-        line 4347: 368
-        line 4350: 378
-        line 4351: 382
-        line 4356: 384
-        line 4359: 391
-        line 4360: 397
-        line 4361: 407
-        line 4362: 411
-        line 4363: 416
-        line 4364: 422
-        line 4365: 433
-        line 4366: 442
-        line 4367: 446
-        line 4365: 449
-        line 4369: 450
-        line 4371: 464
-        line 4372: 469
-        line 4373: 477
-        line 4374: 490
-        line 4377: 495
-        line 4380: 507
-        line 4381: 518
-        line 4382: 528
-        line 4383: 540
-        line 4384: 544
-        line 4387: 556
-        line 4388: 566
-        line 4389: 591
-        line 4388: 605
-        line 4394: 611
-        line 4397: 620
-        line 4398: 635
-        line 4401: 655
-        line 4402: 667
-        line 4407: 682
-        line 4414: 704
-        line 4421: 714
+        line 4463: 0
+        line 4464: 12
+        line 4465: 17
+        line 4464: 25
+        line 4469: 28
+        line 4471: 264
+        line 4472: 279
+        line 4473: 287
+        line 4474: 294
+        line 4478: 330
+        line 4483: 335
+        line 4486: 340
+        line 4489: 356
+        line 4490: 360
+        line 4493: 362
+        line 4494: 366
+        line 4497: 368
+        line 4500: 378
+        line 4501: 382
+        line 4506: 384
+        line 4509: 391
+        line 4510: 397
+        line 4511: 407
+        line 4512: 411
+        line 4513: 416
+        line 4514: 422
+        line 4515: 433
+        line 4516: 442
+        line 4517: 446
+        line 4515: 449
+        line 4519: 450
+        line 4521: 464
+        line 4522: 469
+        line 4523: 477
+        line 4524: 490
+        line 4527: 495
+        line 4530: 507
+        line 4531: 518
+        line 4532: 528
+        line 4533: 540
+        line 4534: 544
+        line 4537: 556
+        line 4538: 566
+        line 4539: 591
+        line 4538: 605
+        line 4544: 611
+        line 4547: 620
+        line 4548: 635
+        line 4551: 655
+        line 4552: 667
+        line 4557: 682
+        line 4564: 704
+        line 4571: 714
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           294      36     7   plh   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonLambdaHandler;
           279      56     6  that   Ljava/lang/Object;
           397      53     4 klass   Ljava/lang/Class;
           407      43     5 lookup   Ljava/lang/invoke/MethodHandles$Lookup;
           416      34     6 allowedModes   Ljava/lang/reflect/Field;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0ec8d3fab15eca615b419a8b056babb21d9800d5693081b6ef6d02475375bfa6
+  SHA-256 checksum 11599fd3dca601f04592d0c430726b75475166a5357cd16835675655c3351566
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackBiPredicate<T extends java.lang.Object, U extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<java.lang.Object> implements java.util.function.BiPredicate<T, U>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #21                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate
   super_class: #22                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -135,17 +135,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 4223: 0
-        line 4224: 5
-        line 4225: 12
+        line 4373: 0
+        line 4374: 5
+        line 4375: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -165,15 +165,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/BiPredicate
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 4233: 0
+        line 4383: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate<TT;TU;>;
 
@@ -254,27 +254,27 @@
             55    79    90   Class com/deshaw/pjrmi/PythonCallbackException
             80    89    90   Class com/deshaw/pjrmi/PythonCallbackException
              0    31   105   Class java/lang/Throwable
             32    54   105   Class java/lang/Throwable
             55    79   105   Class java/lang/Throwable
             80    89   105   Class java/lang/Throwable
       LineNumberTable:
-        line 4245: 0
-        line 4246: 17
-        line 4247: 24
-        line 4249: 32
-        line 4250: 39
-        line 4252: 55
-        line 4253: 62
-        line 4256: 80
-        line 4259: 90
-        line 4260: 91
-        line 4261: 98
-        line 4263: 105
-        line 4264: 106
+        line 4395: 0
+        line 4396: 17
+        line 4397: 24
+        line 4399: 32
+        line 4400: 39
+        line 4402: 55
+        line 4403: 62
+        line 4406: 80
+        line 4409: 90
+        line 4410: 91
+        line 4411: 98
+        line 4413: 105
+        line 4414: 106
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            17      73     3 result   Ljava/lang/Object;
            91      14     3     e   Lcom/deshaw/pjrmi/PythonCallbackException;
           106      11     3     t   Ljava/lang/Throwable;
             0     117     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiPredicate;
             0     117     1  arg1   Ljava/lang/Object;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0409241684652b4eab3e20cd3f77fbcce11830c84ce479a1090bbb33bf0afc1a
+  SHA-256 checksum 4d1cf997ca5f5c9218093aa78c94ebb7f235a4af1e5a6e1753bf77706a911709
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackPredicate<T extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<java.lang.Object> implements java.util.function.Predicate<T>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #21                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate
   super_class: #22                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -133,17 +133,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 4164: 0
-        line 4165: 5
-        line 4166: 12
+        line 4314: 0
+        line 4315: 5
+        line 4316: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -163,15 +163,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/Predicate
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 4174: 0
+        line 4324: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate<TT;>;
 
@@ -248,27 +248,27 @@
             51    75    86   Class com/deshaw/pjrmi/PythonCallbackException
             76    85    86   Class com/deshaw/pjrmi/PythonCallbackException
              0    27   101   Class java/lang/Throwable
             28    50   101   Class java/lang/Throwable
             51    75   101   Class java/lang/Throwable
             76    85   101   Class java/lang/Throwable
       LineNumberTable:
-        line 4186: 0
-        line 4187: 13
-        line 4188: 20
-        line 4190: 28
-        line 4191: 35
-        line 4193: 51
-        line 4194: 58
-        line 4197: 76
-        line 4200: 86
-        line 4201: 87
-        line 4202: 94
-        line 4204: 101
-        line 4205: 102
+        line 4336: 0
+        line 4337: 13
+        line 4338: 20
+        line 4340: 28
+        line 4341: 35
+        line 4343: 51
+        line 4344: 58
+        line 4347: 76
+        line 4350: 86
+        line 4351: 87
+        line 4352: 94
+        line 4354: 101
+        line 4355: 102
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            13      73     2 result   Ljava/lang/Object;
            87      14     2     e   Lcom/deshaw/pjrmi/PythonCallbackException;
           102      11     2     t   Ljava/lang/Throwable;
             0     113     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackPredicate;
             0     113     1   arg   Ljava/lang/Object;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4b5da58c319b87631e0a3ed25862e792dea65d28db111ad113af0a508cbc632e
+  SHA-256 checksum 27f693efb6becb2b37cd918da19955ead61523d73d9d72aebe483b3144d9a3e5
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackBiConsumer<T extends java.lang.Object, U extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<java.lang.Object> implements java.util.function.BiConsumer<T, U>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -117,17 +117,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 4120: 0
-        line 4121: 5
-        line 4122: 12
+        line 4270: 0
+        line 4271: 5
+        line 4272: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -147,15 +147,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/BiConsumer
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 4130: 0
+        line 4280: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer<TT;TU;>;
 
@@ -195,22 +195,22 @@
         46: athrow
         47: return
       Exception table:
          from    to  target type
              0    17    20   Class com/deshaw/pjrmi/PythonCallbackException
              0    17    35   Class java/lang/Throwable
       LineNumberTable:
-        line 4140: 0
-        line 4148: 17
-        line 4142: 20
-        line 4143: 21
-        line 4144: 28
-        line 4146: 35
-        line 4147: 36
-        line 4149: 47
+        line 4290: 0
+        line 4298: 17
+        line 4292: 20
+        line 4293: 21
+        line 4294: 28
+        line 4296: 35
+        line 4297: 36
+        line 4299: 47
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            21      14     3     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            36      11     3     t   Ljava/lang/Throwable;
             0      48     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiConsumer;
             0      48     1  arg1   Ljava/lang/Object;
             0      48     2  arg2   Ljava/lang/Object;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 93e1723c4c259ae2419fd7815e9d8220c54ed214ff2140929495552e20e5c6e3
+  SHA-256 checksum 12ba842f09a9255ddea9d49cfa4b47a8ad15bcd53ae1216f3beb7dab1dcb6e9f
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackConsumer<T extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<java.lang.Object> implements java.util.function.Consumer<T>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -115,17 +115,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 4076: 0
-        line 4077: 5
-        line 4078: 12
+        line 4226: 0
+        line 4227: 5
+        line 4228: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -145,15 +145,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/Consumer
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 4086: 0
+        line 4236: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer<TT;>;
 
@@ -189,22 +189,22 @@
         42: athrow
         43: return
       Exception table:
          from    to  target type
              0    13    16   Class com/deshaw/pjrmi/PythonCallbackException
              0    13    31   Class java/lang/Throwable
       LineNumberTable:
-        line 4096: 0
-        line 4104: 13
-        line 4098: 16
-        line 4099: 17
-        line 4100: 24
-        line 4102: 31
-        line 4103: 32
-        line 4105: 43
+        line 4246: 0
+        line 4254: 13
+        line 4248: 16
+        line 4249: 17
+        line 4250: 24
+        line 4252: 31
+        line 4253: 32
+        line 4255: 43
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            17      14     2     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            32      11     2     t   Ljava/lang/Throwable;
             0      44     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackConsumer;
             0      44     1   arg   Ljava/lang/Object;
       LocalVariableTypeTable:
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum a1e750578ad666eca18958652d8d9abd504bf5f13776001e957853ca7e57d59b
+  SHA-256 checksum 60cd9948f7379ebd971debc64dcfa9ca5da6a6ac1fa67db4b758517d640b9f7b
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackBiFunction<T extends java.lang.Object, R extends java.lang.Object, U extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<R> implements java.util.function.BiFunction<T, U, R>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -117,17 +117,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 4032: 0
-        line 4033: 5
-        line 4034: 12
+        line 4182: 0
+        line 4183: 5
+        line 4184: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -147,15 +147,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/BiFunction
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 4042: 0
+        line 4192: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction<TT;TR;TU;>;
 
@@ -193,20 +193,20 @@
         40: invokespecial #13                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/String;Ljava/lang/Throwable;)V
         43: athrow
       Exception table:
          from    to  target type
              0    16    17   Class com/deshaw/pjrmi/PythonCallbackException
              0    16    32   Class java/lang/Throwable
       LineNumberTable:
-        line 4052: 0
-        line 4054: 17
-        line 4055: 18
-        line 4056: 25
-        line 4058: 32
-        line 4059: 33
+        line 4202: 0
+        line 4204: 17
+        line 4205: 18
+        line 4206: 25
+        line 4208: 32
+        line 4209: 33
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            18      14     3     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            33      11     3     t   Ljava/lang/Throwable;
             0      44     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackBiFunction;
             0      44     1  arg1   Ljava/lang/Object;
             0      44     2  arg2   Ljava/lang/Object;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4284f8e42f63c7a1a092f43f3d9cc4f87cac941f198ccfafb89bcc86180bcfc7
+  SHA-256 checksum ebee0e8cc9d1db33ae15de96630dbc847dbf35c4e77bc92d16fce330d2a31fc1
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackFunction<T extends java.lang.Object, R extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<R> implements java.util.function.Function<T, R>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -115,17 +115,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 3988: 0
-        line 3989: 5
-        line 3990: 12
+        line 4138: 0
+        line 4139: 5
+        line 4140: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -145,15 +145,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/Function
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 3998: 0
+        line 4148: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction<TT;TR;>;
 
@@ -187,20 +187,20 @@
         36: invokespecial #13                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/String;Ljava/lang/Throwable;)V
         39: athrow
       Exception table:
          from    to  target type
              0    12    13   Class com/deshaw/pjrmi/PythonCallbackException
              0    12    28   Class java/lang/Throwable
       LineNumberTable:
-        line 4008: 0
-        line 4010: 13
-        line 4011: 14
-        line 4012: 21
-        line 4014: 28
-        line 4015: 29
+        line 4158: 0
+        line 4160: 13
+        line 4161: 14
+        line 4162: 21
+        line 4164: 28
+        line 4165: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            14      14     2     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            29      11     2     t   Ljava/lang/Throwable;
             0      40     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackFunction;
             0      40     1   arg   Ljava/lang/Object;
       LocalVariableTypeTable:
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c277c11f22b2046d53a5975e8281118fe9b55a4bd6fe71a8b91ceaa8679000df
+  SHA-256 checksum deb013ac00b32012eff7143d4534f442ed2a90154dcc473ae392110ad389e375
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackUnaryOperator<T extends java.lang.Object> extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<T> implements java.util.function.UnaryOperator<T>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -115,17 +115,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 3944: 0
-        line 3945: 5
-        line 3946: 12
+        line 4094: 0
+        line 4095: 5
+        line 4096: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -145,15 +145,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/util/function/UnaryOperator
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 3954: 0
+        line 4104: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator<TT;>;
 
@@ -187,20 +187,20 @@
         36: invokespecial #13                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/String;Ljava/lang/Throwable;)V
         39: athrow
       Exception table:
          from    to  target type
              0    12    13   Class com/deshaw/pjrmi/PythonCallbackException
              0    12    28   Class java/lang/Throwable
       LineNumberTable:
-        line 3964: 0
-        line 3966: 13
-        line 3967: 14
-        line 3968: 21
-        line 3970: 28
-        line 3971: 29
+        line 4114: 0
+        line 4116: 13
+        line 4117: 14
+        line 4118: 21
+        line 4120: 28
+        line 4121: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            14      14     2     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            29      11     2     t   Ljava/lang/Throwable;
             0      40     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackUnaryOperator;
             0      40     1   arg   Ljava/lang/Object;
       LocalVariableTypeTable:
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6307de6970929cbd8054880052a95907c2118962d7dd28c68516a5769c0aa8ce
+  SHA-256 checksum ea6266cfaca599fd51d63f59d939a944a400d13a229962e4911775d3618ac079
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackRunnable extends com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<java.lang.Object> implements java.lang.Runnable
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #15                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable
   super_class: #16                        // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
@@ -109,17 +109,17 @@
          5: aload_0
          6: aload_1
          7: iload_2
          8: aload_3
          9: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$Connection$PythonCallback."<init>":(Lcom/deshaw/pjrmi/PJRmi$Connection;ILjava/io/DataOutputStream;)V
         12: return
       LineNumberTable:
-        line 3900: 0
-        line 3901: 5
-        line 3902: 12
+        line 4050: 0
+        line 4051: 5
+        line 4052: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable;
             0      13     2 functionId   I
             0      13     3   out   Ljava/io/DataOutputStream;
     MethodParameters:
       Name                           Flags
@@ -136,15 +136,15 @@
          1: getfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          4: getfield      #3                  // Field com/deshaw/pjrmi/PJRmi$Connection.this$0:Lcom/deshaw/pjrmi/PJRmi;
          7: getfield      #4                  // Field com/deshaw/pjrmi/PJRmi.myTypeMapping:Lcom/deshaw/pjrmi/PJRmi$TypeMapping;
         10: ldc           #5                  // class java/lang/Runnable
         12: invokevirtual #6                  // Method com/deshaw/pjrmi/PJRmi$TypeMapping.getDescription:(Ljava/lang/Class;)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
         15: areturn
       LineNumberTable:
-        line 3910: 0
+        line 4060: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable;
 
   public void run();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
@@ -173,22 +173,22 @@
         38: athrow
         39: return
       Exception table:
          from    to  target type
              0     9    12   Class com/deshaw/pjrmi/PythonCallbackException
              0     9    27   Class java/lang/Throwable
       LineNumberTable:
-        line 3920: 0
-        line 3928: 9
-        line 3922: 12
-        line 3923: 13
-        line 3924: 20
-        line 3926: 27
-        line 3927: 28
-        line 3929: 39
+        line 4070: 0
+        line 4078: 9
+        line 4072: 12
+        line 4073: 13
+        line 4074: 20
+        line 4076: 27
+        line 4077: 28
+        line 4079: 39
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            13      14     1     e   Lcom/deshaw/pjrmi/PythonCallbackException;
            28      11     1     t   Ljava/lang/Throwable;
             0      40     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackRunnable;
       StackMapTable: number_of_entries = 3
         frame_type = 76 /* same_locals_1_stack_item */
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallback.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 979f9bfd9412f807a03472f74389eb3f408b33a26b22115ab971c97647a3e6a2
+  SHA-256 checksum 006955abaa21e43ef99b1fbfa4c6e0afe9f8cb16e6d938197d5d2eb08516ed4b
   Compiled from "PJRmi.java"
 abstract class com.deshaw.pjrmi.PJRmi$Connection$PythonCallback<T extends java.lang.Object> extends java.lang.Object implements com.deshaw.pjrmi.PythonKwargsFunction<T>
   minor version: 0
   major version: 55
   flags: (0x0420) ACC_SUPER, ACC_ABSTRACT
   this_class: #49                         // com/deshaw/pjrmi/PJRmi$Connection$PythonCallback
   super_class: #50                        // java/lang/Object
@@ -310,18 +310,18 @@
         10: iload_2
         11: putfield      #4                  // Field myFunctionId:I
         14: aload_0
         15: aload_3
         16: putfield      #5                  // Field myOut:Ljava/io/DataOutputStream;
         19: return
       LineNumberTable:
-        line 3784: 0
-        line 3785: 9
-        line 3786: 14
-        line 3787: 19
+        line 3934: 0
+        line 3935: 9
+        line 3936: 14
+        line 3937: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback;
             0      20     2 functionId   I
             0      20     3   out   Ljava/io/DataOutputStream;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -343,15 +343,15 @@
       stack=3, locals=3, args_size=3
          0: aload_0
          1: aload_1
          2: aload_2
          3: invokevirtual #6                  // Method doInvoke:(Ljava/util/Map;[Ljava/lang/Object;)Ljava/lang/Object;
          6: areturn
       LineNumberTable:
-        line 3803: 0
+        line 3953: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback;
             0       7     1 kwargs   Ljava/util/Map;
             0       7     2  args   [Ljava/lang/Object;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -374,15 +374,15 @@
          1: invokevirtual #7                  // Method java/lang/Object.getClass:()Ljava/lang/Class;
          4: invokevirtual #8                  // Method java/lang/Class.getSimpleName:()Ljava/lang/String;
          7: aload_0
          8: getfield      #4                  // Field myFunctionId:I
         11: invokedynamic #9,  0              // InvokeDynamic #0:makeConcatWithConstants:(Ljava/lang/String;I)Ljava/lang/String;
         16: areturn
       LineNumberTable:
-        line 3812: 0
+        line 3962: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback<TT;>;
 
@@ -537,45 +537,45 @@
        357: invokevirtual #47                 // Method com/deshaw/pjrmi/PJRmi$Connection.sendMessage:(Ljava/io/DataOutputStream;Lcom/deshaw/pjrmi/PJRmi$MessageType;JILjava/io/ByteArrayOutputStream;)V
        360: aload_0
        361: getfield      #2                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
        364: aload         8
        366: invokevirtual #48                 // Method com/deshaw/pjrmi/PJRmi$Connection.awaitCallbackReponse:(Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;)Ljava/lang/Object;
        369: areturn
       LineNumberTable:
-        line 3825: 0
-        line 3826: 12
-        line 3827: 17
-        line 3826: 25
-        line 3831: 28
-        line 3832: 32
-        line 3833: 39
-        line 3834: 51
-        line 3837: 56
-        line 3840: 68
-        line 3841: 79
-        line 3842: 89
-        line 3843: 101
-        line 3844: 105
-        line 3847: 117
-        line 3848: 127
-        line 3849: 152
-        line 3848: 166
-        line 3854: 172
-        line 3855: 176
-        line 3858: 188
-        line 3859: 202
-        line 3861: 237
-        line 3862: 255
-        line 3863: 274
-        line 3867: 277
-        line 3868: 291
-        line 3871: 311
-        line 3872: 323
-        line 3877: 338
-        line 3884: 360
+        line 3975: 0
+        line 3976: 12
+        line 3977: 17
+        line 3976: 25
+        line 3981: 28
+        line 3982: 32
+        line 3983: 39
+        line 3984: 51
+        line 3987: 56
+        line 3990: 68
+        line 3991: 79
+        line 3992: 89
+        line 3993: 101
+        line 3994: 105
+        line 3997: 117
+        line 3998: 127
+        line 3999: 152
+        line 3998: 166
+        line 4004: 172
+        line 4005: 176
+        line 4008: 188
+        line 4009: 202
+        line 4011: 237
+        line 4012: 255
+        line 4013: 274
+        line 4017: 277
+        line 4018: 291
+        line 4021: 311
+        line 4022: 323
+        line 4027: 338
+        line 4034: 360
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           152      14    11   arg   Ljava/lang/Object;
           237      37     9 entry   Ljava/util/Map$Entry;
             0     370     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallback;
             0     370     1 kwargs   Ljava/util/Map;
             0     370     2  args   [Ljava/lang/Object;
```

#### com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 183db1c6e1462a415277cb47ff52274c8ce1d12e62319a243db6922ed06060f9
+  SHA-256 checksum 99427d5be55f5d5b380c0c9c690c6d9a7ce150bb513f06467d2d399b3aed835c
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$PythonCallbackResult
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #8                          // com/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult
   super_class: #9                         // java/lang/Object
@@ -105,19 +105,19 @@
         15: aconst_null
         16: putfield      #4                  // Field myResult:Ljava/lang/Object;
         19: aload_0
         20: iconst_0
         21: putfield      #5                  // Field myReady:Z
         24: return
       LineNumberTable:
-        line 3721: 0
-        line 3722: 9
-        line 3723: 14
-        line 3724: 19
-        line 3725: 24
+        line 3871: 0
+        line 3872: 9
+        line 3873: 14
+        line 3874: 19
+        line 3875: 24
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      25     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;
             0      25     2 receiver   Ljava/lang/Thread;
     MethodParameters:
       Name                           Flags
       this$1                         final synthetic
@@ -138,19 +138,19 @@
         11: iconst_1
         12: putfield      #5                  // Field myReady:Z
         15: aload_0
         16: getfield      #3                  // Field myReceiver:Ljava/lang/Thread;
         19: invokestatic  #7                  // Method java/util/concurrent/locks/LockSupport.unpark:(Ljava/lang/Thread;)V
         22: return
       LineNumberTable:
-        line 3732: 0
-        line 3733: 5
-        line 3734: 10
-        line 3735: 15
-        line 3736: 22
+        line 3882: 0
+        line 3883: 5
+        line 3884: 10
+        line 3885: 15
+        line 3886: 22
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      23     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;
             0      23     1 isException   Z
             0      23     2 result   Ljava/lang/Object;
     MethodParameters:
       Name                           Flags
@@ -162,43 +162,43 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #5                  // Field myReady:Z
          4: ireturn
       LineNumberTable:
-        line 3743: 0
+        line 3893: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;
 
   public boolean isException();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #6                  // Field myIsException:Z
          4: ireturn
       LineNumberTable:
-        line 3751: 0
+        line 3901: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;
 
   public java.lang.Object getResult();
     descriptor: ()Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field myResult:Ljava/lang/Object;
          4: areturn
       LineNumberTable:
-        line 3759: 0
+        line 3909: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$PythonCallbackResult;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3e9b36a9bb2989731bc77c84bb5d746fe14488b57972326b2b9875cffcd09c36
+  SHA-256 checksum 6a4c299031deeb89223566c9e17f2b2484c1c1b8e7a4556a5ca7f091ff4216a3
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$BestEffortPythonPickle extends com.deshaw.pjrmi.PJRmi$PJRmiPythonPickle
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #21                         // com/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle
   super_class: #22                        // com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle
@@ -135,15 +135,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$1:Lcom/deshaw/pjrmi/PJRmi$Connection;
          5: aload_0
          6: invokespecial #2                  // Method com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle."<init>":()V
          9: return
       LineNumberTable:
-        line 3657: 0
+        line 3807: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle;
     MethodParameters:
       Name                           Flags
       this$1                         final synthetic
 
@@ -194,27 +194,27 @@
         80: getstatic     #18                 // Field com/deshaw/python/Operations.TUPLE3:Lcom/deshaw/python/Operations;
         83: invokevirtual #19                 // Method write:(Lcom/deshaw/python/Operations;)V
         86: aload_0
         87: getstatic     #20                 // Field com/deshaw/python/Operations.REDUCE:Lcom/deshaw/python/Operations;
         90: invokevirtual #19                 // Method write:(Lcom/deshaw/python/Operations;)V
         93: return
       LineNumberTable:
-        line 3668: 0
-        line 3670: 10
-        line 3669: 23
-        line 3672: 27
-        line 3673: 31
-        line 3674: 35
-        line 3679: 47
-        line 3680: 55
-        line 3681: 66
-        line 3682: 74
-        line 3683: 79
-        line 3684: 86
-        line 3685: 93
+        line 3818: 0
+        line 3820: 10
+        line 3819: 23
+        line 3822: 27
+        line 3823: 31
+        line 3824: 35
+        line 3829: 47
+        line 3830: 55
+        line 3831: 66
+        line 3832: 74
+        line 3833: 79
+        line 3834: 86
+        line 3835: 93
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      94     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$BestEffortPythonPickle;
             0      94     1   obj   Ljava/lang/Object;
            27      67     2  type   Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
            47      47     3 handle   J
       StackMapTable: number_of_entries = 4
```

#### com/deshaw/pjrmi/PJRmi$Connection$MethodCaller.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum ecdd3d286743575518853bb57e4cb55831b3e1a3d1f1fb137901b773d822e1a0
+  SHA-256 checksum 848caf7ee8313e7ff6d3e7a100676267f608c7b070a1cb426f22dcac6fcebabb
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$MethodCaller extends java.lang.Thread implements com.deshaw.pjrmi.PJRmi$ThreadId
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #43                         // com/deshaw/pjrmi/PJRmi$Connection$MethodCaller
   super_class: #44                        // java/lang/Thread
@@ -269,25 +269,25 @@
         71: invokestatic  #2                  // Method java/lang/System.nanoTime:()J
         74: putfield      #18                 // Field myLastCallNs:J
         77: aload_0
         78: iconst_1
         79: invokevirtual #19                 // Method setDaemon:(Z)V
         82: return
       LineNumberTable:
-        line 3544: 0
-        line 3549: 5
-        line 3551: 6
-        line 3549: 26
-        line 3553: 29
-        line 3554: 45
-        line 3555: 60
-        line 3556: 65
-        line 3557: 70
-        line 3558: 77
-        line 3559: 82
+        line 3694: 0
+        line 3699: 5
+        line 3701: 6
+        line 3699: 26
+        line 3703: 29
+        line 3704: 45
+        line 3705: 60
+        line 3706: 65
+        line 3707: 70
+        line 3708: 77
+        line 3709: 82
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      83     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$MethodCaller;
     MethodParameters:
       Name                           Flags
       this$1                         final synthetic
 
@@ -309,19 +309,19 @@
         24: aload_0
         25: aload_1
         26: putfield      #16                 // Field myRunnable:Ljava/lang/Runnable;
         29: aload_0
         30: invokestatic  #23                 // Method java/util/concurrent/locks/LockSupport.unpark:(Ljava/lang/Thread;)V
         33: return
       LineNumberTable:
-        line 3570: 0
-        line 3571: 7
-        line 3577: 24
-        line 3578: 29
-        line 3579: 33
+        line 3720: 0
+        line 3721: 7
+        line 3727: 24
+        line 3728: 29
+        line 3729: 33
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      34     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$MethodCaller;
             0      34     1 runnable   Ljava/lang/Runnable;
       StackMapTable: number_of_entries = 1
         frame_type = 24 /* same */
     Exceptions:
@@ -336,30 +336,30 @@
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: iconst_0
          2: putfield      #17                 // Field myActive:Z
          5: return
       LineNumberTable:
-        line 3586: 0
-        line 3587: 5
+        line 3736: 0
+        line 3737: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$MethodCaller;
 
   public long getThreadId();
     descriptor: ()J
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: getfield      #12                 // Field myThreadId:J
          4: lreturn
       LineNumberTable:
-        line 3595: 0
+        line 3745: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$MethodCaller;
 
   public void run();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
@@ -438,38 +438,38 @@
        161: return
       Exception table:
          from    to  target type
             29    45    67   Class java/lang/Throwable
             29    45   102   any
             67    80   102   any
       LineNumberTable:
-        line 3604: 0
-        line 3608: 8
-        line 3611: 15
-        line 3613: 22
-        line 3616: 29
-        line 3617: 36
-        line 3630: 45
-        line 3631: 50
-        line 3632: 64
-        line 3619: 67
-        line 3622: 68
-        line 3630: 80
-        line 3631: 85
-        line 3632: 99
-        line 3630: 102
-        line 3631: 108
-        line 3632: 122
-        line 3641: 127
-        line 3644: 133
-        line 3643: 141
-        line 3642: 144
-        line 3641: 147
-        line 3649: 153
-        line 3650: 161
+        line 3754: 0
+        line 3758: 8
+        line 3761: 15
+        line 3763: 22
+        line 3766: 29
+        line 3767: 36
+        line 3780: 45
+        line 3781: 50
+        line 3782: 64
+        line 3769: 67
+        line 3772: 68
+        line 3780: 80
+        line 3781: 85
+        line 3782: 99
+        line 3780: 102
+        line 3781: 108
+        line 3782: 122
+        line 3791: 127
+        line 3794: 133
+        line 3793: 141
+        line 3792: 144
+        line 3791: 147
+        line 3799: 153
+        line 3800: 161
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            68      12     1     t   Ljava/lang/Throwable;
             0     162     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$MethodCaller;
       StackMapTable: number_of_entries = 6
         frame_type = 15 /* same */
         frame_type = 115 /* same_locals_1_stack_item */
```

#### com/deshaw/pjrmi/PJRmi$Connection$Worker.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum de10b87a53204e30af41d5077e064d725b94318b6b4afa8f4fa4eecd582e9f4b
+  SHA-256 checksum 78b0615f93708468efd6efb93c05ae555927135eefe9a73e1dd84423240301bc
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$Connection$Worker extends java.lang.Thread implements com.deshaw.pjrmi.PJRmi$ThreadId
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #80                         // com/deshaw/pjrmi/PJRmi$Connection$Worker
   super_class: #81                        // java/lang/Thread
@@ -456,26 +456,26 @@
         62: invokespecial #17                 // Method com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream."<init>":()V
         65: putfield      #18                 // Field mySendBuf:Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
         68: aload_0
         69: iconst_1
         70: invokevirtual #19                 // Method setDaemon:(Z)V
         73: return
       LineNumberTable:
-        line 3280: 0
-        line 3281: 5
-        line 3254: 10
-        line 3255: 17
-        line 3256: 24
-        line 3257: 29
-        line 3258: 34
-        line 3259: 47
-        line 3266: 52
-        line 3273: 57
-        line 3282: 68
-        line 3283: 73
+        line 3430: 0
+        line 3431: 5
+        line 3404: 10
+        line 3405: 17
+        line 3406: 24
+        line 3407: 29
+        line 3408: 34
+        line 3409: 47
+        line 3416: 52
+        line 3423: 57
+        line 3432: 68
+        line 3433: 73
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      74     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$Worker;
             0      74     2  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       this$1                         final synthetic
@@ -506,22 +506,22 @@
         32: aload_0
         33: aload         7
         35: putfield      #14                 // Field myOut:Ljava/io/DataOutputStream;
         38: aload_0
         39: invokestatic  #21                 // Method java/util/concurrent/locks/LockSupport.unpark:(Ljava/lang/Thread;)V
         42: return
       LineNumberTable:
-        line 3296: 0
-        line 3297: 5
-        line 3298: 10
-        line 3299: 16
-        line 3300: 22
-        line 3301: 32
-        line 3304: 38
-        line 3305: 42
+        line 3446: 0
+        line 3447: 5
+        line 3448: 10
+        line 3449: 16
+        line 3450: 22
+        line 3451: 32
+        line 3454: 38
+        line 3455: 42
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      43     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$Worker;
             0      43     1  type   Lcom/deshaw/pjrmi/PJRmi$MessageType;
             0      43     2 threadId   J
             0      43     4 thread   Lcom/deshaw/util/concurrent/VirtualThreadLock$VirtualThread;
             0      43     5 reqId   I
@@ -557,21 +557,21 @@
         32: invokestatic  #28                 // Method java/util/concurrent/locks/LockSupport.parkNanos:(J)V
         35: goto          8
         38: getstatic     #22                 // Field com/deshaw/pjrmi/PJRmi.LOG:Ljava/util/logging/Logger;
         41: ldc           #29                 // String Worker thread stops
         43: invokevirtual #24                 // Method java/util/logging/Logger.fine:(Ljava/lang/String;)V
         46: return
       LineNumberTable:
-        line 3313: 0
-        line 3315: 8
-        line 3317: 15
-        line 3318: 22
-        line 3325: 29
-        line 3329: 38
-        line 3330: 46
+        line 3463: 0
+        line 3465: 8
+        line 3467: 15
+        line 3468: 22
+        line 3475: 29
+        line 3479: 38
+        line 3480: 46
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      47     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$Worker;
       StackMapTable: number_of_entries = 3
         frame_type = 8 /* same */
         frame_type = 20 /* same */
         frame_type = 8 /* same */
@@ -582,30 +582,30 @@
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: iconst_0
          2: putfield      #15                 // Field myActive:Z
          5: return
       LineNumberTable:
-        line 3340: 0
-        line 3341: 5
+        line 3490: 0
+        line 3491: 5
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$Worker;
 
   public long getThreadId();
     descriptor: ()J
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=2, locals=1, args_size=1
          0: aload_0
          1: getfield      #7                  // Field myThreadId:J
          4: lreturn
       LineNumberTable:
-        line 3349: 0
+        line 3499: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$Connection$Worker;
 
   private void work();
     descriptor: ()V
     flags: (0x0002) ACC_PRIVATE
@@ -999,115 +999,115 @@
            435   504   507   Class java/io/IOException
            546   561   564   Class java/lang/Throwable
             85   154   712   any
            345   521   712   any
            739   754   757   Class java/lang/Throwable
            712   714   712   any
       LineNumberTable:
-        line 3358: 0
-        line 3359: 12
-        line 3362: 35
-        line 3359: 43
-        line 3366: 46
-        line 3367: 65
-        line 3370: 72
-        line 3373: 75
-        line 3376: 82
-        line 3384: 85
-        line 3387: 92
-        line 3388: 102
-        line 3389: 116
-        line 3393: 119
-        line 3448: 154
-        line 3449: 159
-        line 3451: 172
-        line 3457: 179
-        line 3472: 194
-        line 3459: 197
-        line 3463: 199
-        line 3464: 207
-        line 3466: 223
-        line 3467: 228
-        line 3470: 244
-        line 3475: 259
-        line 3476: 266
-        line 3477: 271
-        line 3478: 278
-        line 3479: 283
-        line 3480: 290
-        line 3483: 295
-        line 3490: 299
-        line 3491: 309
-        line 3496: 314
-        line 3499: 337
-        line 3401: 345
-        line 3403: 347
-        line 3410: 351
-        line 3411: 363
-        line 3413: 374
-        line 3414: 379
-        line 3411: 387
-        line 3418: 390
-        line 3421: 401
-        line 3422: 413
-        line 3423: 421
-        line 3427: 435
-        line 3428: 448
-        line 3429: 458
-        line 3433: 467
-        line 3434: 474
-        line 3444: 504
-        line 3440: 507
-        line 3443: 509
-        line 3448: 521
-        line 3449: 526
-        line 3451: 539
-        line 3457: 546
-        line 3472: 561
-        line 3459: 564
-        line 3463: 566
-        line 3464: 574
-        line 3466: 590
-        line 3467: 595
-        line 3470: 611
-        line 3475: 626
-        line 3476: 633
-        line 3477: 638
-        line 3478: 645
-        line 3479: 650
-        line 3480: 657
-        line 3483: 662
-        line 3490: 666
-        line 3491: 676
-        line 3496: 681
-        line 3499: 704
-        line 3448: 712
-        line 3449: 719
-        line 3451: 732
-        line 3457: 739
-        line 3472: 754
-        line 3459: 757
-        line 3463: 759
-        line 3464: 767
-        line 3466: 783
-        line 3467: 788
-        line 3470: 804
-        line 3475: 819
-        line 3476: 826
-        line 3477: 831
-        line 3478: 838
-        line 3479: 843
-        line 3480: 850
-        line 3483: 855
-        line 3490: 859
-        line 3491: 869
-        line 3496: 874
-        line 3499: 897
-        line 3501: 902
-        line 3502: 905
+        line 3508: 0
+        line 3509: 12
+        line 3512: 35
+        line 3509: 43
+        line 3516: 46
+        line 3517: 65
+        line 3520: 72
+        line 3523: 75
+        line 3526: 82
+        line 3534: 85
+        line 3537: 92
+        line 3538: 102
+        line 3539: 116
+        line 3543: 119
+        line 3598: 154
+        line 3599: 159
+        line 3601: 172
+        line 3607: 179
+        line 3622: 194
+        line 3609: 197
+        line 3613: 199
+        line 3614: 207
+        line 3616: 223
+        line 3617: 228
+        line 3620: 244
+        line 3625: 259
+        line 3626: 266
+        line 3627: 271
+        line 3628: 278
+        line 3629: 283
+        line 3630: 290
+        line 3633: 295
+        line 3640: 299
+        line 3641: 309
+        line 3646: 314
+        line 3649: 337
+        line 3551: 345
+        line 3553: 347
+        line 3560: 351
+        line 3561: 363
+        line 3563: 374
+        line 3564: 379
+        line 3561: 387
+        line 3568: 390
+        line 3571: 401
+        line 3572: 413
+        line 3573: 421
+        line 3577: 435
+        line 3578: 448
+        line 3579: 458
+        line 3583: 467
+        line 3584: 474
+        line 3594: 504
+        line 3590: 507
+        line 3593: 509
+        line 3598: 521
+        line 3599: 526
+        line 3601: 539
+        line 3607: 546
+        line 3622: 561
+        line 3609: 564
+        line 3613: 566
+        line 3614: 574
+        line 3616: 590
+        line 3617: 595
+        line 3620: 611
+        line 3625: 626
+        line 3626: 633
+        line 3627: 638
+        line 3628: 645
+        line 3629: 650
+        line 3630: 657
+        line 3633: 662
+        line 3640: 666
+        line 3641: 676
+        line 3646: 681
+        line 3649: 704
+        line 3598: 712
+        line 3599: 719
+        line 3601: 732
+        line 3607: 739
+        line 3622: 754
+        line 3609: 757
+        line 3613: 759
+        line 3614: 767
+        line 3616: 783
+        line 3617: 788
+        line 3620: 804
+        line 3625: 819
+        line 3626: 826
+        line 3627: 831
+        line 3628: 838
+        line 3629: 843
+        line 3630: 850
+        line 3633: 855
+        line 3640: 859
+        line 3641: 869
+        line 3646: 874
+        line 3649: 897
+        line 3651: 902
+        line 3652: 905
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           199      60     6     e   Ljava/lang/Throwable;
           509      12    11   ioe   Ljava/io/IOException;
           401     120     7 bados   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
           421     100     8 exDesc   Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
           435      86     9 exHandle   J
```

#### com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum e21c514fc3a61fcc084066dd14a55b00c6abd4844236047d653fc362ae3cc832
+  SHA-256 checksum f358d606b96f4f9c2f3095251d12c66a2d049a69f3119eda14ff401886a26ed6
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$ThreadLocalByteArrayDataOutputStream extends java.lang.ThreadLocal<com.deshaw.pjrmi.PJRmi$ByteArrayDataOutputStream>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #8                          // com/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream
   super_class: #9                         // java/lang/ThreadLocal
@@ -55,15 +55,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/ThreadLocal."<init>":()V
          4: return
       LineNumberTable:
-        line 3200: 0
+        line 3350: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream;
 
   public com.deshaw.pjrmi.PJRmi$ByteArrayDataOutputStream get();
     descriptor: ()Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
     flags: (0x0001) ACC_PUBLIC
@@ -74,17 +74,17 @@
          4: checkcast     #3                  // class com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream
          7: astore_1
          8: aload_1
          9: invokevirtual #4                  // Method com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.reset:()V
         12: aload_1
         13: areturn
       LineNumberTable:
-        line 3209: 0
-        line 3210: 8
-        line 3211: 12
+        line 3359: 0
+        line 3360: 8
+        line 3361: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      14     0  this   Lcom/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream;
             8       6     1 buffer   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
 
   protected com.deshaw.pjrmi.PJRmi$ByteArrayDataOutputStream initialValue();
     descriptor: ()Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
@@ -92,43 +92,43 @@
     Code:
       stack=2, locals=1, args_size=1
          0: new           #3                  // class com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream
          3: dup
          4: invokespecial #5                  // Method com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream."<init>":()V
          7: areturn
       LineNumberTable:
-        line 3220: 0
+        line 3370: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream;
 
   public java.lang.Object get();
     descriptor: ()Ljava/lang/Object;
     flags: (0x1041) ACC_PUBLIC, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #6                  // Method get:()Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
          4: areturn
       LineNumberTable:
-        line 3200: 0
+        line 3350: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream;
 
   protected java.lang.Object initialValue();
     descriptor: ()Ljava/lang/Object;
     flags: (0x1044) ACC_PROTECTED, ACC_BRIDGE, ACC_SYNTHETIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokevirtual #7                  // Method initialValue:()Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
          4: areturn
       LineNumberTable:
-        line 3200: 0
+        line 3350: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$ThreadLocalByteArrayDataOutputStream;
 }
 Signature: #27                          // Ljava/lang/ThreadLocal<Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 93a37b18f10a56f773ffd8d3419e442edcb0169cffee99baafb4ee0c424261af
+  SHA-256 checksum eccc6c840a4d79352ac14bedd3415307d3d0984196cd58bb2ee164fcb6392ea4
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$ByteArrayDataOutputStream
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #9                          // com/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream
   super_class: #10                        // java/lang/Object
@@ -76,32 +76,32 @@
         22: dup
         23: aload_0
         24: getfield      #4                  // Field bytes:Ljava/io/ByteArrayOutputStream;
         27: invokespecial #6                  // Method java/io/DataOutputStream."<init>":(Ljava/io/OutputStream;)V
         30: putfield      #7                  // Field dataOut:Ljava/io/DataOutputStream;
         33: return
       LineNumberTable:
-        line 3187: 0
-        line 3190: 4
-        line 3191: 18
+        line 3337: 0
+        line 3340: 4
+        line 3341: 18
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      34     0  this   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
 
   public void reset();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field bytes:Ljava/io/ByteArrayOutputStream;
          4: invokevirtual #8                  // Method java/io/ByteArrayOutputStream.reset:()V
          7: return
       LineNumberTable:
-        line 3194: 0
+        line 3344: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/pjrmi/PJRmi$ByteArrayDataOutputStream;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$ClassInjector.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum b3d07281421878fb6191a72ad59c31c91f9901d1fd246510f6b0026bee878b70
+  SHA-256 checksum 6917b97cf469e7ad202c419202ee36e8334ea16b84e02067f78d6601d12a23b8
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$ClassInjector extends java.lang.ClassLoader
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$ClassInjector
   super_class: #5                         // java/lang/ClassLoader
@@ -62,15 +62,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/ClassLoader."<init>":()V
          4: return
       LineNumberTable:
-        line 3167: 0
+        line 3317: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$ClassInjector;
 
   public java.lang.Class<?> inject(byte[], int) throws java.lang.ClassFormatError, java.lang.IndexOutOfBoundsException, java.lang.SecurityException;
     descriptor: ([BI)Ljava/lang/Class;
     flags: (0x0001) ACC_PUBLIC
@@ -85,17 +85,17 @@
          8: astore_3
          9: aload_0
         10: aload_3
         11: invokevirtual #3                  // Method resolveClass:(Ljava/lang/Class;)V
         14: aload_3
         15: areturn
       LineNumberTable:
-        line 3178: 0
-        line 3179: 9
-        line 3180: 14
+        line 3328: 0
+        line 3329: 9
+        line 3330: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$ClassInjector;
             0      16     1 buffer   [B
             0      16     2   len   I
             9       7     3 result   Ljava/lang/Class;
       LocalVariableTypeTable:
```

#### com/deshaw/pjrmi/PJRmi$HandleMapping.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum d1fd48c1c3bda5139d02902b9722a565a6cb24a0f5cbdeff57b79f6a4f63ec0e
+  SHA-256 checksum ecc9b6982fb02459e841c20bc4e29d82711401f0680a4f3df4ccab19dc1eb62b
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$HandleMapping
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #31                         // com/deshaw/pjrmi/PJRmi$HandleMapping
   super_class: #32                        // java/lang/Object
@@ -210,19 +210,19 @@
         31: lshl
         32: invokestatic  #8                  // Method java/lang/Math.abs:(J)J
         35: lconst_1
         36: ladd
         37: putfield      #9                  // Field myNextHandle:J
         40: return
       LineNumberTable:
-        line 3054: 0
-        line 3040: 4
-        line 3042: 15
-        line 3057: 26
-        line 3058: 40
+        line 3204: 0
+        line 3190: 4
+        line 3192: 15
+        line 3207: 26
+        line 3208: 40
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      41     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
             0      41     1  salt   I
     MethodParameters:
       Name                           Flags
       salt
@@ -302,29 +302,29 @@
        146: getfield      #18                 // Field com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.handle:J
        149: invokedynamic #27,  0             // InvokeDynamic #1:makeConcatWithConstants:(IJ)Ljava/lang/String;
        154: invokevirtual #25                 // Method java/util/logging/Logger.finest:(Ljava/lang/String;)V
        157: aload_2
        158: getfield      #18                 // Field com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.handle:J
        161: lreturn
       LineNumberTable:
-        line 3065: 0
-        line 3066: 4
-        line 3072: 14
-        line 3073: 28
-        line 3074: 32
-        line 3075: 52
-        line 3076: 67
-        line 3078: 85
-        line 3079: 97
-        line 3082: 105
-        line 3079: 113
-        line 3088: 116
-        line 3089: 126
-        line 3090: 138
-        line 3096: 157
+        line 3215: 0
+        line 3216: 4
+        line 3222: 14
+        line 3223: 28
+        line 3224: 32
+        line 3225: 52
+        line 3226: 67
+        line 3228: 85
+        line 3229: 97
+        line 3232: 105
+        line 3229: 113
+        line 3238: 116
+        line 3239: 126
+        line 3240: 138
+        line 3246: 157
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     162     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
             0     162     1 object   Ljava/lang/Object;
            28     134     2   ref   Lcom/deshaw/pjrmi/PJRmi$HandleMapping$Reference;
       StackMapTable: number_of_entries = 3
         frame_type = 14 /* same */
@@ -364,20 +364,20 @@
         46: aload_3
         47: getfield      #26                 // Field com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.count:I
         50: lload_1
         51: invokedynamic #27,  0             // InvokeDynamic #1:makeConcatWithConstants:(IJ)Ljava/lang/String;
         56: invokevirtual #25                 // Method java/util/logging/Logger.finest:(Ljava/lang/String;)V
         59: return
       LineNumberTable:
-        line 3104: 0
-        line 3105: 17
-        line 3106: 21
-        line 3108: 31
-        line 3109: 43
-        line 3114: 59
+        line 3254: 0
+        line 3255: 17
+        line 3256: 21
+        line 3258: 31
+        line 3259: 43
+        line 3264: 59
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      60     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
             0      60     1 handle   J
            17      43     3   ref   Lcom/deshaw/pjrmi/PJRmi$HandleMapping$Reference;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
@@ -442,26 +442,26 @@
        115: getfield      #7                  // Field myObjectToReference:Ljava/util/Map;
        118: aload_3
        119: getfield      #16                 // Field com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.object:Ljava/lang/Object;
        122: invokeinterface #29,  2           // InterfaceMethod java/util/Map.remove:(Ljava/lang/Object;)Ljava/lang/Object;
        127: pop
        128: return
       LineNumberTable:
-        line 3121: 0
-        line 3122: 17
-        line 3124: 21
-        line 3128: 22
-        line 3129: 32
-        line 3130: 44
-        line 3136: 63
-        line 3137: 70
-        line 3138: 82
-        line 3140: 97
-        line 3141: 114
-        line 3143: 128
+        line 3271: 0
+        line 3272: 17
+        line 3274: 21
+        line 3278: 22
+        line 3279: 32
+        line 3280: 44
+        line 3286: 63
+        line 3287: 70
+        line 3288: 82
+        line 3290: 97
+        line 3291: 114
+        line 3293: 128
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0     129     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
             0     129     1 handle   J
            17     112     3   ref   Lcom/deshaw/pjrmi/PJRmi$HandleMapping$Reference;
       StackMapTable: number_of_entries = 4
         frame_type = 252 /* append */
@@ -490,16 +490,16 @@
         18: ifnonnull     25
         21: aconst_null
         22: goto          29
         25: aload_3
         26: getfield      #16                 // Field com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.object:Ljava/lang/Object;
         29: areturn
       LineNumberTable:
-        line 3150: 0
-        line 3151: 17
+        line 3300: 0
+        line 3301: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      30     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
             0      30     1 handle   J
            17      13     3   ref   Lcom/deshaw/pjrmi/PJRmi$HandleMapping$Reference;
       StackMapTable: number_of_entries = 2
         frame_type = 252 /* append */
@@ -520,17 +520,17 @@
          1: getfield      #4                  // Field myHandleToReference:Ljava/util/Map;
          4: invokeinterface #30,  1           // InterfaceMethod java/util/Map.clear:()V
          9: aload_0
         10: getfield      #7                  // Field myObjectToReference:Ljava/util/Map;
         13: invokeinterface #30,  1           // InterfaceMethod java/util/Map.clear:()V
         18: return
       LineNumberTable:
-        line 3159: 0
-        line 3160: 9
-        line 3161: 18
+        line 3309: 0
+        line 3310: 9
+        line 3311: 18
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$HandleMapping$Reference.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8219183253ab88cbf12be9136872c23666bc60737f6a9f9cfec8b92ad2678251
+  SHA-256 checksum f38ba554d7b3e6c3165eeee381543273fd06a5cfc325a259842e9a2dc64f9b19
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$HandleMapping$Reference
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #5                          // com/deshaw/pjrmi/PJRmi$HandleMapping$Reference
   super_class: #6                         // java/lang/Object
@@ -72,19 +72,19 @@
         10: lload_2
         11: putfield      #3                  // Field handle:J
         14: aload_0
         15: iconst_0
         16: putfield      #4                  // Field count:I
         19: return
       LineNumberTable:
-        line 3025: 0
-        line 3026: 4
-        line 3027: 9
-        line 3028: 14
-        line 3029: 19
+        line 3175: 0
+        line 3176: 4
+        line 3177: 9
+        line 3178: 14
+        line 3179: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$HandleMapping$Reference;
             0      20     1 object   Ljava/lang/Object;
             0      20     2 handle   J
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/pjrmi/PJRmi$TypeMapping.class

##### procyon -ec {}

```diff
@@ -47,14 +47,35 @@
             if (PJRmi.LOG.isLoggable(Level.FINEST)) {
                 PJRmi.LOG.finest("Created type mapping from " + klass + " to " + desc);
             }
         }
         return desc;
     }
     
+    public synchronized PJRmi.TypeDescription replaceDescription(final int id, final Class<?> klass) {
+        if (klass == null) {
+            throw new NullPointerException("Given a null replacement class");
+        }
+        if (id < 0 || id >= this.myIdToDescription.length) {
+            throw new IllegalArgumentException("Given a bad type ID " + id);
+        }
+        final PJRmi.TypeDescription cur = this.myIdToDescription[id];
+        if (cur == null) {
+            throw new IllegalArgumentException("Given a bad type ID " + id);
+        }
+        this.myClassToDescription.remove(cur.getRepresentedClass());
+        final PJRmi.TypeDescription desc = new PJRmi.TypeDescription(this.this$0, (Class)klass, id);
+        this.myClassToDescription.put(klass, desc);
+        this.myIdToDescription[id] = desc;
+        if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+            PJRmi.LOG.finest("Updated type mapping from " + klass + " to " + desc);
+        }
+        return desc;
+    }
+    
     public synchronized PJRmi.TypeDescription getDescription(final int id) {
         return (0 <= id && id < this.myIdToDescription.length) ? this.myIdToDescription[id] : null;
     }
     
     public synchronized int getId(final Class<?> klass) {
         return this.getDescription(klass).getTypeId();
     }
```

#### com/deshaw/pjrmi/PJRmi$MethodDescription.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3fb78df19365a73d8c259d393a0896f845acd96fb0086135eeebf545398ae3e6
+  SHA-256 checksum a10fe8cbf5c3df719de3904190bb096b0db258ed2c2bdca6b752cf750c9914d3
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$MethodDescription
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #40                         // com/deshaw/pjrmi/PJRmi$MethodDescription
   super_class: #41                        // java/lang/Object
@@ -295,24 +295,24 @@
         58: invokevirtual #6                  // Method java/lang/String.trim:()Ljava/lang/String;
         61: aastore
         62: iinc          3, 1
         65: goto          47
         68: aload_2
         69: areturn
       LineNumberTable:
-        line 2715: 0
-        line 2716: 5
-        line 2717: 14
-        line 2719: 25
-        line 2722: 27
-        line 2723: 39
-        line 2724: 45
-        line 2725: 53
-        line 2724: 62
-        line 2727: 68
+        line 2824: 0
+        line 2825: 5
+        line 2826: 14
+        line 2828: 25
+        line 2831: 27
+        line 2832: 39
+        line 2833: 45
+        line 2834: 53
+        line 2833: 62
+        line 2836: 68
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            47      21     3     i   I
             0      70     0 kwargs   Lcom/deshaw/pjrmi/PJRmi$Kwargs;
            39      31     1 split   [Ljava/lang/String;
            45      25     2 result   [Ljava/lang/String;
       StackMapTable: number_of_entries = 4
@@ -449,40 +449,40 @@
        244: ifeq          259
        247: getstatic     #31                 // Field com/deshaw/pjrmi/PJRmi.LOG:Ljava/util/logging/Logger;
        250: aload_0
        251: invokedynamic #34,  0             // InvokeDynamic #0:makeConcatWithConstants:(Lcom/deshaw/pjrmi/PJRmi$MethodDescription;)Ljava/lang/String;
        256: invokevirtual #35                 // Method java/util/logging/Logger.finest:(Ljava/lang/String;)V
        259: return
       LineNumberTable:
-        line 2744: 0
-        line 2745: 4
-        line 2746: 9
-        line 2747: 14
-        line 2748: 20
-        line 2749: 26
-        line 2750: 32
-        line 2751: 38
-        line 2753: 47
-        line 2755: 61
-        line 2756: 76
-        line 2757: 92
-        line 2758: 108
-        line 2761: 128
-        line 2762: 137
-        line 2763: 153
-        line 2764: 162
-        line 2765: 166
-        line 2766: 192
-        line 2767: 208
-        line 2765: 212
-        line 2769: 218
-        line 2771: 226
-        line 2774: 235
-        line 2775: 247
-        line 2777: 259
+        line 2853: 0
+        line 2854: 4
+        line 2855: 9
+        line 2856: 14
+        line 2857: 20
+        line 2858: 26
+        line 2859: 32
+        line 2860: 38
+        line 2862: 47
+        line 2864: 61
+        line 2865: 76
+        line 2866: 92
+        line 2867: 108
+        line 2870: 128
+        line 2871: 137
+        line 2872: 153
+        line 2873: 162
+        line 2874: 166
+        line 2875: 192
+        line 2876: 208
+        line 2874: 212
+        line 2878: 218
+        line 2880: 226
+        line 2883: 235
+        line 2884: 247
+        line 2886: 259
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           192      20    18    td   Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
             0     260     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
             0     260     1 index   I
             0     260     2  name   Ljava/lang/String;
             0     260     3 isStatic   Z
@@ -562,43 +562,43 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #8                  // Field myIndex:I
          4: ireturn
       LineNumberTable:
-        line 2784: 0
+        line 2893: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public java.lang.String getName();
     descriptor: ()Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #9                  // Field myName:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 2792: 0
+        line 2901: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public short getFlags();
     descriptor: ()S
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #21                 // Field myFlags:S
          4: ireturn
       LineNumberTable:
-        line 2800: 0
+        line 2909: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public boolean isStatic();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
@@ -611,15 +611,15 @@
         10: iand
         11: ifeq          18
         14: iconst_1
         15: goto          19
         18: iconst_0
         19: ireturn
       LineNumberTable:
-        line 2808: 0
+        line 2917: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
       StackMapTable: number_of_entries = 2
         frame_type = 18 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -636,15 +636,15 @@
         10: iand
         11: ifeq          18
         14: iconst_1
         15: goto          19
         18: iconst_0
         19: ireturn
       LineNumberTable:
-        line 2816: 0
+        line 2925: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
       StackMapTable: number_of_entries = 2
         frame_type = 18 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -661,15 +661,15 @@
         10: iand
         11: ifeq          18
         14: iconst_1
         15: goto          19
         18: iconst_0
         19: ireturn
       LineNumberTable:
-        line 2824: 0
+        line 2933: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
       StackMapTable: number_of_entries = 2
         frame_type = 18 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -686,15 +686,15 @@
         10: iand
         11: ifeq          18
         14: iconst_1
         15: goto          19
         18: iconst_0
         19: ireturn
       LineNumberTable:
-        line 2832: 0
+        line 2941: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
       StackMapTable: number_of_entries = 2
         frame_type = 18 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -704,29 +704,29 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #10                 // Field myReturnType:Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
          4: areturn
       LineNumberTable:
-        line 2840: 0
+        line 2949: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public boolean isGenericReturnType();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #11                 // Field myIsGenericReturnType:Z
          4: ireturn
       LineNumberTable:
-        line 2849: 0
+        line 2958: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public short getNumArguments();
     descriptor: ()S
     flags: (0x0001) ACC_PUBLIC
@@ -734,15 +734,15 @@
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #12                 // Field myArguments:[Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
          4: arraylength
          5: i2s
          6: ireturn
       LineNumberTable:
-        line 2857: 0
+        line 2966: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 
   public com.deshaw.pjrmi.PJRmi$TypeDescription getArgument(short);
     descriptor: (S)Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
     flags: (0x0001) ACC_PUBLIC
@@ -750,15 +750,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: getfield      #12                 // Field myArguments:[Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
          4: iload_1
          5: aaload
          6: areturn
       LineNumberTable:
-        line 2865: 0
+        line 2974: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
             0       7     1 index   S
     MethodParameters:
       Name                           Flags
       index
@@ -770,15 +770,15 @@
       stack=2, locals=2, args_size=2
          0: aload_0
          1: getfield      #13                 // Field myParameterNames:[Ljava/lang/String;
          4: iload_1
          5: aaload
          6: areturn
       LineNumberTable:
-        line 2873: 0
+        line 2982: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       7     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
             0       7     1 index   S
     MethodParameters:
       Name                           Flags
       index
@@ -797,18 +797,18 @@
         12: sipush        32767
         15: invokestatic  #37                 // Method java/lang/Math.min:(II)I
         18: i2s
         19: goto          23
         22: iconst_0
         23: ireturn
       LineNumberTable:
-        line 2881: 0
-        line 2882: 7
-        line 2883: 22
-        line 2881: 23
+        line 2990: 0
+        line 2991: 7
+        line 2992: 22
+        line 2990: 23
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      24     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
       StackMapTable: number_of_entries = 2
         frame_type = 22 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -828,17 +828,17 @@
         15: athrow
         16: aload_0
         17: getfield      #15                 // Field myAcceptedKwargs:[Ljava/lang/String;
         20: iload_1
         21: aaload
         22: areturn
       LineNumberTable:
-        line 2891: 0
-        line 2892: 7
-        line 2895: 16
+        line 3000: 0
+        line 3001: 7
+        line 3004: 16
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      23     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
             0      23     1 index   S
       StackMapTable: number_of_entries = 1
         frame_type = 16 /* same */
     MethodParameters:
@@ -850,15 +850,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #30                 // Field myString:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 2905: 0
+        line 3014: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3ba40cf139d3c8de55f6f39466766c660f2cde76dd6788974a253ae1ffe9ed1c
+  SHA-256 checksum c50c9b60d3a6d021f71a38c8a8e39bb5b7e7636bc29a7dfee19cc3b5cdb82529
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$MethodDescription$ArgumentType extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$MethodDescription$ArgumentType>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
   super_class: #25                        // java/lang/Enum
@@ -163,28 +163,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;"
          9: areturn
       LineNumberTable:
-        line 2616: 0
+        line 2725: 0
 
   public static com.deshaw.pjrmi.PJRmi$MethodDescription$ArgumentType valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType
          9: areturn
       LineNumberTable:
-        line 2616: 0
+        line 2725: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -207,18 +207,18 @@
         19: iload_0
         20: invokedynamic #9,  0              // InvokeDynamic #0:makeConcatWithConstants:(CI)Ljava/lang/String;
         25: invokespecial #10                 // Method java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
         28: athrow
         29: aload_1
         30: areturn
       LineNumberTable:
-        line 2645: 0
-        line 2646: 9
-        line 2647: 13
-        line 2651: 29
+        line 2754: 0
+        line 2755: 9
+        line 2756: 13
+        line 2760: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      31     0    id   B
             9      22     1 result   Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
           offset_delta = 29
@@ -237,17 +237,17 @@
          2: iload_2
          3: invokespecial #11                 // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #12                 // Field id:B
         11: return
       LineNumberTable:
-        line 2658: 0
-        line 2659: 6
-        line 2660: 11
+        line 2767: 0
+        line 2768: 6
+        line 2769: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
             0      12     3    id   B
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -341,25 +341,25 @@
        146: invokestatic  #7                  // Method java/lang/Byte.toUnsignedInt:(B)I
        149: aload_3
        150: aastore
        151: iinc          2, 1
        154: goto          130
        157: return
       LineNumberTable:
-        line 2618: 0
-        line 2619: 15
-        line 2620: 30
-        line 2621: 45
-        line 2622: 60
-        line 2616: 75
-        line 2628: 112
-        line 2630: 121
-        line 2631: 139
-        line 2630: 151
-        line 2633: 157
+        line 2727: 0
+        line 2728: 15
+        line 2729: 30
+        line 2730: 45
+        line 2731: 60
+        line 2725: 75
+        line 2737: 112
+        line 2739: 121
+        line 2740: 139
+        line 2739: 151
+        line 2742: 157
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           139      12     3    mt   Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;
       StackMapTable: number_of_entries = 2
         frame_type = 254 /* append */
           offset_delta = 130
           locals = [ class "[Lcom/deshaw/pjrmi/PJRmi$MethodDescription$ArgumentType;", int, int ]
```

#### com/deshaw/pjrmi/PJRmi$MethodCallFuture.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 282cabcb1fc04503c38f00950740a16f7d1c4d47b968fbb626861b0ac7dede2e
+  SHA-256 checksum 7f2456d07d157ba940b71d24f18d87b34669c0a7e04be47356d3b1aced21683e
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$MethodCallFuture extends java.lang.Object implements java.util.concurrent.Future<java.lang.Object>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #27                         // com/deshaw/pjrmi/PJRmi$MethodCallFuture
   super_class: #28                        // java/lang/Object
@@ -179,20 +179,20 @@
         15: iconst_0
         16: putfield      #4                  // Field myIsDone:Z
         19: aload_0
         20: iconst_0
         21: putfield      #5                  // Field myIsException:Z
         24: return
       LineNumberTable:
-        line 2467: 0
-        line 2468: 4
-        line 2469: 9
-        line 2470: 14
-        line 2471: 19
-        line 2472: 24
+        line 2576: 0
+        line 2577: 4
+        line 2578: 9
+        line 2579: 14
+        line 2580: 19
+        line 2581: 24
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      25     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
             0      25     1  desc   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       desc                           final
@@ -209,18 +209,18 @@
          6: iload_2
          7: putfield      #5                  // Field myIsException:Z
         10: aload_0
         11: iconst_1
         12: putfield      #4                  // Field myIsDone:Z
         15: return
       LineNumberTable:
-        line 2480: 0
-        line 2481: 5
-        line 2482: 10
-        line 2483: 15
+        line 2589: 0
+        line 2590: 5
+        line 2591: 10
+        line 2592: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
             0      16     1 result   Ljava/lang/Object;
             0      16     2 isException   Z
     MethodParameters:
       Name                           Flags
@@ -231,15 +231,15 @@
     descriptor: (Z)Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=2, args_size=2
          0: iconst_0
          1: ireturn
       LineNumberTable:
-        line 2492: 0
+        line 2601: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
             0       2     1 mayInterruptIfRunning   Z
     MethodParameters:
       Name                           Flags
       mayInterruptIfRunning
@@ -248,29 +248,29 @@
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: iconst_0
          1: ireturn
       LineNumberTable:
-        line 2502: 0
+        line 2611: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       2     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
 
   public boolean isDone();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field myIsDone:Z
          4: ireturn
       LineNumberTable:
-        line 2511: 0
+        line 2620: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
 
   public java.lang.Object get() throws java.util.concurrent.ExecutionException, java.lang.InterruptedException;
     descriptor: ()Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -288,17 +288,17 @@
         18: aload_1
         19: invokespecial #14                 // Method java/util/concurrent/ExecutionException."<init>":(Ljava/lang/String;Ljava/lang/Throwable;)V
         22: athrow
       Exception table:
          from    to  target type
              0    10    11   Class java/util/concurrent/TimeoutException
       LineNumberTable:
-        line 2526: 0
-        line 2528: 11
-        line 2529: 12
+        line 2635: 0
+        line 2637: 11
+        line 2638: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12      11     1     e   Ljava/util/concurrent/TimeoutException;
             0      23     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
       StackMapTable: number_of_entries = 1
         frame_type = 75 /* same_locals_1_stack_item */
           stack = [ class java/util/concurrent/TimeoutException ]
@@ -383,31 +383,31 @@
        148: invokespecial #25                 // Method java/util/concurrent/TimeoutException."<init>":()V
        151: athrow
        152: lconst_0
        153: sipush        1000
        156: invokestatic  #26                 // Method java/lang/Thread.sleep:(JI)V
        159: goto          42
       LineNumberTable:
-        line 2550: 0
-        line 2551: 6
-        line 2556: 14
-        line 2557: 25
-        line 2563: 42
-        line 2565: 49
-        line 2566: 56
-        line 2567: 63
-        line 2570: 78
-        line 2580: 95
-        line 2581: 101
-        line 2583: 114
-        line 2584: 119
-        line 2585: 132
-        line 2588: 135
-        line 2589: 144
-        line 2593: 152
+        line 2659: 0
+        line 2660: 6
+        line 2665: 14
+        line 2666: 25
+        line 2672: 42
+        line 2674: 49
+        line 2675: 56
+        line 2676: 63
+        line 2679: 78
+        line 2689: 95
+        line 2690: 101
+        line 2692: 114
+        line 2693: 119
+        line 2694: 132
+        line 2697: 135
+        line 2698: 144
+        line 2702: 152
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            11       3     4 untilMs   J
            25      17     6   end   J
           101      34     6 result   Ljava/lang/Object;
             0     162     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
             0     162     1 timeout   J
@@ -440,15 +440,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field myDescription:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 2604: 0
+        line 2713: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodCallFuture;
 }
 Signature: #76                          // Ljava/lang/Object;Ljava/util/concurrent/Future<Ljava/lang/Object;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$SyncMode.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 4ca89b74588483852a449a50b3ca88f4be31a4a771d4226633775129a4f0058f
+  SHA-256 checksum 913e7e5d63c518cbf67e58b25b87f7be7b1f23ad612bbd7487914018eb6d9ff4
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$SyncMode extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$SyncMode>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$SyncMode
   super_class: #19                        // java/lang/Enum
@@ -136,28 +136,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$SyncMode;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$SyncMode;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$SyncMode;"
          9: areturn
       LineNumberTable:
-        line 2394: 0
+        line 2503: 0
 
   public static com.deshaw.pjrmi.PJRmi$SyncMode valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$SyncMode;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$SyncMode
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$SyncMode
          9: areturn
       LineNumberTable:
-        line 2394: 0
+        line 2503: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -180,18 +180,18 @@
         19: iload_0
         20: invokedynamic #9,  0              // InvokeDynamic #0:makeConcatWithConstants:(CI)Ljava/lang/String;
         25: invokespecial #10                 // Method java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
         28: athrow
         29: aload_1
         30: areturn
       LineNumberTable:
-        line 2419: 0
-        line 2420: 9
-        line 2421: 13
-        line 2425: 29
+        line 2528: 0
+        line 2529: 9
+        line 2530: 13
+        line 2534: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      31     0    id   B
             9      22     1 result   Lcom/deshaw/pjrmi/PJRmi$SyncMode;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
           offset_delta = 29
@@ -210,17 +210,17 @@
          2: iload_2
          3: invokespecial #11                 // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #12                 // Field id:B
         11: return
       LineNumberTable:
-        line 2432: 0
-        line 2433: 6
-        line 2434: 11
+        line 2541: 0
+        line 2542: 6
+        line 2543: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$SyncMode;
             0      12     3    id   B
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -281,22 +281,22 @@
         83: invokestatic  #7                  // Method java/lang/Byte.toUnsignedInt:(B)I
         86: aload_3
         87: aastore
         88: iinc          2, 1
         91: goto          67
         94: return
       LineNumberTable:
-        line 2396: 0
-        line 2397: 15
-        line 2394: 30
-        line 2402: 49
-        line 2404: 58
-        line 2405: 76
-        line 2404: 88
-        line 2407: 94
+        line 2505: 0
+        line 2506: 15
+        line 2503: 30
+        line 2511: 49
+        line 2513: 58
+        line 2514: 76
+        line 2513: 88
+        line 2516: 94
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            76      12     3    sm   Lcom/deshaw/pjrmi/PJRmi$SyncMode;
       StackMapTable: number_of_entries = 2
         frame_type = 254 /* append */
           offset_delta = 67
           locals = [ class "[Lcom/deshaw/pjrmi/PJRmi$SyncMode;", int, int ]
```

#### com/deshaw/pjrmi/PJRmi$MethodFlags.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 0cc3e1c7af6070ce2afa7d63111223f7f6a6728946b2b3993c934b6b44ca5b97
+  SHA-256 checksum 87d083c2cd1ac489fa5f2fab02bbf0bbc135fce576c2b49f1c1b8c66d1685b49
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$MethodFlags extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$MethodFlags>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$MethodFlags
   super_class: #27                        // java/lang/Enum
@@ -149,28 +149,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$MethodFlags;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$MethodFlags;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$MethodFlags;"
          9: areturn
       LineNumberTable:
-        line 2371: 0
+        line 2480: 0
 
   public static com.deshaw.pjrmi.PJRmi$MethodFlags valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$MethodFlags;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$MethodFlags
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$MethodFlags
          9: areturn
       LineNumberTable:
-        line 2371: 0
+        line 2480: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -184,17 +184,17 @@
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #7                  // Field value:S
         11: return
       LineNumberTable:
-        line 2386: 0
-        line 2387: 6
-        line 2388: 11
+        line 2495: 0
+        line 2496: 6
+        line 2497: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodFlags;
             0      12     3 value   S
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -307,23 +307,23 @@
        192: dup
        193: bipush        8
        195: getstatic     #26                 // Field IS_DEFAULT:Lcom/deshaw/pjrmi/PJRmi$MethodFlags;
        198: aastore
        199: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$MethodFlags;
        202: return
       LineNumberTable:
-        line 2373: 0
-        line 2374: 14
-        line 2375: 28
-        line 2376: 42
-        line 2377: 57
-        line 2378: 72
-        line 2379: 87
-        line 2380: 103
-        line 2381: 120
-        line 2371: 137
+        line 2482: 0
+        line 2483: 14
+        line 2484: 28
+        line 2485: 42
+        line 2486: 57
+        line 2487: 72
+        line 2488: 87
+        line 2489: 103
+        line 2490: 120
+        line 2480: 137
 }
 Signature: #63                          // Ljava/lang/Enum<Lcom/deshaw/pjrmi/PJRmi$MethodFlags;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
   private static final #29= #4 of #67;    // MethodFlags=class com/deshaw/pjrmi/PJRmi$MethodFlags of class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$FieldDescription.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3d0fcd7dbd212120a25026570ed6a2f3ad506fd4847a9f92d8ff3282c568c0fa
+  SHA-256 checksum 0a45cf6f0a906d8fe349a382e982a0f1ba84f336ca66899e4b4d3506ab556251
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$FieldDescription
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #10                         // com/deshaw/pjrmi/PJRmi$FieldDescription
   super_class: #11                        // java/lang/Object
@@ -130,21 +130,21 @@
         28: ifeq          43
         31: getstatic     #5                  // Field com/deshaw/pjrmi/PJRmi.LOG:Ljava/util/logging/Logger;
         34: aload_0
         35: invokedynamic #8,  0              // InvokeDynamic #0:makeConcatWithConstants:(Lcom/deshaw/pjrmi/PJRmi$FieldDescription;)Ljava/lang/String;
         40: invokevirtual #9                  // Method java/util/logging/Logger.finest:(Ljava/lang/String;)V
         43: return
       LineNumberTable:
-        line 2323: 0
-        line 2324: 4
-        line 2325: 9
-        line 2326: 14
-        line 2329: 19
-        line 2330: 31
-        line 2332: 43
+        line 2432: 0
+        line 2433: 4
+        line 2434: 9
+        line 2435: 14
+        line 2438: 19
+        line 2439: 31
+        line 2441: 43
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      44     0  this   Lcom/deshaw/pjrmi/PJRmi$FieldDescription;
             0      44     1  name   Ljava/lang/String;
             0      44     2  type   Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
             0      44     3 isStatic   Z
       StackMapTable: number_of_entries = 1
@@ -163,57 +163,57 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field myName:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 2339: 0
+        line 2448: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$FieldDescription;
 
   public com.deshaw.pjrmi.PJRmi$TypeDescription getType();
     descriptor: ()Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #3                  // Field myType:Lcom/deshaw/pjrmi/PJRmi$TypeDescription;
          4: areturn
       LineNumberTable:
-        line 2347: 0
+        line 2456: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$FieldDescription;
 
   public boolean isStatic();
     descriptor: ()Z
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #4                  // Field myIsStatic:Z
          4: ireturn
       LineNumberTable:
-        line 2355: 0
+        line 2464: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$FieldDescription;
 
   public java.lang.String toString();
     descriptor: ()Ljava/lang/String;
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #2                  // Field myName:Ljava/lang/String;
          4: areturn
       LineNumberTable:
-        line 2364: 0
+        line 2473: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$FieldDescription;
 }
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
```

#### com/deshaw/pjrmi/PJRmi$ReadObjectResult.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c507a727e44ecf12c400a29e6e4a8c35c71677e806d25d3d03f21872f1d8a936
+  SHA-256 checksum 2f878f0061e401d5b9b6cb0aff4d034f0e5f36d51dd4a773619315c49363fd37
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$ReadObjectResult
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$ReadObjectResult
   super_class: #5                         // java/lang/Object
@@ -58,18 +58,18 @@
          5: iload_1
          6: putfield      #2                  // Field offset:I
          9: aload_0
         10: aload_2
         11: putfield      #3                  // Field object:Ljava/lang/Object;
         14: return
       LineNumberTable:
-        line 2291: 0
-        line 2292: 4
-        line 2293: 9
-        line 2294: 14
+        line 2400: 0
+        line 2401: 4
+        line 2402: 9
+        line 2403: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$ReadObjectResult;
             0      15     1 offset   I
             0      15     2 object   Ljava/lang/Object;
     MethodParameters:
       Name                           Flags
```

#### com/deshaw/pjrmi/PJRmi$MethodSignature.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 62ad82dbd650fe6c0a4768b6f8ca361e942ef4ec233e6c5faa85009c6c2c4280
+  SHA-256 checksum 29f134ad70827ccee99cf2e273f0fb7251badcd01404d94956a5c039f4c081c1
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$MethodSignature
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #6                          // com/deshaw/pjrmi/PJRmi$MethodSignature
   super_class: #9                         // java/lang/Object
@@ -83,18 +83,18 @@
          5: aload_1
          6: putfield      #2                  // Field myName:Ljava/lang/String;
          9: aload_0
         10: aload_2
         11: putfield      #3                  // Field myParamTypes:Ljava/util/List;
         14: return
       LineNumberTable:
-        line 2246: 0
-        line 2247: 4
-        line 2248: 9
-        line 2249: 14
+        line 2355: 0
+        line 2356: 4
+        line 2357: 9
+        line 2358: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodSignature;
             0      15     1  name   Ljava/lang/String;
             0      15     2 paramTypes   Ljava/util/List;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -115,17 +115,17 @@
          4: invokevirtual #4                  // Method java/lang/String.hashCode:()I
          7: aload_0
          8: getfield      #3                  // Field myParamTypes:Ljava/util/List;
         11: invokeinterface #5,  1            // InterfaceMethod java/util/List.hashCode:()I
         16: ixor
         17: ireturn
       LineNumberTable:
-        line 2257: 0
-        line 2258: 11
-        line 2257: 17
+        line 2366: 0
+        line 2367: 11
+        line 2366: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodSignature;
 
   public boolean equals(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Z
     flags: (0x0001) ACC_PUBLIC
@@ -152,20 +152,20 @@
         42: iconst_1
         43: goto          47
         46: iconst_0
         47: ireturn
         48: iconst_0
         49: ireturn
       LineNumberTable:
-        line 2267: 0
-        line 2268: 7
-        line 2269: 12
-        line 2270: 34
-        line 2269: 47
-        line 2273: 48
+        line 2376: 0
+        line 2377: 7
+        line 2378: 12
+        line 2379: 34
+        line 2378: 47
+        line 2382: 48
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            12      36     2  that   Lcom/deshaw/pjrmi/PJRmi$MethodSignature;
             0      50     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodSignature;
             0      50     1   obj   Ljava/lang/Object;
       StackMapTable: number_of_entries = 3
         frame_type = 252 /* append */
```

#### com/deshaw/pjrmi/PJRmi$MethodComparator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 22c6fde3998205d369984e9e8fe12d28722525b0c0dc532c019009e7773670e2
+  SHA-256 checksum 894c62e09be97c815c220a7e23aa57c3703880c8e48fde93821845a013c4bc67
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$MethodComparator extends java.lang.Object implements java.util.Comparator<java.lang.reflect.Method>
   minor version: 0
   major version: 55
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #12                         // com/deshaw/pjrmi/PJRmi$MethodComparator
   super_class: #24                        // java/lang/Object
@@ -146,16 +146,16 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 2139: 0
-        line 2141: 4
+        line 2248: 0
+        line 2250: 4
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodComparator;
 
   public int compare(java.lang.reflect.Method, java.lang.reflect.Method);
     descriptor: (Ljava/lang/reflect/Method;Ljava/lang/reflect/Method;)I
     flags: (0x0001) ACC_PUBLIC
@@ -301,48 +301,48 @@
        275: iload         9
        277: ireturn
        278: iinc          8, 1
        281: goto          241
        284: iconst_0
        285: ireturn
       LineNumberTable:
-        line 2150: 0
-        line 2151: 12
-        line 2152: 16
-        line 2156: 18
-        line 2157: 24
-        line 2158: 30
-        line 2159: 38
-        line 2160: 42
-        line 2164: 44
-        line 2168: 55
-        line 2169: 70
-        line 2170: 85
-        line 2171: 102
-        line 2175: 108
-        line 2176: 134
-        line 2178: 140
-        line 2180: 142
-        line 2181: 168
-        line 2183: 174
-        line 2164: 176
-        line 2191: 182
-        line 2192: 188
-        line 2193: 194
-        line 2194: 208
-        line 2196: 214
-        line 2198: 216
-        line 2199: 230
-        line 2201: 236
-        line 2206: 238
-        line 2207: 249
-        line 2208: 270
-        line 2209: 275
-        line 2206: 278
-        line 2214: 284
+        line 2259: 0
+        line 2260: 12
+        line 2261: 16
+        line 2265: 18
+        line 2266: 24
+        line 2267: 30
+        line 2268: 38
+        line 2269: 42
+        line 2273: 44
+        line 2277: 55
+        line 2278: 70
+        line 2279: 85
+        line 2280: 102
+        line 2284: 108
+        line 2285: 134
+        line 2287: 140
+        line 2289: 142
+        line 2290: 168
+        line 2292: 174
+        line 2273: 176
+        line 2300: 182
+        line 2301: 188
+        line 2302: 194
+        line 2303: 208
+        line 2305: 214
+        line 2307: 216
+        line 2308: 230
+        line 2310: 236
+        line 2315: 238
+        line 2316: 249
+        line 2317: 270
+        line 2318: 275
+        line 2315: 278
+        line 2323: 284
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            70     106     7    i1   I
            85      91     8    i2   I
            47     135     6     i   I
           270       8     9   cmp   I
           241      43     8     i   I
@@ -402,15 +402,15 @@
          1: aload_1
          2: if_acmpne     9
          5: iconst_1
          6: goto          10
          9: iconst_0
         10: ireturn
       LineNumberTable:
-        line 2223: 0
+        line 2332: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodComparator;
             0      11     1  that   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 9 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
@@ -428,15 +428,15 @@
          1: aload_1
          2: checkcast     #10                 // class java/lang/reflect/Method
          5: aload_2
          6: checkcast     #10                 // class java/lang/reflect/Method
          9: invokevirtual #11                 // Method compare:(Ljava/lang/reflect/Method;Ljava/lang/reflect/Method;)I
         12: ireturn
       LineNumberTable:
-        line 2110: 0
+        line 2219: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$MethodComparator;
     MethodParameters:
       Name                           Flags
       m1                             synthetic
       m2                             synthetic
@@ -476,22 +476,22 @@
         79: pop
         80: getstatic     #5                  // Field PRIMITIVE_PRIORITIES:Ljava/util/List;
         83: getstatic     #23                 // Field java/lang/Byte.TYPE:Ljava/lang/Class;
         86: invokeinterface #18,  2           // InterfaceMethod java/util/List.add:(Ljava/lang/Object;)Z
         91: pop
         92: return
       LineNumberTable:
-        line 2116: 0
-        line 2126: 10
-        line 2127: 20
-        line 2128: 32
-        line 2129: 44
-        line 2130: 56
-        line 2131: 68
-        line 2132: 80
-        line 2133: 92
+        line 2225: 0
+        line 2235: 10
+        line 2236: 20
+        line 2237: 32
+        line 2238: 44
+        line 2239: 56
+        line 2240: 68
+        line 2241: 80
+        line 2242: 92
 }
 Signature: #70                          // Ljava/lang/Object;Ljava/util/Comparator<Ljava/lang/reflect/Method;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
   private static final #27= #12 of #74;   // MethodComparator=class com/deshaw/pjrmi/PJRmi$MethodComparator of class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$WrappedArrayLike.class

##### procyon -ec {}

```diff
@@ -102,15 +102,14 @@
         this.toStringBuilder(sb, this.myArray);
         return sb.toString();
     }
     
     private void toStringBuilder(final StringBuilder sb, final Object array) {
         sb.append('[');
         if (array != null) {
-            final boolean isArray = array.getClass().getComponentType().isArray();
             for (int i = 0, len = Array.getLength(array); i < len; ++i) {
                 final Object element = Array.get(array, i);
                 if (element.getClass().isArray()) {
                     this.toStringBuilder(sb, element);
                 }
                 else {
                     sb.append(element);
```

#### com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 5489d3bb2c5c066465018a4bafc51e4cbd87094e4d2b2e07106f1608f24206d2
+  SHA-256 checksum 5565086d8477cb27fa46045769d5dceb2718c8150e3a7ab4aa496697a481fca2
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$WrappedArrayLike$ArrayIterator extends java.lang.Object implements java.util.Iterator<java.lang.Object>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #13                         // com/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator
   super_class: #14                        // java/lang/Object
@@ -101,16 +101,16 @@
          5: aload_0
          6: invokespecial #2                  // Method java/lang/Object."<init>":()V
          9: aload_0
         10: iconst_0
         11: putfield      #3                  // Field myIndex:I
         14: return
       LineNumberTable:
-        line 1797: 0
-        line 1803: 9
+        line 1865: 0
+        line 1871: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator;
     MethodParameters:
       Name                           Flags
       this$0                         final synthetic
 
@@ -128,15 +128,15 @@
         12: lcmp
         13: ifge          20
         16: iconst_1
         17: goto          21
         20: iconst_0
         21: ireturn
       LineNumberTable:
-        line 1811: 0
+        line 1879: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lcom/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator;
       StackMapTable: number_of_entries = 2
         frame_type = 20 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -180,21 +180,21 @@
         63: aload_1
         64: areturn
         65: new           #11                 // class java/util/NoSuchElementException
         68: dup
         69: invokespecial #12                 // Method java/util/NoSuchElementException."<init>":()V
         72: athrow
       LineNumberTable:
-        line 1821: 0
-        line 1822: 16
-        line 1823: 38
-        line 1824: 52
-        line 1825: 63
-        line 1823: 64
-        line 1828: 65
+        line 1889: 0
+        line 1890: 16
+        line 1891: 38
+        line 1892: 52
+        line 1893: 63
+        line 1891: 64
+        line 1896: 65
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            38      27     1 value   Ljava/lang/Object;
             0      73     0  this   Lcom/deshaw/pjrmi/PJRmi$WrappedArrayLike$ArrayIterator;
       StackMapTable: number_of_entries = 3
         frame_type = 252 /* append */
           offset_delta = 63
```

#### com/deshaw/pjrmi/PJRmi$TypeDescription.class

##### procyon -ec {}

```diff
@@ -1,24 +1,24 @@
 
 package com.deshaw.pjrmi;
 
 import java.lang.annotation.Annotation;
 import java.util.Collection;
-import java.util.ArrayList;
 import java.util.stream.Collector;
 import java.util.stream.Collectors;
 import java.util.function.Function;
-import java.util.List;
 import java.util.Arrays;
 import java.lang.reflect.InvocationTargetException;
 import java.lang.reflect.Parameter;
 import java.util.Iterator;
+import java.util.List;
 import java.util.Map;
-import java.util.logging.Level;
+import java.util.ArrayList;
 import java.util.HashMap;
+import java.util.logging.Level;
 import java.util.EnumSet;
 import com.deshaw.util.Instrumentor;
 import java.lang.reflect.Method;
 import java.lang.reflect.Constructor;
 import java.lang.reflect.Field;
 import java.util.Set;
 
@@ -41,95 +41,98 @@
     
     public TypeDescription(final PJRmi this$0, final Class<?> klass, final int id) {
         this.this$0 = this$0;
         this.myFlags = EnumSet.noneOf(PJRmi.TypeFlags.class);
         if (klass == null) {
             throw new NullPointerException("Attempt to create TypeDescription for null");
         }
+        if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+            PJRmi.LOG.finest("Creating TypeDescription for " + klass);
+        }
         this.myClass = klass;
         this.myName = klass.getName();
         this.myTypeId = id;
         final Class<?> superClass = klass.getSuperclass();
         final Class<?>[] interfaces = klass.getInterfaces();
         this.mySupertypeIds = new int[interfaces.length + ((superClass != null) ? 1 : 0)];
         int index = 0;
         if (superClass != null) {
             this.mySupertypeIds[index++] = this$0.myTypeMapping.getDescription((Class)superClass).getTypeId();
         }
         for (final Class<?> i : interfaces) {
             this.mySupertypeIds[index++] = this$0.myTypeMapping.getDescription((Class)i).getTypeId();
         }
         final String myName = this.myName;
-        int n = -1;
+        int n2 = -1;
         switch (myName.hashCode()) {
             case 3625364: {
                 if (myName.equals("void")) {
-                    n = 0;
+                    n2 = 0;
                     break;
                 }
                 break;
             }
             case 64711720: {
                 if (myName.equals("boolean")) {
-                    n = 1;
+                    n2 = 1;
                     break;
                 }
                 break;
             }
             case 3039496: {
                 if (myName.equals("byte")) {
-                    n = 2;
+                    n2 = 2;
                     break;
                 }
                 break;
             }
             case 3052374: {
                 if (myName.equals("char")) {
-                    n = 3;
+                    n2 = 3;
                     break;
                 }
                 break;
             }
             case -1325958191: {
                 if (myName.equals("double")) {
-                    n = 4;
+                    n2 = 4;
                     break;
                 }
                 break;
             }
             case 97526364: {
                 if (myName.equals("float")) {
-                    n = 5;
+                    n2 = 5;
                     break;
                 }
                 break;
             }
             case 104431: {
                 if (myName.equals("int")) {
-                    n = 6;
+                    n2 = 6;
                     break;
                 }
                 break;
             }
             case 3327612: {
                 if (myName.equals("long")) {
-                    n = 7;
+                    n2 = 7;
                     break;
                 }
                 break;
             }
             case 109413500: {
                 if (myName.equals("short")) {
-                    n = 8;
+                    n2 = 8;
                     break;
                 }
                 break;
             }
         }
-        switch (n) {
+        switch (n2) {
             case 0:
             case 1:
             case 2:
             case 3:
             case 4:
             case 5:
             case 6:
@@ -151,49 +154,94 @@
         if (klass.isEnum()) {
             this.myFlags.add(PJRmi.TypeFlags.IS_ENUM);
         }
         if (klass.isInterface()) {
             this.myFlags.add(PJRmi.TypeFlags.IS_INTERFACE);
         }
         final Map<String, Field> fields = new HashMap<String, Field>();
-        for (final Field field : klass.getFields()) {
-            final String name = field.getName();
-            final Class<?> container = field.getDeclaringClass();
-            final Field current = (Field)fields.get(name);
-            if (current == null || current.getDeclaringClass().isAssignableFrom(container)) {
-                fields.put(name, field);
+        final Field[] fields2 = klass.getFields();
+        for (int length2 = fields2.length, n3 = 0; n3 < length2; ++n3) {
+            final Field field = fields2[n3];
+            if (!this$0.isClassPermitted((Class)field.getType())) {
+                if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+                    PJRmi.LOG.finest("Omitting field with a disallowed class: " + field);
+                }
+            }
+            else {
+                final String name = field.getName();
+                final Class<?> container = field.getDeclaringClass();
+                final Field current = (Field)fields.get(name);
+                if (current == null || current.getDeclaringClass().isAssignableFrom(container)) {
+                    fields.put(name, field);
+                }
             }
         }
         this.myFields = fields.values().toArray(new Field[fields.size()]);
         this.myFieldDescriptions = new PJRmi.FieldDescription[this.myFields.length];
-        this.myConstructors = klass.getConstructors();
+        final List<Constructor<?>> ctors = new ArrayList<Constructor<?>>();
+        final Constructor<?>[] constructors = klass.getConstructors();
+        for (int length3 = constructors.length, n4 = 0; n4 < length3; ++n4) {
+            final Constructor<?> ctor = constructors[n4];
+            boolean permitted = true;
+            for (final Class<?> type : ctor.getParameterTypes()) {
+                if (!this$0.isClassPermitted((Class)type)) {
+                    permitted = false;
+                    break;
+                }
+            }
+            if (permitted) {
+                ctors.add(ctor);
+            }
+            else if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+                PJRmi.LOG.finest("Omitting constructor with a disallowed class: " + ctor);
+            }
+        }
+        this.myConstructors = ctors.toArray(new Constructor[ctors.size()]);
         this.myConstructorSpecificities = new byte[this.myConstructors.length][];
         for (int j = 0; j < this.myConstructors.length; ++j) {
             this.myConstructorSpecificities[j] = new byte[this.myConstructors.length];
         }
         this.myConstructorDescriptions = new PJRmi.MethodDescription[this.myConstructors.length];
         for (int j = 0; j < this.myConstructors.length; ++j) {
             for (int k = 0; k < j; ++k) {
-                final int cmp = MethodUtil.compareBySpecificity(this.myConstructors[j], this.myConstructors[k]);
+                final int cmp = PJRmi.ourMethodUtil.compareConstructorBySpecificity(this.myConstructors[j], this.myConstructors[k]);
                 this.myConstructorSpecificities[j][k] = (byte)Math.signum((float)cmp);
                 this.myConstructorSpecificities[k][j] = (byte)Math.signum((float)(-cmp));
             }
         }
-        this.myMethods = (klass.isInterface() ? this.findInterfaceMethods(klass) : this.findClassMethods(klass));
+        final List<Method> permittedMethods = new ArrayList<Method>();
+        final Method[] array2 = klass.isInterface() ? this.findInterfaceMethods(klass) : this.findClassMethods(klass);
+        for (int length5 = array2.length, n6 = 0; n6 < length5; ++n6) {
+            final Method method = array2[n6];
+            boolean permitted2 = true;
+            for (final Class<?> type2 : method.getParameterTypes()) {
+                if (!this$0.isClassPermitted((Class)type2)) {
+                    permitted2 = false;
+                    break;
+                }
+            }
+            if (permitted2 && this$0.isClassPermitted((Class)method.getReturnType())) {
+                permittedMethods.add(method);
+            }
+            else if (PJRmi.LOG.isLoggable(Level.FINEST)) {
+                PJRmi.LOG.finest("Omitting method with a disallowed class: " + method);
+            }
+        }
+        this.myMethods = permittedMethods.toArray(new Method[permittedMethods.size()]);
         this.myMethodSpecificities = new byte[this.myMethods.length][];
-        for (int j = 0; j < this.myMethods.length; ++j) {
-            this.myMethodSpecificities[j] = new byte[this.myMethods.length];
+        for (int l = 0; l < this.myMethods.length; ++l) {
+            this.myMethodSpecificities[l] = new byte[this.myMethods.length];
         }
         this.myMethodDescriptions = new PJRmi.MethodDescription[this.myMethods.length];
         this.myMethodInstrumentors = (Instrumentor[])(this$0.instrumentMethodCalls() ? new Instrumentor[this.myMethods.length] : null);
-        for (int j = 0; j < this.myMethods.length; ++j) {
-            for (int k = 0; k < j; ++k) {
-                final int cmp = MethodUtil.compareBySpecificity(this.myMethods[j], this.myMethods[k]);
-                this.myMethodSpecificities[j][k] = (byte)Math.signum((float)cmp);
-                this.myMethodSpecificities[k][j] = (byte)Math.signum((float)(-cmp));
+        for (int l = 0; l < this.myMethods.length; ++l) {
+            for (int m = 0; m < l; ++m) {
+                final int cmp2 = PJRmi.ourMethodUtil.compareMethodBySpecificity(this.myMethods[l], this.myMethods[m]);
+                this.myMethodSpecificities[l][m] = (byte)Math.signum((float)cmp2);
+                this.myMethodSpecificities[m][l] = (byte)Math.signum((float)(-cmp2));
             }
         }
         if (PJRmi.LOG.isLoggable(Level.FINEST)) {
             PJRmi.LOG.finest("Created " + this);
         }
     }
```

#### com/deshaw/pjrmi/PJRmi$TypeFlags.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum e5423e4f0b72e05d5dd358f3385ea2d397dc25b1fce28bf95536b3dc9f6b9bea
+  SHA-256 checksum 036b525beac2836467c2fd81ab4adfdd7a2f73d194b8c91d848d2f52496bdbd3
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$TypeFlags extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$TypeFlags>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$TypeFlags
   super_class: #21                        // java/lang/Enum
@@ -125,28 +125,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$TypeFlags;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$TypeFlags;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$TypeFlags;"
          9: areturn
       LineNumberTable:
-        line 917: 0
+        line 919: 0
 
   public static com.deshaw.pjrmi.PJRmi$TypeFlags valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$TypeFlags;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$TypeFlags
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$TypeFlags
          9: areturn
       LineNumberTable:
-        line 917: 0
+        line 919: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -160,17 +160,17 @@
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #7                  // Field value:I
         11: return
       LineNumberTable:
-        line 929: 0
-        line 930: 6
-        line 931: 11
+        line 931: 0
+        line 932: 6
+        line 933: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$TypeFlags;
             0      12     3 value   I
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -250,20 +250,20 @@
        122: dup
        123: iconst_5
        124: getstatic     #20                 // Field IS_FUNCTIONAL_INTERFACE:Lcom/deshaw/pjrmi/PJRmi$TypeFlags;
        127: aastore
        128: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$TypeFlags;
        131: return
       LineNumberTable:
-        line 919: 0
-        line 920: 14
-        line 921: 28
-        line 922: 42
-        line 923: 57
-        line 924: 72
-        line 917: 87
+        line 921: 0
+        line 922: 14
+        line 923: 28
+        line 924: 42
+        line 925: 57
+        line 926: 72
+        line 919: 87
 }
 Signature: #54                          // Ljava/lang/Enum<Lcom/deshaw/pjrmi/PJRmi$TypeFlags;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
   private static final #23= #4 of #58;    // TypeFlags=class com/deshaw/pjrmi/PJRmi$TypeFlags of class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$PythonValueFormat.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3341fbd0c252e3891c31fbf91f4b81c7ba1c3cfa4be0e2cc448d0847b294dcdc
+  SHA-256 checksum f3e215fbaf816fe5ad5e968ab5f1d1cce8699507a721650077379b348f84db3a
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$PythonValueFormat extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$PythonValueFormat>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$PythonValueFormat
   super_class: #29                        // java/lang/Enum
@@ -176,28 +176,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;"
          9: areturn
       LineNumberTable:
-        line 864: 0
+        line 866: 0
 
   public static com.deshaw.pjrmi.PJRmi$PythonValueFormat valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$PythonValueFormat
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$PythonValueFormat
          9: areturn
       LineNumberTable:
-        line 864: 0
+        line 866: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -220,18 +220,18 @@
         19: iload_0
         20: invokedynamic #9,  0              // InvokeDynamic #0:makeConcatWithConstants:(CI)Ljava/lang/String;
         25: invokespecial #10                 // Method java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
         28: athrow
         29: aload_1
         30: areturn
       LineNumberTable:
-        line 896: 0
-        line 897: 9
-        line 898: 13
-        line 902: 29
+        line 898: 0
+        line 899: 9
+        line 900: 13
+        line 904: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      31     0    id   B
             9      22     1 result   Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
           offset_delta = 29
@@ -250,17 +250,17 @@
          2: iload_2
          3: invokespecial #11                 // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #12                 // Field id:B
         11: return
       LineNumberTable:
-        line 909: 0
-        line 910: 6
-        line 911: 11
+        line 911: 0
+        line 912: 6
+        line 913: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
             0      12     3    id   B
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -376,27 +376,27 @@
        191: invokestatic  #7                  // Method java/lang/Byte.toUnsignedInt:(B)I
        194: aload_3
        195: aastore
        196: iinc          2, 1
        199: goto          175
        202: return
       LineNumberTable:
-        line 866: 0
-        line 867: 15
-        line 868: 30
-        line 869: 45
-        line 870: 60
-        line 871: 75
-        line 872: 90
-        line 864: 106
-        line 878: 157
-        line 881: 166
-        line 882: 184
-        line 881: 196
-        line 884: 202
+        line 868: 0
+        line 869: 15
+        line 870: 30
+        line 871: 45
+        line 872: 60
+        line 873: 75
+        line 874: 90
+        line 866: 106
+        line 880: 157
+        line 883: 166
+        line 884: 184
+        line 883: 196
+        line 886: 202
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
           184      12     3    rf   Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;
       StackMapTable: number_of_entries = 2
         frame_type = 254 /* append */
           offset_delta = 175
           locals = [ class "[Lcom/deshaw/pjrmi/PJRmi$PythonValueFormat;", int, int ]
```

#### com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 450388cf922f520ed3c748923163a160db2967c2437e13c9dfcbb3738582a7c6
+  SHA-256 checksum 782279489820941e0447e1ea3a976c4dd65507187f567328fd2365afe1b690f1
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$PJRmiPythonPickle extends com.deshaw.python.PythonPickle
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #31                         // com/deshaw/pjrmi/PJRmi$PJRmiPythonPickle
   super_class: #32                        // com/deshaw/python/PythonPickle
@@ -155,15 +155,15 @@
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method com/deshaw/python/PythonPickle."<init>":()V
          4: return
       LineNumberTable:
-        line 795: 0
+        line 797: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiPythonPickle;
 
   protected void saveObject(java.lang.Object) throws java.lang.UnsupportedOperationException;
     descriptor: (Ljava/lang/Object;)V
     flags: (0x0004) ACC_PROTECTED
@@ -255,35 +255,35 @@
        201: invokevirtual #28                 // Method write:(Lcom/deshaw/python/Operations;)V
        204: goto          212
        207: aload_0
        208: aload_1
        209: invokespecial #30                 // Method com/deshaw/python/PythonPickle.saveObject:(Ljava/lang/Object;)V
        212: return
       LineNumberTable:
-        line 807: 0
-        line 816: 35
-        line 820: 40
-        line 824: 48
-        line 825: 55
-        line 827: 71
-        line 828: 78
-        line 830: 94
-        line 831: 101
-        line 833: 117
-        line 834: 124
-        line 836: 140
-        line 837: 147
-        line 840: 163
-        line 841: 168
-        line 848: 180
-        line 852: 190
-        line 853: 197
-        line 854: 204
-        line 856: 207
-        line 858: 212
+        line 809: 0
+        line 818: 35
+        line 822: 40
+        line 826: 48
+        line 827: 55
+        line 829: 71
+        line 830: 78
+        line 832: 94
+        line 833: 101
+        line 835: 117
+        line 836: 124
+        line 838: 140
+        line 839: 147
+        line 842: 163
+        line 843: 168
+        line 850: 180
+        line 854: 190
+        line 855: 197
+        line 856: 204
+        line 858: 207
+        line 860: 212
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            40     164     2  cube   Lcom/deshaw/hypercube/Hypercube;
             0     213     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiPythonPickle;
             0     213     1   obj   Ljava/lang/Object;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
```

#### com/deshaw/pjrmi/PJRmi$MessageType.class

##### procyon -ec {}

```diff
@@ -20,14 +20,15 @@
     public static final enum MessageType INJECT_CLASS;
     public static final enum MessageType GET_VALUE_OF;
     public static final enum MessageType GET_CALLBACK_HANDLE;
     public static final enum MessageType CALLBACK_RESPONSE;
     public static final enum MessageType GET_PROXY;
     public static final enum MessageType INVOKE_AND_GET_OBJECT;
     public static final enum MessageType INJECT_SOURCE;
+    public static final enum MessageType REPLACE_CLASS;
     public static final enum MessageType OBJECT_REFERENCE;
     public static final enum MessageType TYPE_DESCRIPTION;
     public static final enum MessageType ARBITRARY_ITEM;
     public static final enum MessageType EXCEPTION;
     public static final enum MessageType ASCII_VALUE;
     public static final enum MessageType EMPTY_ACK;
     public static final enum MessageType ARRAY_LENGTH;
@@ -81,32 +82,33 @@
         MessageType.INJECT_CLASS = new MessageType("INJECT_CLASS", 14, (byte)78, false);
         MessageType.GET_VALUE_OF = new MessageType("GET_VALUE_OF", 15, (byte)79, true);
         MessageType.GET_CALLBACK_HANDLE = new MessageType("GET_CALLBACK_HANDLE", 16, (byte)80, false);
         MessageType.CALLBACK_RESPONSE = new MessageType("CALLBACK_RESPONSE", 17, (byte)81, false);
         MessageType.GET_PROXY = new MessageType("GET_PROXY", 18, (byte)82, false);
         MessageType.INVOKE_AND_GET_OBJECT = new MessageType("INVOKE_AND_GET_OBJECT", 19, (byte)83, false);
         MessageType.INJECT_SOURCE = new MessageType("INJECT_SOURCE", 20, (byte)84, false);
-        MessageType.OBJECT_REFERENCE = new MessageType("OBJECT_REFERENCE", 21, (byte)97, false);
-        MessageType.TYPE_DESCRIPTION = new MessageType("TYPE_DESCRIPTION", 22, (byte)98, false);
-        MessageType.ARBITRARY_ITEM = new MessageType("ARBITRARY_ITEM", 23, (byte)99, false);
-        MessageType.EXCEPTION = new MessageType("EXCEPTION", 24, (byte)100, false);
-        MessageType.ASCII_VALUE = new MessageType("ASCII_VALUE", 25, (byte)101, false);
-        MessageType.EMPTY_ACK = new MessageType("EMPTY_ACK", 26, (byte)102, false);
-        MessageType.ARRAY_LENGTH = new MessageType("ARRAY_LENGTH", 27, (byte)103, false);
-        MessageType.UTF16_VALUE = new MessageType("UTF16_VALUE", 28, (byte)104, false);
-        MessageType.PICKLE_BYTES = new MessageType("PICKLE_BYTES", 29, (byte)105, false);
-        MessageType.CALLBACK = new MessageType("CALLBACK", 30, (byte)106, false);
-        MessageType.PYTHON_EVAL_OR_EXEC = new MessageType("PYTHON_EVAL_OR_EXEC", 31, (byte)107, false);
-        MessageType.PYTHON_INVOKE = new MessageType("PYTHON_INVOKE", 32, (byte)108, false);
-        MessageType.OBJECT_CALLBACK = new MessageType("OBJECT_CALLBACK", 33, (byte)109, false);
-        MessageType.GET_OBJECT = new MessageType("GET_OBJECT", 34, (byte)110, false);
-        MessageType.PYTHON_REFERENCE = new MessageType("PYTHON_REFERENCE", 35, (byte)111, false);
-        MessageType.GETATTR = new MessageType("GETATTR", 36, (byte)112, false);
-        MessageType.SET_GLOBAL_VARIABLE = new MessageType("SET_GLOBAL_VARIABLE", 37, (byte)113, false);
-        MessageType.SHMDATA_BYTES = new MessageType("SHMDATA_BYTES", 38, (byte)114, false);
-        MessageType.$VALUES = new MessageType[] { MessageType.NONE, MessageType.INSTANCE_REQUEST, MessageType.ADD_REFERENCE, MessageType.DROP_REFERENCES, MessageType.TYPE_REQUEST, MessageType.METHOD_CALL, MessageType.TO_STRING, MessageType.GET_FIELD, MessageType.SET_FIELD, MessageType.GET_ARRAY_LENGTH, MessageType.NEW_ARRAY_INSTANCE, MessageType.OBJECT_CAST, MessageType.LOCK, MessageType.UNLOCK, MessageType.INJECT_CLASS, MessageType.GET_VALUE_OF, MessageType.GET_CALLBACK_HANDLE, MessageType.CALLBACK_RESPONSE, MessageType.GET_PROXY, MessageType.INVOKE_AND_GET_OBJECT, MessageType.INJECT_SOURCE, MessageType.OBJECT_REFERENCE, MessageType.TYPE_DESCRIPTION, MessageType.ARBITRARY_ITEM, MessageType.EXCEPTION, MessageType.ASCII_VALUE, MessageType.EMPTY_ACK, MessageType.ARRAY_LENGTH, MessageType.UTF16_VALUE, MessageType.PICKLE_BYTES, MessageType.CALLBACK, MessageType.PYTHON_EVAL_OR_EXEC, MessageType.PYTHON_INVOKE, MessageType.OBJECT_CALLBACK, MessageType.GET_OBJECT, MessageType.PYTHON_REFERENCE, MessageType.GETATTR, MessageType.SET_GLOBAL_VARIABLE, MessageType.SHMDATA_BYTES };
+        MessageType.REPLACE_CLASS = new MessageType("REPLACE_CLASS", 21, (byte)85, false);
+        MessageType.OBJECT_REFERENCE = new MessageType("OBJECT_REFERENCE", 22, (byte)97, false);
+        MessageType.TYPE_DESCRIPTION = new MessageType("TYPE_DESCRIPTION", 23, (byte)98, false);
+        MessageType.ARBITRARY_ITEM = new MessageType("ARBITRARY_ITEM", 24, (byte)99, false);
+        MessageType.EXCEPTION = new MessageType("EXCEPTION", 25, (byte)100, false);
+        MessageType.ASCII_VALUE = new MessageType("ASCII_VALUE", 26, (byte)101, false);
+        MessageType.EMPTY_ACK = new MessageType("EMPTY_ACK", 27, (byte)102, false);
+        MessageType.ARRAY_LENGTH = new MessageType("ARRAY_LENGTH", 28, (byte)103, false);
+        MessageType.UTF16_VALUE = new MessageType("UTF16_VALUE", 29, (byte)104, false);
+        MessageType.PICKLE_BYTES = new MessageType("PICKLE_BYTES", 30, (byte)105, false);
+        MessageType.CALLBACK = new MessageType("CALLBACK", 31, (byte)106, false);
+        MessageType.PYTHON_EVAL_OR_EXEC = new MessageType("PYTHON_EVAL_OR_EXEC", 32, (byte)107, false);
+        MessageType.PYTHON_INVOKE = new MessageType("PYTHON_INVOKE", 33, (byte)108, false);
+        MessageType.OBJECT_CALLBACK = new MessageType("OBJECT_CALLBACK", 34, (byte)109, false);
+        MessageType.GET_OBJECT = new MessageType("GET_OBJECT", 35, (byte)110, false);
+        MessageType.PYTHON_REFERENCE = new MessageType("PYTHON_REFERENCE", 36, (byte)111, false);
+        MessageType.GETATTR = new MessageType("GETATTR", 37, (byte)112, false);
+        MessageType.SET_GLOBAL_VARIABLE = new MessageType("SET_GLOBAL_VARIABLE", 38, (byte)113, false);
+        MessageType.SHMDATA_BYTES = new MessageType("SHMDATA_BYTES", 39, (byte)114, false);
+        MessageType.$VALUES = new MessageType[] { MessageType.NONE, MessageType.INSTANCE_REQUEST, MessageType.ADD_REFERENCE, MessageType.DROP_REFERENCES, MessageType.TYPE_REQUEST, MessageType.METHOD_CALL, MessageType.TO_STRING, MessageType.GET_FIELD, MessageType.SET_FIELD, MessageType.GET_ARRAY_LENGTH, MessageType.NEW_ARRAY_INSTANCE, MessageType.OBJECT_CAST, MessageType.LOCK, MessageType.UNLOCK, MessageType.INJECT_CLASS, MessageType.GET_VALUE_OF, MessageType.GET_CALLBACK_HANDLE, MessageType.CALLBACK_RESPONSE, MessageType.GET_PROXY, MessageType.INVOKE_AND_GET_OBJECT, MessageType.INJECT_SOURCE, MessageType.REPLACE_CLASS, MessageType.OBJECT_REFERENCE, MessageType.TYPE_DESCRIPTION, MessageType.ARBITRARY_ITEM, MessageType.EXCEPTION, MessageType.ASCII_VALUE, MessageType.EMPTY_ACK, MessageType.ARRAY_LENGTH, MessageType.UTF16_VALUE, MessageType.PICKLE_BYTES, MessageType.CALLBACK, MessageType.PYTHON_EVAL_OR_EXEC, MessageType.PYTHON_INVOKE, MessageType.OBJECT_CALLBACK, MessageType.GET_OBJECT, MessageType.PYTHON_REFERENCE, MessageType.GETATTR, MessageType.SET_GLOBAL_VARIABLE, MessageType.SHMDATA_BYTES };
         MessageType.VALUES = new MessageType[255];
         for (final MessageType mt : values()) {
             MessageType.VALUES[Byte.toUnsignedInt(mt.id)] = mt;
         }
     }
 }
```

#### com/deshaw/pjrmi/PJRmi$Flags.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 145b2ec544de9dabd40e4e7bcf384e203fd415aae339e8d41a84e041870cbbee
+  SHA-256 checksum e873554fe0a4f4c6725e587dc9d987a813d9429b30306d4960448140eb08f9b0
   Compiled from "PJRmi.java"
 final class com.deshaw.pjrmi.PJRmi$Flags extends java.lang.Enum<com.deshaw.pjrmi.PJRmi$Flags>
   minor version: 0
   major version: 55
   flags: (0x4030) ACC_FINAL, ACC_SUPER, ACC_ENUM
   this_class: #4                          // com/deshaw/pjrmi/PJRmi$Flags
   super_class: #11                        // java/lang/Enum
@@ -85,28 +85,28 @@
     Code:
       stack=1, locals=0, args_size=0
          0: getstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$Flags;
          3: invokevirtual #2                  // Method "[Lcom/deshaw/pjrmi/PJRmi$Flags;".clone:()Ljava/lang/Object;
          6: checkcast     #3                  // class "[Lcom/deshaw/pjrmi/PJRmi$Flags;"
          9: areturn
       LineNumberTable:
-        line 682: 0
+        line 683: 0
 
   public static com.deshaw.pjrmi.PJRmi$Flags valueOf(java.lang.String);
     descriptor: (Ljava/lang/String;)Lcom/deshaw/pjrmi/PJRmi$Flags;
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
       stack=2, locals=1, args_size=1
          0: ldc           #4                  // class com/deshaw/pjrmi/PJRmi$Flags
          2: aload_0
          3: invokestatic  #5                  // Method java/lang/Enum.valueOf:(Ljava/lang/Class;Ljava/lang/String;)Ljava/lang/Enum;
          6: checkcast     #4                  // class com/deshaw/pjrmi/PJRmi$Flags
          9: areturn
       LineNumberTable:
-        line 682: 0
+        line 683: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  name   Ljava/lang/String;
     MethodParameters:
       Name                           Flags
       name                           mandated
 
@@ -120,17 +120,17 @@
          2: iload_2
          3: invokespecial #6                  // Method java/lang/Enum."<init>":(Ljava/lang/String;I)V
          6: aload_0
          7: iload_3
          8: putfield      #7                  // Field value:B
         11: return
       LineNumberTable:
-        line 689: 0
-        line 690: 6
-        line 691: 11
+        line 690: 0
+        line 691: 6
+        line 692: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      12     0  this   Lcom/deshaw/pjrmi/PJRmi$Flags;
             0      12     3 value   B
     MethodParameters:
       Name                           Flags
       $enum$name                     synthetic
@@ -155,15 +155,15 @@
         18: dup
         19: iconst_0
         20: getstatic     #10                 // Field USE_WORKERS:Lcom/deshaw/pjrmi/PJRmi$Flags;
         23: aastore
         24: putstatic     #1                  // Field $VALUES:[Lcom/deshaw/pjrmi/PJRmi$Flags;
         27: return
       LineNumberTable:
-        line 684: 0
-        line 682: 14
+        line 685: 0
+        line 683: 14
 }
 Signature: #39                          // Ljava/lang/Enum<Lcom/deshaw/pjrmi/PJRmi$Flags;>;
 SourceFile: "PJRmi.java"
 NestHost: class com/deshaw/pjrmi/PJRmi
 InnerClasses:
   private static final #13= #4 of #43;    // Flags=class com/deshaw/pjrmi/PJRmi$Flags of class com/deshaw/pjrmi/PJRmi
```

#### com/deshaw/pjrmi/PJRmi$PJRmiLockManager.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum a759f5074f6c3c88979773279b4c11505183f6f6d92f768b923bdb3a557a9fbd
+  SHA-256 checksum 8626b93e04156735d0a0907ceaf2cc54a6976abb7b757ce976ad8fa46bfb90a4
   Compiled from "PJRmi.java"
 public class com.deshaw.pjrmi.PJRmi$PJRmiLockManager extends com.deshaw.util.concurrent.LockManager
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #50                         // com/deshaw/pjrmi/PJRmi$PJRmiLockManager
   super_class: #51                        // com/deshaw/util/concurrent/LockManager
@@ -314,21 +314,21 @@
         29: putfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         32: goto          40
         35: aload_0
         36: aconst_null
         37: putfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         40: return
       LineNumberTable:
-        line 330: 0
-        line 331: 9
-        line 332: 13
-        line 334: 18
-        line 333: 26
-        line 338: 35
-        line 340: 40
+        line 331: 0
+        line 332: 9
+        line 333: 13
+        line 335: 18
+        line 334: 26
+        line 339: 35
+        line 341: 40
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      41     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      41     1 this$0   Lcom/deshaw/pjrmi/PJRmi;
             0      41     2 useGlobalLock   Z
       StackMapTable: number_of_entries = 2
         frame_type = 255 /* full_frame */
@@ -350,15 +350,15 @@
          1: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
          4: ifnull        11
          7: iconst_1
          8: goto          12
         11: iconst_0
         12: ireturn
       LineNumberTable:
-        line 350: 0
+        line 351: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
           stack = [ int ]
@@ -368,15 +368,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
          4: areturn
       LineNumberTable:
-        line 360: 0
+        line 361: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
 
   public com.deshaw.util.concurrent.LockManager$SafeLock lockGlobal() throws com.deshaw.util.concurrent.LockManager$DeadlockException;
     descriptor: ()Lcom/deshaw/util/concurrent/LockManager$SafeLock;
     flags: (0x0001) ACC_PUBLIC
@@ -411,23 +411,23 @@
         74: aload_0
         75: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         78: invokevirtual #18                 // Method com/deshaw/util/concurrent/LockManager$SafeLock.lock:()V
         81: aload_0
         82: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         85: areturn
       LineNumberTable:
-        line 374: 0
-        line 375: 7
-        line 376: 19
-        line 377: 26
-        line 376: 41
-        line 380: 47
-        line 381: 59
-        line 383: 74
-        line 385: 81
+        line 375: 0
+        line 376: 7
+        line 377: 19
+        line 378: 26
+        line 377: 41
+        line 381: 47
+        line 382: 59
+        line 384: 74
+        line 386: 81
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      86     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
       StackMapTable: number_of_entries = 3
         frame_type = 47 /* same */
         frame_type = 26 /* same */
         frame_type = 6 /* same */
@@ -466,23 +466,23 @@
         66: invokedynamic #19,  0             // InvokeDynamic #2:makeConcatWithConstants:(Ljava/lang/Thread;)Ljava/lang/String;
         71: invokevirtual #17                 // Method java/util/logging/Logger.finer:(Ljava/lang/String;)V
         74: aload_0
         75: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         78: invokevirtual #20                 // Method com/deshaw/util/concurrent/LockManager$SafeLock.unlock:()V
         81: return
       LineNumberTable:
-        line 393: 0
-        line 394: 7
-        line 395: 19
-        line 396: 26
-        line 395: 41
-        line 399: 47
-        line 400: 59
-        line 402: 74
-        line 404: 81
+        line 394: 0
+        line 395: 7
+        line 396: 19
+        line 397: 26
+        line 396: 41
+        line 400: 47
+        line 401: 59
+        line 403: 74
+        line 405: 81
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      82     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
       StackMapTable: number_of_entries = 3
         frame_type = 47 /* same */
         frame_type = 26 /* same */
         frame_type = 6 /* same */
@@ -498,17 +498,17 @@
          7: aload_0
          8: getfield      #7                  // Field myGlobalLock:Lcom/deshaw/util/concurrent/LockManager$SafeLock;
         11: invokevirtual #21                 // Method com/deshaw/util/concurrent/LockManager$SafeLock.isHeldByCurrentThread:()Z
         14: ireturn
         15: iconst_0
         16: ireturn
       LineNumberTable:
-        line 413: 0
-        line 414: 7
-        line 417: 15
+        line 414: 0
+        line 415: 7
+        line 418: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      17     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
       StackMapTable: number_of_entries = 1
         frame_type = 15 /* same */
 
   public void invokeWithoutGlobalLock(java.lang.Runnable) throws com.deshaw.util.concurrent.LockManager$DeadlockException, java.lang.reflect.UndeclaredThrowableException;
@@ -523,16 +523,16 @@
          6: aload_1
          7: invokespecial #23                 // Method com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1."<init>":(Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;Ljava/lang/Runnable;)V
         10: aconst_null
         11: invokevirtual #24                 // Method invokeWithoutGlobalLock:(Ljava/util/function/Function;Ljava/lang/Object;)Ljava/lang/Object;
         14: pop
         15: return
       LineNumberTable:
-        line 436: 0
-        line 445: 15
+        line 437: 0
+        line 446: 15
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      16     1 runnable   Ljava/lang/Runnable;
     Exceptions:
       throws com.deshaw.util.concurrent.LockManager$DeadlockException, java.lang.reflect.UndeclaredThrowableException
     MethodParameters:
@@ -550,15 +550,15 @@
          5: aload_0
          6: aload_1
          7: invokespecial #26                 // Method com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2."<init>":(Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;Ljava/util/function/Supplier;)V
         10: aconst_null
         11: invokevirtual #24                 // Method invokeWithoutGlobalLock:(Ljava/util/function/Function;Ljava/lang/Object;)Ljava/lang/Object;
         14: areturn
       LineNumberTable:
-        line 465: 0
+        line 466: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      15     1 function   Ljava/util/function/Supplier;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      15     1 function   Ljava/util/function/Supplier<TT;>;
@@ -614,29 +614,29 @@
         77: athrow
       Exception table:
          from    to  target type
              2    28    46   Class java/lang/Throwable
              2    28    58   any
             46    60    58   any
       LineNumberTable:
-        line 499: 0
-        line 503: 2
-        line 504: 9
-        line 505: 13
-        line 509: 19
-        line 516: 28
-        line 517: 32
-        line 518: 37
-        line 509: 43
-        line 511: 46
-        line 512: 48
-        line 516: 58
-        line 517: 64
-        line 518: 69
-        line 520: 75
+        line 500: 0
+        line 504: 2
+        line 505: 9
+        line 506: 13
+        line 510: 19
+        line 517: 28
+        line 518: 32
+        line 519: 37
+        line 510: 43
+        line 512: 46
+        line 513: 48
+        line 517: 58
+        line 518: 64
+        line 519: 69
+        line 521: 75
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            48      10     4     t   Ljava/lang/Throwable;
             0      78     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      78     1 function   Ljava/util/function/Function;
             0      78     2 argument   Ljava/lang/Object;
             2      76     3 lockCount   I
@@ -688,19 +688,19 @@
         19: invokespecial #36                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/Throwable;)V
         22: athrow
         23: return
       Exception table:
          from    to  target type
              0    10    13   Class java/lang/reflect/UndeclaredThrowableException
       LineNumberTable:
-        line 535: 0
-        line 549: 10
-        line 546: 13
-        line 548: 14
-        line 550: 23
+        line 536: 0
+        line 550: 10
+        line 547: 13
+        line 549: 14
+        line 551: 23
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            14       9     3     e   Ljava/lang/reflect/UndeclaredThrowableException;
             0      24     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      24     1 millis   J
       StackMapTable: number_of_entries = 2
         frame_type = 77 /* same_locals_1_stack_item */
@@ -729,19 +729,19 @@
         19: invokespecial #36                 // Method java/lang/RuntimeException."<init>":(Ljava/lang/Throwable;)V
         22: athrow
         23: return
       Exception table:
          from    to  target type
              0    10    13   Class java/lang/reflect/UndeclaredThrowableException
       LineNumberTable:
-        line 566: 0
-        line 578: 10
-        line 575: 13
-        line 577: 14
-        line 579: 23
+        line 567: 0
+        line 579: 10
+        line 576: 13
+        line 578: 14
+        line 580: 23
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            14       9     2     e   Ljava/lang/reflect/UndeclaredThrowableException;
             0      24     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      24     1 monitor   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 77 /* same_locals_1_stack_item */
@@ -760,15 +760,15 @@
       stack=3, locals=2, args_size=2
          0: new           #38                 // class java/lang/UnsupportedOperationException
          3: dup
          4: ldc           #39                 // String Shared locks not supported
          6: invokespecial #40                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
          9: athrow
       LineNumberTable:
-        line 588: 0
+        line 589: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      10     1 lockName   Ljava/lang/CharSequence;
     MethodParameters:
       Name                           Flags
       lockName                       final
@@ -789,17 +789,17 @@
         16: invokespecial #43                 // Method com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock."<init>":(Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;Ljava/lang/CharSequence;)V
         19: goto          27
         22: aload_0
         23: aload_1
         24: invokespecial #44                 // Method com/deshaw/util/concurrent/LockManager.newNamedLock:(Ljava/lang/CharSequence;)Lcom/deshaw/util/concurrent/LockManager$LockManagerLock;
         27: areturn
       LineNumberTable:
-        line 599: 0
-        line 600: 22
-        line 599: 27
+        line 600: 0
+        line 601: 22
+        line 600: 27
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
             0      28     1  name   Ljava/lang/CharSequence;
       StackMapTable: number_of_entries = 2
         frame_type = 22 /* same */
         frame_type = 68 /* same_locals_1_stack_item */
@@ -819,17 +819,17 @@
          7: ifeq          16
         10: invokestatic  #45                 // Method com/deshaw/util/concurrent/VirtualThreadLock.getThread:()Lcom/deshaw/util/concurrent/VirtualThreadLock$VirtualThread;
         13: goto          20
         16: aload_0
         17: invokespecial #46                 // Method com/deshaw/util/concurrent/LockManager.currentThread:()Ljava/lang/Thread;
         20: areturn
       LineNumberTable:
-        line 609: 0
-        line 610: 16
-        line 609: 20
+        line 610: 0
+        line 611: 16
+        line 610: 20
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      21     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
       StackMapTable: number_of_entries = 2
         frame_type = 16 /* same */
         frame_type = 67 /* same_locals_1_stack_item */
           stack = [ class java/lang/Thread ]
@@ -844,18 +844,18 @@
          4: goto          8
          7: astore_1
          8: return
       Exception table:
          from    to  target type
              0     4     7   Class java/lang/InterruptedException
       LineNumberTable:
-        line 568: 0
-        line 572: 4
-        line 570: 7
-        line 573: 8
+        line 569: 0
+        line 573: 4
+        line 571: 7
+        line 574: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 monitor   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 71 /* same_locals_1_stack_item */
           stack = [ class java/lang/InterruptedException ]
         frame_type = 0 /* same */
@@ -870,18 +870,18 @@
          4: goto          8
          7: astore_2
          8: return
       Exception table:
          from    to  target type
              0     4     7   Class java/lang/InterruptedException
       LineNumberTable:
-        line 538: 0
-        line 542: 4
-        line 540: 7
-        line 543: 8
+        line 539: 0
+        line 543: 4
+        line 541: 7
+        line 544: 8
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       9     0 millis   J
       StackMapTable: number_of_entries = 2
         frame_type = 71 /* same_locals_1_stack_item */
           stack = [ class java/lang/InterruptedException ]
         frame_type = 0 /* same */
```

#### com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 6e15602d4edc27ee4298a50819e6b2b91a2071db6b734067f1e3ab7371513ed5
+  SHA-256 checksum c9f522db9e2624a21613c73df769dbb400aec41737f4ac8b0dbe57a84c0ce57b
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$PJRmiLockManager$2 extends java.lang.Object implements java.util.function.Function<java.lang.Object, T>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #5                          // com/deshaw/pjrmi/PJRmi$PJRmiLockManager$2
   super_class: #6                         // java/lang/Object
@@ -79,15 +79,15 @@
          5: aload_0
          6: aload_2
          7: putfield      #2                  // Field val$function:Ljava/util/function/Supplier;
         10: aload_0
         11: invokespecial #3                  // Method java/lang/Object."<init>":()V
         14: return
       LineNumberTable:
-        line 466: 0
+        line 467: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$2;
             0      15     1 this$1   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
     MethodParameters:
       Name                           Flags
       this$1                         final mandated
@@ -99,15 +99,15 @@
     Code:
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field val$function:Ljava/util/function/Supplier;
          4: invokeinterface #4,  1            // InterfaceMethod java/util/function/Supplier.get:()Ljava/lang/Object;
          9: areturn
       LineNumberTable:
-        line 468: 0
+        line 469: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$2;
             0      10     1 notused   Ljava/lang/Object;
     MethodParameters:
       Name                           Flags
       notused
```

#### com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 40c92fca1c71647487e2fc5e5eaaba35108e5f7223b8d6db76851730e55dea3c
+  SHA-256 checksum efdac815511709904ea510db6f13ca1b1a031fa54a6bacc37b9aab83d33daafa
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$PJRmiLockManager$1 extends java.lang.Object implements java.util.function.Function<java.lang.Object, java.lang.Object>
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #5                          // com/deshaw/pjrmi/PJRmi$PJRmiLockManager$1
   super_class: #6                         // java/lang/Object
@@ -77,15 +77,15 @@
          5: aload_0
          6: aload_2
          7: putfield      #2                  // Field val$runnable:Ljava/lang/Runnable;
         10: aload_0
         11: invokespecial #3                  // Method java/lang/Object."<init>":()V
         14: return
       LineNumberTable:
-        line 437: 0
+        line 438: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      15     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$1;
             0      15     1 this$1   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager;
     MethodParameters:
       Name                           Flags
       this$1                         final mandated
@@ -98,16 +98,16 @@
       stack=1, locals=2, args_size=2
          0: aload_0
          1: getfield      #2                  // Field val$runnable:Ljava/lang/Runnable;
          4: invokeinterface #4,  1            // InterfaceMethod java/lang/Runnable.run:()V
          9: aconst_null
         10: areturn
       LineNumberTable:
-        line 439: 0
-        line 440: 9
+        line 440: 0
+        line 441: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$1;
             0      11     1 notused   Ljava/lang/Object;
     MethodParameters:
       Name                           Flags
       notused
```

#### com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 1878955ee0b43c3004a563ea64a9f6f148ee33899ea7a8a9d5a50c1b8d6014d4
+  SHA-256 checksum 28fe0588f1c75333e14bc725333393490924f85a33986e6334df86e83aacd742
   Compiled from "PJRmi.java"
 class com.deshaw.pjrmi.PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock extends com.deshaw.util.concurrent.VirtualThreadLock implements com.deshaw.util.concurrent.LockManager$LockManagerLock
   minor version: 0
   major version: 55
   flags: (0x0020) ACC_SUPER
   this_class: #22                         // com/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock
   super_class: #23                        // com/deshaw/util/concurrent/VirtualThreadLock
@@ -166,19 +166,19 @@
         21: invokespecial #5                  // Method com/deshaw/util/concurrent/LockManager$ColouredList."<init>":(I)V
         24: putfield      #6                  // Field myLockers:Lcom/deshaw/util/concurrent/LockManager$ColouredList;
         27: aload_0
         28: getstatic     #7                  // Field java/util/logging/Level.FINEST:Ljava/util/logging/Level;
         31: putfield      #8                  // Field myLogLevel:Ljava/util/logging/Level;
         34: return
       LineNumberTable:
-        line 169: 0
-        line 170: 5
-        line 171: 15
-        line 172: 27
-        line 173: 34
+        line 170: 0
+        line 171: 5
+        line 172: 15
+        line 173: 27
+        line 174: 34
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      35     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      35     2  name   Ljava/lang/CharSequence;
     MethodParameters:
       Name                           Flags
       this$1                         final synthetic
@@ -189,15 +189,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #6                  // Field myLockers:Lcom/deshaw/util/concurrent/LockManager$ColouredList;
          4: areturn
       LineNumberTable:
-        line 181: 0
+        line 182: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
     Signature: #53                          // ()Lcom/deshaw/util/concurrent/LockManager$ColouredList<Lcom/deshaw/util/concurrent/LockManager$LockManagerLock$Locker;>;
 
   public void lock(boolean);
     descriptor: (Z)V
@@ -212,18 +212,18 @@
         11: new           #10                 // class java/lang/UnsupportedOperationException
         14: dup
         15: ldc           #11                 // String Shared locks not supported
         17: invokespecial #12                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
         20: athrow
         21: return
       LineNumberTable:
-        line 190: 0
-        line 191: 4
-        line 194: 11
-        line 198: 21
+        line 191: 0
+        line 192: 4
+        line 195: 11
+        line 199: 21
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      22     1 isExclusive   Z
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 9 /* same */
@@ -243,17 +243,17 @@
          8: ireturn
          9: new           #10                 // class java/lang/UnsupportedOperationException
         12: dup
         13: ldc           #11                 // String Shared locks not supported
         15: invokespecial #12                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
         18: athrow
       LineNumberTable:
-        line 206: 0
-        line 207: 4
-        line 210: 9
+        line 207: 0
+        line 208: 4
+        line 211: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      19     1 isExclusive   Z
       StackMapTable: number_of_entries = 1
         frame_type = 9 /* same */
     MethodParameters:
@@ -274,17 +274,17 @@
         11: ireturn
         12: new           #10                 // class java/lang/UnsupportedOperationException
         15: dup
         16: ldc           #11                 // String Shared locks not supported
         18: invokespecial #12                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
         21: athrow
       LineNumberTable:
-        line 225: 0
-        line 226: 4
-        line 229: 12
+        line 226: 0
+        line 227: 4
+        line 230: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      22     1 isExclusive   Z
             0      22     2  time   J
             0      22     4  unit   Ljava/util/concurrent/TimeUnit;
       StackMapTable: number_of_entries = 1
@@ -310,18 +310,18 @@
         11: new           #10                 // class java/lang/UnsupportedOperationException
         14: dup
         15: ldc           #11                 // String Shared locks not supported
         17: invokespecial #12                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
         20: athrow
         21: return
       LineNumberTable:
-        line 241: 0
-        line 242: 4
-        line 245: 11
-        line 249: 21
+        line 242: 0
+        line 243: 4
+        line 246: 11
+        line 250: 21
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      22     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      22     1 isExclusive   Z
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 9 /* same */
@@ -341,17 +341,17 @@
          8: areturn
          9: new           #10                 // class java/lang/UnsupportedOperationException
         12: dup
         13: ldc           #11                 // String Shared locks not supported
         15: invokespecial #12                 // Method java/lang/UnsupportedOperationException."<init>":(Ljava/lang/String;)V
         18: athrow
       LineNumberTable:
-        line 257: 0
-        line 258: 4
-        line 261: 9
+        line 258: 0
+        line 259: 4
+        line 262: 9
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      19     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      19     1 isExclusive   Z
       StackMapTable: number_of_entries = 1
         frame_type = 9 /* same */
     MethodParameters:
@@ -367,15 +367,15 @@
          1: ifeq          11
          4: aload_0
          5: invokespecial #17                 // Method com/deshaw/util/concurrent/VirtualThreadLock.isHeldByCurrentThread:()Z
          8: goto          12
         11: iconst_0
         12: ireturn
       LineNumberTable:
-        line 276: 0
+        line 277: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      13     1 isExclusive   Z
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
@@ -393,15 +393,15 @@
          1: ifeq          11
          4: aload_0
          5: invokespecial #18                 // Method com/deshaw/util/concurrent/VirtualThreadLock.getHoldCount:()I
          8: goto          12
         11: iconst_0
         12: ireturn
       LineNumberTable:
-        line 287: 0
+        line 288: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      13     1 isExclusive   Z
       StackMapTable: number_of_entries = 2
         frame_type = 11 /* same */
         frame_type = 64 /* same_locals_1_stack_item */
@@ -415,15 +415,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #8                  // Field myLogLevel:Ljava/util/logging/Level;
          4: areturn
       LineNumberTable:
-        line 296: 0
+        line 297: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
 
   public void setLogLevel(java.util.logging.Level);
     descriptor: (Ljava/util/logging/Level;)V
     flags: (0x0001) ACC_PUBLIC
@@ -437,18 +437,18 @@
         10: invokespecial #21                 // Method java/lang/NullPointerException."<init>":(Ljava/lang/String;)V
         13: athrow
         14: aload_0
         15: aload_1
         16: putfield      #8                  // Field myLogLevel:Ljava/util/logging/Level;
         19: return
       LineNumberTable:
-        line 305: 0
-        line 306: 4
-        line 308: 14
-        line 309: 19
+        line 306: 0
+        line 307: 4
+        line 309: 14
+        line 310: 19
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lcom/deshaw/pjrmi/PJRmi$PJRmiLockManager$PJRmiVirtualThreadLock;
             0      20     1 level   Ljava/util/logging/Level;
       StackMapTable: number_of_entries = 1
         frame_type = 14 /* same */
     MethodParameters:
```

#### com/deshaw/pjrmi/MethodUtil.class

##### procyon -ec {}

```diff
@@ -3,90 +3,33 @@
 
 import java.util.Objects;
 import java.lang.reflect.Constructor;
 import java.lang.reflect.Method;
 
 public class MethodUtil
 {
+    public static final MethodUtil INSTANCE;
+    
     public static int compareBySpecificity(final Method m1, final Method m2) {
-        return compareBySpecificity((MethodUtil.CallableWrapper)new MethodUtil.MethodWrapper(m1), (MethodUtil.CallableWrapper)new MethodUtil.MethodWrapper(m2));
+        return MethodUtil.INSTANCE.compareMethodBySpecificity(m1, m2);
     }
     
     public static int compareBySpecificity(final Constructor<?> m1, final Constructor<?> m2) {
-        return compareBySpecificity((MethodUtil.CallableWrapper)new MethodUtil.ConstructorWrapper((Constructor)m1), (MethodUtil.CallableWrapper)new MethodUtil.ConstructorWrapper((Constructor)m2));
+        return MethodUtil.INSTANCE.compareConstructorBySpecificity(m1, m2);
     }
     
-    private static int compareBySpecificity(final MethodUtil.CallableWrapper w1, final MethodUtil.CallableWrapper w2) {
-        final String n1 = w1.getName();
-        final String n2 = w2.getName();
-        if (!n1.equals(n2)) {
-            return 0;
-        }
-        final Class<?>[] a1 = w1.getParameterTypes();
-        final Class<?>[] a2 = w2.getParameterTypes();
-        if (a1.length != a2.length) {
-            return 0;
-        }
-        boolean match = true;
-        int cmp = 0;
-        for (int i = 0; i < a1.length; ++i) {
-            final Class<?> c1 = a1[i];
-            final Class<?> c2 = a2[i];
-            if (!areEquivalent(c1, c2)) {
-                if (isAssignableFrom(c1, c2)) {
-                    if (cmp < 0) {
-                        return 0;
-                    }
-                    cmp = 1;
-                    match = false;
-                }
-                else if (isAssignableFrom(c2, c1)) {
-                    if (cmp > 0) {
-                        return 0;
-                    }
-                    cmp = -1;
-                    match = false;
-                }
-                else if (c1.isArray() && c2.isArray() && isArrayMoreSpecific(c2, c1)) {
-                    if (cmp < 0) {
-                        return 0;
-                    }
-                    cmp = 1;
-                    match = false;
-                }
-                else {
-                    if (!c1.isArray() || !c2.isArray() || !isArrayMoreSpecific(c1, c2)) {
-                        return 0;
-                    }
-                    if (cmp > 0) {
-                        return 0;
-                    }
-                    cmp = -1;
-                    match = false;
-                }
-            }
-        }
-        if (!match) {
-            return cmp;
-        }
-        final Class<?> r1 = w1.getReturnType();
-        final Class<?> r2 = w2.getReturnType();
-        if (r1.equals(r2)) {
-            return 0;
-        }
-        if (isAssignableFrom(r1, r2)) {
-            return 1;
-        }
-        if (isAssignableFrom(r2, r1)) {
-            return -1;
-        }
-        return 0;
+    public int compareMethodBySpecificity(final Method m1, final Method m2) {
+        return this.compareBySpecificity((MethodUtil.CallableWrapper)new MethodUtil.MethodWrapper(m1), (MethodUtil.CallableWrapper)new MethodUtil.MethodWrapper(m2));
+    }
+    
+    public int compareConstructorBySpecificity(final Constructor<?> m1, final Constructor<?> m2) {
+        return this.compareBySpecificity((MethodUtil.CallableWrapper)new MethodUtil.ConstructorWrapper((Constructor)m1), (MethodUtil.CallableWrapper)new MethodUtil.ConstructorWrapper((Constructor)m2));
     }
     
-    private static boolean areEquivalent(final Class<?> c1, final Class<?> c2) {
+    protected boolean areEquivalent(final Class<?> c1, final Class<?> c2) {
         if (Objects.equals(c1, c2)) {
             return true;
         }
         if (c1 == null || c2 == null) {
             return false;
         }
         if (c1.isPrimitive() && !c2.isPrimitive()) {
@@ -150,15 +93,19 @@
             if (c2.equals(Void.TYPE)) {
                 return c1.equals(Void.class);
             }
             throw new UnsupportedOperationException("Unhandled native type: " + c2);
         }
     }
     
-    private static boolean isAssignableFrom(final Class<?> c1, final Class<?> c2) {
+    protected boolean isMoreSpecific(final Class<?> c1, final Class<?> c2) {
+        return false;
+    }
+    
+    protected boolean isAssignableFrom(final Class<?> c1, final Class<?> c2) {
         if (c1 == null || c2 == null) {
             return false;
         }
         if (!c1.isPrimitive() && !c2.isPrimitive()) {
             return c1.isAssignableFrom(c2);
         }
         if (c1.isPrimitive() && c2.isPrimitive()) {
@@ -252,16 +199,101 @@
             if (c2.equals(Void.TYPE)) {
                 return c1.equals(Void.class);
             }
             throw new UnsupportedOperationException("Unhandled native type: " + c2);
         }
     }
     
-    private static boolean isArrayMoreSpecific(final Class<?> c1, final Class<?> c2) {
+    protected boolean isArrayMoreSpecific(final Class<?> c1, final Class<?> c2) {
         final Class<?> t1 = c1.getComponentType();
         final Class<?> t2 = c2.getComponentType();
         if (t1.isArray() && t2.isArray()) {
-            return isArrayMoreSpecific(t1, t2);
+            return this.isArrayMoreSpecific(t1, t2);
         }
-        return (t1.isPrimitive() && !t2.isPrimitive() && !t2.isArray() && !isAssignableFrom(t1, t2)) || (isAssignableFrom(t2, t1) && !isAssignableFrom(t1, t2));
+        return (t1.isPrimitive() && !t2.isPrimitive() && !t2.isArray() && !this.isAssignableFrom(t1, t2)) || (this.isAssignableFrom(t2, t1) && !this.isAssignableFrom(t1, t2));
+    }
+    
+    private int compareBySpecificity(final MethodUtil.CallableWrapper w1, final MethodUtil.CallableWrapper w2) {
+        final String n1 = w1.getName();
+        final String n2 = w2.getName();
+        if (!n1.equals(n2)) {
+            return 0;
+        }
+        final Class<?>[] a1 = w1.getParameterTypes();
+        final Class<?>[] a2 = w2.getParameterTypes();
+        if (a1.length != a2.length) {
+            return 0;
+        }
+        boolean match = true;
+        int cmp = 0;
+        for (int i = 0; i < a1.length; ++i) {
+            final Class<?> c1 = a1[i];
+            final Class<?> c2 = a2[i];
+            if (!this.areEquivalent(c1, c2)) {
+                if (this.isMoreSpecific(c2, c1)) {
+                    if (cmp < 0) {
+                        return 0;
+                    }
+                    cmp = 1;
+                    match = false;
+                }
+                else if (this.isMoreSpecific(c1, c2)) {
+                    if (cmp > 0) {
+                        return 0;
+                    }
+                    cmp = -1;
+                    match = false;
+                }
+                else if (this.isAssignableFrom(c1, c2)) {
+                    if (cmp < 0) {
+                        return 0;
+                    }
+                    cmp = 1;
+                    match = false;
+                }
+                else if (this.isAssignableFrom(c2, c1)) {
+                    if (cmp > 0) {
+                        return 0;
+                    }
+                    cmp = -1;
+                    match = false;
+                }
+                else if (c1.isArray() && c2.isArray() && this.isArrayMoreSpecific(c2, c1)) {
+                    if (cmp < 0) {
+                        return 0;
+                    }
+                    cmp = 1;
+                    match = false;
+                }
+                else {
+                    if (!c1.isArray() || !c2.isArray() || !this.isArrayMoreSpecific(c1, c2)) {
+                        return 0;
+                    }
+                    if (cmp > 0) {
+                        return 0;
+                    }
+                    cmp = -1;
+                    match = false;
+                }
+            }
+        }
+        if (!match) {
+            return cmp;
+        }
+        final Class<?> r1 = w1.getReturnType();
+        final Class<?> r2 = w2.getReturnType();
+        if (r1.equals(r2)) {
+            return 0;
+        }
+        if (this.isAssignableFrom(r1, r2)) {
+            return 1;
+        }
+        if (this.isAssignableFrom(r2, r1)) {
+            return -1;
+        }
+        return 0;
+    }
+    
+    static {
+        INSTANCE = new MethodUtil();
     }
 }
```

#### com/deshaw/pjrmi/SourceInjector.class

##### procyon -ec {}

```diff
@@ -48,15 +48,14 @@
         final JavaCompiler.CompilationTask task = compiler.getTask(null, fileManager, diagnostics, Arrays.asList("-parameters"), null, (Iterable<? extends JavaFileObject>)Arrays.asList(stringObject));
         if (!(boolean)task.call()) {
             final StringBuilder errorMsg = new StringBuilder();
             for (final Diagnostic d : diagnostics.getDiagnostics()) {
                 final int lineNumber = (int)d.getLineNumber();
                 errorMsg.append("Compilation error: line ").append(lineNumber).append(' ').append(d.getMessage((Locale)null));
                 boolean found = false;
-                final StringBuilder sb = new StringBuilder();
                 for (int i = 0, line = 1; i < source.length() && line <= lineNumber; ++i) {
                     final char c = source.charAt(i);
                     if (c == '\n') {
                         ++line;
                     }
                     else if (line == lineNumber) {
                         if (!found) {
```

#### com/deshaw/util/StringUtil.class

##### procyon -ec {}

```diff
@@ -4,15 +4,14 @@
 import java.text.ParseException;
 import java.io.Writer;
 import java.io.PrintWriter;
 import java.io.StringWriter;
 
 public class StringUtil
 {
-    private static final ThreadLocalStringBuilder ourStringBuilder;
     private static final char[] HEX_DIGITS;
     
     public static String stackTraceToString(final Throwable e) {
         final StringWriter sw = new StringWriter();
         final PrintWriter pw = new PrintWriter(sw);
         e.printStackTrace(pw);
         return sw.toString();
@@ -67,11 +66,10 @@
         if (equalsIgnoreCase("false", s)) {
             return false;
         }
         throw new ParseException("'" + s + "' does not describe a boolean value", 0);
     }
     
     static {
-        ourStringBuilder = new ThreadLocalStringBuilder(1024);
         HEX_DIGITS = new char[] { '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 'A', 'B', 'C', 'D', 'E', 'F' };
     }
 }
```

#### com/deshaw/util/StringUtil$HashableSubSequence.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum c73f0d6ac29487f8027bf244834fcf8ef04ac9ef4d02f92a6697673efebe0c72
+  SHA-256 checksum ad73d50d35b9ae9d00ee0ef898cf9da81798349ab74558c5a742ef6ea49f94be
   Compiled from "StringUtil.java"
 public class com.deshaw.util.StringUtil$HashableSubSequence implements java.lang.CharSequence
   minor version: 0
   major version: 55
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #12                         // com/deshaw/util/StringUtil$HashableSubSequence
   super_class: #22                        // java/lang/Object
@@ -148,16 +148,16 @@
          0: aload_0
          1: aconst_null
          2: iconst_0
          3: iconst_0
          4: invokespecial #1                  // Method "<init>":(Ljava/lang/CharSequence;II)V
          7: return
       LineNumberTable:
-        line 65: 0
-        line 66: 7
+        line 47: 0
+        line 48: 7
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       8     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
 
   public com.deshaw.util.StringUtil$HashableSubSequence(java.lang.CharSequence);
     descriptor: (Ljava/lang/CharSequence;)V
     flags: (0x0001) ACC_PUBLIC
@@ -170,17 +170,17 @@
          6: iconst_0
          7: aload_1
          8: invokeinterface #3,  1            // InterfaceMethod java/lang/CharSequence.length:()I
         13: invokevirtual #4                  // Method wrap:(Ljava/lang/CharSequence;II)Lcom/deshaw/util/StringUtil$HashableSubSequence;
         16: pop
         17: return
       LineNumberTable:
-        line 72: 0
-        line 73: 4
-        line 74: 17
+        line 54: 0
+        line 55: 4
+        line 56: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      18     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      18     1   seq   Ljava/lang/CharSequence;
     MethodParameters:
       Name                           Flags
       seq
@@ -196,17 +196,17 @@
          5: aload_1
          6: iload_2
          7: iload_3
          8: invokevirtual #4                  // Method wrap:(Ljava/lang/CharSequence;II)Lcom/deshaw/util/StringUtil$HashableSubSequence;
         11: pop
         12: return
       LineNumberTable:
-        line 80: 0
-        line 81: 4
-        line 82: 12
+        line 62: 0
+        line 63: 4
+        line 64: 12
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      13     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      13     1   seq   Ljava/lang/CharSequence;
             0      13     2 start   I
             0      13     3 length   I
     MethodParameters:
@@ -220,15 +220,15 @@
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: getfield      #5                  // Field myLength:I
          4: ireturn
       LineNumberTable:
-        line 90: 0
+        line 72: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
 
   public char charAt(int);
     descriptor: (I)C
     flags: (0x0001) ACC_PUBLIC
@@ -253,17 +253,17 @@
         34: aload_0
         35: getfield      #10                 // Field myStart:I
         38: iload_1
         39: iadd
         40: invokeinterface #11,  2           // InterfaceMethod java/lang/CharSequence.charAt:(I)C
         45: ireturn
       LineNumberTable:
-        line 99: 0
-        line 100: 12
-        line 104: 30
+        line 81: 0
+        line 82: 12
+        line 86: 30
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      46     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      46     1 index   I
       StackMapTable: number_of_entries = 2
         frame_type = 12 /* same */
         frame_type = 17 /* same */
@@ -291,17 +291,17 @@
         18: getfield      #5                  // Field myLength:I
         21: iload_1
         22: isub
         23: invokestatic  #13                 // Method java/lang/Math.min:(II)I
         26: invokespecial #1                  // Method "<init>":(Ljava/lang/CharSequence;II)V
         29: areturn
       LineNumberTable:
-        line 113: 0
-        line 116: 23
-        line 113: 29
+        line 95: 0
+        line 98: 23
+        line 95: 29
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      30     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      30     1 start   I
             0      30     2   end   I
     MethodParameters:
       Name                           Flags
@@ -337,19 +337,19 @@
         36: iadd
         37: istore_1
         38: iinc          2, 1
         41: goto          17
         44: iload_1
         45: ireturn
       LineNumberTable:
-        line 127: 0
-        line 128: 2
-        line 129: 22
-        line 128: 38
-        line 131: 44
+        line 109: 0
+        line 110: 2
+        line 111: 22
+        line 110: 38
+        line 113: 44
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             7      37     2     i   I
            17      27     3   end   I
             0      46     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             2      44     1 result   I
       StackMapTable: number_of_entries = 2
@@ -406,28 +406,28 @@
         72: iconst_0
         73: ireturn
         74: iinc          3, 1
         77: goto          49
         80: iconst_1
         81: ireturn
       LineNumberTable:
-        line 141: 0
-        line 142: 4
-        line 146: 6
-        line 147: 18
-        line 149: 20
-        line 152: 25
-        line 153: 30
-        line 157: 32
-        line 158: 45
-        line 162: 47
-        line 163: 57
-        line 164: 72
-        line 162: 74
-        line 169: 80
+        line 123: 0
+        line 124: 4
+        line 128: 6
+        line 129: 18
+        line 131: 20
+        line 134: 25
+        line 135: 30
+        line 139: 32
+        line 140: 45
+        line 144: 47
+        line 145: 57
+        line 146: 72
+        line 144: 74
+        line 151: 80
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            49      31     3     i   I
             0      82     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      82     1     o   Ljava/lang/Object;
            25      57     2  that   Ljava/lang/CharSequence;
       StackMapTable: number_of_entries = 7
@@ -476,20 +476,20 @@
         42: aload_0
         43: getfield      #5                  // Field myLength:I
         46: iadd
         47: invokeinterface #19,  3           // InterfaceMethod java/lang/CharSequence.subSequence:(II)Ljava/lang/CharSequence;
         52: invokeinterface #20,  1           // InterfaceMethod java/lang/CharSequence.toString:()Ljava/lang/String;
         57: areturn
       LineNumberTable:
-        line 178: 0
-        line 179: 7
-        line 185: 10
-        line 186: 15
-        line 187: 22
-        line 190: 33
+        line 160: 0
+        line 161: 7
+        line 167: 10
+        line 168: 15
+        line 169: 22
+        line 172: 33
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
            15      43     1   seq   Ljava/lang/CharSequence;
             0      58     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
       StackMapTable: number_of_entries = 3
         frame_type = 10 /* same */
         frame_type = 252 /* append */
@@ -514,17 +514,17 @@
         15: aload_1
         16: iconst_0
         17: aload_1
         18: invokeinterface #3,  1            // InterfaceMethod java/lang/CharSequence.length:()I
         23: invokevirtual #4                  // Method wrap:(Ljava/lang/CharSequence;II)Lcom/deshaw/util/StringUtil$HashableSubSequence;
         26: areturn
       LineNumberTable:
-        line 206: 0
-        line 207: 14
-        line 206: 26
+        line 188: 0
+        line 189: 14
+        line 188: 26
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      27     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      27     1   seq   Ljava/lang/CharSequence;
       StackMapTable: number_of_entries = 2
         frame_type = 14 /* same */
         frame_type = 75 /* same_locals_1_stack_item */
@@ -585,27 +585,27 @@
         88: putfield      #10                 // Field myStart:I
         91: aload_0
         92: iload_3
         93: putfield      #5                  // Field myLength:I
         96: aload_0
         97: areturn
       LineNumberTable:
-        line 225: 0
-        line 226: 4
-        line 227: 9
-        line 228: 14
-        line 229: 19
-        line 233: 21
-        line 234: 52
-        line 236: 60
-        line 240: 67
-        line 243: 81
-        line 244: 86
-        line 245: 91
-        line 247: 96
+        line 207: 0
+        line 208: 4
+        line 209: 9
+        line 210: 14
+        line 211: 19
+        line 215: 21
+        line 216: 52
+        line 218: 60
+        line 222: 67
+        line 225: 81
+        line 226: 86
+        line 227: 91
+        line 229: 96
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      98     0  this   Lcom/deshaw/util/StringUtil$HashableSubSequence;
             0      98     1   seq   Ljava/lang/CharSequence;
             0      98     2 start   I
             0      98     3 length   I
       StackMapTable: number_of_entries = 4
```

### Comparing `pjrmi-1.13.0/README.md` & `pjrmi-1.13.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 -   Support for lambdas and duck-typed Python implementations of Java
     interfaces.
 -   Versatile and extensible connectivity options, ranging from in-process
     to network-based.
 -   Thread-safe execution, with built-in locking support and asynchronous
     execution via futures.
 -   Realtime code injection.
+-   A [numpy](https://numpy.org/)-like math library for Java, which is also
+    directly interoperable with Python.
 
 Use-case examples:
 -   Scriptification of Java applications.
 -   Exposing Java service interfaces to Python clients.
 -   Command and control.
 -   On-the-fly debugging and/or dev-ops.
 
@@ -44,14 +46,17 @@
 -   [py4j](https://www.py4j.org/) allows Python to call into Java. It also
     supports Java calling back into Python so that Python clients can implement
     Java interfaces. It works by communicating over a socket. It is probably
     the most feature-rich of the these implementations.
 -   [jpy](https://pypi.org/project/jpy/) is another in-process implementation.
     One of its key features is support for fast pass-by-value operations with
     arrays by use of pointer hand-off.
+-   [jpype](https://pypi.org/project/JPype1/) is another in-process
+    implementation. Since it uses internal C-based handoff it's highly
+    performant.
 
 As well as the feature sets of the above, PJRmi supports complex Java
 constructs, has smooth integration of the two languages' type systems, and can
 be used in different modes of operation transparently to the user.
 
 
 ## A Simple Example
@@ -101,14 +106,35 @@
     >>> hash(a)
     30817
     >>> sum(a)
     6
     >>> 1 in a
     True
 
+The `hypercube` package supports `ndarray`-like Java classes, as well as
+providing a subset of `numpy` math library operations. Hypercubes also duck-type
+as `ndarray`s in Python:
+
+    >>> DoubleArrayHypercube = c.class_for_name('com.deshaw.hypercube.DoubleArrayHypercube')
+    >>> Dimension            = c.class_for_name('com.deshaw.hypercube.Dimension')
+    >>> CubeMath             = c.class_for_name('com.deshaw.hypercube.CubeMath')
+    >>> dac = DoubleArrayHypercube(Dimension.of((3,3,3)))
+    >>> dac.reshape((27,))[:] = tuple(range(27))
+    >>> dac[0]
+    DoubleSlicedHypercube([ [0.0, 1.0, 2.0] ,
+                            [3.0, 4.0, 5.0] ,
+                            [6.0, 7.0, 8.0] ])
+    >>> numpy.sum(dac)
+    351.0
+    >>> CubeMath.sum(dac)
+    351.0
+
+These are covered in more detail in the Jupyter
+[notebook](python/tests/hypercube.ipynb).
+
 
 ## Accessing Existing Object Instances
 
     >>> foo = c.object_for_name('Foo')
 
 You can get a reference to a java object with the command
 `c.object_for_name(<string>)`. This calls into a Java method on the server, and
@@ -666,14 +692,28 @@
   and Python processes are on the same host. It is not required for general use.
 
 The build of PJRmi which is available in [PyPI](https://pypi.org/project/pjrmi/)
 only contains the platform-independent Python code and Java JARs; it does not
 come with the C extensions.
 
 
+### Security Model
+
+Access from a remote Python client to a Java server may be controlled using SSL
+keys. This is recommended for any deployment environment since, once connected,
+a client is effectively inside the server process and can execute abitrary code.
+
+The caveat to the above is that a server may choose to have a class allow list
+which restricts the set of Java classes which a Python client may access. This
+limits the capabilities of a client since they may not access classes which, for
+example, allow sub-processes to be spawned. This can be controlled in the server
+processes by overriding the `isClassBlockingOn()` and `isClassPermitted()`
+methods in the `PJRmi` subclass.
+
+
 ### Threading Model
 
 The PJRmi service runs as a separate thread inside the Java process. As such you
 have to figure out any thread-safety issues. The framework provides support for
 a `ReentrantLock` which will be held for the duration of calls which can help in
 this.
```

### Comparing `pjrmi-1.13.0/pyproject.toml` & `pjrmi-1.13.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 artifacts = [ "pjrmi/lib/*.jar",
 ]
 
 [project]
 name = "pjrmi"
 dependencies = [
-    "snappy", "numpy"
+    "python-snappy", "numpy"
 ]
 
 # Using https://peps.python.org/pep-0639/ which is still in draft
 license = {text = "BSD-3-Clause"}
 
 description = "PJRmi, RMI between Python and Java"
 authors = [{name = "D. E. Shaw & Co LP"}]
```

### Comparing `pjrmi-1.13.0/PKG-INFO` & `pjrmi-1.13.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pjrmi
-Version: 1.13.0
+Version: 1.13.8
 Summary: PJRmi, RMI between Python and Java
 Project-URL: Source code, https://github.com/deshaw/pjrmi
 Author: D. E. Shaw & Co LP
 Maintainer-email: "D. E. Shaw & Co LP" <pjrmi@deshaw.com>
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Requires-Dist: numpy
-Requires-Dist: snappy
+Requires-Dist: python-snappy
 Description-Content-Type: text/markdown
 
 PJRmi
 =====
 
 ## Overview
 
@@ -55,14 +55,16 @@
 -   Support for lambdas and duck-typed Python implementations of Java
     interfaces.
 -   Versatile and extensible connectivity options, ranging from in-process
     to network-based.
 -   Thread-safe execution, with built-in locking support and asynchronous
     execution via futures.
 -   Realtime code injection.
+-   A [numpy](https://numpy.org/)-like math library for Java, which is also
+    directly interoperable with Python.
 
 Use-case examples:
 -   Scriptification of Java applications.
 -   Exposing Java service interfaces to Python clients.
 -   Command and control.
 -   On-the-fly debugging and/or dev-ops.
 
@@ -76,14 +78,17 @@
 -   [py4j](https://www.py4j.org/) allows Python to call into Java. It also
     supports Java calling back into Python so that Python clients can implement
     Java interfaces. It works by communicating over a socket. It is probably
     the most feature-rich of the these implementations.
 -   [jpy](https://pypi.org/project/jpy/) is another in-process implementation.
     One of its key features is support for fast pass-by-value operations with
     arrays by use of pointer hand-off.
+-   [jpype](https://pypi.org/project/JPype1/) is another in-process
+    implementation. Since it uses internal C-based handoff it's highly
+    performant.
 
 As well as the feature sets of the above, PJRmi supports complex Java
 constructs, has smooth integration of the two languages' type systems, and can
 be used in different modes of operation transparently to the user.
 
 
 ## A Simple Example
@@ -133,14 +138,35 @@
     >>> hash(a)
     30817
     >>> sum(a)
     6
     >>> 1 in a
     True
 
+The `hypercube` package supports `ndarray`-like Java classes, as well as
+providing a subset of `numpy` math library operations. Hypercubes also duck-type
+as `ndarray`s in Python:
+
+    >>> DoubleArrayHypercube = c.class_for_name('com.deshaw.hypercube.DoubleArrayHypercube')
+    >>> Dimension            = c.class_for_name('com.deshaw.hypercube.Dimension')
+    >>> CubeMath             = c.class_for_name('com.deshaw.hypercube.CubeMath')
+    >>> dac = DoubleArrayHypercube(Dimension.of((3,3,3)))
+    >>> dac.reshape((27,))[:] = tuple(range(27))
+    >>> dac[0]
+    DoubleSlicedHypercube([ [0.0, 1.0, 2.0] ,
+                            [3.0, 4.0, 5.0] ,
+                            [6.0, 7.0, 8.0] ])
+    >>> numpy.sum(dac)
+    351.0
+    >>> CubeMath.sum(dac)
+    351.0
+
+These are covered in more detail in the Jupyter
+[notebook](python/tests/hypercube.ipynb).
+
 
 ## Accessing Existing Object Instances
 
     >>> foo = c.object_for_name('Foo')
 
 You can get a reference to a java object with the command
 `c.object_for_name(<string>)`. This calls into a Java method on the server, and
@@ -698,14 +724,28 @@
   and Python processes are on the same host. It is not required for general use.
 
 The build of PJRmi which is available in [PyPI](https://pypi.org/project/pjrmi/)
 only contains the platform-independent Python code and Java JARs; it does not
 come with the C extensions.
 
 
+### Security Model
+
+Access from a remote Python client to a Java server may be controlled using SSL
+keys. This is recommended for any deployment environment since, once connected,
+a client is effectively inside the server process and can execute abitrary code.
+
+The caveat to the above is that a server may choose to have a class allow list
+which restricts the set of Java classes which a Python client may access. This
+limits the capabilities of a client since they may not access classes which, for
+example, allow sub-processes to be spawned. This can be controlled in the server
+processes by overriding the `isClassBlockingOn()` and `isClassPermitted()`
+methods in the `PJRmi` subclass.
+
+
 ### Threading Model
 
 The PJRmi service runs as a separate thread inside the Java process. As such you
 have to figure out any thread-safety issues. The framework provides support for
 a `ReentrantLock` which will be held for the duration of calls which can help in
 this.
```

