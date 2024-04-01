# Comparing `tmp/drl_microgrid_ems-0.1.0.tar.gz` & `tmp/drl_microgrid_ems-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drl_microgrid_ems-0.1.0.tar", last modified: Sun Mar 31 14:54:23 2024, max compression
+gzip compressed data, was "drl_microgrid_ems-0.1.1.tar", last modified: Mon Apr  1 19:18:06 2024, max compression
```

## Comparing `drl_microgrid_ems-0.1.0.tar` & `drl_microgrid_ems-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 14:54:23.766673 drl_microgrid_ems-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-03-19 19:55:57.000000 drl_microgrid_ems-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      849 2024-03-31 14:54:23.765673 drl_microgrid_ems-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-03-31 12:59:48.000000 drl_microgrid_ems-0.1.0/README.md
--rw-rw-rw-   0        0        0      663 2024-03-31 14:54:00.000000 drl_microgrid_ems-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-31 14:54:23.766673 drl_microgrid_ems-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-31 14:54:23.739676 drl_microgrid_ems-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 14:54:23.752674 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/
--rw-rw-rw-   0        0        0    10165 2024-02-17 14:34:50.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/A3C_basic.py
--rw-rw-rw-   0        0        0    16820 2024-03-31 13:48:41.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/A3C_plusplus.py
--rw-rw-rw-   0        0        0        0 2024-03-19 19:55:57.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/__init__.py
--rw-rw-rw-   0        0        0    22833 2024-03-31 12:51:05.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/tcl_env_dqn.py
--rw-rw-rw-   0        0        0    28048 2024-03-31 13:43:08.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/tcl_env_dqn_1.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:54:23.763674 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/
--rw-rw-rw-   0        0        0      849 2024-03-31 14:54:23.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-03-31 14:54:23.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 14:54:23.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-03-31 14:54:23.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-03-31 14:54:23.000000 drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 19:18:06.910526 drl_microgrid_ems-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-02-27 12:37:30.000000 drl_microgrid_ems-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      796 2024-04-01 19:18:06.909155 drl_microgrid_ems-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-01 18:33:19.000000 drl_microgrid_ems-0.1.1/README.md
+-rw-rw-rw-   0        0        0      580 2024-04-01 19:17:12.000000 drl_microgrid_ems-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:18:06.910526 drl_microgrid_ems-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 19:18:06.880089 drl_microgrid_ems-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 19:18:06.897101 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/
+-rw-rw-rw-   0        0        0    10165 2024-04-01 18:20:30.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/A3C_basic.py
+-rw-rw-rw-   0        0        0    16859 2024-04-01 19:13:26.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/A3C_plusplus.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 12:31:39.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/__init__.py
+-rw-rw-rw-   0        0        0    22833 2024-04-01 18:20:30.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/tcl_env_dqn.py
+-rw-rw-rw-   0        0        0    28048 2024-04-01 18:20:30.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/tcl_env_dqn_1.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:18:06.907068 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/
+-rw-rw-rw-   0        0        0      796 2024-04-01 19:18:06.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-04-01 19:18:06.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:18:06.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-01 19:18:06.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-01 19:18:06.000000 drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/top_level.txt
```

### Comparing `drl_microgrid_ems-0.1.0/LICENSE` & `drl_microgrid_ems-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drl_microgrid_ems-0.1.0/PKG-INFO` & `drl_microgrid_ems-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: drl_microgrid_ems
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fork of  https://github.com/tahanakabi/DRL-for-microgrid-energy-management.git
 Author-email: Rupert Young <rupert@perceptualrobots.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
-Requires-Dist: numpy==1.22.4
-Requires-Dist: tensorflow==2.4.1
-Requires-Dist: keras==2.4.3
-Requires-Dist: pandas==1.1.0
 
 Fork of https://github.com/tahanakabi/DRL-for-microgrid-energy-management.git
 
 https://pypi.org/project/drl-microgrid-ems/
 
 https://code.visualstudio.com/docs/python/environments
 
 py -m build
 py -m twine upload dist/*
+
+
+
+  "tensorflow==2.5.0",
+  "keras==2.4.3",
+  "pandas==1.1.0"
+
```

### Comparing `drl_microgrid_ems-0.1.0/pyproject.toml` & `drl_microgrid_ems-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drl_microgrid_ems"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Rupert Young", email="rupert@perceptualrobots.com" },
 ]
 description = "Fork of  https://github.com/tahanakabi/DRL-for-microgrid-energy-management.git"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "tqdm",
-  "scikit-learn",
-  "numpy==1.22.4",
-  "tensorflow==2.4.1",
-  "keras==2.4.3",
-  "pandas==1.1.0"
+  "scikit-learn"
 ]
```

### Comparing `drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/A3C_basic.py` & `drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/A3C_basic.py`

 * *Files identical despite different names*

### Comparing `drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/A3C_plusplus.py` & `drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/A3C_plusplus.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import tensorflow as tf
 import numpy as np
 import gym, time, random, threading
 from keras.callbacks import TensorBoard
 from keras.models import *
 from keras.layers import *
 from keras import backend as K
-
-from drl_microgrid_ems.tcl_env_dqn_1 import *
+from tcl_env_dqn_1 import MicroGridEnv
+#from drl_microgrid_ems.tcl_env_dqn_1 import *
 print("after import")
 import os
 
 
 
 # This is where the models are saved and retrieved from
 MODELS_DIRECTORY = 'success01'
```

### Comparing `drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/tcl_env_dqn.py` & `drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/tcl_env_dqn.py`

 * *Files identical despite different names*

### Comparing `drl_microgrid_ems-0.1.0/src/drl_microgrid_ems/tcl_env_dqn_1.py` & `drl_microgrid_ems-0.1.1/src/drl_microgrid_ems/tcl_env_dqn_1.py`

 * *Files identical despite different names*

### Comparing `drl_microgrid_ems-0.1.0/src/drl_microgrid_ems.egg-info/PKG-INFO` & `drl_microgrid_ems-0.1.1/src/drl_microgrid_ems.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: drl_microgrid_ems
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fork of  https://github.com/tahanakabi/DRL-for-microgrid-energy-management.git
 Author-email: Rupert Young <rupert@perceptualrobots.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
-Requires-Dist: numpy==1.22.4
-Requires-Dist: tensorflow==2.4.1
-Requires-Dist: keras==2.4.3
-Requires-Dist: pandas==1.1.0
 
 Fork of https://github.com/tahanakabi/DRL-for-microgrid-energy-management.git
 
 https://pypi.org/project/drl-microgrid-ems/
 
 https://code.visualstudio.com/docs/python/environments
 
 py -m build
 py -m twine upload dist/*
+
+
+
+  "tensorflow==2.5.0",
+  "keras==2.4.3",
+  "pandas==1.1.0"
+
```

