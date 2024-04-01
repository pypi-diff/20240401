# Comparing `tmp/findly_unified_reporting_sdk-0.6.0.tar.gz` & `tmp/findly_unified_reporting_sdk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findly_unified_reporting_sdk-0.6.0.tar", max compression
+gzip compressed data, was "findly_unified_reporting_sdk-0.6.2.tar", max compression
```

## Comparing `findly_unified_reporting_sdk-0.6.0.tar` & `findly_unified_reporting_sdk-0.6.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.0/LICENSE
--rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.0/README.md
--rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.0/findly/__init__.py
--rw-r--r--   0        0        0      332 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/__init__.py
--rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/common_parser.py
--rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
--rw-r--r--   0        0        0     3886 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/reports_client.py
--rw-r--r--   0        0        0     5727 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
--rw-r--r--   0        0        0    20681 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
--rw-r--r--   0        0        0    31158 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
--rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
--rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
--rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
--rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
--rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
--rw-r--r--   0        0        0    33529 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
--rw-r--r--   0        0        0    29863 2024-03-25 16:26:03.949872 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
--rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
--rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
--rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/.gitignore
--rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/__init__.py
--rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
--rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
--rw-r--r--   0        0        0     2993 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/urs.py
--rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/util/__init__.py
--rw-r--r--   0        0        0      451 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/util/create_numeric_string_series.py
--rw-r--r--   0        0        0     1237 2024-03-25 16:27:04.446810 findly_unified_reporting_sdk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-05 17:34:31.649998 findly_unified_reporting_sdk-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2182 2024-03-14 18:26:39.724288 findly_unified_reporting_sdk-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-22 11:31:41.156543 findly_unified_reporting_sdk-0.6.2/findly/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/__init__.py
+-rw-r--r--   0        0        0     7897 2024-03-22 17:41:32.233479 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/common_parser.py
+-rw-r--r--   0        0        0      971 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py
+-rw-r--r--   0        0        0     3886 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/reports_client.py
+-rw-r--r--   0        0        0     5727 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/__init__.py
+-rw-r--r--   0        0        0    20681 2024-03-22 11:30:17.371131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py
+-rw-r--r--   0        0        0    31158 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py
+-rw-r--r--   0        0        0     1492 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv
+-rw-r--r--   0        0        0     5778 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv
+-rw-r--r--   0        0        0    16489 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0    17708 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv
+-rw-r--r--   0        0        0    20146 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/__init__.py
+-rw-r--r--   0        0        0    33529 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py
+-rw-r--r--   0        0        0    30004 2024-04-01 16:01:21.633515 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py
+-rw-r--r--   0        0        0    33511 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_client.py
+-rw-r--r--   0        0        0     1038 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py
+-rw-r--r--   0        0        0       27 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/.gitignore
+-rw-r--r--   0        0        0      137 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/__init__.py
+-rw-r--r--   0        0        0     6569 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py
+-rw-r--r--   0        0        0    29515 2024-03-22 11:32:22.277139 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi
+-rw-r--r--   0        0        0     2993 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/urs.py
+-rw-r--r--   0        0        0        0 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/util/__init__.py
+-rw-r--r--   0        0        0      451 2024-03-22 11:30:17.375131 findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/util/create_numeric_string_series.py
+-rw-r--r--   0        0        0     1237 2024-04-01 16:01:45.173544 findly_unified_reporting_sdk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 findly_unified_reporting_sdk-0.6.2/PKG-INFO
```

### Comparing `findly_unified_reporting_sdk-0.6.0/LICENSE` & `findly_unified_reporting_sdk-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/README.md` & `findly_unified_reporting_sdk-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/common_parser.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/common_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/date_range_helper.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/reports_client.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/reports_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/common/where_string_comparison.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/fb_ads_query_args_parser.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/action_breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/breakdowns.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/fields.csv`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/fb_ads/metadata/metrics.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_client.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/ga4_query_args_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     "firstSessionDate": ("%Y%m%d", "%Y-%m-%d"),
     "yearMonth": ("%Y%m", "%Y-%m"),
 }
 
 DATE_RANGE_HEADER = "dateRange"
 
 
-def format_ga4_date_ranges_default(start: datetime, end: datetime) -> DateRange:
+def format_ga4_date_ranges_default(start_date: datetime, end_date: datetime) -> DateRange:
     return DateRange(
-        start_date=start.strftime("%Y-%m-%d"), end_date=end.strftime("%Y-%m-%d")
+        start_date=start_date.strftime("%Y-%m-%d"), end_date=end_date.strftime("%Y-%m-%d")
     )
 
 
 class GA4QueryArgsParser(CommonParser):
     def __init__(self) -> None:
         super().__init__()
 
@@ -234,21 +234,21 @@
 
         ga4_dimensions_list = await self.get_dimensions(
             dimensions_name_list=list(query_args.group_by_columns),
         )
         logger.info("sucessfully got dimensions")
 
         ga4_date_ranges = self.get_date_ranges(
-            date_str_range_list=query_args.date_ranges,
+            date_str_range_list=list(query_args.date_ranges) if query_args.date_ranges is not None else None,
             format_function=format_ga4_date_ranges_default,
         )
         logger.info("sucessfully got date ranges")
 
         ga4_order_by_list = await self.get_order_by(
-            order_by_list=query_args.order_by,
+            order_by_list=list(query_args.order_by) if query_args.order_by is not None else None,
             order_by_metrics_candidates=list(query_args.metrics),
             order_by_dimensions_candidates=list(query_args.group_by_columns),
         )
         logger.info("sucessfully got order by")
 
         ga4_dimension_filter_list = await self.get_filter_clause(
             filter_clause=query_args.where_clause
@@ -279,15 +279,15 @@
         ga4_request = {
             "metrics": ga4_metrics_list,
             "dimensions": ga4_dimensions_list,
             "date_ranges": ga4_date_ranges,
             "dimension_filter": ga4_dimension_filter_list,
             "metric_filter": ga4_metrics_filter_list,
             "order_bys": ga4_order_by_list,
-            "limit": query_args.limit,
+            "limit": query_args.limit or None,
             "offset": None,
             "property_id": property_id,
         }
         return ga4_request
 
     # TODO: Allow metric expressions or more complex metrics.
     async def get_dimensions(self, dimensions_name_list: List[str]) -> List[Dimension]:
@@ -342,15 +342,15 @@
 
         Note:
             A "-" sign can be used to specify reverse order, e.g. "-ds".
             This will be used for the GA4 API.
         """
         order_bys: List[OrderBy] = []
 
-        for order_by in order_by_list:
+        for order_by in (order_by_list or []):
             if order_by.startswith("-"):
                 order_by = order_by[1:]
                 if order_by in order_by_metrics_candidates:
                     order_bys.append(
                         OrderBy(
                             metric=OrderBy.MetricOrderBy(
                                 metric_name=order_by,
```

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/ga4/metadata/dimensions.jsonl`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/data_sources/gsc/gsc_service.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/protos/findly_semantic_layer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/findly/unified_reporting_sdk/urs.py` & `findly_unified_reporting_sdk-0.6.2/findly/unified_reporting_sdk/urs.py`

 * *Files identical despite different names*

### Comparing `findly_unified_reporting_sdk-0.6.0/pyproject.toml` & `findly_unified_reporting_sdk-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findly.unified-reporting-sdk"
-version = "0.6.0"
+version = "0.6.2"
 license = "GPL-3.0-only"
 description = ""
 authors = []
 readme = "README.md"
 packages = [
     { include = "findly" },
 ]
```

### Comparing `findly_unified_reporting_sdk-0.6.0/PKG-INFO` & `findly_unified_reporting_sdk-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findly-unified-reporting-sdk
-Version: 0.6.0
+Version: 0.6.2
 Summary: 
 License: GPL-3.0-only
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

