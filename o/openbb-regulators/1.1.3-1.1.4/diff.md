# Comparing `tmp/openbb_regulators-1.1.3.tar.gz` & `tmp/openbb_regulators-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_regulators-1.1.3.tar", max compression
+gzip compressed data, was "openbb_regulators-1.1.4.tar", max compression
```

## Comparing `openbb_regulators-1.1.3.tar` & `openbb_regulators-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      470 2024-01-17 14:26:16.646465 openbb_regulators-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.646708 openbb_regulators-1.1.3/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-01-17 14:26:16.646818 openbb_regulators-1.1.3/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1885 2024-03-11 10:41:33.392570 openbb_regulators-1.1.3/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      370 2024-01-17 14:26:16.646970 openbb_regulators-1.1.3/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.647047 openbb_regulators-1.1.3/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-11 10:41:33.392692 openbb_regulators-1.1.3/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0      502 2024-03-11 19:57:44.086336 openbb_regulators-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 openbb_regulators-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      470 2024-02-29 11:03:36.742659 openbb_regulators-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.742882 openbb_regulators-1.1.4/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-02-29 11:03:36.742976 openbb_regulators-1.1.4/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1885 2024-03-13 16:36:51.582869 openbb_regulators-1.1.4/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      370 2024-02-29 11:03:36.743107 openbb_regulators-1.1.4/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.743161 openbb_regulators-1.1.4/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-13 16:36:51.583283 openbb_regulators-1.1.4/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0      502 2024-04-01 14:19:19.714644 openbb_regulators-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 openbb_regulators-1.1.4/PKG-INFO
```

### Comparing `openbb_regulators-1.1.3/openbb_regulators/cftc/cftc_router.py` & `openbb_regulators-1.1.4/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.1.3/openbb_regulators/sec/sec_router.py` & `openbb_regulators-1.1.4/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.1.3/PKG-INFO` & `openbb_regulators-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-regulators
-Version: 1.1.3
+Version: 1.1.4
 Summary: Markets and Agency Regulators extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Regulators Extension
 
 This extension provides a structure for data sourced from various global market regulators.
 
 ## Installation
```

