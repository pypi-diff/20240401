# Comparing `tmp/imt-ikarus-1.0.0.tar.gz` & `tmp/imt-ikarus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imt-ikarus-1.0.0.tar", last modified: Wed Mar 27 11:31:23 2024, max compression
+gzip compressed data, was "imt-ikarus-1.0.1.tar", last modified: Mon Apr  1 16:13:04 2024, max compression
```

## Comparing `imt-ikarus-1.0.0.tar` & `imt-ikarus-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.280204 imt-ikarus-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-27 11:31:23.280204 imt-ikarus-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-27 11:31:23.280204 imt-ikarus-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.272204 imt-ikarus-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.276204 imt-ikarus-1.0.0/src/ikarus/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/_src.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.276204 imt-ikarus-1.0.0/src/ikarus/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/baselines/qmt_baselines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.276204 imt-ikarus-1.0.0/src/ikarus/baselines/riann/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/baselines/riann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/baselines/riann/riann.onnx
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/baselines/riann/riann.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.276204 imt-ikarus-1.0.0/src/ikarus/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/benchmark/_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.276204 imt-ikarus-1.0.0/src/ikarus/benchmark/xmls/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/benchmark/xmls/arm.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/benchmark/xmls/gait.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/test_src.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-03-27 11:31:19.000000 imt-ikarus-1.0.0/src/ikarus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:31:23.280204 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-27 11:31:23.000000 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-27 11:31:23.000000 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:31:23.000000 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-27 11:31:23.000000 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 11:31:23.000000 imt-ikarus-1.0.0/src/imt_ikarus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.831690 imt-ikarus-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.831690 imt-ikarus-1.0.1/src/ikarus/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/_src.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.831690 imt-ikarus-1.0.1/src/ikarus/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/baselines/qmt_baselines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/src/ikarus/baselines/riann/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/baselines/riann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1471345 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/baselines/riann/riann.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/baselines/riann/riann.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/src/ikarus/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/benchmark/_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/src/ikarus/benchmark/xmls/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/benchmark/xmls/arm.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/benchmark/xmls/gait.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/test_src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-04-01 16:13:01.000000 imt-ikarus-1.0.1/src/ikarus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:13:04.835690 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-01 16:13:04.000000 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 16:13:04.000000 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:13:04.000000 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 16:13:04.000000 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 16:13:04.000000 imt-ikarus-1.0.1/src/imt_ikarus.egg-info/top_level.txt
```

### Comparing `imt-ikarus-1.0.0/PKG-INFO` & `imt-ikarus-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.0.0
+Version: 1.0.1
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,15 +106,15 @@
 ## `preprocess/*`
 Refer to the readme in the subfolder.
 
 ## `src/*`
 Requires Python 3.10 or higher.
 
 The Python Package allows convenient access to the data and can be installed with
-> pip install 'ikarus @ git+https://github.com/SimiPixel/ikarus'
+> pip install imt-ikarus
 
 Note that the Python Package will automatically download the required data on-demand. By default it comes with no data at all and there is no data stored in a redundant way.
 
 ### Quickstart
 ```python
 import ikarus
```

### Comparing `imt-ikarus-1.0.0/pyproject.toml` & `imt-ikarus-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "imt-ikarus"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Simon Bachhuber", email="simon.bachhuber@fau.de" },
 ]
 description = "IKArus - Inertial and Optical Data of Kinematic ChAin Motion"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `imt-ikarus-1.0.0/readme.md` & `imt-ikarus-1.0.1/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 ## `preprocess/*`
 Refer to the readme in the subfolder.
 
 ## `src/*`
 Requires Python 3.10 or higher.
 
 The Python Package allows convenient access to the data and can be installed with
-> pip install 'ikarus @ git+https://github.com/SimiPixel/ikarus'
+> pip install imt-ikarus
 
 Note that the Python Package will automatically download the required data on-demand. By default it comes with no data at all and there is no data stored in a redundant way.
 
 ### Quickstart
 ```python
 import ikarus
```

### Comparing `imt-ikarus-1.0.0/src/ikarus/_src.py` & `imt-ikarus-1.0.1/src/ikarus/_src.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/baselines/qmt_baselines.py` & `imt-ikarus-1.0.1/src/ikarus/baselines/qmt_baselines.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/baselines/riann/riann.onnx` & `imt-ikarus-1.0.1/src/ikarus/baselines/riann/riann.onnx`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/baselines/riann/riann.py` & `imt-ikarus-1.0.1/src/ikarus/baselines/riann/riann.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/benchmark/_benchmark.py` & `imt-ikarus-1.0.1/src/ikarus/benchmark/_benchmark.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/benchmark/xmls/arm.xml` & `imt-ikarus-1.0.1/src/ikarus/benchmark/xmls/arm.xml`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/benchmark/xmls/gait.xml` & `imt-ikarus-1.0.1/src/ikarus/benchmark/xmls/gait.xml`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/github.py` & `imt-ikarus-1.0.1/src/ikarus/github.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/test_src.py` & `imt-ikarus-1.0.1/src/ikarus/test_src.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/test_utils.py` & `imt-ikarus-1.0.1/src/ikarus/test_utils.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/ikarus/utils.py` & `imt-ikarus-1.0.1/src/ikarus/utils.py`

 * *Files identical despite different names*

### Comparing `imt-ikarus-1.0.0/src/imt_ikarus.egg-info/PKG-INFO` & `imt-ikarus-1.0.1/src/imt_ikarus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imt-ikarus
-Version: 1.0.0
+Version: 1.0.1
 Summary: IKArus - Inertial and Optical Data of Kinematic ChAin Motion
 Author-email: Simon Bachhuber <simon.bachhuber@fau.de>
 Project-URL: Homepage, https://github.com/SimiPixel/ikarus
 Project-URL: Issues, https://github.com/SimiPixel/ikarus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -106,15 +106,15 @@
 ## `preprocess/*`
 Refer to the readme in the subfolder.
 
 ## `src/*`
 Requires Python 3.10 or higher.
 
 The Python Package allows convenient access to the data and can be installed with
-> pip install 'ikarus @ git+https://github.com/SimiPixel/ikarus'
+> pip install imt-ikarus
 
 Note that the Python Package will automatically download the required data on-demand. By default it comes with no data at all and there is no data stored in a redundant way.
 
 ### Quickstart
 ```python
 import ikarus
```

### Comparing `imt-ikarus-1.0.0/src/imt_ikarus.egg-info/SOURCES.txt` & `imt-ikarus-1.0.1/src/imt_ikarus.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 pyproject.toml
 readme.md
 setup.cfg
-setup.py
 src/ikarus/__init__.py
 src/ikarus/_src.py
 src/ikarus/github.py
 src/ikarus/test_github.py
 src/ikarus/test_src.py
 src/ikarus/test_utils.py
 src/ikarus/utils.py
```

