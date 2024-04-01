# Comparing `tmp/answerrocket-client-0.1.8.tar.gz` & `tmp/answerrocket-client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket-client-0.1.8.tar", last modified: Fri Dec  8 21:08:23 2023, max compression
+gzip compressed data, was "answerrocket-client-0.1.9.tar", last modified: Mon Dec 11 17:34:12 2023, max compression
```

## Comparing `answerrocket-client-0.1.8.tar` & `answerrocket-client-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14089 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22240 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-08 21:08:23.000000 answerrocket-client-0.1.8/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-08 21:08:23.000000 answerrocket-client-0.1.8/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 21:08:23.000000 answerrocket-client-0.1.8/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-08 21:08:23.000000 answerrocket-client-0.1.8/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-08 21:08:23.000000 answerrocket-client-0.1.8/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 21:08:23.029597 answerrocket-client-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-08 21:08:15.000000 answerrocket-client-0.1.8/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.430043 answerrocket-client-0.1.9/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22240 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-11 17:34:12.000000 answerrocket-client-0.1.9/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 17:34:12.434043 answerrocket-client-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-12-11 17:34:04.000000 answerrocket-client-0.1.9/test/test_client.py
```

### Comparing `answerrocket-client-0.1.8/PKG-INFO` & `answerrocket-client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket-client-0.1.8/answer_rocket/auth.py` & `answerrocket-client-0.1.9/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/chat.py` & `answerrocket-client-0.1.9/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/client.py` & `answerrocket-client-0.1.9/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/config.py` & `answerrocket-client-0.1.9/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/data.py` & `answerrocket-client-0.1.9/answer_rocket/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Helper for accessing data from the server.
     """
 
     def __init__(self, auth_helper: AuthHelper, gql_client: GraphQlClient) -> None:
         self._auth_helper = auth_helper
         self._gql_client = gql_client
 
-    def execute_sql_query(self, database_id: UUID, sql_query: str, row_limit: Optional[int]) -> ExecuteSqlQueryResult:
+    def execute_sql_query(self, database_id: UUID, sql_query: str, row_limit: Optional[int] = None) -> ExecuteSqlQueryResult:
         try:
             """
             database_id: the database_id of the connection to execute against.
             sql_query: the SQL query to execute.
             row_limit: the optional row limit of the query results.
             """
             query_args = {
```

### Comparing `answerrocket-client-0.1.8/answer_rocket/graphql/client.py` & `answerrocket-client-0.1.9/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/graphql/schema.py` & `answerrocket-client-0.1.9/answer_rocket/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/output.py` & `answerrocket-client-0.1.9/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answer_rocket/skill.py` & `answerrocket-client-0.1.9/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/answerrocket_client.egg-info/PKG-INFO` & `answerrocket-client-0.1.9/answerrocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket-client-0.1.8/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket-client-0.1.9/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket-client-0.1.8/readme.md` & `answerrocket-client-0.1.9/readme.md`

 * *Files identical despite different names*

