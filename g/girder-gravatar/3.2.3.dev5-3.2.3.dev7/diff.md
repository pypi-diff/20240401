# Comparing `tmp/girder-gravatar-3.2.3.dev5.tar.gz` & `tmp/girder-gravatar-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-gravatar-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:07 2024, max compression
+gzip compressed data, was "girder-gravatar-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:31 2024, max compression
```

## Comparing `girder-gravatar-3.2.3.dev5.tar` & `girder-gravatar-3.2.3.dev7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.335098 girder-gravatar-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-02-14 15:49:07.000000 girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:07.331098 girder-gravatar-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:07.335098 girder-gravatar-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-02-14 15:48:26.000000 girder-gravatar-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.089302 girder-gravatar-3.2.3.dev7/girder_gravatar/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-02-14 18:47:31.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-02-14 18:47:30.000000 girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/plugin_tests/gravatar_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:31.093302 girder-gravatar-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-02-14 18:46:47.000000 girder-gravatar-3.2.3.dev7/setup.py
```

### Comparing `girder-gravatar-3.2.3.dev5/PKG-INFO` & `girder-gravatar-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar/__init__.py` & `girder-gravatar-3.2.3.dev7/girder_gravatar/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/package.json` & `girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/templates/configView.pug` & `girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar/web_client/views/ConfigView.js` & `girder-gravatar-3.2.3.dev7/girder_gravatar/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/PKG-INFO` & `girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-gravatar-3.2.3.dev5/girder_gravatar.egg-info/SOURCES.txt` & `girder-gravatar-3.2.3.dev7/girder_gravatar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/plugin_tests/gravatar_test.py` & `girder-gravatar-3.2.3.dev7/plugin_tests/gravatar_test.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.3.dev5/setup.py` & `girder-gravatar-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

