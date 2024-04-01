# Comparing `tmp/allure-python-commons-test-2.9.44.tar.gz` & `tmp/allure-python-commons-test-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-python-commons-test-2.9.44.tar", last modified: Wed Sep 29 20:24:14 2021, max compression
+gzip compressed data, was "allure-python-commons-test-2.9.45.tar", last modified: Fri Oct 15 08:22:07 2021, max compression
```

## Comparing `allure-python-commons-test-2.9.44.tar` & `allure-python-commons-test-2.9.45.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:14.869453 allure-python-commons-test-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-09-29 20:24:14.869453 allure-python-commons-test-2.9.44/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:14.869453 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-09-29 20:24:14.000000 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-09-29 20:24:14.000000 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:14.000000 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-29 20:24:14.000000 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-09-29 20:24:14.000000 allure-python-commons-test-2.9.44/allure_python_commons_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:14.869453 allure-python-commons-test-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:14.869453 allure-python-commons-test-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5528 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/src/container.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/src/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/src/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/src/result.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-09-29 20:24:05.000000 allure-python-commons-test-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:07.208789 allure-python-commons-test-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-10-15 08:22:07.208789 allure-python-commons-test-2.9.45/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:07.208789 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-10-15 08:22:06.000000 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2021-10-15 08:22:07.000000 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:06.000000 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-15 08:22:06.000000 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-10-15 08:22:06.000000 allure-python-commons-test-2.9.45/allure_python_commons_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:07.208789 allure-python-commons-test-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:07.208789 allure-python-commons-test-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5528 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/src/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/src/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4492 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/src/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4107 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/src/result.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-10-15 08:21:54.000000 allure-python-commons-test-2.9.45/tox.ini
```

### Comparing `allure-python-commons-test-2.9.44/setup.py` & `allure-python-commons-test-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-test-2.9.44/src/container.py` & `allure-python-commons-test-2.9.45/src/container.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-test-2.9.44/src/label.py` & `allure-python-commons-test-2.9.45/src/label.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-test-2.9.44/src/report.py` & `allure-python-commons-test-2.9.45/src/report.py`

 * *Files identical despite different names*

### Comparing `allure-python-commons-test-2.9.44/src/result.py` & `allure-python-commons-test-2.9.45/src/result.py`

 * *Files identical despite different names*

