# Comparing `tmp/waii-sdk-py-1.9.0.tar.gz` & `tmp/waii-sdk-py-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waii-sdk-py-1.9.0.tar", last modified: Fri Jan 19 22:49:58 2024, max compression
+gzip compressed data, was "waii-sdk-py-1.9.1.tar", last modified: Mon Jan 22 22:20:23 2024, max compression
```

## Comparing `waii-sdk-py-1.9.0.tar` & `waii-sdk-py-1.9.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.748324 waii-sdk-py-1.9.0/
--rw-r--r--   0 wangdatan   (501) staff       (20)    11357 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/LICENSE
--rw-r--r--   0 wangdatan   (501) staff       (20)    20729 2024-01-19 22:49:58.748201 waii-sdk-py-1.9.0/PKG-INFO
--rw-r--r--   0 wangdatan   (501) staff       (20)    20201 2023-11-22 22:53:43.000000 waii-sdk-py-1.9.0/README.md
--rw-r--r--   0 wangdatan   (501) staff       (20)       90 2023-08-18 22:53:20.000000 waii-sdk-py-1.9.0/pyproject.toml
--rw-r--r--   0 wangdatan   (501) staff       (20)      570 2024-01-19 22:49:58.748625 waii-sdk-py-1.9.0/setup.cfg
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.743664 waii-sdk-py-1.9.0/tests/
--rw-r--r--   0 wangdatan   (501) staff       (20)      127 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.0/tests/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     4273 2023-10-18 21:39:50.000000 waii-sdk-py-1.9.0/tests/database_tests.py
--rw-r--r--   0 wangdatan   (501) staff       (20)      880 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.0/tests/history_tests.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     2679 2023-11-02 07:20:51.000000 waii-sdk-py-1.9.0/tests/query_tests.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     1299 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.0/tests/semantic_context_tests.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.744423 waii-sdk-py-1.9.0/waii_sdk_py/
--rw-r--r--   0 wangdatan   (501) staff       (20)       29 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/__init__.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.745578 waii-sdk-py-1.9.0/waii_sdk_py/database/
--rw-r--r--   0 wangdatan   (501) staff       (20)       23 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/database/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     6541 2024-01-19 22:17:43.000000 waii-sdk-py-1.9.0/waii_sdk_py/database/database.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.746081 waii-sdk-py-1.9.0/waii_sdk_py/history/
--rw-r--r--   0 wangdatan   (501) staff       (20)       22 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/history/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)      878 2023-10-18 17:14:07.000000 waii-sdk-py-1.9.0/waii_sdk_py/history/history.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.746654 waii-sdk-py-1.9.0/waii_sdk_py/query/
--rw-r--r--   0 wangdatan   (501) staff       (20)       20 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/query/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)    10547 2024-01-19 22:18:26.000000 waii-sdk-py-1.9.0/waii_sdk_py/query/query.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.747159 waii-sdk-py-1.9.0/waii_sdk_py/semantic_context/
--rw-r--r--   0 wangdatan   (501) staff       (20)       31 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/semantic_context/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     1342 2023-10-18 17:14:07.000000 waii-sdk-py-1.9.0/waii_sdk_py/semantic_context/semantic_context.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.747454 waii-sdk-py-1.9.0/waii_sdk_py/waii_http_client/
--rw-r--r--   0 wangdatan   (501) staff       (20)       44 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.0/waii_sdk_py/waii_http_client/__init__.py
--rw-r--r--   0 wangdatan   (501) staff       (20)     2607 2023-11-02 07:15:34.000000 waii-sdk-py-1.9.0/waii_sdk_py/waii_http_client/waii_http_client.py
--rw-r--r--   0 wangdatan   (501) staff       (20)      578 2023-10-18 21:36:17.000000 waii-sdk-py-1.9.0/waii_sdk_py/waii_sdk_py.py
-drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-19 22:49:58.747826 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/
--rw-r--r--   0 wangdatan   (501) staff       (20)    20729 2024-01-19 22:49:58.000000 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/PKG-INFO
--rw-r--r--   0 wangdatan   (501) staff       (20)      751 2024-01-19 22:49:58.000000 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/SOURCES.txt
--rw-r--r--   0 wangdatan   (501) staff       (20)        1 2024-01-19 22:49:58.000000 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/dependency_links.txt
--rw-r--r--   0 wangdatan   (501) staff       (20)       27 2024-01-19 22:49:58.000000 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/requires.txt
--rw-r--r--   0 wangdatan   (501) staff       (20)       18 2024-01-19 22:49:58.000000 waii-sdk-py-1.9.0/waii_sdk_py.egg-info/top_level.txt
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.065240 waii-sdk-py-1.9.1/
+-rw-r--r--   0 wangdatan   (501) staff       (20)    11357 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/LICENSE
+-rw-r--r--   0 wangdatan   (501) staff       (20)    22003 2024-01-22 22:20:23.065171 waii-sdk-py-1.9.1/PKG-INFO
+-rw-r--r--   0 wangdatan   (501) staff       (20)    21475 2024-01-19 23:56:01.000000 waii-sdk-py-1.9.1/README.md
+-rw-r--r--   0 wangdatan   (501) staff       (20)       90 2023-08-18 22:53:20.000000 waii-sdk-py-1.9.1/pyproject.toml
+-rw-r--r--   0 wangdatan   (501) staff       (20)      570 2024-01-22 22:20:23.065484 waii-sdk-py-1.9.1/setup.cfg
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.060823 waii-sdk-py-1.9.1/tests/
+-rw-r--r--   0 wangdatan   (501) staff       (20)      127 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.1/tests/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     4273 2023-10-18 21:39:50.000000 waii-sdk-py-1.9.1/tests/database_tests.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)      880 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.1/tests/history_tests.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     2679 2023-11-02 07:20:51.000000 waii-sdk-py-1.9.1/tests/query_tests.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     1299 2023-10-18 19:20:50.000000 waii-sdk-py-1.9.1/tests/semantic_context_tests.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.061655 waii-sdk-py-1.9.1/waii_sdk_py/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       29 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/__init__.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.062729 waii-sdk-py-1.9.1/waii_sdk_py/database/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       23 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/database/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     6541 2024-01-19 22:59:27.000000 waii-sdk-py-1.9.1/waii_sdk_py/database/database.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.063226 waii-sdk-py-1.9.1/waii_sdk_py/history/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       22 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/history/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)      878 2023-10-18 17:14:07.000000 waii-sdk-py-1.9.1/waii_sdk_py/history/history.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.064011 waii-sdk-py-1.9.1/waii_sdk_py/query/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       20 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/query/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)    10615 2024-01-22 22:07:29.000000 waii-sdk-py-1.9.1/waii_sdk_py/query/query.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.064499 waii-sdk-py-1.9.1/waii_sdk_py/semantic_context/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       31 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/semantic_context/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     1342 2023-10-18 17:14:07.000000 waii-sdk-py-1.9.1/waii_sdk_py/semantic_context/semantic_context.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.064769 waii-sdk-py-1.9.1/waii_sdk_py/waii_http_client/
+-rw-r--r--   0 wangdatan   (501) staff       (20)       44 2023-08-03 12:14:54.000000 waii-sdk-py-1.9.1/waii_sdk_py/waii_http_client/__init__.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)     2607 2023-11-02 07:15:34.000000 waii-sdk-py-1.9.1/waii_sdk_py/waii_http_client/waii_http_client.py
+-rw-r--r--   0 wangdatan   (501) staff       (20)      578 2023-10-18 21:36:17.000000 waii-sdk-py-1.9.1/waii_sdk_py/waii_sdk_py.py
+drwxr-xr-x   0 wangdatan   (501) staff       (20)        0 2024-01-22 22:20:23.064940 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/
+-rw-r--r--   0 wangdatan   (501) staff       (20)    22003 2024-01-22 22:20:23.000000 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/PKG-INFO
+-rw-r--r--   0 wangdatan   (501) staff       (20)      751 2024-01-22 22:20:23.000000 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/SOURCES.txt
+-rw-r--r--   0 wangdatan   (501) staff       (20)        1 2024-01-22 22:20:23.000000 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/dependency_links.txt
+-rw-r--r--   0 wangdatan   (501) staff       (20)       27 2024-01-22 22:20:23.000000 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/requires.txt
+-rw-r--r--   0 wangdatan   (501) staff       (20)       18 2024-01-22 22:20:23.000000 waii-sdk-py-1.9.1/waii_sdk_py.egg-info/top_level.txt
```

### Comparing `waii-sdk-py-1.9.0/LICENSE` & `waii-sdk-py-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/PKG-INFO` & `waii-sdk-py-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waii-sdk-py
-Version: 1.9.0
+Version: 1.9.1
 Summary: Provides access to the Waii APIs
 Home-page: http://www.waii.ai
 Author: Waii, Inc.
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -213,18 +213,21 @@
       - `summary`: generated description of the schema 
       - `common_questions`: list of generated common questions
       - `common_tables`: list of common tables used in the schema
       - `tables`: all tables belong to the schema
         - `name`: Name of the table
         - `columns`: List of columns 
           - `name`: Name of the column 
