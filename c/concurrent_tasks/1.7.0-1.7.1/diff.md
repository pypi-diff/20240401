# Comparing `tmp/concurrent_tasks-1.7.0.tar.gz` & `tmp/concurrent_tasks-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concurrent_tasks-1.7.0.tar", max compression
+gzip compressed data, was "concurrent_tasks-1.7.1.tar", max compression
```

## Comparing `concurrent_tasks-1.7.0.tar` & `concurrent_tasks-1.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/LICENSE
--rw-r--r--   0        0        0     6063 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/README.md
--rw-r--r--   0        0        0      518 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/__init__.py
--rw-r--r--   0        0        0     1458 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/background.py
--rw-r--r--   0        0        0     3551 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/exception_handler.py
--rw-r--r--   0        0        0     1081 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/periodic.py
--rw-r--r--   0        0        0        0 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/py.typed
--rw-r--r--   0        0        0     3097 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/restartable.py
--rw-r--r--   0        0        0     4208 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/thread_safe_pool.py
--rw-r--r--   0        0        0      228 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/__init__.py
--rw-r--r--   0        0        0     1696 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/aio.py
--rw-r--r--   0        0        0     4655 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/base.py
--rw-r--r--   0        0        0     1638 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/blocking.py
--rw-r--r--   0        0        0      912 2024-02-12 15:55:55.046606 concurrent_tasks-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 concurrent_tasks-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/LICENSE
+-rw-r--r--   0        0        0     6078 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/README.md
+-rw-r--r--   0        0        0      518 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/__init__.py
+-rw-r--r--   0        0        0     1458 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/background.py
+-rw-r--r--   0        0        0     3551 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/exception_handler.py
+-rw-r--r--   0        0        0     1081 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/periodic.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/py.typed
+-rw-r--r--   0        0        0     3097 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/restartable.py
+-rw-r--r--   0        0        0     4208 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/thread_safe_pool.py
+-rw-r--r--   0        0        0      228 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/__init__.py
+-rw-r--r--   0        0        0     1696 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/aio.py
+-rw-r--r--   0        0        0     4655 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/base.py
+-rw-r--r--   0        0        0     1638 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/blocking.py
+-rw-r--r--   0        0        0      932 2024-04-01 15:44:46.582647 concurrent_tasks-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6852 1970-01-01 00:00:00.000000 concurrent_tasks-1.7.1/PKG-INFO
```

### Comparing `concurrent_tasks-1.7.0/LICENSE` & `concurrent_tasks-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/README.md` & `concurrent_tasks-1.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # asyncio-concurrent-tasks
 
-[![tests](https://github.com/gpajot/asyncio-concurrent-tasks/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/asyncio-concurrent-tasks/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
+[![tests](https://github.com/gpajot/asyncio-concurrent-tasks/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/asyncio-concurrent-tasks/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
 [![version](https://img.shields.io/pypi/v/concurrent_tasks?label=stable)](https://pypi.org/project/concurrent_tasks/)
 [![python](https://img.shields.io/pypi/pyversions/concurrent_tasks)](https://pypi.org/project/concurrent_tasks/)
 
 Tooling to run asyncio tasks.
 - [Background task](#background-task)
 - [Periodic task](#periodic-task)
 - [Thread safe task pool](#thread-safe-task-pool)
```

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/__init__.py` & `concurrent_tasks-1.7.1/concurrent_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/background.py` & `concurrent_tasks-1.7.1/concurrent_tasks/background.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/exception_handler.py` & `concurrent_tasks-1.7.1/concurrent_tasks/exception_handler.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/periodic.py` & `concurrent_tasks-1.7.1/concurrent_tasks/periodic.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/restartable.py` & `concurrent_tasks-1.7.1/concurrent_tasks/restartable.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/thread_safe_pool.py` & `concurrent_tasks-1.7.1/concurrent_tasks/thread_safe_pool.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/aio.py` & `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/aio.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/base.py` & `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/base.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/concurrent_tasks/threaded_pool/blocking.py` & `concurrent_tasks-1.7.1/concurrent_tasks/threaded_pool/blocking.py`

 * *Files identical despite different names*

### Comparing `concurrent_tasks-1.7.0/pyproject.toml` & `concurrent_tasks-1.7.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "concurrent_tasks"
-version = "1.7.0"
+version = "1.7.1"
 description = "Tools to run asyncio tasks concurrently."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/asyncio-concurrent-tasks"
 include = ["concurrent_tasks/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+typing-extensions = ">=4.10"
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.0.0"
+pytest = "==8.1.1"
 pytest-asyncio = "==0.21.1"
-pytest-mock = "==3.12.0"
-ruff = "==0.2.1"
-mypy = "==1.8.0"
-black = "==24.1.1"
+pytest-mock = "==3.14.0"
+ruff = "==0.3.4"
+mypy = "==1.9.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
@@ -29,13 +29,13 @@
 install_types = true
 non_interactive = true
 check_untyped_defs = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["A", "B", "E", "F", "I", "PT"]
 ignore = ["E501"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `concurrent_tasks-1.7.0/PKG-INFO` & `concurrent_tasks-1.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: concurrent_tasks
-Version: 1.7.0
+Version: 1.7.1
 Summary: Tools to run asyncio tasks concurrently.
 Home-page: https://github.com/gpajot/asyncio-concurrent-tasks
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: typing-extensions (>=4.10)
 Project-URL: Repository, https://github.com/gpajot/asyncio-concurrent-tasks
 Description-Content-Type: text/markdown
 
 # asyncio-concurrent-tasks
 
-[![tests](https://github.com/gpajot/asyncio-concurrent-tasks/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/asyncio-concurrent-tasks/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
+[![tests](https://github.com/gpajot/asyncio-concurrent-tasks/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/asyncio-concurrent-tasks/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
 [![version](https://img.shields.io/pypi/v/concurrent_tasks?label=stable)](https://pypi.org/project/concurrent_tasks/)
 [![python](https://img.shields.io/pypi/pyversions/concurrent_tasks)](https://pypi.org/project/concurrent_tasks/)
 
 Tooling to run asyncio tasks.
 - [Background task](#background-task)
 - [Periodic task](#periodic-task)
 - [Thread safe task pool](#thread-safe-task-pool)
```

