# Comparing `tmp/nutshell-0.2.1.tar.gz` & `tmp/nutshell-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutshell-0.2.1.tar", max compression
+gzip compressed data, was "nutshell-0.2.2.tar", max compression
```

## Comparing `nutshell-0.2.1.tar` & `nutshell-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      611 2024-03-30 20:30:42.741253 nutshell-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 13:07:34.650501 nutshell-0.2.1/nutshell/__init__.py
--rw-r--r--   0        0        0     1175 2024-03-28 21:59:56.846699 nutshell-0.2.1/nutshell/api_call.py
--rw-r--r--   0        0        0     2118 2024-03-28 23:46:13.081066 nutshell-0.2.1/nutshell/methods.py
--rw-r--r--   0        0        0     1851 2024-03-29 01:29:17.616144 nutshell-0.2.1/nutshell/responses.py
--rw-r--r--   0        0        0      471 2024-03-30 20:31:36.600066 nutshell-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 nutshell-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1821 2024-04-01 15:52:35.633585 nutshell-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 13:07:34.650501 nutshell-0.2.2/nutshell/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-01 15:21:52.563895 nutshell-0.2.2/nutshell/methods.py
+-rw-r--r--   0        0        0     2411 2024-04-01 15:42:22.465668 nutshell-0.2.2/nutshell/nutshell_api.py
+-rw-r--r--   0        0        0     2221 2024-04-01 15:15:06.717802 nutshell-0.2.2/nutshell/responses.py
+-rw-r--r--   0        0        0      620 2024-04-01 15:58:08.944212 nutshell-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2444 1970-01-01 00:00:00.000000 nutshell-0.2.2/PKG-INFO
```

### Comparing `nutshell-0.2.1/nutshell/methods.py` & `nutshell-0.2.2/nutshell/methods.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,107 @@
 from enum import StrEnum
 from typing import Optional
 
 from pydantic import BaseModel, computed_field
 
 
-class FindUsers(BaseModel):
+class APIMethod(BaseModel):
+    """Base class for all method calls to the Nutshell API."""
+    api_method: str
+
+    @computed_field
+    @property
+    def params(self) -> dict:
+        return {}
+
+
+class FindUsers(APIMethod):
     """findUsers method for Nutshell API."""
     query: Optional[dict] = None
     order_by: str = "last_name"
     order_direction: str = "ASC"
-    limit: None | int = 100
+    limit: int = 50
     page: int = 1
     api_method: str = "findUsers"
 
     @computed_field
     @property
     def params(self) -> dict:
-        params = {}
+        params = {
+            "orderBy": self.order_by,
+            "orderDirection": self.order_direction,
+            "limit": self.limit,
+            "page": self.page
+        }
         if self.query:
             params["query"] = self.query
-        if self.order_by:
-            params["orderBy"] = self.order_by
-        if self.order_direction:
-            params["orderDirection"] = self.order_direction
-        if self.limit:
-            params["limit"] = self.limit
-        if self.page:
-            params["page"] = self.page
 
         return params
 
 
-class GetUser(BaseModel):
+class GetUser(APIMethod):
     """For retrieving a single user from the Nutshell API."""
-    user_id: int
+    user_id: int = None  # with no user_id, the API will return the current user
+    rev: str = None  # included to match API documentation
     api_method: str = "getUser"
 
     @computed_field
     @property
     def params(self) -> dict:
-        return {"userId": self.user_id}
+        params = {}
+        if self.user_id:
+            params["userId"] = self.user_id
+        if self.rev:
+            params["rev"] = self.rev
+        return params
+
+
+class FindTeams(APIMethod):
+    """For retrieving a list of teams from the Nutshell API."""
+    order_by: str = "name"
+    order_direction: str = "ASC"
+    limit: int = 50
+    page: int = 1
+    api_method: str = "findTeams"
+
+    @computed_field
+    @property
+    def params(self) -> dict:
+        params = {
+            "orderBy": self.order_by,
+            "orderDirection": self.order_direction,
+            "limit": self.limit,
+            "page": self.page
+        }
+
+        return params
+
+
+class FindActivityTypes(APIMethod):
+    """For retrieving a list of activity types from the Nutshell API."""
+    order_by: str = "name"
+    order_direction: str = "ASC"
+    limit: int = 50
+    page: int = 1
+    api_method: str = "findActivityTypes"
+
+    @computed_field
+    @property
+    def params(self) -> dict:
+        params = {
+            "orderBy": self.order_by,
+            "orderDirection": self.order_direction,
+            "limit": self.limit,
+            "page": self.page
+        }
+
+        return params
 
 
+# TODO: add more types to match the API documentation
 class ReportType(StrEnum):
     EFFORT = "Effort"
     PIPELINE = "Pipeline"
 
 
 class FilterEntity(StrEnum):
     USERS = "Users"
