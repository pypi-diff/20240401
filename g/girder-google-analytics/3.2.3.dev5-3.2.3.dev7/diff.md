# Comparing `tmp/girder-google-analytics-3.2.3.dev5.tar.gz` & `tmp/girder-google-analytics-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-google-analytics-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:03 2024, max compression
+gzip compressed data, was "girder-google-analytics-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:27 2024, max compression
```

## Comparing `girder-google-analytics-3.2.3.dev5.tar` & `girder-google-analytics-3.2.3.dev7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.371076 girder-google-analytics-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      627 2024-02-14 15:49:03.371076 girder-google-analytics-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/lib/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/lib/backbone.analytics.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2186 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.371076 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      627 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 15:49:03.000000 girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:03.367076 girder-google-analytics-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/plugin_tests/google_analytics_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:03.371076 girder-google-analytics-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-02-14 15:48:26.000000 girder-google-analytics-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      627 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.257296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/lib/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2295 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/lib/backbone.analytics.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      453 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2186 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      627 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-02-14 18:47:27.000000 girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/plugin_tests/google_analytics_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:27.261296 girder-google-analytics-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-02-14 18:46:47.000000 girder-google-analytics-3.2.3.dev7/setup.py
```

### Comparing `girder-google-analytics-3.2.3.dev5/PKG-INFO` & `girder-google-analytics-3.2.3.dev7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-google-analytics
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow the tracking of page views via Google Analytics.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#google-analytics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/rest.py` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/rest.py`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/lib/backbone.analytics.js` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/lib/backbone.analytics.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/main.js` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/package.json` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/templates/configView.pug` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics/web_client/views/ConfigView.js` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/PKG-INFO` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-google-analytics
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow the tracking of page views via Google Analytics.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#google-analytics
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-google-analytics-3.2.3.dev5/girder_google_analytics.egg-info/SOURCES.txt` & `girder-google-analytics-3.2.3.dev7/girder_google_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/plugin_tests/google_analytics_test.py` & `girder-google-analytics-3.2.3.dev7/plugin_tests/google_analytics_test.py`

 * *Files identical despite different names*

### Comparing `girder-google-analytics-3.2.3.dev5/setup.py` & `girder-google-analytics-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

