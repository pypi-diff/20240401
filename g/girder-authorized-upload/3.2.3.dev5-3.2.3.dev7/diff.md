# Comparing `tmp/girder-authorized-upload-3.2.3.dev5.tar.gz` & `tmp/girder-authorized-upload-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-authorized-upload-3.2.3.dev5.tar", last modified: Wed Feb 14 15:48:46 2024, max compression
+gzip compressed data, was "girder-authorized-upload-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:10 2024, max compression
```

## Comparing `girder-authorized-upload-3.2.3.dev5.tar` & `girder-authorized-upload-3.2.3.dev7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.406984 girder-authorized-upload-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 15:48:46.406984 girder-authorized-upload-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.398984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.402984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.402984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.402984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.402984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.402984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.406984 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1240 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-02-14 15:48:46.000000 girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:46.406984 girder-authorized-upload-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:48:46.406984 girder-authorized-upload-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-02-14 15:48:26.000000 girder-authorized-upload-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.337270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/authorizeUpload.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/authorizedUpload.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/folderActions.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1240 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-02-14 18:47:10.000000 girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/plugin_tests/authorizedUploadSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/plugin_tests/upload_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:10.341270 girder-authorized-upload-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-02-14 18:46:47.000000 girder-authorized-upload-3.2.3.dev7/setup.py
```

### Comparing `girder-authorized-upload-3.2.3.dev5/PKG-INFO` & `girder-authorized-upload-3.2.3.dev7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/__init__.py` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/rest.py` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/rest.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/main.js` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/package.json` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/routes.js` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/authorizeUpload.pug` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/authorizeUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/templates/authorizedUpload.pug` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/templates/authorizedUpload.pug`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/views/AuthorizeUploadView.js` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/views/AuthorizeUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload/web_client/views/AuthorizedUploadView.js` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload/web_client/views/AuthorizedUploadView.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/PKG-INFO` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-authorized-upload-3.2.3.dev5/girder_authorized_upload.egg-info/SOURCES.txt` & `girder-authorized-upload-3.2.3.dev7/girder_authorized_upload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/plugin_tests/authorizedUploadSpec.js` & `girder-authorized-upload-3.2.3.dev7/plugin_tests/authorizedUploadSpec.js`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/plugin_tests/upload_test.py` & `girder-authorized-upload-3.2.3.dev7/plugin_tests/upload_test.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.3.dev5/setup.py` & `girder-authorized-upload-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

