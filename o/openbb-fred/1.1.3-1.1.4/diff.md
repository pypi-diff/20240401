# Comparing `tmp/openbb_fred-1.1.3.tar.gz` & `tmp/openbb_fred-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fred-1.1.3.tar", max compression
+gzip compressed data, was "openbb_fred-1.1.4.tar", max compression
```

## Comparing `openbb_fred-1.1.3.tar` & `openbb_fred-1.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      444 2024-01-17 14:26:16.756722 openbb_fred-1.1.3/README.md
--rw-r--r--   0        0        0     3126 2024-02-23 17:14:57.463885 openbb_fred-1.1.3/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-01-17 14:26:16.756991 openbb_fred-1.1.3/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-01-17 14:26:16.757055 openbb_fred-1.1.3/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-02-23 17:14:57.463992 openbb_fred-1.1.3/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-01-30 08:17:02.059329 openbb_fred-1.1.3/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-01-17 14:26:16.757257 openbb_fred-1.1.3/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-01-17 14:26:16.757309 openbb_fred-1.1.3/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-01-17 14:26:16.757372 openbb_fred-1.1.3/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-01-17 14:26:16.757443 openbb_fred-1.1.3/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-01-17 14:26:16.757511 openbb_fred-1.1.3/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-01-26 17:52:27.966598 openbb_fred-1.1.3/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-01-17 14:26:16.757672 openbb_fred-1.1.3/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-01-17 14:26:16.757741 openbb_fred-1.1.3/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-01-17 14:26:16.757806 openbb_fred-1.1.3/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-02-23 17:14:57.464071 openbb_fred-1.1.3/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6338 2024-02-23 17:14:57.464200 openbb_fred-1.1.3/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6253 2024-02-23 17:14:57.464317 openbb_fred-1.1.3/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-01-17 14:26:16.758056 openbb_fred-1.1.3/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-01-17 14:26:16.758119 openbb_fred-1.1.3/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-03-11 10:41:33.407470 openbb_fred-1.1.3/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-01-17 14:26:16.758259 openbb_fred-1.1.3/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-01-17 14:26:16.758330 openbb_fred-1.1.3/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-01-17 14:26:16.758409 openbb_fred-1.1.3/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-01-17 14:26:16.758553 openbb_fred-1.1.3/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-01-17 14:26:16.759051 openbb_fred-1.1.3/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-01-17 14:26:16.759201 openbb_fred-1.1.3/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-01-26 17:52:27.966829 openbb_fred-1.1.3/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-03-11 10:41:33.407597 openbb_fred-1.1.3/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-01-17 14:26:16.759654 openbb_fred-1.1.3/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-01-17 14:26:16.759877 openbb_fred-1.1.3/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      439 2024-03-11 19:58:56.090282 openbb_fred-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_fred-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      444 2024-02-29 11:03:36.865850 openbb_fred-1.1.4/README.md
+-rw-r--r--   0        0        0     3126 2024-03-21 17:38:35.646889 openbb_fred-1.1.4/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-02-29 11:03:36.866196 openbb_fred-1.1.4/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-02-29 11:03:36.866284 openbb_fred-1.1.4/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2980 2024-03-13 16:36:51.737518 openbb_fred-1.1.4/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-03-13 16:36:51.737624 openbb_fred-1.1.4/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-02-29 11:03:36.866494 openbb_fred-1.1.4/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-02-29 11:03:36.866551 openbb_fred-1.1.4/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-02-29 11:03:36.866626 openbb_fred-1.1.4/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-02-29 11:03:36.866706 openbb_fred-1.1.4/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-02-29 11:03:36.866781 openbb_fred-1.1.4/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-03-13 16:36:51.737725 openbb_fred-1.1.4/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-02-29 11:03:36.866951 openbb_fred-1.1.4/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-02-29 11:03:36.867021 openbb_fred-1.1.4/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-02-29 11:03:36.867092 openbb_fred-1.1.4/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-03-13 16:36:51.737806 openbb_fred-1.1.4/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6338 2024-03-13 16:36:51.737921 openbb_fred-1.1.4/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6312 2024-03-19 14:52:38.489944 openbb_fred-1.1.4/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-02-29 11:03:36.867365 openbb_fred-1.1.4/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-02-29 11:03:36.867442 openbb_fred-1.1.4/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2720 2024-03-13 16:36:51.738119 openbb_fred-1.1.4/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-02-29 11:03:36.867578 openbb_fred-1.1.4/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-02-29 11:03:36.867653 openbb_fred-1.1.4/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-02-29 11:03:36.867734 openbb_fred-1.1.4/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-02-29 11:03:36.867879 openbb_fred-1.1.4/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-02-29 11:03:36.868080 openbb_fred-1.1.4/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-02-29 11:03:36.868229 openbb_fred-1.1.4/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-03-13 16:36:51.738236 openbb_fred-1.1.4/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-03-13 16:36:51.738365 openbb_fred-1.1.4/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-02-29 11:03:36.868524 openbb_fred-1.1.4/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-02-29 11:03:36.868834 openbb_fred-1.1.4/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      439 2024-04-01 14:20:11.129481 openbb_fred-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 openbb_fred-1.1.4/PKG-INFO
```

### Comparing `openbb_fred-1.1.3/openbb_fred/__init__.py` & `openbb_fred-1.1.4/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/ameribor_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/cp.py` & `openbb_fred-1.1.4/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/cpi.py` & `openbb_fred-1.1.4/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/dwpcr_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/ecb_interest_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/estr_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/fed_projections.py` & `openbb_fred-1.1.4/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/fed_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/ffrmc.py` & `openbb_fred-1.1.4/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/hqm.py` & `openbb_fred-1.1.4/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/ice_bofa.py` & `openbb_fred-1.1.4/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/iorb_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/moody.py` & `openbb_fred-1.1.4/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/regional.py` & `openbb_fred-1.1.4/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/search.py` & `openbb_fred-1.1.4/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/series.py` & `openbb_fred-1.1.4/openbb_fred/models/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,14 +191,15 @@
     @staticmethod
     def transform_data(
         query: FredSeriesQueryParams, data: Dict, **kwargs: Any
     ) -> List[FredSeriesData]:
         """Transform data."""
         results = (
             pd.DataFrame(data)
+            .filter(items=query.symbol.split(","), axis=1)
             .reset_index()
             .rename(columns={"index": "date"})
             .fillna("N/A")
             .replace("N/A", None)
             .to_dict("records")
         )
         return [FredSeriesData.model_validate(d) for d in results]
```

### Comparing `openbb_fred-1.1.3/openbb_fred/models/sofr_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/sonia_rates.py` & `openbb_fred-1.1.4/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/spot.py` & `openbb_fred-1.1.4/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/tbffr.py` & `openbb_fred-1.1.4/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/tmc.py` & `openbb_fred-1.1.4/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/models/us_yield_curve.py` & `openbb_fred-1.1.4/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/commercial_paper.csv` & `openbb_fred-1.1.4/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_fred-1.1.4/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/cpi.csv` & `openbb_fred-1.1.4/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/fred_base.py` & `openbb_fred-1.1.4/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/fred_helpers.py` & `openbb_fred-1.1.4/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/harmonized_cpi.csv` & `openbb_fred-1.1.4/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_fred-1.1.4/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.1.3/PKG-INFO` & `openbb_fred-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-fred
-Version: 1.1.3
+Version: 1.1.4
 Summary: FRED extension for OpenBB
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
 
 # OpenBB FRED Provider
 
 This extension integrates the [FRED](https://fred.stlouisfed.org/docs/api/fred/) data provider into the OpenBB Platform.
 
 ## Installation
```

