# Comparing `tmp/girder-autojoin-3.2.3.dev5.tar.gz` & `tmp/girder-autojoin-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-autojoin-3.2.3.dev5.tar", last modified: Wed Feb 14 15:48:50 2024, max compression
+gzip compressed data, was "girder-autojoin-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:13 2024, max compression
```

## Comparing `girder-autojoin-3.2.3.dev5.tar` & `girder-autojoin-3.2.3.dev7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-02-14 15:48:50.000000 girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:48:50.939009 girder-autojoin-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-02-14 15:48:26.000000 girder-autojoin-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.893276 girder-autojoin-3.2.3.dev7/girder_autojoin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.893276 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.893276 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.893276 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/templates/configView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-02-14 18:47:13.000000 girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/plugin_tests/autojoinSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/plugin_tests/autojoin_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:13.897276 girder-autojoin-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-02-14 18:46:47.000000 girder-autojoin-3.2.3.dev7/setup.py
```

### Comparing `girder-autojoin-3.2.3.dev5/PKG-INFO` & `girder-autojoin-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin/__init__.py` & `girder-autojoin-3.2.3.dev7/girder_autojoin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin/settings.py` & `girder-autojoin-3.2.3.dev7/girder_autojoin/settings.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/package.json` & `girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/templates/configView.pug` & `girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin/web_client/views/ConfigView.js` & `girder-autojoin-3.2.3.dev7/girder_autojoin/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/PKG-INFO` & `girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-autojoin-3.2.3.dev5/girder_autojoin.egg-info/SOURCES.txt` & `girder-autojoin-3.2.3.dev7/girder_autojoin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/plugin_tests/autojoinSpec.js` & `girder-autojoin-3.2.3.dev7/plugin_tests/autojoinSpec.js`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/plugin_tests/autojoin_test.py` & `girder-autojoin-3.2.3.dev7/plugin_tests/autojoin_test.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.3.dev5/setup.py` & `girder-autojoin-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

