# Comparing `tmp/allure-nose2-2.9.44.tar.gz` & `tmp/allure-nose2-2.9.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allure-nose2-2.9.44.tar", last modified: Wed Sep 29 20:24:28 2021, max compression
+gzip compressed data, was "allure-nose2-2.9.45.tar", last modified: Fri Oct 15 08:22:23 2021, max compression
```

## Comparing `allure-nose2-2.9.44.tar` & `allure-nose2-2.9.45.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/allure_nose2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-09-29 20:24:28.000000 allure-nose2-2.9.44/allure_nose2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      581 2021-09-29 20:24:28.000000 allure-nose2-2.9.44/allure_nose2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 20:24:28.000000 allure-nose2-2.9.44/allure_nose2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-09-29 20:24:28.000000 allure-nose2-2.9.44/allure_nose2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-29 20:24:28.000000 allure-nose2-2.9.44/allure_nose2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/src/listener.py
--rw-r--r--   0 runner    (1001) docker     (121)     5160 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/src/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3378 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/example_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/example_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/test/labels/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/labels/test_bdd_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/test/parametrized/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/parametrized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/parametrized/test_parametrized.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/test/result/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/result/test_fullname.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/result/test_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:28.549683 allure-nose2-2.9.44/test/with_mp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/with_mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/test/with_mp/test_pm.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-09-29 20:24:05.000000 allure-nose2-2.9.44/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.076866 allure-nose2-2.9.45/allure_nose2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-10-15 08:22:22.000000 allure-nose2-2.9.45/allure_nose2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2021-10-15 08:22:22.000000 allure-nose2-2.9.45/allure_nose2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 08:22:22.000000 allure-nose2-2.9.45/allure_nose2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-10-15 08:22:22.000000 allure-nose2-2.9.45/allure_nose2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-10-15 08:22:22.000000 allure-nose2-2.9.45/allure_nose2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.076866 allure-nose2-2.9.45/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/src/listener.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5160 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/src/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3378 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.076866 allure-nose2-2.9.45/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1033 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/example_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/example_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/test/labels/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2871 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/labels/test_bdd_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/test/parametrized/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/parametrized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2154 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/parametrized/test_parametrized.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/test/result/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/result/test_fullname.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2566 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/result/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 08:22:23.080866 allure-nose2-2.9.45/test/with_mp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/with_mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/test/with_mp/test_pm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2021-10-15 08:21:54.000000 allure-nose2-2.9.45/tox.ini
```

### Comparing `allure-nose2-2.9.44/PKG-INFO` & `allure-nose2-2.9.45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-nose2
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure nose2 integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting nose2
 Platform: UNKNOWN
```

### Comparing `allure-nose2-2.9.44/allure_nose2.egg-info/PKG-INFO` & `allure-nose2-2.9.45/allure_nose2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allure-nose2
-Version: 2.9.44
+Version: 2.9.45
 Summary: Allure nose2 integration
 Home-page: https://github.com/allure-framework/allure-python
 Author: QAMetaSoftware, Stanislav Seliverstov
 Author-email: sseliverstov@qameta.io
 License: Apache-2.0
 Keywords: allure reporting nose2
 Platform: UNKNOWN
```

### Comparing `allure-nose2-2.9.44/allure_nose2.egg-info/SOURCES.txt` & `allure-nose2-2.9.45/allure_nose2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/setup.py` & `allure-nose2-2.9.45/setup.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/src/plugin.py` & `allure-nose2-2.9.45/src/plugin.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/src/utils.py` & `allure-nose2-2.9.45/src/utils.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/example_loader.py` & `allure-nose2-2.9.45/test/example_loader.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/example_runner.py` & `allure-nose2-2.9.45/test/example_runner.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/labels/test_bdd_labels.py` & `allure-nose2-2.9.45/test/labels/test_bdd_labels.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/parametrized/test_parametrized.py` & `allure-nose2-2.9.45/test/parametrized/test_parametrized.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/result/test_fullname.py` & `allure-nose2-2.9.45/test/result/test_fullname.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/test/result/test_status.py` & `allure-nose2-2.9.45/test/result/test_status.py`

 * *Files identical despite different names*

### Comparing `allure-nose2-2.9.44/tox.ini` & `allure-nose2-2.9.45/tox.ini`

 * *Files identical despite different names*

