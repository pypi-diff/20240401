# Comparing `tmp/openbb_tiingo-1.1.3.tar.gz` & `tmp/openbb_tiingo-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tiingo-1.1.3.tar", max compression
+gzip compressed data, was "openbb_tiingo-1.1.4.tar", max compression
```

## Comparing `openbb_tiingo-1.1.3.tar` & `openbb_tiingo-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      440 2024-01-17 14:26:16.876201 openbb_tiingo-1.1.3/README.md
--rw-r--r--   0        0        0     1120 2024-03-11 10:41:33.416762 openbb_tiingo-1.1.3/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-01-17 14:26:16.876437 openbb_tiingo-1.1.3/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-02-26 09:52:50.868909 openbb_tiingo-1.1.3/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-03-11 10:41:33.416892 openbb_tiingo-1.1.3/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-03-11 10:41:33.417004 openbb_tiingo-1.1.3/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-03-11 10:41:33.417117 openbb_tiingo-1.1.3/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-01-17 14:26:16.876875 openbb_tiingo-1.1.3/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-02-26 09:52:50.869048 openbb_tiingo-1.1.3/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-01-17 14:26:16.877064 openbb_tiingo-1.1.3/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-01-17 14:26:16.877142 openbb_tiingo-1.1.3/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0      451 2024-03-11 19:59:58.921540 openbb_tiingo-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_tiingo-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      440 2024-02-29 11:03:36.971737 openbb_tiingo-1.1.4/README.md
+-rw-r--r--   0        0        0     1120 2024-03-21 17:38:35.656580 openbb_tiingo-1.1.4/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-29 11:03:36.971894 openbb_tiingo-1.1.4/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3651 2024-03-13 16:36:51.788482 openbb_tiingo-1.1.4/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5295 2024-03-13 16:36:51.788634 openbb_tiingo-1.1.4/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4662 2024-03-13 16:36:51.788832 openbb_tiingo-1.1.4/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5323 2024-03-13 16:36:51.789122 openbb_tiingo-1.1.4/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-03-21 17:38:35.656729 openbb_tiingo-1.1.4/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-03-13 16:36:51.789417 openbb_tiingo-1.1.4/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-02-29 11:03:36.972367 openbb_tiingo-1.1.4/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-02-29 11:03:36.972440 openbb_tiingo-1.1.4/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0      451 2024-04-01 14:21:06.588138 openbb_tiingo-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_tiingo-1.1.4/PKG-INFO
```

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/__init__.py` & `openbb_tiingo-1.1.4/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/company_news.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/crypto_historical.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/currency_historical.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/equity_historical.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/models/world_news.py` & `openbb_tiingo-1.1.4/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/openbb_tiingo/utils/helpers.py` & `openbb_tiingo-1.1.4/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.1.3/PKG-INFO` & `openbb_tiingo-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-tiingo
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tiingo extension for OpenBB
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
 
 # OpenBB Tiingo Provider
 
 This extension integrates the [Tiingo](https://www.tiingo.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

