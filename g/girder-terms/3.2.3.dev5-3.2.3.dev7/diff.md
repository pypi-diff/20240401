# Comparing `tmp/girder-terms-3.2.3.dev5.tar.gz` & `tmp/girder-terms-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-terms-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:41 2024, max compression
+gzip compressed data, was "girder-terms-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:07 2024, max compression
```

## Comparing `girder-terms-3.2.3.dev5.tar` & `girder-terms-3.2.3.dev7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.443271 girder-terms-3.2.3.dev5/girder_terms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/girder_terms/web_client/views/TermsAcceptanceView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/girder_terms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1054 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-14 15:49:41.000000 girder-terms-3.2.3.dev5/girder_terms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:41.447271 girder-terms-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-02-14 15:48:27.000000 girder-terms-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.685355 girder-terms-3.2.3.dev7/girder_terms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.685355 girder-terms-3.2.3.dev7/girder_terms/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/girder_terms/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/girder_terms/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/stylesheets/termsAcceptance.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/girder_terms/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/templates/collectionInfoWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/templates/editCollectionTermsWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/templates/termsAcceptance.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/girder_terms/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/views/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/views/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/girder_terms/web_client/views/TermsAcceptanceView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/girder_terms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1054 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-14 18:48:07.000000 girder-terms-3.2.3.dev7/girder_terms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/plugin_tests/termsSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/plugin_tests/terms_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:07.689355 girder-terms-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-02-14 18:46:47.000000 girder-terms-3.2.3.dev7/setup.py
```

### Comparing `girder-terms-3.2.3.dev5/PKG-INFO` & `girder-terms-3.2.3.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-terms-3.2.3.dev5/girder_terms/__init__.py` & `girder-terms-3.2.3.dev7/girder_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/models/CollectionModel.js` & `girder-terms-3.2.3.dev7/girder_terms/web_client/models/CollectionModel.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/package.json` & `girder-terms-3.2.3.dev7/girder_terms/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/routes.js` & `girder-terms-3.2.3.dev7/girder_terms/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/views/CollectionInfoWidget.js` & `girder-terms-3.2.3.dev7/girder_terms/web_client/views/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/views/EditCollectionWidget.js` & `girder-terms-3.2.3.dev7/girder_terms/web_client/views/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms/web_client/views/TermsAcceptanceView.js` & `girder-terms-3.2.3.dev7/girder_terms/web_client/views/TermsAcceptanceView.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/girder_terms.egg-info/PKG-INFO` & `girder-terms-3.2.3.dev7/girder_terms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-terms-3.2.3.dev5/girder_terms.egg-info/SOURCES.txt` & `girder-terms-3.2.3.dev7/girder_terms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/plugin_tests/termsSpec.js` & `girder-terms-3.2.3.dev7/plugin_tests/termsSpec.js`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/plugin_tests/terms_test.py` & `girder-terms-3.2.3.dev7/plugin_tests/terms_test.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.3.dev5/setup.py` & `girder-terms-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

