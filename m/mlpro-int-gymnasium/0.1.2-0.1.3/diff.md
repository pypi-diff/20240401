# Comparing `tmp/mlpro-int-gymnasium-0.1.2.tar.gz` & `tmp/mlpro-int-gymnasium-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpro-int-gymnasium-0.1.2.tar", last modified: Sun Feb 25 19:20:40 2024, max compression
+gzip compressed data, was "mlpro-int-gymnasium-0.1.3.tar", last modified: Mon Apr  1 20:09:41 2024, max compression
```

## Comparing `mlpro-int-gymnasium-0.1.2.tar` & `mlpro-int-gymnasium-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-25 19:20:40.731250 mlpro-int-gymnasium-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.723250 mlpro-int-gymnasium-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/boards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/boards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/boards/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/envs/multicartpole.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/wrappers/basics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-25 19:20:40.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-25 19:20:40.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 19:20:40.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 19:20:40.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 19:20:40.000000 mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 19:20:40.727250 mlpro-int-gymnasium-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-02-25 19:20:28.000000 mlpro-int-gymnasium-0.1.2/test/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 20:09:41.963914 mlpro-int-gymnasium-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.955914 mlpro-int-gymnasium-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13493 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/multicartpole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/basics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:09:41.000000 mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:09:41.959914 mlpro-int-gymnasium-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-01 20:09:37.000000 mlpro-int-gymnasium-0.1.3/test/test_examples.py
```

### Comparing `mlpro-int-gymnasium-0.1.2/LICENSE` & `mlpro-int-gymnasium-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.2/PKG-INFO` & `mlpro-int-gymnasium-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 0.1.2
+Version: 0.1.3
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-gymnasium-0.1.2/README.md` & `mlpro-int-gymnasium-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.2/setup.cfg` & `mlpro-int-gymnasium-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mlpro-int-gymnasium
-version = 0.1.2
+version = 0.1.3
 author = MLPro Team
 author_email = mlpro@listen.fh-swf.de
 description = MLPro: Integration Gymnasium
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://mlpro-int-gymnasium.readthedocs.io
 project_urls =
```

### Comparing `mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/boards/multicartpole.py` & `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/boards/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/envs/multicartpole.py` & `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/envs/multicartpole.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium/wrappers/basics.py` & `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium/wrappers/basics.py`

 * *Files identical despite different names*

### Comparing `mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/PKG-INFO` & `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpro-int-gymnasium
-Version: 0.1.2
+Version: 0.1.3
 Summary: MLPro: Integration Gymnasium
 Home-page: https://mlpro-int-gymnasium.readthedocs.io
 Author: MLPro Team
 Author-email: mlpro@listen.fh-swf.de
 Project-URL: Bug Tracker, https://mlpro-int-gymnasium.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mlpro-int-gymnasium-0.1.2/src/mlpro_int_gymnasium.egg-info/SOURCES.txt` & `mlpro-int-gymnasium-0.1.3/src/mlpro_int_gymnasium.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 src/mlpro_int_gymnasium.egg-info/top_level.txt
 src/mlpro_int_gymnasium/boards/__init__.py
 src/mlpro_int_gymnasium/boards/multicartpole.py
 src/mlpro_int_gymnasium/envs/__init__.py
 src/mlpro_int_gymnasium/envs/multicartpole.py
 src/mlpro_int_gymnasium/wrappers/__init__.py
 src/mlpro_int_gymnasium/wrappers/basics.py
+test/test_environment.py
 test/test_examples.py
```

### Comparing `mlpro-int-gymnasium-0.1.2/test/test_examples.py` & `mlpro-int-gymnasium-0.1.3/test/test_examples.py`

 * *Files identical despite different names*

