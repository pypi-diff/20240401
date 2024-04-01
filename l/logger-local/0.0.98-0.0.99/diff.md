# Comparing `tmp/logger-local-0.0.98.tar.gz` & `tmp/logger-local-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-local-0.0.98.tar", last modified: Sun Feb  4 01:22:22 2024, max compression
+gzip compressed data, was "logger-local-0.0.99.tar", last modified: Sun Feb  4 04:02:05 2024, max compression
```

## Comparing `logger-local-0.0.98.tar` & `logger-local-0.0.99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 01:22:22.569685 logger-local-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-04 01:21:50.000000 logger-local-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-04 01:22:22.569685 logger-local-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-02-04 01:21:50.000000 logger-local-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 01:22:22.565685 logger-local-0.0.98/logger_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 01:22:22.569685 logger-local-0.0.98/logger_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/Component.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/Connector.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/LoggerComponentEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/LoggerLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/LoggerOutputEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/MessageSeverity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/MetaLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/SendToLogzIo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/Writer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/debug_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-04 01:21:50.000000 logger-local-0.0.98/logger_local/src/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 01:22:22.569685 logger-local-0.0.98/logger_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-04 01:22:22.000000 logger-local-0.0.98/logger_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-04 01:22:22.000000 logger-local-0.0.98/logger_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 01:22:22.000000 logger-local-0.0.98/logger_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-04 01:22:22.000000 logger-local-0.0.98/logger_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-04 01:22:22.000000 logger-local-0.0.98/logger_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-04 01:21:50.000000 logger-local-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 01:22:22.569685 logger-local-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-04 01:21:50.000000 logger-local-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 04:02:05.239340 logger-local-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-04 04:01:31.000000 logger-local-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-04 04:02:05.239340 logger-local-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-02-04 04:01:31.000000 logger-local-0.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 04:02:05.235340 logger-local-0.0.99/logger_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 04:02:05.239340 logger-local-0.0.99/logger_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/Connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/LoggerComponentEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/LoggerLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/LoggerOutputEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/MessageSeverity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/MetaLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/SendToLogzIo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/Writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/debug_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-04 04:01:31.000000 logger-local-0.0.99/logger_local/src/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 04:02:05.239340 logger-local-0.0.99/logger_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-04 04:02:05.000000 logger-local-0.0.99/logger_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-04 04:02:05.000000 logger-local-0.0.99/logger_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 04:02:05.000000 logger-local-0.0.99/logger_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-04 04:02:05.000000 logger-local-0.0.99/logger_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-04 04:02:05.000000 logger-local-0.0.99/logger_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-04 04:01:31.000000 logger-local-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 04:02:05.239340 logger-local-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-04 04:01:31.000000 logger-local-0.0.99/setup.py
```

### Comparing `logger-local-0.0.98/LICENSE` & `logger-local-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/PKG-INFO` & `logger-local-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.98/README.md` & `logger-local-0.0.99/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -75,17 +75,27 @@
     'component_name': YOUR_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code,
     "developer_email": YOUR_CIRCLES_EMAIL
 }
 
 
 # you can use the logger object in the class, and you don't have to expicitly create it, or call logger.start/end/exception
+# use `logger = ...` here if you need it inside a static method
 class YourClass(metaclass=MetaLogger, object=your_logger_object):
+    def __init__(self, a, b):
+        self.logger.start("YourClass.__init__", object={'a': a, 'b': b})
+        self.a = a
+        self.b = b
+        self.logger.end("YourClass.__init__")
+
     def some_func(self):
         self.logger.info("whatever")
+
+    def __repr__(self):
+        return f"YourClass(a={self.a}, b={self.b})"
 ```
 
 ## Using with logger object:
 
 ```py
 from logger_local.LoggerLocal import Logger
```

### Comparing `logger-local-0.0.98/logger_local/src/Component.py` & `logger-local-0.0.99/logger_local/src/Component.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/Connector.py` & `logger-local-0.0.99/logger_local/src/Connector.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/LoggerComponentEnum.py` & `logger-local-0.0.99/logger_local/src/LoggerComponentEnum.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/LoggerLocal.py` & `logger-local-0.0.99/logger_local/src/LoggerLocal.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         self.write_to_sql = False
         self.user_context = None
         self.additional_fields = kwargs['object'].copy()
         self.additional_fields["session"] = self.__generate_session_id()
 
         self.logger = self.initiate_logger(handler=handler, formatter=formatter,
                                            level=self.debug_mode.logger_minimum_severity)
+        self.logger.name = kwargs['object']['component_name']
 
         super().__init__(name=self.logger.name)
 
     @staticmethod
     def __generate_session_id(length: int = 32):
         chars = string.ascii_uppercase + string.digits
         return ''.join(random.choice(chars) for _ in range(length))