-          - `type`: Type of the column 
+          - `type`: Type of the column
+          - `description`: Auto generated description of the column
         - `comment`: Comment of the table (fetched from underlying database) 
         - `last_altered_time`: Last altered time of the table 
-        - `refs`: List of referential constraints 
+        - `refs`: List of referential constraints
+        - `inferred_refs`: List of auto-inferred referential constraints
+        - `inferred_constraints`: List of auto-inferred constraints (pks, etc.)
         - `description`: Auto generated table description
 
 Waii automatically generate table/schema descriptions when you add them, you can fetch them by using `description` field of table and schema from `get_catalogs` method.
 
 Description of table looks like: 
 
 ```
@@ -243,15 +246,15 @@
 ## Query
 
 The `Query` module contains methods related to SQL query handling. 
 **Important:** You need to activate the database connection first before using the methods in this module. Otherwise you may trying to generate query from a wrong database.
 
 Here are some of its methods:
 
-### Generate
+### Generate Query
 
 ```python
 Query.generate(params: QueryGenerationRequest) -> GeneratedQuery
 ```
 
 This method generates a SQL query based on the provided parameters.
 
@@ -310,14 +313,33 @@
 - `query`: The generated query text
 - `tables`: Tables used in the generated query
 - `semantic_context`: Semantic context applied to the generated query
 - `detailed_steps`: Detailed steps of how the query work (in natural language)
 - `what_changed`: If you do a tweak, it will tell you what changed in the query
 - `compilation_error`: If there is any compilation error, it will show here. (Waii will try to fix the compilation error automatically, but if it tried multiple times and still cannot fix it, it will show here)
 
+### Generate Question
+
+You can also generate questions based on your database schema, which can be useful when you want to show to your user what kind of questions can be asked to the database.
+
+```python
+>>> Query.generate_question(GenerateQuestionRequest(schema_name='PUBLIC',
+                                                    n_questions=10,
+                                                    complexity=GeneratedQuestionComplexity.hard))
+```
+
+Parameter fields:
+- `schema_name`: The schema name you want to generate questions. This is must be specified.
+- `n_questions`: Number of questions you want to generate. Default is 10. You can choose a number between 1 to 30. 
+- `complexity`: Complexity of the questions you want to generate. Default is `GeneratedQuestionComplexity.hard`. You can choose `easy`, `medium`, `hard`.
+
+Output `GenerateQuestionResponse`, fields:
+- `questions`: List of generated questions. For each question it has `question` (string content of the question), and `complexity` (complexity of the question)
+
+
 ### Transcode
 
 ```python
 >>> WAII.Query.transcode(TranscodeQueryRequest(source_dialect="postgres", source_query="select ...;", target_dialect="snowflake", ask="..."))
 ```
 
 Parameter fields:
@@ -326,16 +348,14 @@
 - `source_query`: The source query you want to transcode
 - `target_dialect`: The dialect of the target query, such as `snowflake`, `postgresql`, `mongodb`
 - `ask`: The intructions you want to ask Waii to add when transcode the query, such as `place tables under schema1`. It is optional.
 
 
 #### `Query.transcode` returns `GeneratedQuery` object
 
-
-
 ### Run a query (sync)
 
 ```python
 Query.run(params: RunQueryRequest) -> GetQueryResultResponse
 ```
 
 Request fields:
@@ -477,15 +497,15 @@
 ```python
 >>> print(WAII.Query.auto_complete(AutoCompleteRequest(text='select from', cursor_offset=11, max_output_tokens=50)))
 
 text='WAII.WORLD.CITY WHERE POPULATION > 1000000'
 ```
 
 
-#### Analyze Performance
+#### Analyze Performance (Experimental)
 
 Note: this feature currently only support Snowflake
 
 ```python
 Query.analyze_performance(params: QueryPerformanceRequest) -> QueryPerformanceResponse
 ```
```

