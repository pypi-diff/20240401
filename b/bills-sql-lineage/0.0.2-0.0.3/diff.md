# Comparing `tmp/bills_sql_lineage-0.0.2.tar.gz` & `tmp/bills_sql_lineage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bills_sql_lineage-0.0.2.tar", max compression
+gzip compressed data, was "bills_sql_lineage-0.0.3.tar", max compression
```

## Comparing `bills_sql_lineage-0.0.2.tar` & `bills_sql_lineage-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3662 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/README.md
--rw-r--r--   0        0        0     1086 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/sql_lineage/__init__.py
--rw-r--r--   0        0        0      277 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/sql_lineage/__main__.py
--rw-r--r--   0        0        0     1562 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/sql_lineage/lineage.py
--rw-r--r--   0        0        0     1086 2024-03-25 11:36:03.656798 bills_sql_lineage-0.0.2/sql_lineage/main.py
--rw-r--r--   0        0        0     4090 1970-01-01 00:00:00.000000 bills_sql_lineage-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3853 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/README.md
+-rw-r--r--   0        0        0     1086 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/sql_lineage/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/sql_lineage/__main__.py
+-rw-r--r--   0        0        0     1792 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/sql_lineage/lineage.py
+-rw-r--r--   0        0        0     1485 2024-04-01 15:30:34.341466 bills_sql_lineage-0.0.3/sql_lineage/main.py
+-rw-r--r--   0        0        0     4281 1970-01-01 00:00:00.000000 bills_sql_lineage-0.0.3/PKG-INFO
```

### Comparing `bills_sql_lineage-0.0.2/README.md` & `bills_sql_lineage-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,18 +61,24 @@
 
 Pass the path to a SQL file to the `lineage` command to generate the lineage as a [Mermaid](https://mermaid.js.org/) diagram:
 
 ```
 lineage path/to/file.sql
 ```
 
-This will write a Mermaid diagram to `path/to/file.mermaid`. You can control the target with the second argument:
+This will write a Mermaid diagram to `path/to/file.mermaid`. You can control the target path with the `--target` argument:
 
 ```
-lineage path/to/file.sql path/to/output.mermaid
+lineage path/to/file.sql --target path/to/output.mermaid
+```
+
+By default, the SQL dialect will be inferred by SQLGlot, but you can specify a dialect with the `--dialect` argument:
+
+```
+lineage path/to/file.sql --dialect snowflake
 ```
 
 ## Example 📝
 
 Given the following SQL query:
 
 ```sql
```

### Comparing `bills_sql_lineage-0.0.2/pyproject.toml` & `bills_sql_lineage-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "bills-sql-lineage"  # For PyPI
-version = "0.0.2"
+version = "0.0.3"
 description = "Personal SQL lineage generator."
 authors = ["Bilbottom"]
 readme = "README.md"
 packages = [{include = "sql_lineage"}]
 
 [tool.poetry.scripts]
 lineage = 'sql_lineage.__main__:app'
```

### Comparing `bills_sql_lineage-0.0.2/sql_lineage/lineage.py` & `bills_sql_lineage-0.0.3/sql_lineage/lineage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 """
 Parsers for SQL queries and Mermaid graphs.
 """
 
 from __future__ import annotations
 
 import contextlib
+import datetime
 
 import sqlglot
 from sqlglot import exp
 from sqlglot.optimizer import qualify
 
 Nodes = list[str]
 Edges = list[tuple[str, str]]  # Directed edges, source --> target.
 
 
-def _parse_ctes(sql: str) -> [Nodes, Edges]:
+def _parse_ctes(sql: str, dialect: str = None) -> [Nodes, Edges]:
     """
     Parse an SQL query into nodes and edges based on CTEs.
     """
     nodes, edges = [], []
-    parsed = sqlglot.parse_one(sql)
+    parsed = sqlglot.parse_one(sql, dialect=dialect)
     with contextlib.suppress(Exception):
         # There isn't a hard requirement for the query to be valid SQL,
         # but it's better if it is
         parsed = qualify.qualify(parsed)
 
     # Lazy and error-prone CTE sourcing
     for cte in parsed.find_all(exp.CTE):
         nodes.append(cte.alias)
         edges.extend((tbl.name, cte.alias) for tbl in cte.find_all(exp.Table))
 
     parsed.args["with"] = None  # Dirty hack to remove the CTEs from the query
-    nodes.append("final")
-    edges.extend((tbl.name, "final") for tbl in parsed.find_all(exp.Table))
+    final = "final" if "final" not in nodes else "final_"
+    nodes.append(final)
+    edges.extend((tbl.name, final) for tbl in parsed.find_all(exp.Table))
 
     return nodes, edges
 
 
 def _to_mermaid(nodes: Nodes, edges: Edges) -> str:
     """
     Convert nodes and edges into a Mermaid graph.
     """
-    mermaid = "graph TD\n"
+    now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    mermaid = f"%% Generated at {now}\nflowchart TD\n"
 
     for node in nodes:
         mermaid += f"    {node}\n"  # pylint: disable=consider-using-join
 
     for edge in edges:
         mermaid += f"    {edge[0]} --> {edge[1]}\n"
 
     return mermaid
 
 
-def sql_to_mermaid(sql: str) -> str:
+def sql_to_mermaid(sql: str, dialect: str = None) -> str:
     """
     Convert an SQL query into a Mermaid graph.
     """
-    nodes, edges = _parse_ctes(sql)
+    nodes, edges = _parse_ctes(sql, dialect)
 
     return _to_mermaid(nodes, edges)
```

### Comparing `bills_sql_lineage-0.0.2/sql_lineage/main.py` & `bills_sql_lineage-0.0.3/sql_lineage/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,20 +22,27 @@
         if not path.is_file():
             raise ValueError(f"Not a file: {file_path}")
 
     return path
 
 
 @arguably.command
-def main(file: str, target: str = None) -> None:
+def main(file: str, *, target: str = None, dialect: str = None) -> None:
     """
     Parse an SQL file into a Mermaid graph by tracing CTEs.
+
+    :param file: The path to the SQL file to parse.
+    :param target: The path to write the Mermaid graph to. If not provided,
+        the graph will be written to a file with the same name as the input
+        file, but with a ``.mermaid`` extension.
+    :param dialect: The SQL dialect to use. If not provided, SQLGlot will
+        attempt to infer the dialect.
     """
     file_path = _to_path(file, validate=True)
     target_path = _to_path(target) if target else file_path.with_suffix(".mermaid")
 
     sql = file_path.read_text(encoding="utf-8")
-    mermaid = lineage.sql_to_mermaid(sql)
+    mermaid = lineage.sql_to_mermaid(sql, dialect)
 
     target_path.write_text(mermaid, encoding="utf-8")
     # Switch to logging at some point
     print(f"Mermaid graph written to: {target_path.absolute()}")
```

### Comparing `bills_sql_lineage-0.0.2/PKG-INFO` & `bills_sql_lineage-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bills-sql-lineage
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal SQL lineage generator.
 Author: Bilbottom
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arguably (>=1.2.5,<2.0.0)
@@ -74,18 +74,24 @@
 
 Pass the path to a SQL file to the `lineage` command to generate the lineage as a [Mermaid](https://mermaid.js.org/) diagram:
 
 ```
 lineage path/to/file.sql
 ```
 
-This will write a Mermaid diagram to `path/to/file.mermaid`. You can control the target with the second argument:
+This will write a Mermaid diagram to `path/to/file.mermaid`. You can control the target path with the `--target` argument:
 
 ```
-lineage path/to/file.sql path/to/output.mermaid
+lineage path/to/file.sql --target path/to/output.mermaid
+```
+
+By default, the SQL dialect will be inferred by SQLGlot, but you can specify a dialect with the `--dialect` argument:
+
+```
+lineage path/to/file.sql --dialect snowflake
 ```
 
 ## Example 📝
 
 Given the following SQL query:
 
 ```sql
```

