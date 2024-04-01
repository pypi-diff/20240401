# Comparing `tmp/cycls-0.0.1.2.tar.gz` & `tmp/cycls-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycls-0.0.1.2.tar", max compression
+gzip compressed data, was "cycls-0.0.1.3.tar", max compression
```

## Comparing `cycls-0.0.1.2.tar` & `cycls-0.0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.1.2/LICENSE
--rw-r--r--   0        0        0      657 2024-01-19 19:46:22.891902 cycls-0.0.1.2/cycls/UI.py
--rw-r--r--   0        0        0      108 2024-03-26 19:01:51.033010 cycls-0.0.1.2/cycls/__init__.py
--rw-r--r--   0        0        0     6836 2024-03-26 19:01:21.509200 cycls-0.0.1.2/cycls/client.py
--rw-r--r--   0        0        0      785 2024-03-16 16:47:21.265542 cycls-0.0.1.2/cycls/configuration.py
--rw-r--r--   0        0        0      120 2024-03-26 19:03:40.681161 cycls-0.0.1.2/cycls/static.py
--rw-r--r--   0        0        0     5021 2024-03-26 18:45:36.822911 cycls-0.0.1.2/cycls/typings.py
--rw-r--r--   0        0        0      616 2024-03-26 19:03:51.067195 cycls-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 cycls-0.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-09 08:25:32.798599 cycls-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0      657 2024-01-19 19:46:22.891902 cycls-0.0.1.3/cycls/UI.py
+-rw-r--r--   0        0        0      108 2024-03-26 19:01:51.033010 cycls-0.0.1.3/cycls/__init__.py
+-rw-r--r--   0        0        0     6891 2024-04-01 21:42:27.844515 cycls-0.0.1.3/cycls/client.py
+-rw-r--r--   0        0        0      785 2024-03-16 16:47:21.265542 cycls-0.0.1.3/cycls/configuration.py
+-rw-r--r--   0        0        0      120 2024-03-26 19:03:40.681161 cycls-0.0.1.3/cycls/static.py
+-rw-r--r--   0        0        0     5021 2024-03-26 18:45:36.822911 cycls-0.0.1.3/cycls/typings.py
+-rw-r--r--   0        0        0      616 2024-04-01 21:42:42.483477 cycls-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 cycls-0.0.1.3/PKG-INFO
```

### Comparing `cycls-0.0.1.2/LICENSE` & `cycls-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.2/cycls/UI.py` & `cycls-0.0.1.3/cycls/UI.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.2/cycls/client.py` & `cycls-0.0.1.3/cycls/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from inspect import iscoroutinefunction, signature, Parameter, _empty
 from typing import Callable, Any
 from datetime import datetime
-
+from functools import wraps
 
 from socketio import AsyncClient, Client
 import asyncio
 import re
 
 from .UI import Text, Image
 from .configuration import AppConfiguration
@@ -145,14 +145,15 @@
 
     def publish(self):
         self._run()
 
     def __call__(
         self, func
     ):
+        @wraps
         @self.sio.on(self.app_config.handler)
         def wrapper(data):
             message = SyncContext(sio=self.sio, **data)
             func(**self.process_handler_input(func, message))
             message.send.send_message(None, message.send.user_message_id, True, "finish")
             return 200
 
@@ -202,20 +203,21 @@
     def publish(self):
         asyncio.run(self._run())
 
 
     def __call__(
         self, func
     ):
+        @wraps
         @self.sio.on(self.app_config.handler)
         async def wrapper(data):
             is_async = iscoroutinefunction(func)
             if is_async:
                 message = AsyncContext(sio=self.sio, **data)
-                await func(**self.__process_handler_input(func, message))
+                await func(**self.process_handler_input(func, message))
 
             else:
                 message = SyncContext(sio=self.sio, **data)
                 func(**self.process_handler_input(func, message))
             await message.send.send_message(None, message.send.user_message_id, True, "finish")
             return 200
```

### Comparing `cycls-0.0.1.2/cycls/configuration.py` & `cycls-0.0.1.3/cycls/configuration.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.2/cycls/typings.py` & `cycls-0.0.1.3/cycls/typings.py`

 * *Files identical despite different names*

### Comparing `cycls-0.0.1.2/pyproject.toml` & `cycls-0.0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycls"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "Publish your chat app with cycls"
 authors = ["Khalid Alrasheed <khalid@cycls.io>"]
 packages = [{ include = "cycls" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.3"
```

### Comparing `cycls-0.0.1.2/PKG-INFO` & `cycls-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycls
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Publish your chat app with cycls
 Author: Khalid Alrasheed
 Author-email: khalid@cycls.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

