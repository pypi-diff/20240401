# Comparing `tmp/openbb_finra-1.1.3.tar.gz` & `tmp/openbb_finra-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finra-1.1.3.tar", max compression
+gzip compressed data, was "openbb_finra-1.1.4.tar", max compression
```

## Comparing `openbb_finra-1.1.3.tar` & `openbb_finra-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      423 2024-01-17 14:26:16.699637 openbb_finra-1.1.3/README.md
--rw-r--r--   0        0        0      538 2024-01-26 17:52:27.960864 openbb_finra-1.1.3/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-03-11 10:41:33.399936 openbb_finra-1.1.3/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-02-23 17:14:57.456500 openbb_finra-1.1.3/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-01-26 17:52:27.960986 openbb_finra-1.1.3/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5360 2024-01-17 14:26:16.700113 openbb_finra-1.1.3/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0      445 2024-03-11 19:59:09.443730 openbb_finra-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_finra-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      423 2024-02-29 11:03:36.800341 openbb_finra-1.1.4/README.md
+-rw-r--r--   0        0        0      538 2024-03-21 17:38:35.639158 openbb_finra-1.1.4/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-03-13 16:36:51.707780 openbb_finra-1.1.4/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-03-13 16:36:51.707928 openbb_finra-1.1.4/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-03-13 16:36:51.708062 openbb_finra-1.1.4/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5360 2024-02-29 11:03:36.800831 openbb_finra-1.1.4/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0      445 2024-04-01 14:20:22.391752 openbb_finra-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 openbb_finra-1.1.4/PKG-INFO
```

### Comparing `openbb_finra-1.1.3/openbb_finra/__init__.py` & `openbb_finra-1.1.4/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.3/openbb_finra/models/equity_short_interest.py` & `openbb_finra-1.1.4/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.3/openbb_finra/models/otc_aggregate.py` & `openbb_finra-1.1.4/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.3/openbb_finra/utils/data_storage.py` & `openbb_finra-1.1.4/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.3/openbb_finra/utils/helpers.py` & `openbb_finra-1.1.4/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.1.3/PKG-INFO` & `openbb_finra-1.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-finra
-Version: 1.1.3
+Version: 1.1.4
 Summary: FINRA extension for OpenBB
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
 
 # OpenBB FINRA Provider
 
 This extension integrates the [FINRA](https://finra.org/) data provider into the OpenBB Platform.
 
 ## Installation
```