@@ -350,19 +351,19 @@
     # 90-97 are the same but "bright" foreground
     # 100-107 are the same as the bright ones but for the background.
     # '1' means bold, '2' means dim, '0' means reset, and '4' means underline.
 
     def format(self, record):
         level_colours = [
             (logging.DEBUG, '\x1b[40;1m'),  # Debug level in bold black background
-            (logging.VERBOSE, '\x1b[90m'),  # Verbose level in bright foreground    # noqa
-            (logging.INIT, '\x1b[90m'),  # Init level in bright foreground          # noqa
-            (logging.START, '\x1b[92m'),  # Start level in bright green foreground  # noqa
-            (logging.END, '\x1b[92m'),  # End level in bright green foreground      # noqa
-            (logging.INFO, '\x1b[34;1m'),  # Info level in bold blue foreground     # noqa
+            (logging.VERBOSE, '\x1b[36;1m'),  # Verbose level in bold cyan foreground   # noqa
+            (logging.INIT, '\x1b[46;1m'),  # Init level in bold cyan background         # noqa
+            (logging.START, '\x1b[42;1m'),  # Start level in bold green background      # noqa
+            (logging.END, '\x1b[41;1m'),  # End level in bold red background            # noqa
+            (logging.INFO, '\x1b[34;1m'),  # Info level in bold blue foreground
             (logging.WARNING, '\x1b[33;1m'),  # Warning level in bold yellow foreground
             (logging.ERROR, '\x1b[31m'),  # Error level in red foreground
             (logging.CRITICAL, '\x1b[41m'),  # Critical level with red background
         ]
 
         formats = {
             level: logging.Formatter(
```

### Comparing `logger-local-0.0.98/logger_local/src/MetaLogger.py` & `logger-local-0.0.99/logger_local/src/MetaLogger.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 class MetaLogger(type):
     @classmethod
     def __prepare__(metacls, name, bases, **kwargs):
         """This method is called before the class is created. It is used to create the class namespace."""
         return super().__prepare__(name, bases, **kwargs)
 
     def __new__(cls, name, bases, dct, **kwargs):
-        logger = Logger.create_logger(**kwargs)
-        dct['logger'] = logger
+        # kwargs may be empty if the class is not instantiated with the metaclass
+        if kwargs:
+            logger = Logger.create_logger(**kwargs)
+            dct['logger'] = logger
+        else:
+            logger = None
+
         for key, value in dct.items():
             if callable(value) and not key.endswith("__"):  # Exclude magic methods
                 dct[key] = cls.wrap_function(value, logger)
         return super().__new__(cls, name, bases, dct)
 
     @staticmethod
     def wrap_function(func, logger):
@@ -28,29 +33,38 @@
             function_name = f"{function_module}.{func.__name__}"
 
             signature = inspect.signature(func)
             arg_names = [param.name for param in signature.parameters.values()]
             if len(args) + len(kwargs) == len(arg_names) + 1:  # staticmethod called with class instance
                 args = args[1:]
 
+            args
             kwargs_updated = {**dict(zip(arg_names, args)), **kwargs}
-            logger.start(function_name, object=kwargs_updated)
+            if logger:
+                logger.start(function_name, object=kwargs_updated)
             result = None
             try:
                 result = func(*args, **kwargs)
             except Exception as exception:
                 # Use traceback to capture frame information
                 # Use sys.exc_info() to get exception information
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 # Extract the frame information from the traceback
                 frame = exc_traceback.tb_next.tb_frame
                 # Get the local variables
                 locals_before_exception = frame.f_locals
 
-                logger.error(function_name,
-                             object={"exception": exception, "locals_before_exception": locals_before_exception})
-                raise exception
+                # use logger.exception if the caller is a test
+                if logger:
+                    if function_module.startswith("tests."):
+                        logger.exception(function_name, object={
+                            "exception": exception, "locals_before_exception": locals_before_exception})
+                    else:
+                        logger.error(function_name, object={
+                            "exception": exception, "locals_before_exception": locals_before_exception})
+                        raise exception
             finally:
-                logger.end(function_name, object={"result": result})
+                if logger:
+                    logger.end(function_name, object={"result": result})
             return result
 
         return wrapper
```

### Comparing `logger-local-0.0.98/logger_local/src/SendToLogzIo.py` & `logger-local-0.0.99/logger_local/src/SendToLogzIo.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/Writer.py` & `logger-local-0.0.99/logger_local/src/Writer.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/debug_mode.py` & `logger-local-0.0.99/logger_local/src/debug_mode.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local/src/fields.py` & `logger-local-0.0.99/logger_local/src/fields.py`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/logger_local.egg-info/PKG-INFO` & `logger-local-0.0.99/logger_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-local
-Version: 0.0.98
+Version: 0.0.99
 Summary: PyPI Package for Circles Logger Python Local
 Home-page: https://github.com/circles-zone/logger-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `logger-local-0.0.98/logger_local.egg-info/SOURCES.txt` & `logger-local-0.0.99/logger_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logger-local-0.0.98/setup.py` & `logger-local-0.0.99/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "logger-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.98',  # https://pypi.org/project/logger-local/
+    version='0.0.99',  # https://pypi.org/project/logger-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Logger Python Local",
     long_description="This is a package for sharing common Logger function used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

