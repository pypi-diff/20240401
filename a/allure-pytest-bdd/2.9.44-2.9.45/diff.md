# Comparing `tmp/allure-pytest-bdd-2.9.44.tar.gz` & `tmp/allure-pytest-bdd-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-pytest-bdd-2.9.44.tar", last modified: Wed Sep 29 20:24:37 2021, max compression
+gzip compressed data, was "allure-pytest-bdd-2.9.45.tar", last modified: Fri Oct 15 08:22:32 2021, max compression
```

## Comparing `allure-pytest-bdd-2.9.44.tar` & `allure-pytest-bdd-2.9.45.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:37.145807 allure-pytest-bdd-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-09-29 20:24:37.145807 allure-pytest-bdd-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:37.141807 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-09-29 20:24:36.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-09-29 20:24:37.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:36.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-09-29 20:24:36.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-29 20:24:37.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-29 20:24:37.000000 allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:37.141807 allure-pytest-bdd-2.9.44/features/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/features/background.feature
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/features/outline.feature
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/features/scenario.feature
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:37.145807 allure-pytest-bdd-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:37.145807 allure-pytest-bdd-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/src/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5582 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/src/pytest_bdd_listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:37.145807 allure-pytest-bdd-2.9.44/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/test/outline_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/test/scenario_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/test/steps.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-09-29 20:24:05.000000 allure-pytest-bdd-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:32.468908 allure-pytest-bdd-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-15 08:22:32.468908 allure-pytest-bdd-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:32.464908 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-15 08:22:32.000000 allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:32.464908 allure-pytest-bdd-2.9.45/features/
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/features/background.feature
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/features/outline.feature
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/features/scenario.feature
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:32.468908 allure-pytest-bdd-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:32.468908 allure-pytest-bdd-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/src/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5582 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/src/pytest_bdd_listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:32.468908 allure-pytest-bdd-2.9.45/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/test/outline_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/test/scenario_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/test/steps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-10-15 08:21:54.000000 allure-pytest-bdd-2.9.45/tox.ini
```

### Comparing `allure-pytest-bdd-2.9.44/PKG-INFO` & `allure-pytest-bdd-2.9.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-pytest-bdd
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure pytest-bdd integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting pytest
 Platform: UNKNOWN
```

### Comparing `allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/PKG-INFO` & `allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-pytest-bdd
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure pytest-bdd integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting pytest
 Platform: UNKNOWN
```

### Comparing `allure-pytest-bdd-2.9.44/allure_pytest_bdd.egg-info/SOURCES.txt` & `allure-pytest-bdd-2.9.45/allure_pytest_bdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/features/outline.feature` & `allure-pytest-bdd-2.9.45/features/outline.feature`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/features/scenario.feature` & `allure-pytest-bdd-2.9.45/features/scenario.feature`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/setup.py` & `allure-pytest-bdd-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/src/plugin.py` & `allure-pytest-bdd-2.9.45/src/plugin.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/src/pytest_bdd_listener.py` & `allure-pytest-bdd-2.9.45/src/pytest_bdd_listener.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/src/utils.py` & `allure-pytest-bdd-2.9.45/src/utils.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/test/conftest.py` & `allure-pytest-bdd-2.9.45/test/conftest.py`

 * *Files identical despite different names*

### Comparing `allure-pytest-bdd-2.9.44/test/steps.py` & `allure-pytest-bdd-2.9.45/test/steps.py`

 * *Files identical despite different names*

