# Comparing `tmp/json-handler-registry-1.2.0.tar.gz` & `tmp/json-handler-registry-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-handler-registry-1.2.0.tar", last modified: Thu Mar 28 22:07:31 2024, max compression
+gzip compressed data, was "dist/json-handler-registry-1.3.0.tar", last modified: Mon Apr  1 18:19:20 2024, max compression
```

## Comparing `json-handler-registry-1.2.0.tar` & `json-handler-registry-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.2.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.2.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3321 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2804 2024-03-28 22:05:02.000000 json-handler-registry-1.2.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-03-28 22:03:45.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2452 2024-03-28 18:09:24.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/decoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1269 2024-03-28 18:06:24.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/encoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3666 2024-03-28 21:57:42.000000 json-handler-registry-1.2.0/pkg/json_handler_registry/registry.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3321 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      471 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/pkg/json_handler_registry.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-03-28 22:07:31.000000 json-handler-registry-1.2.0/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.2.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.3.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.3.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4517 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4000 2024-04-01 18:15:05.000000 json-handler-registry-1.3.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-03-31 11:40:57.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2452 2024-03-28 18:09:24.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/decoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1281 2024-03-31 11:37:08.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/encoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3939 2024-04-01 17:44:53.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/registry.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      959 2024-04-01 18:16:02.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-01 18:10:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      282 2024-04-01 18:08:41.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/common.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1243 2024-04-01 18:13:30.000000 json-handler-registry-1.3.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4517 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      676 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/not-zip-safe
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/pkg/json_handler_registry.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-01 18:19:20.000000 json-handler-registry-1.3.0/setup.cfg
+-rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.3.0/setup.py
```

### Comparing `json-handler-registry-1.2.0/LICENSE.txt` & `json-handler-registry-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.2.0/pkg/json_handler_registry/decoder.py` & `json-handler-registry-1.3.0/pkg/json_handler_registry/decoder.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.2.0/pkg/json_handler_registry/encoder.py` & `json-handler-registry-1.3.0/pkg/json_handler_registry/encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 from abc import ABC
 from json import JSONEncoder
 from typing import Any, Dict, Optional, Type, Union
 
-EncodingResult = Union[str, tuple, list, dict]
+EncodingResult = Union[int, float, str, tuple, list, dict]
 
 
 class IJsonEncoder(ABC):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         """Convert object to a JSON serializable data.
         Or return ``None`` instead.
         """
```

### Comparing `json-handler-registry-1.2.0/pkg/json_handler_registry/registry.py` & `json-handler-registry-1.3.0/pkg/json_handler_registry/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright by: P.J. Grochowski
 
 import json
 from functools import partial
-from typing import Any, Type, Union, cast
+from typing import Any, Set, Type, Union, cast
 
 from json_handler_registry import __logger as logger
 from json_handler_registry.decoder import DecoderRegistryDict, IJsonDecoder, _JsonDecoderRegistryProxy
 from json_handler_registry.encoder import EncoderRegistryDict, IJsonEncoder, _JsonEncoderRegistryProxy
 
 JsonEncoder = Union[Type[IJsonEncoder], IJsonEncoder]
 JsonDecoder = Union[Type[IJsonDecoder], IJsonDecoder]
@@ -66,14 +66,22 @@
     @classmethod
     def disable(cls) -> None:
         if cls.isEnabled():
             json.dumps = cast(partial, json.dumps).func
             json.loads = cast(partial, json.loads).func
 
     @classmethod
+    def getRegisteredEncoderTypes(cls) -> Set[Type[IJsonEncoder]]:
+        return set(cls._ENCODER_REGISTRY.keys())
+
+    @classmethod
+    def getRegisteredDecoderTypes(cls) -> Set[Type[IJsonDecoder]]:
+        return set(cls._DECODER_REGISTRY.keys())
+
+    @classmethod
     def registerEncoder(cls, jsonEncoder: JsonEncoder) -> None:
         encoderInstance = cls._getEncoderInstance(jsonEncoder=jsonEncoder)
         cls._ENCODER_REGISTRY[type(encoderInstance)] = encoderInstance
 
     @classmethod
     def unregisterEncoder(cls, jsonEncoder: JsonEncoder) -> None:
         encoderType = cls._getEncoderType(jsonEncoder=jsonEncoder)
```

### Comparing `json-handler-registry-1.2.0/setup.py` & `json-handler-registry-1.3.0/setup.py`

 * *Files identical despite different names*

