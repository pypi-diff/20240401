# Comparing `tmp/approck_sqlalchemy_query_builder-0.1.4.tar.gz` & `tmp/approck_sqlalchemy_query_builder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_sqlalchemy_query_builder-0.1.4.tar", max compression
+gzip compressed data, was "approck_sqlalchemy_query_builder-1.0.0.tar", max compression
```

## Comparing `approck_sqlalchemy_query_builder-0.1.4.tar` & `approck_sqlalchemy_query_builder-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-02-13 13:20:04.902785 approck_sqlalchemy_query_builder-0.1.4/README.md
--rw-r--r--   0        0        0     2692 2024-02-13 13:20:04.878785 approck_sqlalchemy_query_builder-0.1.4/approck_sqlalchemy_query_builder/__init__.py
--rw-r--r--   0        0        0      639 2024-02-13 13:20:04.878785 approck_sqlalchemy_query_builder-0.1.4/approck_sqlalchemy_query_builder/types.py
--rw-r--r--   0        0        0      539 2024-02-13 13:20:04.878785 approck_sqlalchemy_query_builder-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 approck_sqlalchemy_query_builder-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-01 18:27:34.009615 approck_sqlalchemy_query_builder-1.0.0/README.md
+-rw-r--r--   0        0        0     2627 2024-04-01 18:27:33.985615 approck_sqlalchemy_query_builder-1.0.0/approck_sqlalchemy_query_builder/__init__.py
+-rw-r--r--   0        0        0      639 2024-04-01 18:27:33.985615 approck_sqlalchemy_query_builder-1.0.0/approck_sqlalchemy_query_builder/types.py
+-rw-r--r--   0        0        0      506 2024-04-01 18:27:33.985615 approck_sqlalchemy_query_builder-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 approck_sqlalchemy_query_builder-1.0.0/PKG-INFO
```

### Comparing `approck_sqlalchemy_query_builder-0.1.4/approck_sqlalchemy_query_builder/__init__.py` & `approck_sqlalchemy_query_builder-1.0.0/approck_sqlalchemy_query_builder/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
 import time
 from typing import Dict, List
 
-import pytz
 import sqlalchemy as sa
 from dateutil.parser import parse
-from sqlalchemy.sql.elements import BooleanClauseList, ColumnElement
+from sqlalchemy.sql.elements import ColumnElement
 from sqlalchemy.sql.expression import Select
 
 from approck_sqlalchemy_query_builder.types import Condition, Operator, Query, QueryRule
 
 
 def build_rule_condition(map_columns: Dict[str, sa.Column], rule: QueryRule) -> ColumnElement[sa.Boolean]:
     column = map_columns.get(rule.id)
@@ -20,17 +19,17 @@
     value = rule.value
 
     if "DATETIME" in str(column.type).upper():
         if isinstance(value, int):
             if value > time.time():
                 value /= 1000.0
 
-            value = datetime.datetime.fromtimestamp(value, tz=pytz.utc)
+            value = datetime.datetime.fromtimestamp(value, tz=datetime.timezone.utc)
         elif isinstance(value, (str, bytes)):
-            value = parse(value).replace(tzinfo=pytz.utc)
+            value = parse(value).replace(tzinfo=datetime.timezone.utc)
 
     if rule.operator == Operator.OP_EQUAL:
         return column == value
     elif rule.operator == Operator.OP_GREATER_THAN:
         return column > value
     elif rule.operator == Operator.OP_LESS_THAN:
         return column < value
@@ -46,16 +45,16 @@
         return column.not_in(value)
 
     raise ValueError(f"Operator '{rule.operator}' is not supported")
 
 
 def build_condition(
     map_columns: Dict[str, sa.Column], query: Query
-) -> BooleanClauseList[ColumnElement[sa.Boolean]] | None:
-    clauses: List[BooleanClauseList[ColumnElement[sa.Boolean]] | ColumnElement[sa.Boolean]] = []
+) -> List[ColumnElement[sa.Boolean]] | None:
+    clauses: List[ColumnElement[sa.Boolean]] = []
 
     for rule in query.rules:
         if isinstance(rule, Query):
             condition = build_condition(map_columns=map_columns, query=rule)
 
             if condition is not None:
                 clauses.append(condition)
```

### Comparing `approck_sqlalchemy_query_builder-0.1.4/approck_sqlalchemy_query_builder/types.py` & `approck_sqlalchemy_query_builder-1.0.0/approck_sqlalchemy_query_builder/types.py`

 * *Files identical despite different names*

### Comparing `approck_sqlalchemy_query_builder-0.1.4/PKG-INFO` & `approck_sqlalchemy_query_builder-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: approck-sqlalchemy-query-builder
-Version: 0.1.4
+Version: 1.0.0
 Summary: 
 Author: Aleksey Dalekin
 Author-email: adalekin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: SQLAlchemy[mypy] (>=1.4.41,<2.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: SQLAlchemy[mypy] (>=2.0.27,<3.0.0)
+Requires-Dist: pydantic (>=2.4.1,<2.6)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: pytz (>=2024.1,<2025.0)
 Description-Content-Type: text/markdown
```

