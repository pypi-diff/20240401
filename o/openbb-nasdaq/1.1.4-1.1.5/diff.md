# Comparing `tmp/openbb_nasdaq-1.1.4.tar.gz` & `tmp/openbb_nasdaq-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nasdaq-1.1.4.tar", max compression
+gzip compressed data, was "openbb_nasdaq-1.1.5.tar", max compression
```

## Comparing `openbb_nasdaq-1.1.4.tar` & `openbb_nasdaq-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      430 2024-01-17 14:26:16.774055 openbb_nasdaq-1.1.4/README.md
--rw-r--r--   0        0        0     1840 2024-02-06 11:54:53.232836 openbb_nasdaq-1.1.4/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.774254 openbb_nasdaq-1.1.4/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3954 2024-02-06 11:54:53.232950 openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6262 2024-01-17 14:26:16.774385 openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-01-17 14:26:16.774470 openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     5969 2024-02-06 11:54:53.233724 openbb_nasdaq-1.1.4/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2173 2024-01-17 14:26:16.774613 openbb_nasdaq-1.1.4/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5097 2024-03-11 10:41:33.409171 openbb_nasdaq-1.1.4/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-02-07 09:55:40.833885 openbb_nasdaq-1.1.4/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5090 2024-02-23 17:14:57.468371 openbb_nasdaq-1.1.4/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-02-06 11:54:53.233918 openbb_nasdaq-1.1.4/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-02-23 17:14:57.468475 openbb_nasdaq-1.1.4/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-02-23 17:14:57.468572 openbb_nasdaq-1.1.4/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.775081 openbb_nasdaq-1.1.4/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.775174 openbb_nasdaq-1.1.4/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-01-17 14:26:16.775252 openbb_nasdaq-1.1.4/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-02-06 11:54:53.234791 openbb_nasdaq-1.1.4/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-02-23 17:14:57.468862 openbb_nasdaq-1.1.4/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      508 2024-03-11 19:58:34.263709 openbb_nasdaq-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 openbb_nasdaq-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      430 2024-02-29 11:03:36.880528 openbb_nasdaq-1.1.5/README.md
+-rw-r--r--   0        0        0     1840 2024-03-21 17:38:35.650621 openbb_nasdaq-1.1.5/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.880694 openbb_nasdaq-1.1.5/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3954 2024-03-21 17:38:35.650736 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6262 2024-03-21 17:38:35.650845 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-03-21 17:38:35.651100 openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     5969 2024-03-21 17:38:35.651308 openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2173 2024-03-21 17:38:35.651441 openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5105 2024-03-21 17:38:35.651670 openbb_nasdaq-1.1.5/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-03-13 16:36:51.754918 openbb_nasdaq-1.1.5/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5090 2024-03-21 17:38:35.651807 openbb_nasdaq-1.1.5/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-03-21 17:38:35.651935 openbb_nasdaq-1.1.5/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-03-21 17:38:35.652047 openbb_nasdaq-1.1.5/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-03-13 16:36:51.755257 openbb_nasdaq-1.1.5/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-03-13 16:36:51.755288 openbb_nasdaq-1.1.5/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.881374 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-02-29 11:03:36.881453 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-03-13 16:36:51.755367 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-03-13 16:36:51.755567 openbb_nasdaq-1.1.5/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      508 2024-04-01 14:19:55.357414 openbb_nasdaq-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1088 1970-01-01 00:00:00.000000 openbb_nasdaq-1.1.5/PKG-INFO
```

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/__init__.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/cot.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/cot_search.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/economic_calendar.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/economic_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.economic_calendar import (
     EconomicCalendarData,
     EconomicCalendarQueryParams,
 )
-from openbb_nasdaq.utils.helpers import HEADERS, date_range, remove_html_tags
+from openbb_nasdaq.utils.helpers import IPO_HEADERS, date_range, remove_html_tags
 from pydantic import Field, field_validator
 
 
 class NasdaqEconomicCalendarQueryParams(EconomicCalendarQueryParams):
     """Nasdaq Economic Calendar Query.
 
     Source: https://www.nasdaq.com/market-activity/economic-calendar
@@ -103,15 +103,15 @@
         dates = [
             date.strftime("%Y-%m-%d")
             for date in date_range(query.start_date, query.end_date)
         ]
 
         def get_calendar_data(date: str, data: List[Dict]) -> None:
             url = f"https://api.nasdaq.com/api/calendar/economicevents?date={date}"
-            r = requests.get(url, headers=HEADERS, timeout=5)
+            r = requests.get(url, headers=IPO_HEADERS, timeout=5)
             r_json = r.json()
             if "data" in r_json and "rows" in r_json["data"]:
                 response = r_json["data"]["rows"]
             response = [
                 {
                     **{k: v for k, v in item.items() if k != "gmt"},
                     "date": (
```

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/equity_search.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/historical_dividends.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/models/top_retail.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/utils/helpers.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/utils/query_params.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/openbb_nasdaq/utils/series_ids.py` & `openbb_nasdaq-1.1.5/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.1.4/PKG-INFO` & `openbb_nasdaq-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-nasdaq
-Version: 1.1.4
+Version: 1.1.5
 Summary: Nasdaq extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nasdaq-data-link (>=1.0.4,<2.0.0)
-Requires-Dist: openbb-core (>=1.1.3,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Nasdaq Provider
 
 This extension integrates the [Nasdaq](https://www.nasdaq.com) data provider into the OpenBB Platform.
```

