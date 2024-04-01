# Comparing `tmp/girder-dicom-viewer-3.2.3.dev5.tar.gz` & `tmp/girder-dicom-viewer-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-dicom-viewer-3.2.3.dev5.tar", last modified: Wed Feb 14 15:48:54 2024, max compression
+gzip compressed data, was "girder-dicom-viewer-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:17 2024, max compression
```

## Comparing `girder-dicom-viewer-3.2.3.dev5.tar` & `girder-dicom-viewer-3.2.3.dev7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.491028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9428 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/event_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1286 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/templates/dicomItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13597 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/views/DicomView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/webpack.helper.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-02-14 15:48:54.000000 girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/data/000000.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/data/000001.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/data/000002.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/data/000003.dcm.sha512
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11077 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/plugin_tests/dicom_viewer_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:48:54.495028 girder-dicom-viewer-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 15:48:26.000000 girder-dicom-viewer-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.297281 girder-dicom-viewer-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-02-14 18:47:17.297281 girder-dicom-viewer-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.289281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9428 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/event_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.293281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.293281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/stylesheets/dicomItem.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/stylesheets/dicomSliceMetadata.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.293281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1286 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/templates/dicomItem.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/templates/dicomSliceMetadata.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/templates/parseDicomItem.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.293281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13597 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/views/DicomView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      686 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/webpack.helper.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.297281 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-02-14 18:47:17.000000 girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.293281 girder-dicom-viewer-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:17.297281 girder-dicom-viewer-3.2.3.dev7/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/data/000000.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/data/000001.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/data/000002.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/data/000003.dcm.sha512
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11077 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/plugin_tests/dicom_viewer_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:17.297281 girder-dicom-viewer-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-02-14 18:46:47.000000 girder-dicom-viewer-3.2.3.dev7/setup.py
```

### Comparing `girder-dicom-viewer-3.2.3.dev5/PKG-INFO` & `girder-dicom-viewer-3.2.3.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-dicom-viewer
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: View DICOM images in the browser
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#dicom-viewer
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/__init__.py` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/event_helper.py` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/event_helper.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/main.js` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/package.json` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/templates/dicomItem.pug` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/templates/dicomItem.pug`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/views/DicomView.js` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/views/DicomView.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer/web_client/webpack.helper.js` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer/web_client/webpack.helper.js`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/PKG-INFO` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-dicom-viewer
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: View DICOM images in the browser
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#dicom-viewer
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-dicom-viewer-3.2.3.dev5/girder_dicom_viewer.egg-info/SOURCES.txt` & `girder-dicom-viewer-3.2.3.dev7/girder_dicom_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/plugin_tests/dicom_viewer_test.py` & `girder-dicom-viewer-3.2.3.dev7/plugin_tests/dicom_viewer_test.py`

 * *Files identical despite different names*

### Comparing `girder-dicom-viewer-3.2.3.dev5/setup.py` & `girder-dicom-viewer-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

