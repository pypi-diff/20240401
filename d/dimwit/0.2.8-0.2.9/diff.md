# Comparing `tmp/dimwit-0.2.8.tar.gz` & `tmp/dimwit-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimwit-0.2.8.tar", max compression
+gzip compressed data, was "dimwit-0.2.9.tar", max compression
```

## Comparing `dimwit-0.2.8.tar` & `dimwit-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      185 2024-01-23 23:54:43.113339 dimwit-0.2.8/README.md
--rw-r--r--   0        0        0      103 2024-03-03 20:36:55.132719 dimwit-0.2.8/dimwit/__init__.py
--rw-r--r--   0        0        0    11508 2024-02-08 14:55:08.179688 dimwit-0.2.8/dimwit/air_pollution.py
--rw-r--r--   0        0        0     7900 2024-03-03 20:35:32.674573 dimwit-0.2.8/dimwit/airflow.py
--rw-r--r--   0        0        0     3175 2024-02-08 14:34:07.801061 dimwit-0.2.8/dimwit/legacy.py
--rw-r--r--   0        0        0    13178 2024-03-03 12:19:27.904147 dimwit-0.2.8/dimwit/main.py
--rw-r--r--   0        0        0      547 2024-03-03 20:38:01.705427 dimwit-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 dimwit-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      185 2024-01-23 23:54:43.113339 dimwit-0.2.9/README.md
+-rw-r--r--   0        0        0      147 2024-03-03 21:16:55.724275 dimwit-0.2.9/dimwit/__init__.py
+-rw-r--r--   0        0        0    11508 2024-02-08 14:55:08.179688 dimwit-0.2.9/dimwit/air_pollution.py
+-rw-r--r--   0        0        0     7900 2024-03-03 20:35:32.674573 dimwit-0.2.9/dimwit/airflow.py
+-rw-r--r--   0        0        0     3175 2024-02-08 14:34:07.801061 dimwit-0.2.9/dimwit/legacy.py
+-rw-r--r--   0        0        0    13178 2024-03-03 12:19:27.904147 dimwit-0.2.9/dimwit/main.py
+-rw-r--r--   0        0        0     5765 2024-03-03 21:16:37.676404 dimwit-0.2.9/dimwit/pomodoro.py
+-rw-r--r--   0        0        0     1959 2024-03-03 21:04:05.081950 dimwit-0.2.9/dimwit/weight.py
+-rw-r--r--   0        0        0      547 2024-03-03 21:04:28.703722 dimwit-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 dimwit-0.2.9/PKG-INFO
```

### Comparing `dimwit-0.2.8/dimwit/air_pollution.py` & `dimwit-0.2.9/dimwit/air_pollution.py`

 * *Files identical despite different names*

### Comparing `dimwit-0.2.8/dimwit/airflow.py` & `dimwit-0.2.9/dimwit/airflow.py`

 * *Files identical despite different names*

### Comparing `dimwit-0.2.8/dimwit/legacy.py` & `dimwit-0.2.9/dimwit/legacy.py`

 * *Files identical despite different names*

### Comparing `dimwit-0.2.8/dimwit/main.py` & `dimwit-0.2.9/dimwit/main.py`

 * *Files identical despite different names*

### Comparing `dimwit-0.2.8/pyproject.toml` & `dimwit-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dimwit"
-version = "0.2.8"
+version = "0.2.9"
 description = "A package containing various functions and classes for fetching, transforming, and visualising data for personal metrics."
 authors = ["Daniel Soutar <danielsoutar144@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/danielsoutar/dimwit"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dimwit-0.2.8/PKG-INFO` & `dimwit-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimwit
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package containing various functions and classes for fetching, transforming, and visualising data for personal metrics.
 Home-page: https://github.com/danielsoutar/dimwit
 Author: Daniel Soutar
 Author-email: danielsoutar144@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

