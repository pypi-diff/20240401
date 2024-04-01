# Comparing `tmp/openbb_currency-1.1.3.tar.gz` & `tmp/openbb_currency-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_currency-1.1.3.tar", max compression
+gzip compressed data, was "openbb_currency-1.1.4.tar", max compression
```

## Comparing `openbb_currency-1.1.3.tar` & `openbb_currency-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      454 2024-01-17 14:26:16.631925 openbb_currency-1.1.3/README.md
--rw-r--r--   0        0        0       32 2024-01-17 14:26:16.632215 openbb_currency-1.1.3/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3794 2024-03-11 10:41:33.386792 openbb_currency-1.1.3/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-01-17 14:26:16.632371 openbb_currency-1.1.3/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-03-11 10:41:33.386886 openbb_currency-1.1.3/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.632469 openbb_currency-1.1.3/openbb_currency/py.typed
--rw-r--r--   0        0        0      464 2024-03-11 19:57:37.329211 openbb_currency-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_currency-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-02-29 11:03:36.730583 openbb_currency-1.1.4/README.md
+-rw-r--r--   0        0        0       32 2024-02-29 11:03:36.730878 openbb_currency-1.1.4/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3794 2024-03-13 16:36:51.559019 openbb_currency-1.1.4/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-02-29 11:03:36.730995 openbb_currency-1.1.4/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-03-13 16:36:51.559499 openbb_currency-1.1.4/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.731082 openbb_currency-1.1.4/openbb_currency/py.typed
+-rw-r--r--   0        0        0      464 2024-04-01 14:19:13.124194 openbb_currency-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_currency-1.1.4/PKG-INFO
```

### Comparing `openbb_currency-1.1.3/openbb_currency/currency_router.py` & `openbb_currency-1.1.4/openbb_currency/currency_router.py`

 * *Files identical despite different names*

### Comparing `openbb_currency-1.1.3/openbb_currency/price/price_router.py` & `openbb_currency-1.1.4/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_currency-1.1.3/PKG-INFO` & `openbb_currency-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-currency
-Version: 1.1.3
+Version: 1.1.4
 Summary: Currency extension for OpenBB
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
 
 # OpenBB Currency Extension
 
 This extension provides currency exchange related data for the OpenBB Platform.
 
 ## Installation
```

