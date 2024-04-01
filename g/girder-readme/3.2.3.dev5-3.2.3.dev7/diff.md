# Comparing `tmp/girder-readme-3.2.3.dev5.tar.gz` & `tmp/girder-readme-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-readme-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:34 2024, max compression
+gzip compressed data, was "girder-readme-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:01 2024, max compression
```

## Comparing `girder-readme-3.2.3.dev5.tar` & `girder-readme-3.2.3.dev7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.959237 girder-readme-3.2.3.dev5/girder_readme/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/girder_readme/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/girder_readme/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/web_client/stylesheets/readmeWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/girder_readme/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/web_client/templates/readmeWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/girder_readme/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/girder_readme/web_client/views/HierarchyWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/girder_readme.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 15:49:34.000000 girder-readme-3.2.3.dev5/girder_readme.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/plugin_tests/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/plugin_tests/data/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/plugin_tests/readmeSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:34.963237 girder-readme-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-02-14 15:48:27.000000 girder-readme-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.137346 girder-readme-3.2.3.dev7/girder_readme/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/girder_readme/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      470 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/girder_readme/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/web_client/stylesheets/readmeWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/girder_readme/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      101 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/web_client/templates/readmeWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/girder_readme/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      997 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/girder_readme/web_client/views/HierarchyWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/girder_readme.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 18:48:01.000000 girder-readme-3.2.3.dev7/girder_readme.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/plugin_tests/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/plugin_tests/data/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/plugin_tests/readmeSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:01.141346 girder-readme-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2024-02-14 18:46:47.000000 girder-readme-3.2.3.dev7/setup.py
```

### Comparing `girder-readme-3.2.3.dev5/PKG-INFO` & `girder-readme-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Render READMEs from the folder view
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-readme-3.2.3.dev5/girder_readme/rest.py` & `girder-readme-3.2.3.dev7/girder_readme/rest.py`

 * *Files identical despite different names*

### Comparing `girder-readme-3.2.3.dev5/girder_readme/web_client/views/HierarchyWidget.js` & `girder-readme-3.2.3.dev7/girder_readme/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-readme-3.2.3.dev5/girder_readme.egg-info/PKG-INFO` & `girder-readme-3.2.3.dev7/girder_readme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-readme
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Render READMEs from the folder view
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-readme-3.2.3.dev5/girder_readme.egg-info/SOURCES.txt` & `girder-readme-3.2.3.dev7/girder_readme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-readme-3.2.3.dev5/plugin_tests/readmeSpec.js` & `girder-readme-3.2.3.dev7/plugin_tests/readmeSpec.js`

 * *Files identical despite different names*

### Comparing `girder-readme-3.2.3.dev5/setup.py` & `girder-readme-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

