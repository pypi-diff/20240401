# Comparing `tmp/girder-virtual-folders-3.2.3.dev5.tar.gz` & `tmp/girder-virtual-folders-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-virtual-folders-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:54 2024, max compression
+gzip compressed data, was "girder-virtual-folders-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:19 2024, max compression
```

## Comparing `girder-virtual-folders-3.2.3.dev5.tar` & `girder-virtual-folders-3.2.3.dev7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-02-14 15:48:27.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2024-02-14 15:49:53.000000 girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-02-14 15:48:27.000000 girder-virtual-folders-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-virtual-folders-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-02-14 15:48:27.000000 girder-virtual-folders-3.2.3.dev5/plugin_tests/virtual_folders_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:54.023334 girder-virtual-folders-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-02-14 15:48:27.000000 girder-virtual-folders-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:19.529411 girder-virtual-folders-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 18:48:19.529411 girder-virtual-folders-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:19.525411 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8194 2024-02-14 18:46:47.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:19.529411 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2024-02-14 18:48:19.000000 girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-02-14 18:46:47.000000 girder-virtual-folders-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:19.529411 girder-virtual-folders-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-virtual-folders-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6178 2024-02-14 18:46:47.000000 girder-virtual-folders-3.2.3.dev7/plugin_tests/virtual_folders_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:19.529411 girder-virtual-folders-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1645 2024-02-14 18:46:47.000000 girder-virtual-folders-3.2.3.dev7/setup.py
```

### Comparing `girder-virtual-folders-3.2.3.dev5/PKG-INFO` & `girder-virtual-folders-3.2.3.dev7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows folders to list child items using arbitrary database queries
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-virtual-folders-3.2.3.dev5/girder_virtual_folders/__init__.py` & `girder-virtual-folders-3.2.3.dev7/girder_virtual_folders/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.2.3.dev5/girder_virtual_folders.egg-info/PKG-INFO` & `girder-virtual-folders-3.2.3.dev7/girder_virtual_folders.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-virtual-folders
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows folders to list child items using arbitrary database queries
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-virtual-folders-3.2.3.dev5/plugin_tests/virtual_folders_test.py` & `girder-virtual-folders-3.2.3.dev7/plugin_tests/virtual_folders_test.py`

 * *Files identical despite different names*

### Comparing `girder-virtual-folders-3.2.3.dev5/setup.py` & `girder-virtual-folders-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

