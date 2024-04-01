# Comparing `tmp/dagster_ext-0.1.0.tar.gz` & `tmp/dagster_ext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_ext-0.1.0.tar", max compression
+gzip compressed data, was "dagster_ext-0.1.1.tar", max compression
```

## Comparing `dagster_ext-0.1.0.tar` & `dagster_ext-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     2094 2022-12-30 14:45:05.525113 dagster_ext-0.1.0/README.md
--rw-r--r--   0        0        0       33 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/dagster_ext/__init__.py
--rw-r--r--   0        0        0    10588 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/dagster_ext/extension.py
--rw-r--r--   0        0        0     3311 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/dagster_ext/main.py
--rw-r--r--   0        0        0     1079 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/dagster_ext/pass_through.py
--rw-r--r--   0        0        0       95 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/files_dagster_ext/dagster/cookiecutter.json
--rw-r--r--   0        0        0     1800 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/files_dagster_ext/dagster/{{ cookiecutter.project_name }}/repository.py
--rw-r--r--   0        0        0       74 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/files_dagster_ext/github/cookiecutter.json
--rw-r--r--   0        0        0       45 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/meltano/edk/__init__.py
--rw-r--r--   0        0        0     4458 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/meltano/edk/extension.py
--rw-r--r--   0        0        0     3734 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/meltano/edk/logging.py
--rw-r--r--   0        0        0      904 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/meltano/edk/models.py
--rw-r--r--   0        0        0     5290 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/meltano/edk/process.py
--rw-r--r--   0        0        0     1286 2022-12-30 14:45:05.529113 dagster_ext-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 dagster_ext-0.1.0/setup.py
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 dagster_ext-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1024 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/README.md
+-rw-r--r--   0        0        0       33 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/dagster_ext/__init__.py
+-rw-r--r--   0        0        0    10588 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/dagster_ext/extension.py
+-rw-r--r--   0        0        0     3311 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/dagster_ext/main.py
+-rw-r--r--   0        0        0     1079 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/dagster_ext/pass_through.py
+-rw-r--r--   0        0        0       95 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/files_dagster_ext/dagster/cookiecutter.json
+-rw-r--r--   0        0        0     1800 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/files_dagster_ext/dagster/{{ cookiecutter.project_name }}/repository.py
+-rw-r--r--   0        0        0       74 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/files_dagster_ext/github/cookiecutter.json
+-rw-r--r--   0        0        0       45 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/meltano/edk/__init__.py
+-rw-r--r--   0        0        0     4458 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/meltano/edk/extension.py
+-rw-r--r--   0        0        0     3734 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/meltano/edk/logging.py
+-rw-r--r--   0        0        0      904 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/meltano/edk/models.py
+-rw-r--r--   0        0        0     5290 2024-04-01 14:23:19.953875 dagster_ext-0.1.1/meltano/edk/process.py
+-rw-r--r--   0        0        0     1286 2024-04-01 14:23:19.957875 dagster_ext-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 dagster_ext-0.1.1/PKG-INFO
```

### Comparing `dagster_ext-0.1.0/dagster_ext/extension.py` & `dagster_ext-0.1.1/dagster_ext/extension.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/dagster_ext/main.py` & `dagster_ext-0.1.1/dagster_ext/main.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/dagster_ext/pass_through.py` & `dagster_ext-0.1.1/dagster_ext/pass_through.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/files_dagster_ext/dagster/{{ cookiecutter.project_name }}/repository.py` & `dagster_ext-0.1.1/files_dagster_ext/dagster/{{ cookiecutter.project_name }}/repository.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/meltano/edk/extension.py` & `dagster_ext-0.1.1/meltano/edk/extension.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/meltano/edk/logging.py` & `dagster_ext-0.1.1/meltano/edk/logging.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/meltano/edk/models.py` & `dagster_ext-0.1.1/meltano/edk/models.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/meltano/edk/process.py` & `dagster_ext-0.1.1/meltano/edk/process.py`

 * *Files identical despite different names*

### Comparing `dagster_ext-0.1.0/pyproject.toml` & `dagster_ext-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "dagster-ext"
-version = "0.1.0"
+version = "0.1.1"
 description = "`dagster-ext` is a Meltano utility extension."
 authors = ["Jules Huisman"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "dagster_ext" },
     { include = "files_dagster_ext" },
     { include = "meltano" }
 ]
 include = [
    "files_dagster_ext"
 ]
 
 [tool.poetry.dependencies]
-python = "<3.11,>=3.8"
+python = "<3.13,>=3.8"
 click = "^8.1.3"
-typer = "^0.6.1"
+typer = "^0.9.0"
 dagit = ">=1.0"
 dagster = ">=1.0"
 dagster-dbt = ">=0.16"
 cookiecutter = "^2.1.1"
 rich = "^12.5.1"
 dagster-meltano = ">=1.0.0"
 # Dependencies from Meltano EDK, remove when dependency fixed
```

