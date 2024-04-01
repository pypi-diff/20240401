# Comparing `tmp/girder-hashsum-download-3.2.3.dev5.tar.gz` & `tmp/girder-hashsum-download-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-hashsum-download-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:11 2024, max compression
+gzip compressed data, was "girder-hashsum-download-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:34 2024, max compression
```

## Comparing `girder-hashsum-download-3.2.3.dev5.tar` & `girder-hashsum-download-3.2.3.dev7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.203119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/views/FileInfoWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 15:49:11.000000 girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-hashsum-download-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-02-14 15:48:27.000000 girder-hashsum-download-3.2.3.dev5/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-02-14 15:48:27.000000 girder-hashsum-download-3.2.3.dev5/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:11.207119 girder-hashsum-download-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-02-14 15:48:27.000000 girder-hashsum-download-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.797309 girder-hashsum-download-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-02-14 18:47:34.797309 girder-hashsum-download-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.793309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.793309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.793309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.793309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/templates/config.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.793309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/views/FileInfoWidget.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.797309 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 18:47:34.000000 girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:34.797309 girder-hashsum-download-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/plugin_tests/hashsumSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/plugin_tests/hashsum_download_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:34.797309 girder-hashsum-download-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-02-14 18:46:47.000000 girder-hashsum-download-3.2.3.dev7/setup.py
```

### Comparing `girder-hashsum-download-3.2.3.dev5/PKG-INFO` & `girder-hashsum-download-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/__init__.py` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/main.js` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/package.json` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/views/ConfigView.js` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download/web_client/views/FileInfoWidget.js` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download/web_client/views/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/PKG-INFO` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-hashsum-download-3.2.3.dev5/girder_hashsum_download.egg-info/SOURCES.txt` & `girder-hashsum-download-3.2.3.dev7/girder_hashsum_download.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/plugin_tests/hashsumSpec.js` & `girder-hashsum-download-3.2.3.dev7/plugin_tests/hashsumSpec.js`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/plugin_tests/hashsum_download_test.py` & `girder-hashsum-download-3.2.3.dev7/plugin_tests/hashsum_download_test.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.3.dev5/setup.py` & `girder-hashsum-download-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

