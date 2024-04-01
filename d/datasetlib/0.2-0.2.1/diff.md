# Comparing `tmp/datasetlib-0.2.tar.gz` & `tmp/datasetlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasetlib-0.2.tar", last modified: Mon Apr  1 10:42:09 2024, max compression
+gzip compressed data, was "datasetlib-0.2.1.tar", last modified: Mon Apr  1 10:47:40 2024, max compression
```

## Comparing `datasetlib-0.2.tar` & `datasetlib-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.974286 datasetlib-0.2/
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-04-01 10:24:50.000000 datasetlib-0.2/LICENSE
--rw-r--r--   0 neutro2    (501) staff       (20)     4003 2024-04-01 10:42:09.973426 datasetlib-0.2/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1044 2024-04-01 10:41:32.000000 datasetlib-0.2/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     1892 2024-04-01 10:24:50.000000 datasetlib-0.2/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-01 10:42:09.974430 datasetlib-0.2/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.931938 datasetlib-0.2/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.934081 datasetlib-0.2/src/datasetlib/
--rw-r--r--   0 neutro2    (501) staff       (20)      634 2024-04-01 10:26:14.000000 datasetlib-0.2/src/datasetlib/__init__.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.968967 datasetlib-0.2/src/datasetlib/datasets/
--rw-r--r--   0 neutro2    (501) staff       (20)   294994 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/apple.csv
--rw-r--r--   0 neutro2    (501) staff       (20)  4000835 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/babynames.csv
--rw-r--r--   0 neutro2    (501) staff       (20)   396220 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/bmw.csv
--rw-r--r--   0 neutro2    (501) staff       (20)  2605087 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/summergames.csv
--rw-r--r--   0 neutro2    (501) staff       (20)    25173 2024-04-01 10:24:50.000000 datasetlib-0.2/src/datasetlib/datasets/titanic.csv
--rw-r--r--   0 neutro2    (501) staff       (20)     3450 2024-04-01 10:40:32.000000 datasetlib-0.2/src/datasetlib/datasets.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:42:09.972278 datasetlib-0.2/src/datasetlib.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     4003 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      465 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       33 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       11 2024-04-01 10:42:09.000000 datasetlib-0.2/src/datasetlib.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:47:40.517773 datasetlib-0.2.1/
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-04-01 10:24:50.000000 datasetlib-0.2.1/LICENSE
+-rw-r--r--   0 neutro2    (501) staff       (20)     3726 2024-04-01 10:47:40.517204 datasetlib-0.2.1/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1046 2024-04-01 10:47:23.000000 datasetlib-0.2.1/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     1597 2024-04-01 10:47:12.000000 datasetlib-0.2.1/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-01 10:47:40.517902 datasetlib-0.2.1/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:47:40.481548 datasetlib-0.2.1/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:47:40.484239 datasetlib-0.2.1/src/datasetlib/
+-rw-r--r--   0 neutro2    (501) staff       (20)      634 2024-04-01 10:26:14.000000 datasetlib-0.2.1/src/datasetlib/__init__.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:47:40.513181 datasetlib-0.2.1/src/datasetlib/datasets/
+-rw-r--r--   0 neutro2    (501) staff       (20)   294994 2024-04-01 10:24:50.000000 datasetlib-0.2.1/src/datasetlib/datasets/apple.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)  4000835 2024-04-01 10:24:50.000000 datasetlib-0.2.1/src/datasetlib/datasets/babynames.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)   396220 2024-04-01 10:24:50.000000 datasetlib-0.2.1/src/datasetlib/datasets/bmw.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)  2605087 2024-04-01 10:24:50.000000 datasetlib-0.2.1/src/datasetlib/datasets/summergames.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)    25173 2024-04-01 10:24:50.000000 datasetlib-0.2.1/src/datasetlib/datasets/titanic.csv
+-rw-r--r--   0 neutro2    (501) staff       (20)     3450 2024-04-01 10:40:32.000000 datasetlib-0.2.1/src/datasetlib/datasets.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-01 10:47:40.516564 datasetlib-0.2.1/src/datasetlib.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     3726 2024-04-01 10:47:40.000000 datasetlib-0.2.1/src/datasetlib.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      465 2024-04-01 10:47:40.000000 datasetlib-0.2.1/src/datasetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-01 10:47:40.000000 datasetlib-0.2.1/src/datasetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       33 2024-04-01 10:47:40.000000 datasetlib-0.2.1/src/datasetlib.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       11 2024-04-01 10:47:40.000000 datasetlib-0.2.1/src/datasetlib.egg-info/top_level.txt
```

### Comparing `datasetlib-0.2/LICENSE` & `datasetlib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/PKG-INFO` & `datasetlib-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasetlib
-Version: 0.2
+Version: 0.2.1
 Summary: easy access to commonly used datasets in pandas dataframe format
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,45 +37,33 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: basefunctions>=0.3.7
 Requires-Dist: pandas>=2.0
 
