# Comparing `tmp/openbb_index-1.1.3.tar.gz` & `tmp/openbb_index-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_index-1.1.3.tar", max compression
+gzip compressed data, was "openbb_index-1.1.4.tar", max compression
```

## Comparing `openbb_index-1.1.3.tar` & `openbb_index-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      460 2024-01-17 14:26:16.643403 openbb_index-1.1.3/README.md
--rw-r--r--   0        0        0       23 2024-01-17 14:26:16.644016 openbb_index-1.1.3/openbb_index/__init__.py
--rw-r--r--   0        0        0     4053 2024-03-11 10:41:33.391453 openbb_index-1.1.3/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-01-19 11:57:23.692622 openbb_index-1.1.3/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-03-11 10:41:33.391547 openbb_index-1.1.3/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.644163 openbb_index-1.1.3/openbb_index/py.typed
--rw-r--r--   0        0        0      446 2024-03-11 19:57:25.627658 openbb_index-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_index-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      460 2024-02-29 11:03:36.739916 openbb_index-1.1.4/README.md
+-rw-r--r--   0        0        0       23 2024-02-29 11:03:36.740144 openbb_index-1.1.4/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4053 2024-03-13 16:36:51.577125 openbb_index-1.1.4/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-03-13 16:36:51.577211 openbb_index-1.1.4/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-03-13 16:36:51.577338 openbb_index-1.1.4/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740242 openbb_index-1.1.4/openbb_index/py.typed
+-rw-r--r--   0        0        0      446 2024-04-01 14:19:00.666251 openbb_index-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_index-1.1.4/PKG-INFO
```

### Comparing `openbb_index-1.1.3/openbb_index/index_router.py` & `openbb_index-1.1.4/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_index-1.1.3/openbb_index/price/price_router.py` & `openbb_index-1.1.4/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_index-1.1.3/PKG-INFO` & `openbb_index-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-index
-Version: 1.1.3
+Version: 1.1.4
 Summary: Index extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Index Extension
 
 The Index extension provides global and european index data access for the OpenBB Platform.
 
 ## Installation
```

