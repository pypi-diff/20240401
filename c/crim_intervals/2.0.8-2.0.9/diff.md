# Comparing `tmp/crim_intervals-2.0.8.tar.gz` & `tmp/crim_intervals-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crim_intervals-2.0.8.tar", max compression
+gzip compressed data, was "crim_intervals-2.0.9.tar", max compression
```

## Comparing `crim_intervals-2.0.8.tar` & `crim_intervals-2.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      123 2023-08-31 00:09:26.523573 crim_intervals-2.0.8/intervals/__init__.py
--rw-r--r--   0        0        0     8814 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/data/cadences/CVFLabels.csv
--rw-r--r--   0        0        0     2014 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/data/cadences/cadenceLabels.csv
--rw-r--r--   0        0        0     8781 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/data/cadences/groundTruth.csv
--rw-r--r--   0        0        0     6301 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/main.py
--rw-r--r--   0        0        0   199164 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/main_objs.py
--rw-r--r--   0        0        0     2150 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/networks.py
--rw-r--r--   0        0        0    22277 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/visualizations.py
--rw-r--r--   0        0        0    24585 2023-08-31 00:09:03.246744 crim_intervals-2.0.8/intervals/visualizations_demo.py
--rw-r--r--   0        0        0     1255 2023-08-31 00:09:26.511572 crim_intervals-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 crim_intervals-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    12352 2023-08-31 00:18:11.213934 crim_intervals-2.0.9/README.md
+-rw-r--r--   0        0        0      123 2023-08-31 00:18:11.209934 crim_intervals-2.0.9/intervals/__init__.py
+-rw-r--r--   0        0        0     8814 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/data/cadences/CVFLabels.csv
+-rw-r--r--   0        0        0     2014 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/data/cadences/cadenceLabels.csv
+-rw-r--r--   0        0        0     8781 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/data/cadences/groundTruth.csv
+-rw-r--r--   0        0        0     6301 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/main.py
+-rw-r--r--   0        0        0   199164 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/main_objs.py
+-rw-r--r--   0        0        0     2150 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/networks.py
+-rw-r--r--   0        0        0    22277 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/visualizations.py
+-rw-r--r--   0        0        0    24585 2023-08-31 00:17:50.789871 crim_intervals-2.0.9/intervals/visualizations_demo.py
+-rw-r--r--   0        0        0     1276 2023-08-31 00:18:11.193934 crim_intervals-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13769 1970-01-01 00:00:00.000000 crim_intervals-2.0.9/PKG-INFO
```

### Comparing `crim_intervals-2.0.8/intervals/data/cadences/CVFLabels.csv` & `crim_intervals-2.0.9/intervals/data/cadences/CVFLabels.csv`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/data/cadences/cadenceLabels.csv` & `crim_intervals-2.0.9/intervals/data/cadences/cadenceLabels.csv`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/data/cadences/groundTruth.csv` & `crim_intervals-2.0.9/intervals/data/cadences/groundTruth.csv`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/main.py` & `crim_intervals-2.0.9/intervals/main.py`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/main_objs.py` & `crim_intervals-2.0.9/intervals/main_objs.py`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/networks.py` & `crim_intervals-2.0.9/intervals/networks.py`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/visualizations.py` & `crim_intervals-2.0.9/intervals/visualizations.py`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/intervals/visualizations_demo.py` & `crim_intervals-2.0.9/intervals/visualizations_demo.py`

 * *Files identical despite different names*

### Comparing `crim_intervals-2.0.8/pyproject.toml` & `crim_intervals-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "crim_intervals"
-version = "2.0.8"
+version = "2.0.9"
 description = "CRIM intervals package"
+readme = "README.md"
 authors = ["Richard Freedman <rfreedma@haverford.edu>"]
 license = "creative commons"
 packages = [
     { include = "intervals" },
 ]
 
 [tool.poetry.dependencies]
```

