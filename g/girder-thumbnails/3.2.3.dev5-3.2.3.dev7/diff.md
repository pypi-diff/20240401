# Comparing `tmp/girder-thumbnails-3.2.3.dev5.tar.gz` & `tmp/girder-thumbnails-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-thumbnails-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:45 2024, max compression
+gzip compressed data, was "girder-thumbnails-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:12 2024, max compression
```

## Comparing `girder-thumbnails-3.2.3.dev5.tar` & `girder-thumbnails-3.2.3.dev7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.611292 girder-thumbnails-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-02-14 15:49:45.611292 girder-thumbnails-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/models/ThumbnailModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 15:49:45.000000 girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:45.607292 girder-thumbnails-3.2.3.dev5/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:45.611292 girder-thumbnails-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-14 15:48:27.000000 girder-thumbnails-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.309361 girder-thumbnails-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-02-14 18:48:12.309361 girder-thumbnails-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/models/ThumbnailModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/stylesheets/flowView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/flowView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/itemView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/CreateThumbnailView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/FileListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/FlowView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails/worker.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.309361 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 18:48:12.000000 girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.305361 girder-thumbnails-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/plugin_tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:12.309361 girder-thumbnails-3.2.3.dev7/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/plugin_tests/data/sample_dicom.dcm
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/plugin_tests/thumbnail_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/plugin_tests/thumbnailsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:12.309361 girder-thumbnails-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-02-14 18:46:47.000000 girder-thumbnails-3.2.3.dev7/setup.py
```

### Comparing `girder-thumbnails-3.2.3.dev5/PKG-INFO` & `girder-thumbnails-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Generate thumbnails from files.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/__init__.py` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/rest.py` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/rest.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/utils.py` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/utils.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/package.json` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/CreateThumbnailView.js` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/CreateThumbnailView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/FileListWidget.js` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/FlowView.js` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/FlowView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/web_client/views/ItemView.js` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails/worker.py` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails/worker.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/PKG-INFO` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Generate thumbnails from files.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-thumbnails-3.2.3.dev5/girder_thumbnails.egg-info/SOURCES.txt` & `girder-thumbnails-3.2.3.dev7/girder_thumbnails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/plugin_tests/data/sample_dicom.dcm` & `girder-thumbnails-3.2.3.dev7/plugin_tests/data/sample_dicom.dcm`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/plugin_tests/thumbnail_test.py` & `girder-thumbnails-3.2.3.dev7/plugin_tests/thumbnail_test.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/plugin_tests/thumbnailsSpec.js` & `girder-thumbnails-3.2.3.dev7/plugin_tests/thumbnailsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.3.dev5/setup.py` & `girder-thumbnails-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

