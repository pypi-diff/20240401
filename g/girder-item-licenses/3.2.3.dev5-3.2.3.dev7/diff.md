# Comparing `tmp/girder-item-licenses-3.2.3.dev5.tar.gz` & `tmp/girder-item-licenses-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-item-licenses-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:19 2024, max compression
+gzip compressed data, was "girder-item-licenses-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:42 2024, max compression
```

## Comparing `girder-item-licenses-3.2.3.dev5.tar` & `girder-item-licenses-3.2.3.dev7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.979163 girder-item-licenses-3.2.3.dev5/girder_item_licenses/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.979163 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.979163 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.979163 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/ItemLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/SelectLicenseWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/UploadWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 15:49:19.000000 girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/plugin_tests/itemLicensesSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/plugin_tests/item_licenses_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:19.983163 girder-item-licenses-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-02-14 15:48:27.000000 girder-item-licenses-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.593322 girder-item-licenses-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-02-14 18:47:42.593322 girder-item-licenses-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2831 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4514 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/templates/itemLicenseWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/templates/selectLicenseWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2499 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1480 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/EditItemWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/HierarchyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/ItemLicenseWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1047 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/SelectLicenseWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1576 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/UploadWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      519 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 18:47:42.000000 girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:42.589322 girder-item-licenses-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/plugin_tests/itemLicensesSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12348 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/plugin_tests/item_licenses_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:42.593322 girder-item-licenses-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1599 2024-02-14 18:46:47.000000 girder-item-licenses-3.2.3.dev7/setup.py
```

### Comparing `girder-item-licenses-3.2.3.dev5/PKG-INFO` & `girder-item-licenses-3.2.3.dev7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Add a license field to items.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/__init__.py` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/rest.py` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/rest.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/settings.py` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/settings.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/ConfigView.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/EditItemWidget.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/HierarchyWidget.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/ItemView.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/SelectLicenseWidget.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/SelectLicenseWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses/web_client/views/UploadWidget.js` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/PKG-INFO` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-item-licenses
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Add a license field to items.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-item-licenses-3.2.3.dev5/girder_item_licenses.egg-info/SOURCES.txt` & `girder-item-licenses-3.2.3.dev7/girder_item_licenses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/plugin_tests/itemLicensesSpec.js` & `girder-item-licenses-3.2.3.dev7/plugin_tests/itemLicensesSpec.js`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/plugin_tests/item_licenses_test.py` & `girder-item-licenses-3.2.3.dev7/plugin_tests/item_licenses_test.py`

 * *Files identical despite different names*

### Comparing `girder-item-licenses-3.2.3.dev5/setup.py` & `girder-item-licenses-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

