# Comparing `tmp/dagster_meltano-1.5.3.tar.gz` & `tmp/dagster_meltano-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_meltano-1.5.3.tar", max compression
+gzip compressed data, was "dagster_meltano-1.5.4.tar", max compression
```

## Comparing `dagster_meltano-1.5.3.tar` & `dagster_meltano-1.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/LICENSE
--rw-r--r--   0        0        0     2103 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/README.md
--rw-r--r--   0        0        0      313 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/__init__.py
--rw-r--r--   0        0        0       47 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/exceptions.py
--rw-r--r--   0        0        0     2348 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/generation.py
--rw-r--r--   0        0        0     1856 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/job.py
--rw-r--r--   0        0        0      592 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/logging.yaml
--rw-r--r--   0        0        0     5855 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/meltano_resource.py
--rw-r--r--   0        0        0     3978 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/ops.py
--rw-r--r--   0        0        0      859 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/schedule.py
--rw-r--r--   0        0        0     1029 2023-10-16 10:02:56.980047 dagster_meltano-1.5.3/dagster_meltano/utils.py
--rw-r--r--   0        0        0      674 2023-10-16 10:02:56.984047 dagster_meltano-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 dagster_meltano-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/LICENSE
+-rw-r--r--   0        0        0     2103 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/README.md
+-rw-r--r--   0        0        0      313 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/exceptions.py
+-rw-r--r--   0        0        0     2348 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/generation.py
+-rw-r--r--   0        0        0     1856 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/job.py
+-rw-r--r--   0        0        0      592 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/logging.yaml
+-rw-r--r--   0        0        0     5855 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/meltano_resource.py
+-rw-r--r--   0        0        0     3978 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/ops.py
+-rw-r--r--   0        0        0      859 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/schedule.py
+-rw-r--r--   0        0        0     1029 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/dagster_meltano/utils.py
+-rw-r--r--   0        0        0      674 2024-04-01 18:05:46.763949 dagster_meltano-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2716 1970-01-01 00:00:00.000000 dagster_meltano-1.5.4/PKG-INFO
```

### Comparing `dagster_meltano-1.5.3/LICENSE` & `dagster_meltano-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/README.md` & `dagster_meltano-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/generation.py` & `dagster_meltano-1.5.4/dagster_meltano/generation.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/job.py` & `dagster_meltano-1.5.4/dagster_meltano/job.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/logging.yaml` & `dagster_meltano-1.5.4/dagster_meltano/logging.yaml`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/meltano_resource.py` & `dagster_meltano-1.5.4/dagster_meltano/meltano_resource.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/ops.py` & `dagster_meltano-1.5.4/dagster_meltano/ops.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/schedule.py` & `dagster_meltano-1.5.4/dagster_meltano/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/dagster_meltano/utils.py` & `dagster_meltano-1.5.4/dagster_meltano/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_meltano-1.5.3/pyproject.toml` & `dagster_meltano-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "dagster-meltano"
-version = "1.5.3"
+version = "1.5.4"
 description = "A dagster plugin that allows you to run your Meltano project inside Dagster."
 authors = ["Quantile Development"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [
     { include = "dagster_meltano" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8,<3.13"
 dagster = ">=1.3,<2"
 dagster-shell = ">=0,<1"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.15.9"
 pytest = "^7.2.0"
 black = "^23.3.0"
```

### Comparing `dagster_meltano-1.5.3/PKG-INFO` & `dagster_meltano-1.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dagster-meltano
-Version: 1.5.3
+Version: 1.5.4
 Summary: A dagster plugin that allows you to run your Meltano project inside Dagster.
 License: Apache 2.0
 Author: Quantile Development
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dagster (>=1.3,<2)
 Requires-Dist: dagster-shell (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Dagster-meltano
 
 A dagster plugin that allows you to run Meltano using Dagster.
```

