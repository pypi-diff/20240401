# Comparing `tmp/mypy-protobuf-3.5.0.tar.gz` & `tmp/mypy-protobuf-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-protobuf-3.5.0.tar", last modified: Sat Jul 29 00:22:30 2023, max compression
+gzip compressed data, was "mypy-protobuf-3.6.0.tar", last modified: Mon Apr  1 20:24:08 2024, max compression
```

## Comparing `mypy-protobuf-3.5.0.tar` & `mypy-protobuf-3.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727557 mypy-protobuf-3.5.0/
--rw-r--r--   0 nipunn     (501) staff       (20)    11348 2022-01-28 23:16:18.000000 mypy-protobuf-3.5.0/LICENSE
--rw-r--r--   0 nipunn     (501) staff       (20)      395 2023-07-29 00:22:30.727609 mypy-protobuf-3.5.0/PKG-INFO
--rw-r--r--   0 nipunn     (501) staff       (20)    10565 2023-07-29 00:15:31.000000 mypy-protobuf-3.5.0/README.md
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.726272 mypy-protobuf-3.5.0/mypy_protobuf/
--rw-r--r--   0 nipunn     (501) staff       (20)        0 2021-12-24 22:07:25.000000 mypy-protobuf-3.5.0/mypy_protobuf/__init__.py
--rw-r--r--   0 nipunn     (501) staff       (20)     2178 2023-07-28 22:09:30.000000 mypy-protobuf-3.5.0/mypy_protobuf/extensions_pb2.py
--rw-r--r--   0 nipunn     (501) staff       (20)    44145 2023-07-29 00:22:05.000000 mypy-protobuf-3.5.0/mypy_protobuf/main.py
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727057 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/
--rw-r--r--   0 nipunn     (501) staff       (20)      395 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 nipunn     (501) staff       (20)      428 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 nipunn     (501) staff       (20)        1 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 nipunn     (501) staff       (20)      107 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/entry_points.txt
--rw-r--r--   0 nipunn     (501) staff       (20)       42 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/requires.txt
--rw-r--r--   0 nipunn     (501) staff       (20)       14 2023-07-29 00:22:30.000000 mypy-protobuf-3.5.0/mypy_protobuf.egg-info/top_level.txt
--rw-r--r--   0 nipunn     (501) staff       (20)      584 2023-07-29 00:08:49.000000 mypy-protobuf-3.5.0/pyproject.toml
--rw-r--r--   0 nipunn     (501) staff       (20)      728 2023-07-29 00:22:30.727854 mypy-protobuf-3.5.0/setup.cfg
-drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2023-07-29 00:22:30.727453 mypy-protobuf-3.5.0/test/
--rw-r--r--   0 nipunn     (501) staff       (20)    18031 2023-07-28 22:09:30.000000 mypy-protobuf-3.5.0/test/test_generated_mypy.py
--rw-r--r--   0 nipunn     (501) staff       (20)     2413 2023-07-28 20:41:01.000000 mypy-protobuf-3.5.0/test/test_grpc_async_usage.py
--rw-r--r--   0 nipunn     (501) staff       (20)     2585 2022-08-23 09:57:11.000000 mypy-protobuf-3.5.0/test/test_grpc_usage.py
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2024-04-01 20:24:08.506965 mypy-protobuf-3.6.0/
+-rw-r--r--   0 nipunn     (501) staff       (20)    11348 2022-01-28 23:16:18.000000 mypy-protobuf-3.6.0/LICENSE
+-rw-r--r--   0 nipunn     (501) staff       (20)      463 2024-04-01 20:24:08.506917 mypy-protobuf-3.6.0/PKG-INFO
+-rw-r--r--   0 nipunn     (501) staff       (20)    10561 2024-04-01 20:06:31.000000 mypy-protobuf-3.6.0/README.md
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2024-04-01 20:24:08.505511 mypy-protobuf-3.6.0/mypy_protobuf/
+-rw-r--r--   0 nipunn     (501) staff       (20)        0 2021-12-24 22:07:25.000000 mypy-protobuf-3.6.0/mypy_protobuf/__init__.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     1952 2024-04-01 20:06:31.000000 mypy-protobuf-3.6.0/mypy_protobuf/extensions_pb2.py
+-rw-r--r--   0 nipunn     (501) staff       (20)    44302 2024-04-01 20:06:42.000000 mypy-protobuf-3.6.0/mypy_protobuf/main.py
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2024-04-01 20:24:08.506736 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/
+-rw-r--r--   0 nipunn     (501) staff       (20)      463 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 nipunn     (501) staff       (20)      428 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)        1 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)      107 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/entry_points.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)       38 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/requires.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)       14 2024-04-01 20:24:08.000000 mypy-protobuf-3.6.0/mypy_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 nipunn     (501) staff       (20)      584 2023-07-29 00:08:49.000000 mypy-protobuf-3.6.0/pyproject.toml
+-rw-r--r--   0 nipunn     (501) staff       (20)      724 2024-04-01 20:24:08.507200 mypy-protobuf-3.6.0/setup.cfg
+drwxr-xr-x   0 nipunn     (501) staff       (20)        0 2024-04-01 20:24:08.506568 mypy-protobuf-3.6.0/test/
+-rw-r--r--   0 nipunn     (501) staff       (20)    18031 2023-07-28 22:09:30.000000 mypy-protobuf-3.6.0/test/test_generated_mypy.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     2413 2023-07-28 20:41:01.000000 mypy-protobuf-3.6.0/test/test_grpc_async_usage.py
+-rw-r--r--   0 nipunn     (501) staff       (20)     2585 2022-08-23 09:57:11.000000 mypy-protobuf-3.6.0/test/test_grpc_usage.py
```

### Comparing `mypy-protobuf-3.5.0/LICENSE` & `mypy-protobuf-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-protobuf-3.5.0/README.md` & `mypy-protobuf-3.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 See [Changelog](CHANGELOG.md) for recent changes.
 
 ## Requirements to run mypy-protobuf
 
 Earlier releases might work, but aren't tested
 
 - [protoc >= 23.4](https://github.com/protocolbuffers/protobuf/releases)
-- [python-protobuf >= 4.23.4](https://pypi.org/project/protobuf/) - matching protoc release
+- [python-protobuf >= 4.25.3](https://pypi.org/project/protobuf/) - matching protoc release
 - [python >= 3.8](https://www.python.org/downloads/source/) - for running mypy-protobuf plugin.
 
 ## Requirements to run typecheckers on stubs generated by mypy-protobuf
 
 Earlier releases might work, but aren't tested
 
 - [mypy >= v1.4.1](https://pypi.org/project/mypy) or [pyright >= 1.1.206](https://github.com/microsoft/pyright)
-- [python-protobuf >= 4.23.4](https://pypi.org/project/protobuf/) - matching protoc release
-- [types-protobuf >= 4.23.0.2](https://pypi.org/project/types-protobuf/) - for stubs from the google.protobuf library
+- [python-protobuf >= 4.25.3](https://pypi.org/project/protobuf/) - matching protoc release
+- [types-protobuf >= 4.24](https://pypi.org/project/types-protobuf/) - for stubs from the google.protobuf library
 
 ### To run typecheckers on code generated with grpc plugin - you'll additionally need
 
 Earlier releases might work, but aren't tested
 
 - [grpcio>=1.56.2](https://pypi.org/project/grpcio/)
 - [grpcio-tools>=1.56.2](https://pypi.org/project/grpcio-tools/)
```

### Comparing `mypy-protobuf-3.5.0/mypy_protobuf/extensions_pb2.py` & `mypy-protobuf-3.6.0/mypy_protobuf/extensions_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: mypy_protobuf/extensions.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,22 +17,17 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emypy_protobuf/extensions.proto\x12\rmypy_protobuf\x1a google/protobuf/descriptor.proto\"D\n\x0c\x46ieldOptions\x12\x10\n\x08\x63\x61sttype\x18\x01 \x01(\t\x12\x0f\n\x07keytype\x18\x02 \x01(\t\x12\x11\n\tvaluetype\x18\x03 \x01(\t:L\n\x07options\x12\x1d.google.protobuf.FieldOptions\x18\x82\t \x01(\x0b\x32\x1b.mypy_protobuf.FieldOptions:4\n\x08\x63\x61sttype\x12\x1d.google.protobuf.FieldOptions\x18\xff\x08 \x01(\tB\x02\x18\x01:3\n\x07keytype\x12\x1d.google.protobuf.FieldOptions\x18\x80\t \x01(\tB\x02\x18\x01:5\n\tvaluetype\x12\x1d.google.protobuf.FieldOptions\x18\x81\t \x01(\tB\x02\x18\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mypy_protobuf.extensions_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(options)
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(casttype)
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(keytype)
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(valuetype)
-
   DESCRIPTOR._options = None
-  casttype._options = None
-  casttype._serialized_options = b'\030\001'
-  keytype._options = None
-  keytype._serialized_options = b'\030\001'
-  valuetype._options = None
-  valuetype._serialized_options = b'\030\001'
+  _globals['casttype']._options = None
+  _globals['casttype']._serialized_options = b'\030\001'
+  _globals['keytype']._options = None
+  _globals['keytype']._serialized_options = b'\030\001'
+  _globals['valuetype']._options = None
+  _globals['valuetype']._serialized_options = b'\030\001'
   _globals['_FIELDOPTIONS']._serialized_start=83
   _globals['_FIELDOPTIONS']._serialized_end=151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mypy-protobuf-3.5.0/mypy_protobuf/main.py` & `mypy-protobuf-3.6.0/mypy_protobuf/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import google.protobuf.descriptor_pb2 as d
 from google.protobuf.compiler import plugin_pb2 as plugin_pb2
 from google.protobuf.internal.containers import RepeatedCompositeFieldContainer
 from google.protobuf.internal.well_known_types import WKTBASES
 from . import extensions_pb2
 
-__version__ = "3.5.0"
+__version__ = "3.6.0"
 
 # SourceCodeLocation is defined by `message Location` here
 # https://github.com/protocolbuffers/protobuf/blob/master/src/google/protobuf/descriptor.proto
 SourceCodeLocation = List[int]
 
 # So phabricator doesn't think mypy_protobuf.py is generated
 GENERATED = "@ge" + "nerated"
@@ -165,17 +165,15 @@
 
     def _import(self, path: str, name: str) -> str:
         """Imports a stdlib path and returns a handle to it
         eg. self._import("typing", "Literal") -> "Literal"
         """
         if path == "typing_extensions":
             stabilization = {
-                "Literal": (3, 8),
                 "TypeAlias": (3, 10),
-                "final": (3, 8),
             }
             assert name in stabilization
             if not self.typing_extensions_min or self.typing_extensions_min < stabilization[name]:
                 self.typing_extensions_min = stabilization[name]
             return "typing_extensions." + name
 
         imp = path.replace("/", ".")
@@ -403,15 +401,15 @@
                 addl_base = ", " + self._import(
                     "google.protobuf.internal.well_known_types",
                     well_known_type.__name__,
                 )
 
             class_name = desc.name if desc.name not in PYTHON_RESERVED else "_r_" + desc.name
             message_class = self._import("google.protobuf.message", "Message")
-            wl("@{}", self._import("typing_extensions", "final"))
+            wl("@{}", self._import("typing", "final"))
             wl(f"class {class_name}({message_class}{addl_base}):")
             with self._indent():
                 scl = scl_prefix + [i]
                 if self._write_comments(scl):
                     wl("")
 
                 desc_type = self._import("google.protobuf.descriptor", "Descriptor")
@@ -434,28 +432,33 @@
                 for f in desc.field:
                     wl(f"{f.name.upper()}_FIELD_NUMBER: {self._builtin('int')}")
 
                 for idx, field in enumerate(desc.field):
                     if field.name in PYTHON_RESERVED:
                         continue
                     field_type = self.python_type(field)
-
                     if is_scalar(field) and field.label != d.FieldDescriptorProto.LABEL_REPEATED:
                         # Scalar non repeated fields are r/w
                         wl(f"{field.name}: {field_type}")
                         self._write_comments(scl + [d.DescriptorProto.FIELD_FIELD_NUMBER, idx])
-                    else:
+
+                for idx, field in enumerate(desc.field):
+                    if field.name in PYTHON_RESERVED:
+                        continue
+                    field_type = self.python_type(field)
+                    if not (is_scalar(field) and field.label != d.FieldDescriptorProto.LABEL_REPEATED):
                         # r/o Getters for non-scalar fields and scalar-repeated fields
                         scl_field = scl + [d.DescriptorProto.FIELD_FIELD_NUMBER, idx]
                         wl("@property")
                         body = " ..." if not self._has_comments(scl_field) else ""
                         wl(f"def {field.name}(self) -> {field_type}:{body}")
                         if self._has_comments(scl_field):
                             with self._indent():
                                 self._write_comments(scl_field)
+                            wl("")
 
                 self.write_extensions(desc.extension, scl + [d.DescriptorProto.EXTENSION_FIELD_NUMBER])
 
                 # Constructor
                 wl("def __init__(")
                 with self._indent():
                     if any(f.name == "self" for f in desc.field):
@@ -502,34 +505,34 @@
 
         if not hf_fields and not cf_fields and not wo_fields:
             return
 
         if hf_fields:
             wl(
                 "def HasField(self, field_name: {}[{}]) -> {}: ...",
-                self._import("typing_extensions", "Literal"),
+                self._import("typing", "Literal"),
                 hf_fields_text,
                 self._builtin("bool"),
             )
         if cf_fields:
             wl(
                 "def ClearField(self, field_name: {}[{}]) -> None: ...",
-                self._import("typing_extensions", "Literal"),
+                self._import("typing", "Literal"),
                 cf_fields_text,
             )
 
         for wo_field, members in sorted(wo_fields.items()):
             if len(wo_fields) > 1:
                 wl("@{}", self._import("typing", "overload"))
             wl(
                 "def WhichOneof(self, oneof_group: {}[{}]) -> {}[{}] | None: ...",
-                self._import("typing_extensions", "Literal"),
+                self._import("typing", "Literal"),
                 # Accepts both str and bytes
                 f'"{wo_field}", b"{wo_field}"',
-                self._import("typing_extensions", "Literal"),
+                self._import("typing", "Literal"),
                 # Returns `str`
                 ", ".join(f'"{m}"' for m in members),
             )
 
     def write_extensions(
         self,
         extensions: Sequence[d.FieldDescriptorProto],
@@ -595,14 +598,15 @@
                 self._import_message(method.output_type),
                 " ..." if not self._has_comments(scl_method) else "",
             )
             if self._has_comments(scl_method):
                 with self._indent():
                     if not self._write_comments(scl_method):
                         wl("...")
+            wl("")
 
     def write_services(
         self,
         services: Iterable[d.ServiceDescriptorProto],
         scl_prefix: SourceCodeLocation,
     ) -> None:
         wl = self._write_line
@@ -616,28 +620,26 @@
                 self._import("google.protobuf.service", "Service"),
                 self._import("abc", "ABCMeta"),
             )
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 self.write_methods(service, class_name, is_abstract=True, scl_prefix=scl)
-            wl("")
 
             # The stub client
             stub_class_name = service.name + "_Stub"
             wl("class {}({}):", stub_class_name, class_name)
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 wl(
                     "def __init__(self, rpc_channel: {}) -> None: ...",
                     self._import("google.protobuf.service", "RpcChannel"),
                 )
                 self.write_methods(service, stub_class_name, is_abstract=False, scl_prefix=scl)
-            wl("")
 
     def _import_casttype(self, casttype: str) -> str:
         split = casttype.split(".")
         assert len(split) == 2, "mypy_protobuf.[casttype,keytype,valuetype] is expected to be of format path/to/file.TypeInFile"
         pkg = split[0].replace("/", ".")
         return self._import(pkg, split[1])
 
@@ -705,30 +707,28 @@
             result = f"{self._import('typing', 'Union')}[{result}, {awaitable}]"
         return result
 
     def write_grpc_async_hacks(self) -> None:
         wl = self._write_line
         # _MaybeAsyncIterator[Req] is supertyped by Iterator[Req] and AsyncIterator[Req].
         # So both can be used in the contravariant function parameter position.
-        wl("_T = {}('_T')", self._import("typing", "TypeVar"))
+        wl('_T = {}("_T")', self._import("typing", "TypeVar"))
         wl("")
         wl(
-            "class _MaybeAsyncIterator({}[_T], {}[_T], metaclass={}):",
+            "class _MaybeAsyncIterator({}[_T], {}[_T], metaclass={}): ...",
             self._import("collections.abc", "AsyncIterator"),
             self._import("collections.abc", "Iterator"),
             self._import("abc", "ABCMeta"),
         )
-        with self._indent():
-            wl("...")
         wl("")
 
         # _ServicerContext is supertyped by grpc.ServicerContext and grpc.aio.ServicerContext
         # So both can be used in the contravariant function parameter position.
         wl(
-            "class _ServicerContext({}, {}):  # type: ignore",
+            "class _ServicerContext({}, {}):  # type: ignore[misc, type-arg]",
             self._import("grpc", "ServicerContext"),
             self._import("grpc.aio", "ServicerContext"),
         )
         with self._indent():
             wl("...")
         wl("")
 
@@ -754,14 +754,15 @@
                 self._servicer_output_type(method),
                 " ..." if not self._has_comments(scl) else "",
             )
             if self._has_comments(scl):
                 with self._indent():
                     if not self._write_comments(scl):
                         wl("...")
+            wl("")
 
     def write_grpc_stub_methods(self, service: d.ServiceDescriptorProto, scl_prefix: SourceCodeLocation, is_async: bool = False) -> None:
         wl = self._write_line
         methods = [(i, m) for i, m in enumerate(service.method) if m.name not in PYTHON_RESERVED]
         if not methods:
             wl("...")
             wl("")
@@ -770,14 +771,15 @@
 
             wl("{}: {}[", method.name, self._callable_type(method, is_async=is_async))
             with self._indent():
                 wl("{},", self._input_type(method))
                 wl("{},", self._output_type(method))
             wl("]")
             self._write_comments(scl)
+            wl("")
 
     def write_grpc_services(
         self,
         services: Iterable[d.ServiceDescriptorProto],
         scl_prefix: SourceCodeLocation,
     ) -> None:
         wl = self._write_line
@@ -795,39 +797,36 @@
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 # To support casting into FooAsyncStub, allow both Channel and aio.Channel here.
                 channel = f"{self._import('typing', 'Union')}[{self._import('grpc', 'Channel')}, {self._import('grpc.aio', 'Channel')}]"
                 wl("def __init__(self, channel: {}) -> None: ...", channel)
                 self.write_grpc_stub_methods(service, scl)
-            wl("")
 
             # The (fake) async stub client
             wl(
                 "class {}AsyncStub:",
                 service.name,
             )
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 # No __init__ since this isn't a real class (yet), and requires manual casting to work.
                 self.write_grpc_stub_methods(service, scl, is_async=True)
-            wl("")
 
             # The service definition interface
             wl(
                 "class {}Servicer(metaclass={}):",
                 service.name,
                 self._import("abc", "ABCMeta"),
             )
             with self._indent():
                 if self._write_comments(scl):
                     wl("")
                 self.write_grpc_methods(service, scl)
-            wl("")
             server = self._import("grpc", "Server")
             aserver = self._import("grpc.aio", "Server")
             wl(
                 "def add_{}Servicer_to_server(servicer: {}Servicer, server: {}) -> None: ...",
                 service.name,
                 service.name,
                 f"{self._import('typing', 'Union')}[{server}, {aserver}]",
@@ -921,16 +920,17 @@
         # module docstring may exist as comment before syntax (optional) or package name
         if not self._write_comments([d.FileDescriptorProto.PACKAGE_FIELD_NUMBER]):
             self._write_comments([d.FileDescriptorProto.SYNTAX_FIELD_NUMBER])
 
         if self.lines:
             assert self.lines[0].startswith('"""')
             self.lines[0] = f'"""{HEADER}{self.lines[0][3:]}'
+            self._write_line("")
         else:
-            self._write_line(f'"""{HEADER}"""')
+            self._write_line(f'"""{HEADER}"""\n')
 
         for reexport_idx in self.fd.public_dependency:
             reexport_file = self.fd.dependency[reexport_idx]
             reexport_fd = self.descriptors.files[reexport_file]
             reexport_imp = reexport_file[:-6].replace("-", "_").replace("/", ".") + "_pb2"
             names = [m.name for m in reexport_fd.message_type] + [m.name for m in reexport_fd.enum_type] + [v.name for m in reexport_fd.enum_type for v in m.value] + [m.name for m in reexport_fd.extension]
             if reexport_fd.options.py_generic_services:
```

### Comparing `mypy-protobuf-3.5.0/pyproject.toml` & `mypy-protobuf-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy-protobuf-3.5.0/setup.cfg` & `mypy-protobuf-3.6.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 [options]
 py_modules = 
 	mypy_protobuf
 	mypy_protobuf.main
 	mypy_protobuf.extensions_pb2
 install_requires = 
-	protobuf>=4.23.4
-	types-protobuf>=4.23.0.2
+	protobuf>=4.25.3
+	types-protobuf>=4.24
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	protoc-gen-mypy = mypy_protobuf.main:main
 	protoc-gen-mypy_grpc = mypy_protobuf.main:grpc
```

### Comparing `mypy-protobuf-3.5.0/test/test_generated_mypy.py` & `mypy-protobuf-3.6.0/test/test_generated_mypy.py`

 * *Files identical despite different names*

### Comparing `mypy-protobuf-3.5.0/test/test_grpc_async_usage.py` & `mypy-protobuf-3.6.0/test/test_grpc_async_usage.py`

 * *Files identical despite different names*

### Comparing `mypy-protobuf-3.5.0/test/test_grpc_usage.py` & `mypy-protobuf-3.6.0/test/test_grpc_usage.py`

 * *Files identical despite different names*

