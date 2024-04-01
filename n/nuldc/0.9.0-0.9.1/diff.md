# Comparing `tmp/nuldc-0.9.0.tar.gz` & `tmp/nuldc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuldc-0.9.0.tar", max compression
+gzip compressed data, was "nuldc-0.9.1.tar", max compression
```

## Comparing `nuldc-0.9.0.tar` & `nuldc-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2024-03-15 20:52:49.094823 nuldc-0.9.0/LICENSE
--rw-r--r--   0        0        0     4014 2024-03-15 20:52:49.094823 nuldc-0.9.0/README.md
--rw-r--r--   0        0        0        0 2024-03-15 20:52:49.094823 nuldc-0.9.0/nuldc/__init__.py
--rw-r--r--   0        0        0     2639 2024-03-15 20:52:49.094823 nuldc-0.9.0/nuldc/commandline.py
--rw-r--r--   0        0        0     3297 2024-03-15 20:52:49.094823 nuldc-0.9.0/nuldc/dump.py
--rw-r--r--   0        0        0     7139 2024-03-15 20:52:49.094823 nuldc-0.9.0/nuldc/helpers.py
--rw-r--r--   0        0        0      552 2024-03-15 20:52:49.094823 nuldc-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     4887 1970-01-01 00:00:00.000000 nuldc-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-03-18 16:48:35.839655 nuldc-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4014 2024-03-18 16:48:35.839655 nuldc-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-18 16:48:35.839655 nuldc-0.9.1/nuldc/__init__.py
+-rw-r--r--   0        0        0     2639 2024-03-18 16:48:35.839655 nuldc-0.9.1/nuldc/commandline.py
+-rw-r--r--   0        0        0     3451 2024-03-18 16:48:35.839655 nuldc-0.9.1/nuldc/dump.py
+-rw-r--r--   0        0        0     7139 2024-03-18 16:48:35.839655 nuldc-0.9.1/nuldc/helpers.py
+-rw-r--r--   0        0        0      552 2024-03-18 16:48:35.839655 nuldc-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4887 1970-01-01 00:00:00.000000 nuldc-0.9.1/PKG-INFO
```

### Comparing `nuldc-0.9.0/LICENSE` & `nuldc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuldc-0.9.0/README.md` & `nuldc-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nuldc-0.9.0/nuldc/commandline.py` & `nuldc-0.9.1/nuldc/commandline.py`

 * *Files identical despite different names*

### Comparing `nuldc-0.9.0/nuldc/dump.py` & `nuldc-0.9.1/nuldc/dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from nuldc import helpers
 import json
 import re
 import concurrent.futures
 import datetime
 import os
+import sys
 
 
 API = "https://api.dc.library.northwestern.edu/api/v2"
 
 
 def slugify(s):
     """takes string and removes special characters,
@@ -60,23 +61,25 @@
 
 def dump_collection(col_id):
     """ Takes a collection id and grabs metadata then dumps into
     json, xml, and csv files"""
 
     params = {
         "query": f"collection.id:{col_id}",
-        "size": "25",
+        "size": "100",
         "sort": "id:asc"}
     data = helpers.get_search_results(API,
                                       "works",
-                                      params, all_results=True)
-
-    col_title = data['data'][0]['collection']['title']
-    filename = f"{slugify(col_title)}-{col_id}"
-    save_files(filename, data)
+                                      params, all_results=True, page_limit=5000)
+    try:
+        col_title = data['data'][0]['collection']['title']
+        filename = f"{slugify(col_title)}-{col_id}"
+        save_files(filename, data)
+    except Exception as e:
+        sys.exit(f"Error with collection {col_id}: {e} \n\n CONTEXT: {data}")
 
 
 def dump_collections(query_string):
     """This dumps collections from a collectionlist."""
 
     search_url = f'{API}/search'
     # get collections list
```

### Comparing `nuldc-0.9.0/nuldc/helpers.py` & `nuldc-0.9.1/nuldc/helpers.py`

 * *Files identical despite different names*

### Comparing `nuldc-0.9.0/pyproject.toml` & `nuldc-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuldc"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["davidschober <davidschob@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
```

### Comparing `nuldc-0.9.0/PKG-INFO` & `nuldc-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuldc
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 License: MIT
 Author: davidschober
 Author-email: davidschob@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

