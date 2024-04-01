# Comparing `tmp/datasetlib-0.1.7.1.tar.gz` & `tmp/datasetlib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasetlib-0.1.7.1.tar", last modified: Wed Jan  3 14:04:49 2024, max compression
+gzip compressed data, was "datasetlib-0.2.tar", last modified: Mon Apr  1 10:42:09 2024, max compression
```

## Comparing `datasetlib-0.1.7.1.tar` & `datasetlib-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 neutro2   (1000) neutro2   (1000)        0 2024-01-03 14:04:49.733262 datasetlib-0.1.7.1/
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     1074 2023-12-22 18:23:29.000000 datasetlib-0.1.7.1/LICENSE
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     2173 2024-01-03 14:04:49.733262 datasetlib-0.1.7.1/PKG-INFO
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     1892 2023-12-22 18:41:27.000000 datasetlib-0.1.7.1/README.md
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     1046 2024-01-03 14:04:27.000000 datasetlib-0.1.7.1/pyproject.toml
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)       38 2024-01-03 14:04:49.733262 datasetlib-0.1.7.1/setup.cfg
-drwxr-xr-x   0 neutro2   (1000) neutro2   (1000)        0 2024-01-03 14:04:49.723262 datasetlib-0.1.7.1/src/
-drwxr-xr-x   0 neutro2   (1000) neutro2   (1000)        0 2024-01-03 14:04:49.723262 datasetlib-0.1.7.1/src/datasetlib/
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)      627 2024-01-03 14:04:16.000000 datasetlib-0.1.7.1/src/datasetlib/__init__.py
-drwxr-xr-x   0 neutro2   (1000) neutro2   (1000)        0 2024-01-03 14:04:49.733262 datasetlib-0.1.7.1/src/datasetlib/datasets/
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)   294994 2023-12-22 18:23:29.000000 datasetlib-0.1.7.1/src/datasetlib/datasets/apple.csv
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)  4000835 2024-01-03 13:16:19.000000 datasetlib-0.1.7.1/src/datasetlib/datasets/babynames.csv
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)   396220 2023-12-22 18:23:29.000000 datasetlib-0.1.7.1/src/datasetlib/datasets/bmw.csv
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)  2605087 2023-12-22 18:23:29.000000 datasetlib-0.1.7.1/src/datasetlib/datasets/summergames.csv
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)    25173 2023-12-22 18:23:29.000000 datasetlib-0.1.7.1/src/datasetlib/datasets/titanic.csv
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     3425 2024-01-03 14:03:58.000000 datasetlib-0.1.7.1/src/datasetlib/datasets.py
-drwxr-xr-x   0 neutro2   (1000) neutro2   (1000)        0 2024-01-03 14:04:49.733262 datasetlib-0.1.7.1/src/datasetlib.egg-info/
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)     2173 2024-01-03 14:04:49.000000 datasetlib-0.1.7.1/src/datasetlib.egg-info/PKG-INFO
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)      455 2024-01-03 14:04:49.000000 datasetlib-0.1.7.1/src/datasetlib.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)        1 2024-01-03 14:04:49.000000 datasetlib-0.1.7.1/src/datasetlib.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)       31 2024-01-03 14:04:49.000000 datasetlib-0.1.7.1/src/datasetlib.egg-info/requires.txt
--rw-r--r--   0 neutro2   (1000) neutro2   (1000)       11 2024-01-03 14:04:49.000000 datasetlib-0.1.7.1/src/datasetlib.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.974286 datasetlib-0.2/
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-04-01 10:24:50.000000 datasetlib-0.2/LICENSE
+-rw-r--r--   0 neutro2    (501) staff       (20)     4003 2024-04-01 10:42:09.973426 datasetlib-0.2/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1044 2024-04-01 10:41:32.000000 datasetlib-0.2/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     1892 2024-04-01 10:24:50.000000 datasetlib-0.2/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-01 10:42:09.974430 datasetlib-0.2/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.931938 datasetlib-0.2/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.934081 datasetlib-0.2/src/datasetlib/
+-rw-r--r--   0 neutro2    (501) staff       (20)      634 2024-04-01 10:26:14.000000 datasetlib-0.2/src/datasetlib/__init__.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.968967 datasetlib-0.2/src/datasetlib/datasets/
+-rw-r--r--   0 neutro2    (501) staff       (20)   294994 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/apple.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)  4000835 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/babynames.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)   396220 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/bmw.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)  2605087 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/summergames.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)    25173 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/titanic.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)     3450 2024-04-01 10:40:32.000000 datasetlib-0.2/src/datasetlib/datasets.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.972278 datasetlib-0.2/src/datasetlib.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     4003 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      465 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       33 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       11 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/top_level.txt
```

### Comparing `datasetlib-0.1.7.1/LICENSE` & `datasetlib-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/README.md` & `datasetlib-0.2/readme.md`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/pyproject.toml` & `datasetlib-0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datasetlib"
-version = "0.1.7.1"
+version = "0.2"
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "easy access to commonly used datasets in pandas dataframe format"
 readme = "readme.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -16,15 +16,15 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-dependencies = ['basefunctions >= 0.1', 'pandas >=2.0']
+dependencies = ['basefunctions >= 0.3.7', 'pandas >=2.0']
 
 [tool.setuptools.package-data]
 "datasetlib.datasets" = ["*.csv"]
 
 [project.urls]
 "Homepage" = "https://dev.azure.com/neuraldevelopment/datasetlib"
 "Bug Tracker" = "https://dev.azure.com/neuraldevelopment/datasetlib/_backlogs/backlog/datasetlib%20Team/Epics"
```

