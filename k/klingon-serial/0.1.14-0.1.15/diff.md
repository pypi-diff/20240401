# Comparing `tmp/klingon-serial-0.1.14.tar.gz` & `tmp/klingon-serial-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klingon-serial-0.1.14.tar", last modified: Sat Mar 30 23:22:11 2024, max compression
+gzip compressed data, was "klingon-serial-0.1.15.tar", last modified: Mon Apr  1 13:58:59 2024, max compression
```

## Comparing `klingon-serial-0.1.14.tar` & `klingon-serial-0.1.15.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 23:22:07.000000 klingon-serial-0.1.14/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/klingon_serial/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/klingon_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/klingon_serial/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/klingon_serial/strtobool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/klingon_serial/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/klingon_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-30 23:22:11.000000 klingon-serial-0.1.14/klingon_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 23:22:11.860848 klingon-serial-0.1.14/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/tests/test_klingon_get_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/tests/test_klingon_strtobool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-30 23:21:49.000000 klingon-serial-0.1.14/tests/test_klingon_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 13:58:54.000000 klingon-serial-0.1.15/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/klingon_serial/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/klingon_serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/klingon_serial/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/klingon_serial/strtobool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/klingon_serial/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/klingon_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 13:58:59.000000 klingon-serial-0.1.15/klingon_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:58:59.909865 klingon-serial-0.1.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/tests/test_klingon_get_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/tests/test_klingon_strtobool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-01 13:58:36.000000 klingon-serial-0.1.15/tests/test_klingon_utils.py
```

### Comparing `klingon-serial-0.1.14/LICENSE` & `klingon-serial-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/PKG-INFO` & `klingon-serial-0.1.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klingon-serial
-Version: 0.1.14
+Version: 0.1.15
 Summary: Get a globally unique serial
 Home-page: https://github.com/djh00t/module_klingon_serial
 Author: David Hooton
 Author-email: klingon_serial+david@hooton.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: pytest>=6.0
 Requires-Dist: str2bool
 
 # Klingon Serial Python Module
+[![klingon-serial unit tests](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml)
 [![Pre-PR Merge CI](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml) [![.github/workflows/post-pr-merge.yaml](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml)
 ## Overview
 
 The `klingon_serial` Python module is designed to generate a unique hexadecimal
 serial number, avoiding serial conflicts in a distributed environment. The
 serial number is a concatenation of the machine's MAC address, the process ID
 (PID), and the current time in epoch format with millisecond precision. The
```

### Comparing `klingon-serial-0.1.14/README.md` & `klingon-serial-0.1.15/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Klingon Serial Python Module
+[![klingon-serial unit tests](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml)
 [![Pre-PR Merge CI](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml) [![.github/workflows/post-pr-merge.yaml](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml)
 ## Overview
 
 The `klingon_serial` Python module is designed to generate a unique hexadecimal
 serial number, avoiding serial conflicts in a distributed environment. The
 serial number is a concatenation of the machine's MAC address, the process ID
 (PID), and the current time in epoch format with millisecond precision. The
```

### Comparing `klingon-serial-0.1.14/klingon_serial/generate.py` & `klingon-serial-0.1.15/klingon_serial/generate.py`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/klingon_serial/utils.py` & `klingon-serial-0.1.15/klingon_serial/utils.py`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/klingon_serial.egg-info/PKG-INFO` & `klingon-serial-0.1.15/klingon_serial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klingon-serial
-Version: 0.1.14
+Version: 0.1.15
 Summary: Get a globally unique serial
 Home-page: https://github.com/djh00t/module_klingon_serial
 Author: David Hooton
 Author-email: klingon_serial+david@hooton.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
 Requires-Dist: pytest>=6.0
 Requires-Dist: str2bool
 
 # Klingon Serial Python Module
+[![klingon-serial unit tests](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/klingon-serial-unit-tests.yaml)
 [![Pre-PR Merge CI](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/pre-pr-merge.yaml) [![.github/workflows/post-pr-merge.yaml](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml/badge.svg)](https://github.com/djh00t/module_klingon_serial/actions/workflows/post-pr-merge.yaml)
 ## Overview
 
 The `klingon_serial` Python module is designed to generate a unique hexadecimal
 serial number, avoiding serial conflicts in a distributed environment. The
 serial number is a concatenation of the machine's MAC address, the process ID
 (PID), and the current time in epoch format with millisecond precision. The
```

### Comparing `klingon-serial-0.1.14/setup.py` & `klingon-serial-0.1.15/setup.py`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/tests/test_klingon_get_serial.py` & `klingon-serial-0.1.15/tests/test_klingon_get_serial.py`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/tests/test_klingon_strtobool.py` & `klingon-serial-0.1.15/tests/test_klingon_strtobool.py`

 * *Files identical despite different names*

### Comparing `klingon-serial-0.1.14/tests/test_klingon_utils.py` & `klingon-serial-0.1.15/tests/test_klingon_utils.py`

 * *Files identical despite different names*

