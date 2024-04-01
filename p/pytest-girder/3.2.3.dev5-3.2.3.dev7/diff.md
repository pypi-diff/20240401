# Comparing `tmp/pytest-girder-3.2.3.dev5.tar.gz` & `tmp/pytest-girder-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-girder-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:57 2024, max compression
+gzip compressed data, was "pytest-girder-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:22 2024, max compression
```

## Comparing `pytest-girder-3.2.3.dev5.tar` & `pytest-girder-3.2.3.dev7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:57.867353 pytest-girder-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-02-14 15:49:57.867353 pytest-girder-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:57.863353 pytest-girder-3.2.3.dev5/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/pytest_girder/web_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:57.867353 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      440 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 15:49:57.000000 pytest-girder-3.2.3.dev5/pytest_girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:57.867353 pytest-girder-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-02-14 15:48:27.000000 pytest-girder-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:22.661415 pytest-girder-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-02-14 18:48:22.661415 pytest-girder-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:22.661415 pytest-girder-3.2.3.dev7/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6446 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11468 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/pytest_girder/web_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:22.661415 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      440 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       41 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 18:48:22.000000 pytest-girder-3.2.3.dev7/pytest_girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:22.661415 pytest-girder-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-02-14 18:46:47.000000 pytest-girder-3.2.3.dev7/setup.py
```

### Comparing `pytest-girder-3.2.3.dev5/LICENSE` & `pytest-girder-3.2.3.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/assertions.py` & `pytest-girder-3.2.3.dev7/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/fixtures.py` & `pytest-girder-3.2.3.dev7/pytest_girder/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/plugin.py` & `pytest-girder-3.2.3.dev7/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/plugin_registry.py` & `pytest-girder-3.2.3.dev7/pytest_girder/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/utils.py` & `pytest-girder-3.2.3.dev7/pytest_girder/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/pytest_girder/web_client.py` & `pytest-girder-3.2.3.dev7/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `pytest-girder-3.2.3.dev5/setup.py` & `pytest-girder-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

