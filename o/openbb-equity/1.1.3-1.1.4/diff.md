# Comparing `tmp/openbb_equity-1.1.3.tar.gz` & `tmp/openbb_equity-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_equity-1.1.3.tar", max compression
+gzip compressed data, was "openbb_equity-1.1.4.tar", max compression
```

## Comparing `openbb_equity-1.1.3.tar` & `openbb_equity-1.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      938 2024-01-17 14:26:16.637656 openbb_equity-1.1.3/README.md
--rw-r--r--   0        0        0       19 2024-01-17 14:26:16.638096 openbb_equity-1.1.3/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-01-17 14:26:16.638199 openbb_equity-1.1.3/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-03-11 10:41:33.388358 openbb_equity-1.1.3/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-01-17 14:26:16.638380 openbb_equity-1.1.3/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2326 2024-03-11 10:41:33.388464 openbb_equity-1.1.3/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-01-17 14:26:16.638570 openbb_equity-1.1.3/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1109 2024-03-11 10:41:33.388557 openbb_equity-1.1.3/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-01-17 14:26:16.638739 openbb_equity-1.1.3/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5811 2024-03-11 10:41:33.388691 openbb_equity-1.1.3/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3452 2024-03-11 10:41:33.388788 openbb_equity-1.1.3/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-01-17 14:26:16.638973 openbb_equity-1.1.3/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     2652 2024-03-11 10:41:33.388880 openbb_equity-1.1.3/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-01-17 14:26:16.639137 openbb_equity-1.1.3/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-03-11 10:41:33.388997 openbb_equity-1.1.3/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-01-17 14:26:16.639311 openbb_equity-1.1.3/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3769 2024-03-11 10:41:33.389108 openbb_equity-1.1.3/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-01-17 14:26:16.639488 openbb_equity-1.1.3/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-03-11 10:41:33.389216 openbb_equity-1.1.3/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.639600 openbb_equity-1.1.3/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-01-17 14:26:16.639724 openbb_equity-1.1.3/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-03-11 10:41:33.389321 openbb_equity-1.1.3/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0      452 2024-03-11 19:57:19.641803 openbb_equity-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 openbb_equity-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      938 2024-02-29 11:03:36.734962 openbb_equity-1.1.4/README.md
+-rw-r--r--   0        0        0       19 2024-02-29 11:03:36.735289 openbb_equity-1.1.4/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-02-29 11:03:36.735486 openbb_equity-1.1.4/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-03-13 16:36:51.567454 openbb_equity-1.1.4/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-02-29 11:03:36.735656 openbb_equity-1.1.4/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2326 2024-03-13 16:36:51.567755 openbb_equity-1.1.4/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735800 openbb_equity-1.1.4/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1109 2024-03-13 16:36:51.568234 openbb_equity-1.1.4/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735942 openbb_equity-1.1.4/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5811 2024-03-13 16:36:51.568426 openbb_equity-1.1.4/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3452 2024-03-13 16:36:51.568603 openbb_equity-1.1.4/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-02-29 11:03:36.736112 openbb_equity-1.1.4/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     2652 2024-03-13 16:36:51.568953 openbb_equity-1.1.4/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736244 openbb_equity-1.1.4/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-03-13 16:36:51.569355 openbb_equity-1.1.4/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-02-29 11:03:36.736420 openbb_equity-1.1.4/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3769 2024-03-13 16:36:51.569810 openbb_equity-1.1.4/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736541 openbb_equity-1.1.4/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-03-22 18:22:13.174274 openbb_equity-1.1.4/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.736634 openbb_equity-1.1.4/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-02-29 11:03:36.736696 openbb_equity-1.1.4/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-03-13 16:36:51.570690 openbb_equity-1.1.4/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0      452 2024-04-01 14:18:55.114548 openbb_equity-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 openbb_equity-1.1.4/PKG-INFO
```

### Comparing `openbb_equity-1.1.3/README.md` & `openbb_equity-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/calendar/calendar_router.py` & `openbb_equity-1.1.4/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/compare/compare_router.py` & `openbb_equity-1.1.4/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/darkpool/darkpool_router.py` & `openbb_equity-1.1.4/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/discovery/discovery_router.py` & `openbb_equity-1.1.4/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/equity_router.py` & `openbb_equity-1.1.4/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/estimates/estimates_router.py` & `openbb_equity-1.1.4/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/fundamental/fundamental_router.py` & `openbb_equity-1.1.4/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/ownership/ownership_router.py` & `openbb_equity-1.1.4/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/price/price_router.py` & `openbb_equity-1.1.4/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/openbb_equity/shorts/shorts_router.py` & `openbb_equity-1.1.4/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.1.3/PKG-INFO` & `openbb_equity-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-equity
-Version: 1.1.3
+Version: 1.1.4
 Summary: Equity extension for OpenBB
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
 
 # OpenBB Equity Extension
 
 This extension provides equity market data tools for the OpenBB Platform.
 
 Features of the Equity extension include:
```

