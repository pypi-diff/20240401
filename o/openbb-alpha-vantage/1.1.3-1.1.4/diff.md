# Comparing `tmp/openbb_alpha_vantage-1.1.3.tar.gz` & `tmp/openbb_alpha_vantage-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_alpha_vantage-1.1.3.tar", max compression
+gzip compressed data, was "openbb_alpha_vantage-1.1.4.tar", max compression
```

## Comparing `openbb_alpha_vantage-1.1.3.tar` & `openbb_alpha_vantage-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      457 2024-01-17 14:26:16.655244 openbb_alpha_vantage-1.1.3/README.md
--rw-r--r--   0        0        0     1106 2024-03-11 10:41:33.399034 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.655442 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12446 2024-03-11 19:21:16.059130 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-03-11 10:41:33.399266 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.655567 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.655633 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2516 2024-03-11 10:41:33.399370 openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      493 2024-03-11 19:59:26.648619 openbb_alpha_vantage-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      457 2024-02-29 11:03:36.752466 openbb_alpha_vantage-1.1.4/README.md
+-rw-r--r--   0        0        0     1106 2024-03-28 12:01:02.099630 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752638 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12446 2024-03-21 17:38:35.636494 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5288 2024-03-14 12:31:53.175465 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752779 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752842 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2516 2024-03-13 16:36:51.635177 openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      493 2024-04-01 14:20:39.029115 openbb_alpha_vantage-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.1.4/PKG-INFO
```

### Comparing `openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/__init__.py` & `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/models/equity_historical.py` & `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/models/historical_eps.py` & `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.3/openbb_alpha_vantage/utils/helpers.py` & `openbb_alpha_vantage-1.1.4/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.1.3/PKG-INFO` & `openbb_alpha_vantage-1.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-alpha-vantage
-Version: 1.1.3
+Version: 1.1.4
 Summary: Alpha Vantage extension for OpenBB
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
 
 # OpenBB Alpha Vantage Provider
 
 This extension integrates the [Alpha Vantage](https://www.alphavantage.co/) data provider into the OpenBB Platform.
 
 ## Installation
```

