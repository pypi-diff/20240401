# Comparing `tmp/girder-sentry-3.2.3.dev5.tar.gz` & `tmp/girder-sentry-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-sentry-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:37 2024, max compression
+gzip compressed data, was "girder-sentry-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:04 2024, max compression
```

## Comparing `girder-sentry-3.2.3.dev5.tar` & `girder-sentry-3.2.3.dev7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.535250 girder-sentry-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 15:49:37.535250 girder-sentry-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.531250 girder-sentry-3.2.3.dev5/girder_sentry/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.531250 girder-sentry-3.2.3.dev5/girder_sentry/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.531250 girder-sentry-3.2.3.dev5/girder_sentry/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.531250 girder-sentry-3.2.3.dev5/girder_sentry/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.531250 girder-sentry-3.2.3.dev5/girder_sentry/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/girder_sentry/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:37.535250 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 15:49:37.000000 girder-sentry-3.2.3.dev5/girder_sentry.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/plugin.cmake
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:37.535250 girder-sentry-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-02-14 15:48:27.000000 girder-sentry-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2728 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/girder_sentry/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      569 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-14 18:48:04.000000 girder-sentry-3.2.3.dev7/girder_sentry.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/plugin.cmake
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:04.841351 girder-sentry-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1639 2024-02-14 18:46:47.000000 girder-sentry-3.2.3.dev7/setup.py
```

### Comparing `girder-sentry-3.2.3.dev5/PKG-INFO` & `girder-sentry-3.2.3.dev7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow the automatic tracking of issues using Sentry.
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry/rest.py` & `girder-sentry-3.2.3.dev7/girder_sentry/rest.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry/settings.py` & `girder-sentry-3.2.3.dev7/girder_sentry/settings.py`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry/web_client/package.json` & `girder-sentry-3.2.3.dev7/girder_sentry/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry/web_client/templates/configView.pug` & `girder-sentry-3.2.3.dev7/girder_sentry/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry/web_client/views/ConfigView.js` & `girder-sentry-3.2.3.dev7/girder_sentry/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry.egg-info/PKG-INFO` & `girder-sentry-3.2.3.dev7/girder_sentry.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-sentry
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow the automatic tracking of issues using Sentry.
 Maintainer: Kitware, Inc.
 Maintainer-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-sentry-3.2.3.dev5/girder_sentry.egg-info/SOURCES.txt` & `girder-sentry-3.2.3.dev7/girder_sentry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-sentry-3.2.3.dev5/setup.py` & `girder-sentry-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

