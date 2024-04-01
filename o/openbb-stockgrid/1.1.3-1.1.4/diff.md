# Comparing `tmp/openbb_stockgrid-1.1.3.tar.gz` & `tmp/openbb_stockgrid-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_stockgrid-1.1.3.tar", max compression
+gzip compressed data, was "openbb_stockgrid-1.1.4.tar", max compression
```

## Comparing `openbb_stockgrid-1.1.3.tar` & `openbb_stockgrid-1.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      438 2024-01-17 14:26:16.871150 openbb_stockgrid-1.1.3/README.md
--rw-r--r--   0        0        0      677 2024-01-26 17:52:27.970319 openbb_stockgrid-1.1.3/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-02-23 17:14:57.472278 openbb_stockgrid-1.1.3/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0      497 2024-03-11 20:00:12.110966 openbb_stockgrid-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 openbb_stockgrid-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      438 2024-02-29 11:03:36.970476 openbb_stockgrid-1.1.4/README.md
+-rw-r--r--   0        0        0      677 2024-03-21 17:38:35.656069 openbb_stockgrid-1.1.4/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-03-13 16:36:51.786904 openbb_stockgrid-1.1.4/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0      497 2024-04-01 14:21:20.978388 openbb_stockgrid-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 openbb_stockgrid-1.1.4/PKG-INFO
```

### Comparing `openbb_stockgrid-1.1.3/openbb_stockgrid/__init__.py` & `openbb_stockgrid-1.1.4/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_stockgrid-1.1.3/openbb_stockgrid/models/short_volume.py` & `openbb_stockgrid-1.1.4/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_stockgrid-1.1.3/PKG-INFO` & `openbb_stockgrid-1.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-stockgrid
-Version: 1.1.3
+Version: 1.1.4
 Summary: stockgrid extension for OpenBB
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
 Requires-Dist: pytest-freezegun (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Stockgrid Provider
 
 This extension integrates the [Stockgrid](https://Stockgrid.io/) data provider into the OpenBB Platform.
```

