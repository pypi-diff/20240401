# Comparing `tmp/openbb_tradier-1.0.0.tar.gz` & `tmp/openbb_tradier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradier-1.0.0.tar", max compression
+gzip compressed data, was "openbb_tradier-1.0.1.tar", max compression
```

## Comparing `openbb_tradier-1.0.0.tar` & `openbb_tradier-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      438 2024-03-11 16:19:37.844678 openbb_tradier-1.0.0/README.md
--rw-r--r--   0        0        0     1241 2024-03-11 19:09:39.080632 openbb_tradier-1.0.0/openbb_tradier/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:19:37.844918 openbb_tradier-1.0.0/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6568 2024-03-11 16:19:37.845106 openbb_tradier-1.0.0/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9162 2024-03-11 16:19:37.845380 openbb_tradier-1.0.0/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-03-11 16:19:37.845597 openbb_tradier-1.0.0/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10222 2024-03-11 16:19:37.845838 openbb_tradier-1.0.0/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-03-11 16:19:37.845870 openbb_tradier-1.0.0/openbb_tradier/py.typed
--rw-r--r--   0        0        0        0 2024-03-11 16:19:37.845938 openbb_tradier-1.0.0/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-03-11 16:19:37.846063 openbb_tradier-1.0.0/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      474 2024-03-11 19:58:19.601635 openbb_tradier-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_tradier-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      438 2024-03-13 16:36:51.891842 openbb_tradier-1.0.1/README.md
+-rw-r--r--   0        0        0     1241 2024-03-21 17:38:35.660567 openbb_tradier-1.0.1/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.893874 openbb_tradier-1.0.1/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6568 2024-03-21 17:38:35.660734 openbb_tradier-1.0.1/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9162 2024-03-21 17:38:35.660909 openbb_tradier-1.0.1/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-03-21 17:38:35.661032 openbb_tradier-1.0.1/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10222 2024-03-21 17:38:35.661130 openbb_tradier-1.0.1/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.894734 openbb_tradier-1.0.1/openbb_tradier/py.typed
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.894779 openbb_tradier-1.0.1/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-03-13 16:36:51.894856 openbb_tradier-1.0.1/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      474 2024-04-01 14:19:44.027846 openbb_tradier-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 openbb_tradier-1.0.1/PKG-INFO
```

### Comparing `openbb_tradier-1.0.0/openbb_tradier/__init__.py` & `openbb_tradier-1.0.1/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/openbb_tradier/models/equity_historical.py` & `openbb_tradier-1.0.1/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/openbb_tradier/models/equity_quote.py` & `openbb_tradier-1.0.1/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/openbb_tradier/models/equity_search.py` & `openbb_tradier-1.0.1/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/openbb_tradier/models/options_chains.py` & `openbb_tradier-1.0.1/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/openbb_tradier/utils/constants.py` & `openbb_tradier-1.0.1/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.0.0/PKG-INFO` & `openbb_tradier-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-tradier
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tradier Provider Extension for the OpenBB Platform
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
 
 # OpenBB Tradier Provider
 
 `openbb-tradier` is a data provider extension for the OpenBB Platform.
 
 ## Installation
```