### Comparing `waii-sdk-py-1.9.0/README.md` & `waii-sdk-py-1.9.1/waii_sdk_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: waii-sdk-py
+Version: 1.9.1
+Summary: Provides access to the Waii APIs
+Home-page: http://www.waii.ai
+Author: Waii, Inc.
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pydantic==1.10.12
+
 # Waii Python SDK Documentation
 
 The `waii-sdk-py` is a Python library that allows you to interact with the Waii API. It provides a powerful SQL and AI capability to your Python applications. 
 
 ## Installation
 
 To install the `waii-sdk-py`, you can use pip:
@@ -196,18 +213,21 @@
       - `summary`: generated description of the schema 
       - `common_questions`: list of generated common questions
       - `common_tables`: list of common tables used in the schema
       - `tables`: all tables belong to the schema
         - `name`: Name of the table
         - `columns`: List of columns 
           - `name`: Name of the column 
-          - `type`: Type of the column 
+          - `type`: Type of the column
+          - `description`: Auto generated description of the column
         - `comment`: Comment of the table (fetched from underlying database) 
         - `last_altered_time`: Last altered time of the table 
-        - `refs`: List of referential constraints 
+        - `refs`: List of referential constraints
+        - `inferred_refs`: List of auto-inferred referential constraints
+        - `inferred_constraints`: List of auto-inferred constraints (pks, etc.)
         - `description`: Auto generated table description
 
 Waii automatically generate table/schema descriptions when you add them, you can fetch them by using `description` field of table and schema from `get_catalogs` method.
 
 Description of table looks like: 
 
 ```
@@ -226,15 +246,15 @@
 ## Query
 
 The `Query` module contains methods related to SQL query handling. 
 **Important:** You need to activate the database connection first before using the methods in this module. Otherwise you may trying to generate query from a wrong database.
 
 Here are some of its methods:
 
-### Generate
+### Generate Query
 
 ```python
 Query.generate(params: QueryGenerationRequest) -> GeneratedQuery
 ```
 
 This method generates a SQL query based on the provided parameters.
 
@@ -293,14 +313,33 @@
 - `query`: The generated query text
 - `tables`: Tables used in the generated query
 - `semantic_context`: Semantic context applied to the generated query
 - `detailed_steps`: Detailed steps of how the query work (in natural language)
 - `what_changed`: If you do a tweak, it will tell you what changed in the query
 - `compilation_error`: If there is any compilation error, it will show here. (Waii will try to fix the compilation error automatically, but if it tried multiple times and still cannot fix it, it will show here)
 
+### Generate Question
+
+You can also generate questions based on your database schema, which can be useful when you want to show to your user what kind of questions can be asked to the database.
+
+```python
+>>> Query.generate_question(GenerateQuestionRequest(schema_name='PUBLIC',
+                                                    n_questions=10,
+                                                    complexity=GeneratedQuestionComplexity.hard))
+```
+
+Parameter fields:
+- `schema_name`: The schema name you want to generate questions. This is must be specified.
+- `n_questions`: Number of questions you want to generate. Default is 10. You can choose a number between 1 to 30. 
+- `complexity`: Complexity of the questions you want to generate. Default is `GeneratedQuestionComplexity.hard`. You can choose `easy`, `medium`, `hard`.
+
+Output `GenerateQuestionResponse`, fields:
+- `questions`: List of generated questions. For each question it has `question` (string content of the question), and `complexity` (complexity of the question)
+
+
 ### Transcode
 
 ```python
 >>> WAII.Query.transcode(TranscodeQueryRequest(source_dialect="postgres", source_query="select ...;", target_dialect="snowflake", ask="..."))
 ```
 
 Parameter fields:
@@ -309,16 +348,14 @@
 - `source_query`: The source query you want to transcode
 - `target_dialect`: The dialect of the target query, such as `snowflake`, `postgresql`, `mongodb`
 - `ask`: The intructions you want to ask Waii to add when transcode the query, such as `place tables under schema1`. It is optional.
 
 
 #### `Query.transcode` returns `GeneratedQuery` object
 
-
-
 ### Run a query (sync)
 
 ```python
 Query.run(params: RunQueryRequest) -> GetQueryResultResponse
 ```
 
 Request fields:
@@ -460,15 +497,15 @@
 ```python
 >>> print(WAII.Query.auto_complete(AutoCompleteRequest(text='select from', cursor_offset=11, max_output_tokens=50)))
 
 text='WAII.WORLD.CITY WHERE POPULATION > 1000000'
 ```
 
 
-#### Analyze Performance
+#### Analyze Performance (Experimental)
 
 Note: this feature currently only support Snowflake
 
 ```python
 Query.analyze_performance(params: QueryPerformanceRequest) -> QueryPerformanceResponse
 ```
```

