# Comparing `tmp/openbb_commodity-1.0.1.tar.gz` & `tmp/openbb_commodity-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_commodity-1.0.1.tar", max compression
+gzip compressed data, was "openbb_commodity-1.0.2.tar", max compression
```

## Comparing `openbb_commodity-1.0.1.tar` & `openbb_commodity-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      459 2024-02-06 11:54:53.209054 openbb_commodity-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-02-06 11:54:53.209316 openbb_commodity-1.0.1/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1260 2024-03-11 10:41:33.385783 openbb_commodity-1.0.1/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0      470 2024-03-11 19:56:44.198282 openbb_commodity-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      459 2024-03-13 16:36:51.554064 openbb_commodity-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.554538 openbb_commodity-1.0.2/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1260 2024-03-13 16:36:51.554980 openbb_commodity-1.0.2/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0      470 2024-04-01 14:18:29.422654 openbb_commodity-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_commodity-1.0.2/PKG-INFO
```

### Comparing `openbb_commodity-1.0.1/openbb_commodity/commodity_router.py` & `openbb_commodity-1.0.2/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_commodity-1.0.1/PKG-INFO` & `openbb_commodity-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-commodity
-Version: 1.0.1
+Version: 1.0.2
 Summary: Commodity extension for OpenBB
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
 
 # Commodity Extension for OpenBB Platform
 
 This extension provides a set of commands for commodity-related data.
 
 ## Installation
```

