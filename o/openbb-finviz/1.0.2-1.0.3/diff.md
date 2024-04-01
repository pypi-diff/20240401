# Comparing `tmp/openbb_finviz-1.0.2.tar.gz` & `tmp/openbb_finviz-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finviz-1.0.2.tar", max compression
+gzip compressed data, was "openbb_finviz-1.0.3.tar", max compression
```

## Comparing `openbb_finviz-1.0.2.tar` & `openbb_finviz-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      442 2024-01-23 15:29:39.590912 openbb_finviz-1.0.2/README.md
--rw-r--r--   0        0        0      943 2024-01-26 17:52:27.961120 openbb_finviz-1.0.2/openbb_finviz/__init__.py
--rw-r--r--   0        0        0        0 2024-01-23 15:29:39.591051 openbb_finviz-1.0.2/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9574 2024-01-26 17:52:27.963327 openbb_finviz-1.0.2/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8241 2024-02-23 17:14:57.456998 openbb_finviz-1.0.2/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    10989 2024-02-23 17:14:57.457116 openbb_finviz-1.0.2/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     3974 2024-02-23 17:14:57.457221 openbb_finviz-1.0.2/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-02-23 17:14:57.457335 openbb_finviz-1.0.2/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-01-23 15:29:39.592045 openbb_finviz-1.0.2/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-01-23 15:29:39.592077 openbb_finviz-1.0.2/openbb_finviz/py.typed
--rw-r--r--   0        0        0        0 2024-01-23 15:29:39.592145 openbb_finviz-1.0.2/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-01-23 15:29:39.592352 openbb_finviz-1.0.2/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-01-23 15:29:39.592385 openbb_finviz-1.0.2/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0      477 2024-03-11 19:58:11.139608 openbb_finviz-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 openbb_finviz-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      442 2024-03-13 16:36:51.709028 openbb_finviz-1.0.3/README.md
+-rw-r--r--   0        0        0     1005 2024-03-21 17:38:35.639348 openbb_finviz-1.0.3/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709375 openbb_finviz-1.0.3/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9574 2024-03-21 17:38:35.639523 openbb_finviz-1.0.3/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8241 2024-03-13 16:36:51.709567 openbb_finviz-1.0.3/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    10989 2024-03-13 16:36:51.709649 openbb_finviz-1.0.3/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4379 2024-03-18 09:35:41.452443 openbb_finviz-1.0.3/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3878 2024-03-13 16:36:51.709793 openbb_finviz-1.0.3/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709818 openbb_finviz-1.0.3/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709850 openbb_finviz-1.0.3/openbb_finviz/py.typed
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709895 openbb_finviz-1.0.3/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-03-13 16:36:51.709953 openbb_finviz-1.0.3/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.709976 openbb_finviz-1.0.3/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0      477 2024-04-01 14:19:38.514072 openbb_finviz-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 openbb_finviz-1.0.3/PKG-INFO
```

### Comparing `openbb_finviz-1.0.2/openbb_finviz/__init__.py` & `openbb_finviz-1.0.3/openbb_finviz/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 finviz_provider = Provider(
     name="finviz",
     website="https://finviz.com",
     description="Unofficial Finviz API - https://github.com/lit26/finvizfinance/releases",
     credentials=None,
     fetcher_dict={
         "CompareGroups": FinvizCompareGroupsFetcher,
+        "EtfPricePerformance": FinvizPricePerformanceFetcher,
         "EquityInfo": FinvizEquityProfileFetcher,
         "KeyMetrics": FinvizKeyMetricsFetcher,
         "PricePerformance": FinvizPricePerformanceFetcher,
         "PriceTarget": FinvizPriceTargetFetcher,
     },
 )
```

### Comparing `openbb_finviz-1.0.2/openbb_finviz/models/compare_groups.py` & `openbb_finviz-1.0.3/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.2/openbb_finviz/models/equity_profile.py` & `openbb_finviz-1.0.3/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.2/openbb_finviz/models/key_metrics.py` & `openbb_finviz-1.0.3/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.2/openbb_finviz/models/price_performance.py` & `openbb_finviz-1.0.3/openbb_finviz/models/price_performance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Finviz Price Performance Model."""
 
 # pylint: disable=unused-argument
 from typing import Any, Dict, List, Optional
+from warnings import warn
 
 from finvizfinance.screener import performance
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.recent_performance import (
     RecentPerformanceData,
     RecentPerformanceQueryParams,
 )
@@ -104,15 +105,25 @@
             screen_df = screen.screener_view(verbose=0)
             if screen_df is None:
                 raise EmptyDataError()
             screen_df.columns = screen_df.columns.str.strip()  # type: ignore
             screen_df = screen_df.fillna("N/A").replace("N/A", None)  # type: ignore
         except Exception as e:
             raise e from e
-        return screen_df.to_dict(orient="records")
+        symbols = query.symbol.split(",")
+
+        # Check for missing symbols and warn of the missing symbols.
+        for symbol in symbols:
+            if symbol not in screen_df["Ticker"].tolist():
+                warn(f"Symbol Error: {symbol} was not found.")
+
+        return sorted(
+            screen_df.to_dict(orient="records"),
+            key=(lambda item: (symbols.index(item.get("Ticker", len(symbols))))),
+        )
 
     @staticmethod
     def transform_data(
         query: FinvizPricePerformanceQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[FinvizPricePerformanceData]:
```

### Comparing `openbb_finviz-1.0.2/openbb_finviz/models/price_target.py` & `openbb_finviz-1.0.3/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.2/openbb_finviz/utils/definitions.py` & `openbb_finviz-1.0.3/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.0.2/PKG-INFO` & `openbb_finviz-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-finviz
-Version: 1.0.2
+Version: 1.0.3
 Summary: Finviz extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: finvizfinance (==0.14.7)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Finviz Data Provider Extension
 
 This extension integrates the [Finviz](https://finviz.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