### Comparing `waii-sdk-py-1.9.0/setup.cfg` & `waii-sdk-py-1.9.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = waii-sdk-py
-version = 1.9.0
+version = 1.9.1
 description = Provides access to the Waii APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Waii, Inc.
 license = Apache License 2.0
 url = http://www.waii.ai
 classifiers =
```

### Comparing `waii-sdk-py-1.9.0/tests/database_tests.py` & `waii-sdk-py-1.9.1/tests/database_tests.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/tests/history_tests.py` & `waii-sdk-py-1.9.1/tests/history_tests.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/tests/query_tests.py` & `waii-sdk-py-1.9.1/tests/query_tests.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/tests/semantic_context_tests.py` & `waii-sdk-py-1.9.1/tests/semantic_context_tests.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/database/database.py` & `waii-sdk-py-1.9.1/waii_sdk_py/database/database.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/history/history.py` & `waii-sdk-py-1.9.1/waii_sdk_py/history/history.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/query/query.py` & `waii-sdk-py-1.9.1/waii_sdk_py/query/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     n_questions: Optional[int] = 10  # number of questions to generate
     complexity: Optional[GeneratedQuestionComplexity] = GeneratedQuestionComplexity.hard
 
 
 class GeneratedQuestion(BaseModel):
     question: str
     complexity: GeneratedQuestionComplexity
