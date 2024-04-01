# Comparing `tmp/openbb_etf-1.1.3.tar.gz` & `tmp/openbb_etf-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_etf-1.1.3.tar", max compression
+gzip compressed data, was "openbb_etf-1.1.4.tar", max compression
```

## Comparing `openbb_etf-1.1.3.tar` & `openbb_etf-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      216 2024-01-17 14:26:16.640255 openbb_etf-1.1.3/README.md
--rw-r--r--   0        0        0       28 2024-01-17 14:26:16.640622 openbb_etf-1.1.3/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-01-17 14:26:16.640726 openbb_etf-1.1.3/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-03-11 10:41:33.390072 openbb_etf-1.1.3/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6055 2024-03-11 10:41:33.390179 openbb_etf-1.1.3/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.640892 openbb_etf-1.1.3/openbb_etf/py.typed
--rw-r--r--   0        0        0      441 2024-03-11 19:57:31.731048 openbb_etf-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 openbb_etf-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      216 2024-02-29 11:03:36.737177 openbb_etf-1.1.4/README.md
+-rw-r--r--   0        0        0       28 2024-02-29 11:03:36.737607 openbb_etf-1.1.4/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-02-29 11:03:36.737701 openbb_etf-1.1.4/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-03-13 16:36:51.571874 openbb_etf-1.1.4/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6010 2024-03-18 09:35:41.445390 openbb_etf-1.1.4/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.737920 openbb_etf-1.1.4/openbb_etf/py.typed
+-rw-r--r--   0        0        0      441 2024-04-01 14:19:07.467348 openbb_etf-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 openbb_etf-1.1.4/PKG-INFO
```

### Comparing `openbb_etf-1.1.3/openbb_etf/discovery/discovery_router.py` & `openbb_etf-1.1.4/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_etf-1.1.3/openbb_etf/etf_router.py` & `openbb_etf-1.1.4/openbb_etf/etf_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,27 +112,27 @@
     extra_params: ExtraParams,
 ) -> OBBject:
     """ETF Country weighting."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
-    model="PricePerformance",
+    model="EtfPricePerformance",
     examples=[
         APIEx(parameters={"symbol": "QQQ", "provider": "fmp"}),
         APIEx(parameters={"symbol": "SPY,QQQ,IWM,DJIA", "provider": "fmp"}),
     ],
 )
 async def price_performance(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Price performance as a return, over different periods. This is a proxy for `equity.price.performance`."""
+    """Price performance as a return, over different periods."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="EtfHoldings",
     examples=[
         APIEx(parameters={"symbol": "XLK", "provider": "fmp"}),
```

### Comparing `openbb_etf-1.1.3/PKG-INFO` & `openbb_etf-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-etf
-Version: 1.1.3
+Version: 1.1.4
 Summary: ETF extension for OpenBB
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
 
 # ETF data extension for OpenBB SDK
 
 This extension provides a set of commands for ETF data retrieval.
 
 ## Installation
```

