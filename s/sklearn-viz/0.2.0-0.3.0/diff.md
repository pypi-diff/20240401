# Comparing `tmp/sklearn_viz-0.2.0.tar.gz` & `tmp/sklearn_viz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.2.0.tar", max compression
+gzip compressed data, was "sklearn_viz-0.3.0.tar", max compression
```

## Comparing `sklearn_viz-0.2.0.tar` & `sklearn_viz-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.2.0/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.2.0/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     7873 2023-10-10 12:02:36.000498 sklearn_viz-0.2.0/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.2.0/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.2.0/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.2.0/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.2.0/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1469 2023-11-15 12:38:46.317925 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    14089 2023-11-18 09:09:23.171088 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      318 2023-11-12 09:19:44.575578 sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.2.0/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.2.0/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.2.0/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.2.0/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.2.0/LICENSE
--rw-r--r--   0        0        0      819 2024-03-30 11:59:00.710958 sklearn_viz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.2.0/README.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.3.0/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.3.0/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     7873 2023-10-10 12:02:36.000498 sklearn_viz-0.3.0/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.3.0/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.3.0/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.3.0/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.3.0/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1469 2023-11-15 12:38:46.317925 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    22155 2024-04-01 11:49:20.249010 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      318 2023-11-12 09:19:44.575578 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.3.0/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.3.0/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.3.0/LICENSE
+-rw-r--r--   0        0        0      819 2024-04-01 11:42:33.970861 sklearn_viz-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.3.0/README.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.3.0/PKG-INFO
```

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.3.0/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/LICENSE` & `sklearn_viz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.2.0/pyproject.toml` & `sklearn_viz-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.2.0/PKG-INFO` & `sklearn_viz-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