+    tables: Optional[List[TableName]] # tables used in the question
 
 
 class GenerateQuestionResponse(BaseModel):
     questions: Optional[List[GeneratedQuestion]]
 
 
 def show_progress(func):
```

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/semantic_context/semantic_context.py` & `waii-sdk-py-1.9.1/waii_sdk_py/semantic_context/semantic_context.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/waii_http_client/waii_http_client.py` & `waii-sdk-py-1.9.1/waii_sdk_py/waii_http_client/waii_http_client.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py/waii_sdk_py.py` & `waii-sdk-py-1.9.1/waii_sdk_py/waii_sdk_py.py`

 * *Files identical despite different names*

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py.egg-info/PKG-INFO` & `waii-sdk-py-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: waii-sdk-py
-Version: 1.9.0
-Summary: Provides access to the Waii APIs
-Home-page: http://www.waii.ai
-Author: Waii, Inc.
-License: Apache License 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: pydantic==1.10.12
-
 # Waii Python SDK Documentation
 
 The `waii-sdk-py` is a Python library that allows you to interact with the Waii API. It provides a powerful SQL and AI capability to your Python applications. 
 
 ## Installation
 
 To install the `waii-sdk-py`, you can use pip:
@@ -213,18 +196,21 @@
       - `summary`: generated description of the schema 
       - `common_questions`: list of generated common questions
       - `common_tables`: list of common tables used in the schema
       - `tables`: all tables belong to the schema
         - `name`: Name of the table
         - `columns`: List of columns 
           - `name`: Name of the column 
