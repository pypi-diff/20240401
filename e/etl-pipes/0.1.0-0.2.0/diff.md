# Comparing `tmp/etl_pipes-0.1.0.tar.gz` & `tmp/etl_pipes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipes-0.1.0.tar", max compression
+gzip compressed data, was "etl_pipes-0.2.0.tar", max compression
```

## Comparing `etl_pipes-0.1.0.tar` & `etl_pipes-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.1.0/etl_pipes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.1.0/etl_pipes/actors/__init__.py
--rw-r--r--   0        0        0     2049 2024-03-31 18:15:41.761652 etl_pipes-0.1.0/etl_pipes/actors/actor.py
--rw-r--r--   0        0        0     8182 2024-03-31 18:15:41.762013 etl_pipes-0.1.0/etl_pipes/actors/actor_system.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.1.0/etl_pipes/actors/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.1.0/etl_pipes/actors/common/logging.py
--rw-r--r--   0        0        0     1434 2024-03-31 18:15:41.762619 etl_pipes-0.1.0/etl_pipes/actors/common/types.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.1.0/etl_pipes/common/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.1.0/etl_pipes/common/utils/__init__.py
--rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.1.0/etl_pipes/common/utils/type_hints.py
--rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.1.0/etl_pipes/domain/__init__.py
--rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.1.0/etl_pipes/domain/types.py
--rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.1.0/etl_pipes/pipes/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-30 18:10:45.704990 etl_pipes-0.1.0/etl_pipes/pipes/base_pipe.py
--rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.1.0/etl_pipes/pipes/broadcast_parallel.py
--rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.1.0/etl_pipes/pipes/map_reduce.py
--rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.1.0/etl_pipes/pipes/maybe.py
--rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.1.0/etl_pipes/pipes/parallel.py
--rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.1.0/etl_pipes/pipes/pipeline/__init__.py
--rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.1.0/etl_pipes/pipes/pipeline/exceptions.py
--rw-r--r--   0        0        0     3960 2024-03-30 18:10:45.707062 etl_pipes-0.1.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
--rw-r--r--   0        0        0     1750 2024-03-30 18:10:45.707479 etl_pipes-0.1.0/etl_pipes/pipes/pipeline/pipeline.py
--rw-r--r--   0        0        0     1334 2024-03-31 18:17:33.564013 etl_pipes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7989 1970-01-01 00:00:00.000000 etl_pipes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.2.0/etl_pipes/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.2.0/etl_pipes/actors/__init__.py
+-rw-r--r--   0        0        0     2049 2024-03-31 18:15:41.761652 etl_pipes-0.2.0/etl_pipes/actors/actor.py
+-rw-r--r--   0        0        0     8182 2024-03-31 18:15:41.762013 etl_pipes-0.2.0/etl_pipes/actors/actor_system.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.2.0/etl_pipes/actors/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.2.0/etl_pipes/actors/common/logging.py
+-rw-r--r--   0        0        0     1434 2024-03-31 18:15:41.762619 etl_pipes-0.2.0/etl_pipes/actors/common/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.2.0/etl_pipes/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.2.0/etl_pipes/common/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.2.0/etl_pipes/common/utils/type_hints.py
+-rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.2.0/etl_pipes/domain/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.2.0/etl_pipes/domain/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.2.0/etl_pipes/pipes/__init__.py
+-rw-r--r--   0        0        0     2193 2024-03-30 18:10:45.704990 etl_pipes-0.2.0/etl_pipes/pipes/base_pipe.py
+-rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.2.0/etl_pipes/pipes/broadcast_parallel.py
+-rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.2.0/etl_pipes/pipes/map_reduce.py
+-rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.2.0/etl_pipes/pipes/maybe.py
+-rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.2.0/etl_pipes/pipes/parallel.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.2.0/etl_pipes/pipes/pipeline/__init__.py
+-rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.2.0/etl_pipes/pipes/pipeline/exceptions.py
+-rw-r--r--   0        0        0     3960 2024-03-30 18:10:45.707062 etl_pipes-0.2.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
+-rw-r--r--   0        0        0     1750 2024-03-30 18:10:45.707479 etl_pipes-0.2.0/etl_pipes/pipes/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1334 2024-04-01 10:02:57.236354 etl_pipes-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.2.0/PKG-INFO
```

### Comparing `etl_pipes-0.1.0/README.md` & `etl_pipes-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/actors/actor.py` & `etl_pipes-0.2.0/etl_pipes/actors/actor.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/actors/actor_system.py` & `etl_pipes-0.2.0/etl_pipes/actors/actor_system.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/actors/common/logging.py` & `etl_pipes-0.2.0/etl_pipes/actors/common/logging.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/actors/common/types.py` & `etl_pipes-0.2.0/etl_pipes/actors/common/types.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/base_pipe.py` & `etl_pipes-0.2.0/etl_pipes/pipes/base_pipe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/map_reduce.py` & `etl_pipes-0.2.0/etl_pipes/pipes/map_reduce.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/maybe.py` & `etl_pipes-0.2.0/etl_pipes/pipes/maybe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/parallel.py` & `etl_pipes-0.2.0/etl_pipes/pipes/parallel.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/pipeline/exceptions.py` & `etl_pipes-0.2.0/etl_pipes/pipes/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py` & `etl_pipes-0.2.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/etl_pipes/pipes/pipeline/pipeline.py` & `etl_pipes-0.2.0/etl_pipes/pipes/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.1.0/pyproject.toml` & `etl_pipes-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "etl-pipes"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Tikhon Zaikin <th@thevhs.club>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pip = "^23.2"
-pytest-asyncio = "^0.21.1"
-fastapi = "^0.103.1"
-unicorn = {extras = ["standard"], version = "^2.0.1.post1"}
-sqlalchemy = { version = "^2.0.21", extras = ["mypy"] }
-uvicorn = "^0.23.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.277"
 black = "^23.3.0"
 mypy = "^1.4.1"
 pytest = "^7.4.0"
 pre-commit = "^3.4.0"
 coverage = "^7.3.1"
+pytest-asyncio = "^0.21.1"
+fastapi = "^0.103.1"
+unicorn = {extras = ["standard"], version = "^2.0.1.post1"}
+sqlalchemy = { version = "^2.0.21", extras = ["mypy"] }
+uvicorn = "^0.23.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `etl_pipes-0.1.0/PKG-INFO` & `etl_pipes-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 Metadata-Version: 2.1
 Name: etl-pipes
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Tikhon Zaikin
 Author-email: th@thevhs.club
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.103.1,<0.104.0)
 Requires-Dist: pip (>=23.2,<24.0)
-Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
-Requires-Dist: sqlalchemy[mypy] (>=2.0.21,<3.0.0)
-Requires-Dist: unicorn[standard] (>=2.0.1.post1,<3.0.0)
-Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Description-Content-Type: text/markdown
 
 # Pypelines
 
 ## Description
 
 Pypelines is a Python library for creating flow-based programming pipelines.
```