### Comparing `datasetlib-0.1.7.1/src/datasetlib/__init__.py` & `datasetlib-0.2/src/datasetlib/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 #
 #  Copyright (c) by Ralph Vogl
 #
 #  All rights reserved.
 #
 #  Description:
 #
-#  datasetlib provides quick and easy access to datasets in different fields of interest
+#  datasetlib provides quick and easy access to datasets in different fields 
+#  of interest
 #
 # =============================================================================
 
 # -------------------------------------------------------------
 # IMPORTS
 # -------------------------------------------------------------
-from datasetlib.datasets import getDataSets, getDataSet
+from datasetlib.datasets import get_dataset, get_datasets
```

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets/apple.csv` & `datasetlib-0.2/src/datasetlib/datasets/apple.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets/babynames.csv` & `datasetlib-0.2/src/datasetlib/datasets/babynames.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets/bmw.csv` & `datasetlib-0.2/src/datasetlib/datasets/bmw.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets/summergames.csv` & `datasetlib-0.2/src/datasetlib/datasets/summergames.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets/titanic.csv` & `datasetlib-0.2/src/datasetlib/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.1.7.1/src/datasetlib/datasets.py` & `datasetlib-0.2/src/datasetlib/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 #
 # =============================================================================
 
 # -------------------------------------------------------------
 # IMPORTS
 # -------------------------------------------------------------
 import os
+
 import basefunctions as bf
 import pandas as pd
 
 # -------------------------------------------------------------
 # DEFINITIONS
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # DEFINITIONS REGISTRY
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # DEFINITIONS
 # -------------------------------------------------------------
-_dataSetDict = {
+_dataset_dict = {
     "aapl": (
         "datasets/apple.csv",
         {"index_col": [0], "parse_dates": [0], "header": [0]},
     ),
     "babynames": ("datasets/babynames.csv", {"index_col": [0]}),
     "bmw": ("datasets/bmw.csv", {"index_col": [0], "parse_dates": [0], "header": [0]}),
     "summergames": ("datasets/summergames.csv", {"index_col": [0], "header": [0]}),
@@ -48,77 +49,77 @@
 # VARIABLE DEFINTIONS
 # -------------------------------------------------------------
 
 
 # -------------------------------------------------------------
 # FUNCTION DEFINTIONS
 # -------------------------------------------------------------
-def getDataSets():
+def get_datasets():
     """get a list of all available datasets
 
     Returns
     -------
     list
         list of available datasets
     """
-    return list(_dataSetDict.keys())
+    return list(_dataset_dict.keys())
 
 
-def getDataSetFileName(dataSetName):
+def get_dataset_filename(dataset_name):
     """get the filename for a specific dataset
 
     Parameters
     ----------
-    dataSetName : str
+    dataset_name : str
         name of dataset
 
     Returns
     -------
     str
         file name of dataset
 
     Raises
     ------
     RuntimeError
         raises RuntimeError if dataset name can't be found
     """
     print(
         os.path.sep.join(
-            [bf.getPathName(os.path.abspath(__file__)), _dataSetDict[dataSetName][0]]
+            [bf.get_path_name(os.path.abspath(__file__)), _dataset_dict[dataset_name][0]]
         )
     )
-    if dataSetName in _dataSetDict:
-        return bf.normpath(
+    if dataset_name in _dataset_dict:
+        return bf.norm_path(
             os.path.sep.join(
                 [
-                    bf.getPathName(os.path.abspath(__file__)),
-                    _dataSetDict[dataSetName][0],
+                    bf.get_path_name(os.path.abspath(__file__)),
+                    _dataset_dict[dataset_name][0],
                 ]
             )
         )
     else:
-        raise RuntimeError(f"dataset {dataSetName} not found")
+        raise RuntimeError(f"dataset {dataset_name} not found")
 
 
-def getDataSet(dataSetName):
+def get_dataset(dataset_name):
     """get a specific dataset
 
     Parameters
     ----------
-    dataSetName : str
+    dataset_name : str
         name of dataset
 
     Returns
     -------
     pandas dataframe
         dataframe of dataset
 
     Raises
     ------
     RuntimeError
         raises RuntimeError if dataset name can't be found
     """
-    if dataSetName in _dataSetDict:
-        fileName, kwargs = _dataSetDict[dataSetName]
-        return pd.read_csv(getDataSetFileName(dataSetName), **kwargs)
+    if dataset_name in _dataset_dict:
+        _, kwargs = _dataset_dict[dataset_name]
+        return pd.read_csv(get_dataset_filename(dataset_name), **kwargs)
     else:
-        raise RuntimeError(f"dataset {dataSetName} not found")
+        raise RuntimeError(f"dataset {dataset_name} not found")
```