-          - `type`: Type of the column 
+          - `type`: Type of the column
+          - `description`: Auto generated description of the column
         - `comment`: Comment of the table (fetched from underlying database) 
         - `last_altered_time`: Last altered time of the table 
-        - `refs`: List of referential constraints 
+        - `refs`: List of referential constraints
+        - `inferred_refs`: List of auto-inferred referential constraints
+        - `inferred_constraints`: List of auto-inferred constraints (pks, etc.)
         - `description`: Auto generated table description
 
 Waii automatically generate table/schema descriptions when you add them, you can fetch them by using `description` field of table and schema from `get_catalogs` method.
 
 Description of table looks like: 
 
 ```
@@ -243,15 +229,15 @@
 ## Query
 
 The `Query` module contains methods related to SQL query handling. 
 **Important:** You need to activate the database connection first before using the methods in this module. Otherwise you may trying to generate query from a wrong database.
 
 Here are some of its methods:
 
-### Generate
+### Generate Query
 
 ```python
 Query.generate(params: QueryGenerationRequest) -> GeneratedQuery
 ```
 
 This method generates a SQL query based on the provided parameters.
 
@@ -310,14 +296,33 @@
 - `query`: The generated query text
 - `tables`: Tables used in the generated query
 - `semantic_context`: Semantic context applied to the generated query
 - `detailed_steps`: Detailed steps of how the query work (in natural language)
 - `what_changed`: If you do a tweak, it will tell you what changed in the query
 - `compilation_error`: If there is any compilation error, it will show here. (Waii will try to fix the compilation error automatically, but if it tried multiple times and still cannot fix it, it will show here)
 
+### Generate Question
+
+You can also generate questions based on your database schema, which can be useful when you want to show to your user what kind of questions can be asked to the database.
+
+```python
+>>> Query.generate_question(GenerateQuestionRequest(schema_name='PUBLIC',
+                                                    n_questions=10,
+                                                    complexity=GeneratedQuestionComplexity.hard))
+```
+
+Parameter fields:
+- `schema_name`: The schema name you want to generate questions. This is must be specified.
+- `n_questions`: Number of questions you want to generate. Default is 10. You can choose a number between 1 to 30. 
+- `complexity`: Complexity of the questions you want to generate. Default is `GeneratedQuestionComplexity.hard`. You can choose `easy`, `medium`, `hard`.
+
+Output `GenerateQuestionResponse`, fields:
+- `questions`: List of generated questions. For each question it has `question` (string content of the question), and `complexity` (complexity of the question)
+
+
 ### Transcode
 
 ```python
 >>> WAII.Query.transcode(TranscodeQueryRequest(source_dialect="postgres", source_query="select ...;", target_dialect="snowflake", ask="..."))
 ```
 
 Parameter fields:
@@ -326,16 +331,14 @@
 - `source_query`: The source query you want to transcode
 - `target_dialect`: The dialect of the target query, such as `snowflake`, `postgresql`, `mongodb`
 - `ask`: The intructions you want to ask Waii to add when transcode the query, such as `place tables under schema1`. It is optional.
 
 
 #### `Query.transcode` returns `GeneratedQuery` object
 
-
-
 ### Run a query (sync)
 
 ```python
 Query.run(params: RunQueryRequest) -> GetQueryResultResponse
 ```
 
 Request fields:
@@ -477,15 +480,15 @@
 ```python
 >>> print(WAII.Query.auto_complete(AutoCompleteRequest(text='select from', cursor_offset=11, max_output_tokens=50)))
 
 text='WAII.WORLD.CITY WHERE POPULATION > 1000000'
 ```
 
 
-#### Analyze Performance
+#### Analyze Performance (Experimental)
 
 Note: this feature currently only support Snowflake
 
 ```python
 Query.analyze_performance(params: QueryPerformanceRequest) -> QueryPerformanceResponse
 ```
```

### Comparing `waii-sdk-py-1.9.0/waii_sdk_py.egg-info/SOURCES.txt` & `waii-sdk-py-1.9.1/waii_sdk_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