-# Introduction 
+# DataSetLib
+
+## Introduction
+
 a simple library having access to some often used datasets in pandas dataframe format
 
-# Getting Started
+## Getting Started
+
 There are two main functions in the module:
-- getDataSetList() returns a list with all the available datasets
-- getDataSet() returns a specific dataset identified by a name
 
-# Build and Test
-1. Install virtual environment 
-python3 -m venv .venv
-source .venv/bin/activate
-pip install build
-pip install twine
-pip install pytest
-
-2. Build a package:
-python3 -m build
-
-3. Run the testcases  
-pip install -e .
-pytest -s
+- `get_datasets()` returns a list with all the available datasets
+- `get_dataset()` returns a specific dataset identified by a name
 
-4. Upload the package to pypi.org
-python3 -m twine upload dist/*
+## Usage of datasetlib
 
-# Usage of datasetlib
-```
+```python
 import datasetlib as dsl
 
-dsl.getDataSetList()
+dsl.get_datasets()
 ['aapl', 'bmw', 'summergames', 'titanic']
 
 dsl.getDataSet('titanic')
      survived  pclass     sex   age  sibsp  parch     fare embarked deck
 0           0       3    male  22.0      1      0   7.2500        S  NaN
 1           1       1  female  38.0      1      0  71.2833        C    C
 2           1       3  female  26.0      0      0   7.9250        S  NaN
@@ -87,18 +75,14 @@
 888         0       3  female   NaN      1      2  23.4500        S  NaN
 889         1       1    male  26.0      0      0  30.0000        C    C
 890         0       3    male  32.0      0      0   7.7500        Q  NaN
 
 [891 rows x 9 columns]
 ```
 
+## Project Homepage
 
+<https://dev.azure.com/neuraldevelopment/datasetlib>
 
+## Contribute
 
-
-
-
-# Project Homepage
-https://dev.azure.com/neuraldevelopment/datasetlib
-
-# Contribute
-If you find a defect or suggest a new function, please send an eMail to neutro2@outlook.de
+If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

### Comparing `datasetlib-0.2/pyproject.toml` & `datasetlib-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datasetlib"
-version = "0.2"
+version = "0.2.1"
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "easy access to commonly used datasets in pandas dataframe format"
 readme = "readme.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `datasetlib-0.2/readme.md` & `datasetlib-0.2.1/readme.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-# Introduction 
+# DataSetLib
+
+## Introduction
+
 a simple library having access to some often used datasets in pandas dataframe format
 
-# Getting Started
+## Getting Started
+
 There are two main functions in the module:
-- getDataSetList() returns a list with all the available datasets
-- getDataSet() returns a specific dataset identified by a name
 
-# Build and Test
-1. Install virtual environment 
-python3 -m venv .venv
-source .venv/bin/activate
-pip install build
-pip install twine
-pip install pytest
-
-2. Build a package:
-python3 -m build
-
-3. Run the testcases  
-pip install -e .
-pytest -s
+- `get_datasets()` returns a list with all the available datasets
+- `get_dataset()` returns a specific dataset identified by a name
 
-4. Upload the package to pypi.org
-python3 -m twine upload dist/*
+## Usage of datasetlib
 
-# Usage of datasetlib
-```
+```python
 import datasetlib as dsl
 
-dsl.getDataSetList()
+dsl.get_datasets()
 ['aapl', 'bmw', 'summergames', 'titanic']
 
 dsl.getDataSet('titanic')
      survived  pclass     sex   age  sibsp  parch     fare embarked deck
 0           0       3    male  22.0      1      0   7.2500        S  NaN
 1           1       1  female  38.0      1      0  71.2833        C    C
 2           1       3  female  26.0      0      0   7.9250        S  NaN
@@ -44,18 +32,14 @@
 888         0       3  female   NaN      1      2  23.4500        S  NaN
 889         1       1    male  26.0      0      0  30.0000        C    C
 890         0       3    male  32.0      0      0   7.7500        Q  NaN
 
 [891 rows x 9 columns]
 ```
 
+## Project Homepage
 
+<https://dev.azure.com/neuraldevelopment/datasetlib>
 
+## Contribute
 
-
-
-
-# Project Homepage
-https://dev.azure.com/neuraldevelopment/datasetlib
-
-# Contribute
-If you find a defect or suggest a new function, please send an eMail to neutro2@outlook.de
+If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

### Comparing `datasetlib-0.2/src/datasetlib/__init__.py` & `datasetlib-0.2.1/src/datasetlib/__init__.py`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets/apple.csv` & `datasetlib-0.2.1/src/datasetlib/datasets/apple.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets/babynames.csv` & `datasetlib-0.2.1/src/datasetlib/datasets/babynames.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets/bmw.csv` & `datasetlib-0.2.1/src/datasetlib/datasets/bmw.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets/summergames.csv` & `datasetlib-0.2.1/src/datasetlib/datasets/summergames.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets/titanic.csv` & `datasetlib-0.2.1/src/datasetlib/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib/datasets.py` & `datasetlib-0.2.1/src/datasetlib/datasets.py`

 * *Files identical despite different names*

### Comparing `datasetlib-0.2/src/datasetlib.egg-info/PKG-INFO` & `datasetlib-0.2.1/src/datasetlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasetlib
-Version: 0.2
+Version: 0.2.1
 Summary: easy access to commonly used datasets in pandas dataframe format
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,45 +37,33 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: basefunctions>=0.3.7
 Requires-Dist: pandas>=2.0
 
-# Introduction 
+# DataSetLib
+
+## Introduction
+
 a simple library having access to some often used datasets in pandas dataframe format
 
-# Getting Started
+## Getting Started
+
 There are two main functions in the module:
-- getDataSetList() returns a list with all the available datasets
-- getDataSet() returns a specific dataset identified by a name
 
-# Build and Test
-1. Install virtual environment 
-python3 -m venv .venv
-source .venv/bin/activate
-pip install build
-pip install twine
-pip install pytest
-
-2. Build a package:
-python3 -m build
-
-3. Run the testcases  
-pip install -e .
-pytest -s
+- `get_datasets()` returns a list with all the available datasets
+- `get_dataset()` returns a specific dataset identified by a name
 
-4. Upload the package to pypi.org
-python3 -m twine upload dist/*
+## Usage of datasetlib
 
-# Usage of datasetlib
-```
+```python
 import datasetlib as dsl
 
-dsl.getDataSetList()
+dsl.get_datasets()
 ['aapl', 'bmw', 'summergames', 'titanic']
 
 dsl.getDataSet('titanic')
      survived  pclass     sex   age  sibsp  parch     fare embarked deck
 0           0       3    male  22.0      1      0   7.2500        S  NaN
 1           1       1  female  38.0      1      0  71.2833        C    C
 2           1       3  female  26.0      0      0   7.9250        S  NaN
@@ -87,18 +75,14 @@
 888         0       3  female   NaN      1      2  23.4500        S  NaN
 889         1       1    male  26.0      0      0  30.0000        C    C
 890         0       3    male  32.0      0      0   7.7500        Q  NaN
 
 [891 rows x 9 columns]
 ```
 
+## Project Homepage
 
+<https://dev.azure.com/neuraldevelopment/datasetlib>
 
+## Contribute
 
-
-
-
-# Project Homepage
-https://dev.azure.com/neuraldevelopment/datasetlib
-
-# Contribute
-If you find a defect or suggest a new function, please send an eMail to neutro2@outlook.de
+If you find a defect or suggest a new function, please send an eMail to <neutro2@outlook.de>
```

