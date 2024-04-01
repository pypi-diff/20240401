# Comparing `tmp/cartesify_backend-0.0.8.tar.gz` & `tmp/cartesify_backend-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartesify_backend-0.0.8.tar", last modified: Wed Mar 27 23:58:47 2024, max compression
+gzip compressed data, was "cartesify_backend-0.0.9.tar", last modified: Thu Mar 28 17:59:21 2024, max compression
```

## Comparing `cartesify_backend-0.0.8.tar` & `cartesify_backend-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-27 23:58:47.183259 cartesify_backend-0.0.8/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1081 2024-03-26 23:02:44.000000 cartesify_backend-0.0.8/LICENSE
--rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-03-27 23:58:47.183259 cartesify_backend-0.0.8/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)       19 2024-03-26 23:03:22.000000 cartesify_backend-0.0.8/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-27 23:58:47.179259 cartesify_backend-0.0.8/cartesify_backend/
--rw-rw-r--   0 diego     (1000) diego     (1000)       46 2024-03-27 01:15:22.000000 cartesify_backend-0.0.8/cartesify_backend/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-03-27 23:54:26.000000 cartesify_backend-0.0.8/cartesify_backend/appfactory.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3098 2024-03-27 23:58:32.000000 cartesify_backend-0.0.8/cartesify_backend/cartesifybackend.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-27 23:58:47.183259 cartesify_backend-0.0.8/cartesify_backend.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-03-27 23:58:47.000000 cartesify_backend-0.0.8/cartesify_backend.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      330 2024-03-27 23:58:47.000000 cartesify_backend-0.0.8/cartesify_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-03-27 23:58:47.000000 cartesify_backend-0.0.8/cartesify_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       24 2024-03-27 23:58:47.000000 cartesify_backend-0.0.8/cartesify_backend.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       18 2024-03-27 23:58:47.000000 cartesify_backend-0.0.8/cartesify_backend.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-03-27 23:58:47.183259 cartesify_backend-0.0.8/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      485 2024-03-27 23:58:43.000000 cartesify_backend-0.0.8/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-28 17:59:21.095554 cartesify_backend-0.0.9/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1081 2024-03-26 23:02:44.000000 cartesify_backend-0.0.9/LICENSE
+-rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-03-28 17:59:21.095554 cartesify_backend-0.0.9/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)       19 2024-03-26 23:03:22.000000 cartesify_backend-0.0.9/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-28 17:59:21.091554 cartesify_backend-0.0.9/cartesify_backend/
+-rw-rw-r--   0 diego     (1000) diego     (1000)       46 2024-03-27 01:15:22.000000 cartesify_backend-0.0.9/cartesify_backend/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      115 2024-03-27 23:54:26.000000 cartesify_backend-0.0.9/cartesify_backend/appfactory.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3335 2024-03-28 17:56:28.000000 cartesify_backend-0.0.9/cartesify_backend/cartesifybackend.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-28 17:59:21.095554 cartesify_backend-0.0.9/cartesify_backend.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-03-28 17:59:20.000000 cartesify_backend-0.0.9/cartesify_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      330 2024-03-28 17:59:20.000000 cartesify_backend-0.0.9/cartesify_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-03-28 17:59:20.000000 cartesify_backend-0.0.9/cartesify_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       24 2024-03-28 17:59:20.000000 cartesify_backend-0.0.9/cartesify_backend.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       18 2024-03-28 17:59:20.000000 cartesify_backend-0.0.9/cartesify_backend.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-03-28 17:59:21.095554 cartesify_backend-0.0.9/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      485 2024-03-28 17:59:17.000000 cartesify_backend-0.0.9/setup.py
```

### Comparing `cartesify_backend-0.0.8/LICENSE` & `cartesify_backend-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cartesify_backend-0.0.8/cartesify_backend/cartesifybackend.py` & `cartesify_backend-0.0.9/cartesify_backend/cartesifybackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import json
 import requests
+import logging
 from .appfactory import AppFactory
 from cartesi import Rollup, RollupData
 
+logging.basicConfig(level=logging.INFO)
+
+logger = logging.getLogger(__name__)
+
 def dapp_inspect_decorator(func):
     def wrapper(self, *args, **kwargs):
         return self.dapp.inspect()
     return wrapper
 
 def dapp_advance_decorator(func):
     def wrapper(self, *args, **kwargs):
         return self.dapp.advance()
     return wrapper
 
 class CartesifyBackend:
 
     def __init__(self):
+        logger.info("Starting Cartesify App")
         self.dapp = AppFactory().create_dapp()
     def get_app(self):
         return self.dapp
 
     @dapp_inspect_decorator
     def handle_inspect(self, rollup:Rollup, data: RollupData) -> bool:
+        logger.info("Cartesify handle inspect")
         try:
             payload = data.str_payload()
 
             hex_string = payload.replace('0x', '')
             byte_buffer = bytes.fromhex(hex_string)
             utf8_string = byte_buffer.decode('utf-8')
             json_data = json.loads(utf8_string)
@@ -46,14 +53,16 @@
             buffer = bytes(error_json, "utf8")
             hex_payload = "0x" + buffer.hex()
             rollup.report(hex_payload)
             return False
 
     @dapp_advance_decorator
     def handle_advance(self, rollup:Rollup, data: RollupData) -> bool:
+        logger.info("Cartesify handle advance")
+
         try:
             payload = data.str_payload()
             if not payload.startswith('0x7b22'):
                 return False
 
             hex_string = payload[2:]  # Remove o prefixo '0x'
             buffer = bytes.fromhex(hex_string)
```

