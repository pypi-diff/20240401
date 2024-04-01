# Comparing `tmp/atomic_bomb_engine-0.9.0-cp39-none-win_amd64.whl.zip` & `tmp/atomic_bomb_engine-0.9.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,17 @@
-Zip file size: 3760283 bytes, number of entries: 9
--rw-r--r--  4.6 unx     8284 b- defN 24-Mar-22 03:58 atomic_bomb_engine-0.9.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Mar-22 03:58 atomic_bomb_engine-0.9.0.dist-info/WHEEL
--rw-r--r--  4.6 unx        0 b- defN 24-Mar-22 03:58 atomic_bomb_engine/dist/.gitkeep
--rw-r--r--  4.6 unx      408 b- defN 24-Mar-22 03:58 atomic_bomb_engine/middleware.py
--rw-r--r--  4.6 unx     6135 b- defN 24-Mar-22 03:58 atomic_bomb_engine/server.py
--rw-r--r--  4.6 unx      213 b- defN 24-Mar-22 03:58 atomic_bomb_engine/__init__.py
--rw-r--r--  4.6 unx     5911 b- defN 24-Mar-22 03:58 atomic_bomb_engine/__init__.pyi
--rwxr-xr-x  4.6 unx 12016111 b- defN 24-Mar-22 03:58 atomic_bomb_engine/atomic_bomb_engine.pyd
--rw-r--r--  4.6 unx      774 b- defN 24-Mar-22 03:58 atomic_bomb_engine-0.9.0.dist-info/RECORD
-9 files, 12037930 bytes uncompressed, 3758941 bytes compressed:  68.8%
+Zip file size: 3110638 bytes, number of entries: 15
+-rw-r--r--  4.6 unx     8284 b- defN 24-Mar-22 05:00 atomic_bomb_engine-0.9.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-Mar-22 05:00 atomic_bomb_engine-0.9.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx       85 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/assets/AboutView-C6Dx7pxG.css
+-rw-r--r--  4.6 unx   607141 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/assets/AboutView-D8mMyrr-.js
+-rw-r--r--  4.6 unx   537933 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/assets/atomic-bomb-engine-logo-BvEtY2It.png
+-rw-r--r--  4.6 unx   325714 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/assets/index-BG0hunjj.css
+-rw-r--r--  4.6 unx  1971247 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/assets/index-BhaVtF5l.js
+-rw-r--r--  4.6 unx    79885 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/favicon.ico
+-rw-r--r--  4.6 unx      462 b- defN 24-Mar-22 05:00 atomic_bomb_engine/dist/index.html
+-rw-r--r--  4.6 unx      408 b- defN 24-Mar-22 05:00 atomic_bomb_engine/middleware.py
+-rw-r--r--  4.6 unx     6162 b- defN 24-Mar-22 05:00 atomic_bomb_engine/server.py
+-rw-r--r--  4.6 unx      213 b- defN 24-Mar-22 05:00 atomic_bomb_engine/__init__.py
+-rw-r--r--  4.6 unx     5911 b- defN 24-Mar-22 05:00 atomic_bomb_engine/__init__.pyi
+-rwxr-xr-x  4.6 unx  4493312 b- defN 24-Mar-22 05:00 atomic_bomb_engine/atomic_bomb_engine.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx     1446 b- defN 24-Mar-22 05:00 atomic_bomb_engine-0.9.1.dist-info/RECORD
+15 files, 8038297 bytes uncompressed, 3108198 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,28 +1,46 @@
-Filename: atomic_bomb_engine-0.9.0.dist-info/METADATA
+Filename: atomic_bomb_engine-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: atomic_bomb_engine-0.9.0.dist-info/WHEEL
+Filename: atomic_bomb_engine-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: atomic_bomb_engine/dist/.gitkeep
+Filename: atomic_bomb_engine/dist/assets/AboutView-C6Dx7pxG.css
+Comment: 
+
+Filename: atomic_bomb_engine/dist/assets/AboutView-D8mMyrr-.js
+Comment: 
+
+Filename: atomic_bomb_engine/dist/assets/atomic-bomb-engine-logo-BvEtY2It.png
+Comment: 
+
+Filename: atomic_bomb_engine/dist/assets/index-BG0hunjj.css
+Comment: 
+
+Filename: atomic_bomb_engine/dist/assets/index-BhaVtF5l.js
+Comment: 
+
+Filename: atomic_bomb_engine/dist/favicon.ico
+Comment: 
+
+Filename: atomic_bomb_engine/dist/index.html
 Comment: 
 
 Filename: atomic_bomb_engine/middleware.py
 Comment: 
 
 Filename: atomic_bomb_engine/server.py
 Comment: 
 
 Filename: atomic_bomb_engine/__init__.py
 Comment: 
 
 Filename: atomic_bomb_engine/__init__.pyi
 Comment: 
 
-Filename: atomic_bomb_engine/atomic_bomb_engine.pyd
+Filename: atomic_bomb_engine/atomic_bomb_engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: atomic_bomb_engine-0.9.0.dist-info/RECORD
+Filename: atomic_bomb_engine-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atomic_bomb_engine/server.py

```diff
@@ -7,23 +7,23 @@
 import aiohttp
 import aiosqlite
 import json
 from typing import Dict
 from aiohttp import web
 from atomic_bomb_engine import middleware
 
-db_connection = None
-
 
 def ui(port: int = 8000, auto_open: bool = True):
     if port > 65535 or port < 0:
         raise ValueError(f"端口必须为0-65535")
+    # 数据库连接
+    db_connection = None
 
     async def get_db_connection():
-        global db_connection
+        nonlocal db_connection
         if db_connection is None:
             db_connection = await aiosqlite.connect(":memory:")
             await db_connection.execute('CREATE TABLE results (id INTEGER PRIMARY KEY, data JSON)')
         return db_connection
 
     async def create_table():
         db = await get_db_connection()
```

## Comparing `atomic_bomb_engine-0.9.0.dist-info/METADATA` & `atomic_bomb_engine-0.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: atomic_bomb_engine
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: OS Independent
 Requires-Dist: aiohttp
 Requires-Dist: aiosqlite
 Summary: 使用rust开发的高性能python压测工具
 Keywords: rust,python,binding
```