@@ -60,22 +116,25 @@
 
     @computed_field
     @property
     def filter(self) -> dict:
         return {"entityId": self.entity_id, "entityName": self.entity_name.value}
 
 
-class GetAnalyticsReport(BaseModel):
+class GetAnalyticsReport(APIMethod):
     """For building a valid query to the Nutshell API for the getAnalyticsReport method."""
-    report_type: ReportType = ReportType.EFFORT
-    period: str = "-d30"
+    report_type: ReportType
+    period: str
     filters: list[ReportFilter] = None
+    options: list[dict] = None  # little documentation 
     api_method: str = "getAnalyticsReport"
 
     @computed_field
     @property
     def params(self) -> dict:
         params = {"reportType": self.report_type.value,
                   "period": self.period}
         if self.filters:
             params["filter"] = [entity_filter.filter for entity_filter in self.filters]
+        if self.options:
+            params["options"] = self.options
         return params
```

### Comparing `nutshell-0.2.1/nutshell/responses.py` & `nutshell-0.2.2/nutshell/responses.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,50 @@
 from typing import Dict
 
 from pydantic import BaseModel, Field
 
 
+class APIResponse(BaseModel):
+    """Base class for all API responses."""
+    result: list[BaseModel] | BaseModel
+
+
 class User(BaseModel):
-    stub: bool
+    stub: bool = None
     id: int
-    entity_type: str = Field(..., alias="entityType", pattern=r"Users")
+    entity_type: str = Field(..., validation_alias="entityType", pattern=r"Users")
     rev: str
     name: str
-    first_name: str = Field(None, alias="firstName")
-    last_name: str = Field(None, alias="lastName")
-    is_enabled: bool = Field(..., alias="isEnabled")
-    is_administrator: bool = Field(..., alias="isAdministrator")
+    first_name: str = Field(None, validation_alias="firstName")
+    last_name: str = Field(None, validation_alias="lastName")
+    is_enabled: bool = Field(..., validation_alias="isEnabled")
+    is_administrator: bool = Field(..., validation_alias="isAdministrator")
     emails: list[str]
-    modified_time: str = Field(..., alias="modifiedTime")
-    created_time: str = Field(..., alias="createdTime")
-
-
-class FoundUsersResult(BaseModel):
-    result: list[User]
+    modified_time: str = Field(..., validation_alias="modifiedTime")
+    created_time: str = Field(..., validation_alias="createdTime")
 
 
 class Team(BaseModel):
     stub: bool
     id: int
     name: str
     rev: str
-    entity_type: str = Field(..., alias="entityType", pattern=r"Teams")
-    modified_time: str = Field(..., alias="modifiedTime")
-    created_time: str = Field(..., alias="createdTime")
+    entity_type: str = Field(..., validation_alias="entityType", pattern=r"Teams")
+    modified_time: str = Field(..., validation_alias="modifiedTime")
+    created_time: str = Field(..., validation_alias="createdTime")
 
 
-class FoundTeamsResult(BaseModel):
-    result: list[Team]
-
-
-class Activity(BaseModel):
+class ActivityTypes(BaseModel):
     stub: bool
     id: int
     rev: str
-    entity_type: str = Field(..., alias="entityType", pattern=r"Activity_Types")
+    entity_type: str = Field(..., validation_alias="entityType", pattern=r"Activity_Types")
     name: str
 
 
-class FoundActivityResult(BaseModel):
-    result: list[Activity]
-
-
 class SeriesData(BaseModel):
     total_effort: list[list[int]]
     successful_effort: list[list[int]]
 
 
 class SummaryData(BaseModel):
     sum: float
@@ -61,15 +54,31 @@
     sum_delta: float
     avg_delta: float
     min_delta: float
     max_delta: float
 
 
 class AnalyticsReport(BaseModel):
-    series_data: SeriesData = Field(..., alias="seriesData")
-    summary_data: Dict[str, SummaryData] = Field(..., alias="summaryData")
-    period_description: str = Field(..., alias="periodDescription")
-    delta_period_description: str = Field(..., alias="deltaPeriodDescription")
+    series_data: SeriesData = Field(..., validation_alias="seriesData")
+    summary_data: Dict[str, SummaryData] = Field(..., validation_alias="summaryData")
+    period_description: str = Field(..., validation_alias="periodDescription")
+    delta_period_description: str = Field(..., validation_alias="deltaPeriodDescription")
+
+
+class FindUsersResult(APIResponse):
+    result: list[User]
+
+
+class GetUserResult(APIResponse):
+    result: User
+
+
+class FindTeamsResult(APIResponse):
+    result: list[Team]
+
+
+class FindActivityTypesResult(APIResponse):
+    result: list[ActivityTypes]
 
 
-class AnalyticsResult(BaseModel):
+class GetAnalyticsReportResult(APIResponse):
     result: AnalyticsReport
```

