# Comparing `tmp/openbb_benzinga-1.1.3.tar.gz` & `tmp/openbb_benzinga-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_benzinga-1.1.3.tar", max compression
+gzip compressed data, was "openbb_benzinga-1.1.4.tar", max compression
```

## Comparing `openbb_benzinga-1.1.3.tar` & `openbb_benzinga-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      439 2024-01-17 14:26:16.656659 openbb_benzinga-1.1.3/README.md
--rw-r--r--   0        0        0      877 2024-02-23 17:14:57.420548 openbb_benzinga-1.1.3/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.656934 openbb_benzinga-1.1.3/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    15478 2024-03-11 12:49:24.829605 openbb_benzinga-1.1.3/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-02-26 09:52:50.861461 openbb_benzinga-1.1.3/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9784 2024-02-23 17:14:57.421021 openbb_benzinga-1.1.3/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-02-23 17:14:57.421159 openbb_benzinga-1.1.3/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.657199 openbb_benzinga-1.1.3/openbb_benzinga/py.typed
--rw-r--r--   0        0        0        0 2024-01-17 14:26:16.657267 openbb_benzinga-1.1.3/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      463 2024-03-11 20:00:35.139890 openbb_benzinga-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_benzinga-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      439 2024-02-29 11:03:36.753944 openbb_benzinga-1.1.4/README.md
+-rw-r--r--   0        0        0      877 2024-03-21 17:38:35.636625 openbb_benzinga-1.1.4/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754175 openbb_benzinga-1.1.4/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    14906 2024-03-28 17:15:52.365272 openbb_benzinga-1.1.4/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6173 2024-03-13 16:36:51.636904 openbb_benzinga-1.1.4/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9745 2024-03-14 20:30:27.171935 openbb_benzinga-1.1.4/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-03-13 16:36:51.637143 openbb_benzinga-1.1.4/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754477 openbb_benzinga-1.1.4/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754550 openbb_benzinga-1.1.4/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      463 2024-04-01 14:21:35.794640 openbb_benzinga-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_benzinga-1.1.4/PKG-INFO
```

### Comparing `openbb_benzinga-1.1.3/openbb_benzinga/__init__.py` & `openbb_benzinga-1.1.4/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.3/openbb_benzinga/models/analyst_search.py` & `openbb_benzinga-1.1.4/openbb_benzinga/models/analyst_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Benzinga Analyst Search Model."""
 
 # pylint: disable=unused-argument
 
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.analyst_search import (
     AnalystSearchData,
     AnalystSearchQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
@@ -19,69 +19,51 @@
 class BenzingaAnalystSearchQueryParams(AnalystSearchQueryParams):
     """Benzinga Analyst Search Query.
 
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-analysts
     """
 
     __alias_dict__ = {
-        "analyst_ids": "id",
+        "analyst_ids": "analyst",
         "firm_ids": "firm",
         "limit": "pageSize",
     }
+    __json_schema_extra__ = {
+        "analyst_name": ["multiple_items_allowed"],
+        "firm_name": ["multiple_items_allowed"],
+        "analyst_ids": ["multiple_items_allowed"],
+        "firm_ids": ["multiple_items_allowed"],
+        "fields": ["multiple_items_allowed"],
+    }
 
-    analyst_ids: Optional[Union[str, List[str]]] = Field(
+    analyst_ids: Optional[str] = Field(
         default=None,
-        description="A comma separated list of analyst IDs to bring back.",
+        description="List of analyst IDs to return.",
     )
-    firm_ids: Optional[Union[str, List[str]]] = Field(
+    firm_ids: Optional[str] = Field(
         default=None,
-        description="A comma separated list of firm IDs to bring back.",
+        description="Firm IDs to return.",
     )
     limit: Optional[int] = Field(
         default=100,
         description="Number of results returned. Limit 1000.",
     )
     page: Optional[int] = Field(
         default=0,
         description="Page offset. For optimization,"
         + " performance and technical reasons, page offsets"
         + " are limited from 0 - 100000."
         + " Limit the query results by other parameters such as date.",
     )
-    fields: Optional[Union[List[str], str]] = Field(
+    fields: Optional[str] = Field(
         default=None,
-        description="Comma-separated list of fields to include in the response."
+        description="Fields to include in the response."
         " See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields.",
     )
 
-    @field_validator(
-        "fields", "firm_ids", "analyst_ids", mode="before", check_fields=False
-    )
-    @classmethod
-    def convert_list(cls, v: Union[str, List[str]]):
-        """Convert a List[str] to a string list."""
-        if isinstance(v, str):
-            return v.upper()
-        return ",".join([symbol.upper() for symbol in list(v)])
-
-    @field_validator(
-        "analyst_ids",
-        "firm_ids",
-        "analyst_name",
-        "firm_name",
-        mode="before",
-        check_fields=False,
-    )
-    @classmethod
-    def validate_list(cls, v: Union[str, List[str], None]):
-        """Validate list."""
-        if isinstance(v, str):
-            return v
-        return ",".join(v) if v else None
-
 
 class BenzingaAnalystSearchData(AnalystSearchData):
     """Benzinga Analyst Search Data."""
 
     __alias_dict__ = {
         "analyst_id": "id",
         "last_updated": "updated",
```

### Comparing `openbb_benzinga-1.1.3/openbb_benzinga/models/company_news.py` & `openbb_benzinga-1.1.4/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.3/openbb_benzinga/models/price_target.py` & `openbb_benzinga-1.1.4/openbb_benzinga/models/price_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,29 +79,28 @@
     )
     importance: Optional[int] = Field(
         default=None,
         description="Importance level to filter by."
         + " Uses Greater Than or Equal To the importance indicated",
         alias="parameters[importance]",
     )
-    action: Union[
-        None,
+    action: Optional[
         Literal[
             "downgrades",
             "maintains",
             "reinstates",
             "reiterates",
             "upgrades",
             "assumes",
             "initiates",
             "terminates",
             "removes",
             "suspends",
             "firm_dissolved",
-        ],
+        ]
     ] = Field(
         default=None,
         description="Filter by a specific action_company.",
         alias="parameters[action]",
     )
     analyst_ids: Optional[Union[List[str], str]] = Field(
         default=None,
@@ -162,44 +161,42 @@
         "published_time": "time",
         "analyst_firm": "analyst",
         "company_name": "name",
         "rating_previous": "rating_prior",
         "url_analyst": "url",
     }
 
-    action: Union[
-        None,
+    action: Optional[
         Literal[
             "Downgrades",
             "Maintains",
             "Reinstates",
             "Reiterates",
             "Upgrades",
             "Assumes",
             "Initiates Coverage On",
             "Terminates Coverage On",
             "Removes",
             "Suspends",
             "Firm Dissolved",
-        ],
+        ]
     ] = Field(
         default=None,
         description="Description of the change in rating from firm's last rating."
         "Note that all of these terms are precisely defined.",
         alias="action_company",
     )
-    action_change: Union[
-        None,
-        Literal["Announces", "Maintains", "Lowers", "Raises", "Removes", "Adjusts"],
+    action_change: Optional[
+        Literal["Announces", "Maintains", "Lowers", "Raises", "Removes", "Adjusts"]
     ] = Field(
         default=None,
         description="Description of the change in price target from firm's last price target.",
         alias="action_pt",
     )
-    importance: Union[None, Literal[0, 1, 2, 3, 4, 5]] = Field(
+    importance: Optional[Literal[0, 1, 2, 3, 4, 5]] = Field(
         default=None,
         description="Subjective Basis of How Important Event is to Market. 5 = High",
     )
     notes: Optional[str] = Field(default=None, description="Notes of the price target.")
     analyst_id: Optional[str] = Field(default=None, description="Id of the analyst.")
     url_news: Optional[str] = Field(
         default=None,
```

### Comparing `openbb_benzinga-1.1.3/openbb_benzinga/models/world_news.py` & `openbb_benzinga-1.1.4/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.1.3/PKG-INFO` & `openbb_benzinga-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbb-benzinga
-Version: 1.1.3
+Version: 1.1.4
 Summary: Benzinga extension for OpenBB
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
 
 # OpenBB Benzinga Provider
 
 This extension integrates the [Benzinga](https://www.benzinga.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

