# Comparing `tmp/openbb_federal_reserve-1.1.3.tar.gz` & `tmp/openbb_federal_reserve-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_federal_reserve-1.1.3.tar", max compression
+gzip compressed data, was "openbb_federal_reserve-1.1.4.tar", max compression
```

## Comparing `openbb_federal_reserve-1.1.3.tar` & `openbb_federal_reserve-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      474 2024-01-17 14:26:16.692058 openbb_federal_reserve-1.1.3/README.md
--rw-r--r--   0        0        0      716 2024-01-17 14:26:16.692232 openbb_federal_reserve-1.1.3/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-01-26 17:52:27.960723 openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-01-17 14:26:16.692476 openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3510 2024-02-23 17:14:57.449342 openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      508 2024-03-11 19:59:39.619971 openbb_federal_reserve-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      474 2024-03-13 16:36:51.700295 openbb_federal_reserve-1.1.4/README.md
+-rw-r--r--   0        0        0      716 2024-03-21 17:38:35.639023 openbb_federal_reserve-1.1.4/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-03-13 16:36:51.700491 openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-03-13 16:36:51.700569 openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3510 2024-03-13 16:36:51.700655 openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      508 2024-04-01 14:20:49.344805 openbb_federal_reserve-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.1.4/PKG-INFO
```

### Comparing `openbb_federal_reserve-1.1.3/openbb_federal_reserve/__init__.py` & `openbb_federal_reserve-1.1.4/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/fed_rates.py` & `openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/money_measures.py` & `openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.3/openbb_federal_reserve/models/treasury_rates.py` & `openbb_federal_reserve-1.1.4/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.1.3/PKG-INFO` & `openbb_federal_reserve-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-federal-reserve
-Version: 1.1.3
+Version: 1.1.4
 Summary: US Federal Reserve Data Extension for OpenBB
 Author: OpenBB
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
 
 # OpenBB Federal Reserve Provider
 
 This extension integrates the [Federal Reserve](https://www.federalreserve.gov/data.htm) data provider into the OpenBB Platform.
 
 ## Installation
```

