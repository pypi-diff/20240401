# Comparing `tmp/openbb_cboe-1.1.3.tar.gz` & `tmp/openbb_cboe-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_cboe-1.1.3.tar", max compression
+gzip compressed data, was "openbb_cboe-1.1.4.tar", max compression
```

## Comparing `openbb_cboe-1.1.3.tar` & `openbb_cboe-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      423 2024-01-17 14:26:16.660051 openbb_cboe-1.1.3/README.md
--rw-r--r--   0        0        0     1779 2024-03-11 10:41:33.399837 openbb_cboe-1.1.3/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-01-17 14:26:16.660269 openbb_cboe-1.1.3/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-01-23 15:29:36.184612 openbb_cboe-1.1.3/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-02-23 17:14:57.422520 openbb_cboe-1.1.3/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-02-23 17:14:57.422626 openbb_cboe-1.1.3/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-02-07 09:55:40.832725 openbb_cboe-1.1.3/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2154 2024-01-23 15:29:36.185303 openbb_cboe-1.1.3/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-02-23 17:14:57.422749 openbb_cboe-1.1.3/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-02-23 17:14:57.422885 openbb_cboe-1.1.3/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-01-23 15:29:36.185853 openbb_cboe-1.1.3/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4725 2024-01-23 15:29:36.185957 openbb_cboe-1.1.3/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     5698 2024-01-26 17:52:27.960119 openbb_cboe-1.1.3/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.661146 openbb_cboe-1.1.3/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-01-17 14:26:16.661260 openbb_cboe-1.1.3/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6469 2024-01-26 17:52:27.960252 openbb_cboe-1.1.3/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      494 2024-03-11 19:59:52.928903 openbb_cboe-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 openbb_cboe-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      423 2024-02-29 11:03:36.757989 openbb_cboe-1.1.4/README.md
+-rw-r--r--   0        0        0     1779 2024-03-21 17:38:35.637071 openbb_cboe-1.1.4/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.758231 openbb_cboe-1.1.4/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-03-21 17:38:35.637199 openbb_cboe-1.1.4/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8338 2024-03-21 17:38:35.637321 openbb_cboe-1.1.4/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9657 2024-03-21 17:38:35.637473 openbb_cboe-1.1.4/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-03-21 17:38:35.637646 openbb_cboe-1.1.4/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2154 2024-03-21 17:38:35.637760 openbb_cboe-1.1.4/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-03-21 17:38:35.637910 openbb_cboe-1.1.4/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8336 2024-03-21 17:38:35.638057 openbb_cboe-1.1.4/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-03-21 17:38:35.638181 openbb_cboe-1.1.4/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4725 2024-03-13 16:36:51.640860 openbb_cboe-1.1.4/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     5698 2024-03-21 17:38:35.638327 openbb_cboe-1.1.4/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.759328 openbb_cboe-1.1.4/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-02-29 11:03:36.759398 openbb_cboe-1.1.4/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6469 2024-03-13 16:36:51.641162 openbb_cboe-1.1.4/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      494 2024-04-01 14:21:00.514790 openbb_cboe-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 openbb_cboe-1.1.4/PKG-INFO
```

### Comparing `openbb_cboe-1.1.3/openbb_cboe/__init__.py` & `openbb_cboe-1.1.4/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/available_indices.py` & `openbb_cboe-1.1.4/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/equity_historical.py` & `openbb_cboe-1.1.4/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/equity_quote.py` & `openbb_cboe-1.1.4/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/equity_search.py` & `openbb_cboe-1.1.4/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/futures_curve.py` & `openbb_cboe-1.1.4/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/index_constituents.py` & `openbb_cboe-1.1.4/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/index_historical.py` & `openbb_cboe-1.1.4/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/index_search.py` & `openbb_cboe-1.1.4/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/index_snapshots.py` & `openbb_cboe-1.1.4/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/models/options_chains.py` & `openbb_cboe-1.1.4/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/openbb_cboe/utils/helpers.py` & `openbb_cboe-1.1.4/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.1.3/PKG-INFO` & `openbb_cboe-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-cboe
-Version: 1.1.3
+Version: 1.1.4
 Summary: CBOE extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp-client-cache (>=0.10.0,<0.11.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB CBOE Provider
 
 This extension integrates the [CBOE](https://www.cboe.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

