# Comparing `tmp/allure-python-commons-2.9.44.tar.gz` & `tmp/allure-python-commons-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-python-commons-2.9.44.tar", last modified: Wed Sep 29 20:24:19 2021, max compression
+gzip compressed data, was "allure-python-commons-2.9.45.tar", last modified: Fri Oct 15 08:22:12 2021, max compression
```

## Comparing `allure-python-commons-2.9.44.tar` & `allure-python-commons-2.9.45.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:19.365609 allure-python-commons-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-09-29 20:24:19.365609 allure-python-commons-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/allure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:19.361609 allure-python-commons-2.9.44/allure_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-09-29 20:24:19.000000 allure-python-commons-2.9.44/allure_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-09-29 20:24:19.000000 allure-python-commons-2.9.44/allure_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:19.000000 allure-python-commons-2.9.44/allure_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-29 20:24:19.000000 allure-python-commons-2.9.44/allure_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-29 20:24:19.000000 allure-python-commons-2.9.44/allure_python_commons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:19.365609 allure-python-commons-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:19.361609 allure-python-commons-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/_allure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5901 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2401 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/model2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    10415 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-09-29 20:24:05.000000 allure-python-commons-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:12.704831 allure-python-commons-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-10-15 08:22:12.704831 allure-python-commons-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/allure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:12.704831 allure-python-commons-2.9.45/allure_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-10-15 08:22:12.000000 allure-python-commons-2.9.45/allure_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-15 08:22:12.000000 allure-python-commons-2.9.45/allure_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:12.000000 allure-python-commons-2.9.45/allure_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-15 08:22:12.000000 allure-python-commons-2.9.45/allure_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-15 08:22:12.000000 allure-python-commons-2.9.45/allure_python_commons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:12.704831 allure-python-commons-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:12.704831 allure-python-commons-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7418 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/_allure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2803 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5901 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2763 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2401 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/model2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4553 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10415 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2021-10-15 08:21:54.000000 allure-python-commons-2.9.45/tox.ini
```

### Comparing `allure-python-commons-2.9.44/PKG-INFO` & `allure-python-commons-2.9.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-python-commons
-Version: 2.9.44
+Version: 2.9.45
 Summary: Common module for integrate allure with python-based frameworks
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting report-engine
 Platform: UNKNOWN
```

### Comparing `allure-python-commons-2.9.44/allure.py` & `allure-python-commons-2.9.45/allure.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/allure_python_commons.egg-info/PKG-INFO` & `allure-python-commons-2.9.45/allure_python_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-python-commons
-Version: 2.9.44
+Version: 2.9.45
 Summary: Common module for integrate allure with python-based frameworks
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting report-engine
 Platform: UNKNOWN
```

### Comparing `allure-python-commons-2.9.44/setup.py` & `allure-python-commons-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/_allure.py` & `allure-python-commons-2.9.45/src/_allure.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/_compat.py` & `allure-python-commons-2.9.45/src/_compat.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/_core.py` & `allure-python-commons-2.9.45/src/_core.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/_hooks.py` & `allure-python-commons-2.9.45/src/_hooks.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/lifecycle.py` & `allure-python-commons-2.9.45/src/lifecycle.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/logger.py` & `allure-python-commons-2.9.45/src/logger.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/mapping.py` & `allure-python-commons-2.9.45/src/mapping.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/model2.py` & `allure-python-commons-2.9.45/src/model2.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/reporter.py` & `allure-python-commons-2.9.45/src/reporter.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/types.py` & `allure-python-commons-2.9.45/src/types.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-2.9.44/src/utils.py` & `allure-python-commons-2.9.45/src/utils.py`

 * *Files identical despite different names*

