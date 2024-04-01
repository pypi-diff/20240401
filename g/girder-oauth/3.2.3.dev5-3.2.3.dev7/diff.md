# Comparing `tmp/girder-oauth-3.2.3.dev5.tar.gz` & `tmp/girder-oauth-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-oauth-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:31 2024, max compression
+gzip compressed data, was "girder-oauth-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:53 2024, max compression
```

## Comparing `girder-oauth-3.2.3.dev5.tar` & `girder-oauth-3.2.3.dev7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.079217 girder-oauth-3.2.3.dev5/girder_oauth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.079217 girder-oauth-3.2.3.dev5/girder_oauth/providers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/linkedin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/providers/microsoft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.079217 girder-oauth-3.2.3.dev5/girder_oauth/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.079217 girder-oauth-3.2.3.dev5/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.079217 girder-oauth-3.2.3.dev5/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/RegisterView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1193 2024-02-14 15:49:31.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-14 15:49:30.000000 girder-oauth-3.2.3.dev5/girder_oauth.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:31.083217 girder-oauth-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-02-14 15:48:27.000000 girder-oauth-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.429336 girder-oauth-3.2.3.dev7/girder_oauth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.429336 girder-oauth-3.2.3.dev7/girder_oauth/providers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/bitbucket.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/box.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/github.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/globus.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/google.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/linkedin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/providers/microsoft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.429336 girder-oauth-3.2.3.dev7/girder_oauth/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.429336 girder-oauth-3.2.3.dev7/girder_oauth/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/stylesheets/configView.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/stylesheets/oauthLoginView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/girder_oauth/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/templates/oauthLoginView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/LoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/OAuthLoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/RegisterView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1193 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-02-14 18:47:53.000000 girder-oauth-3.2.3.dev7/girder_oauth.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/plugin_tests/oauth_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:53.433336 girder-oauth-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-02-14 18:46:47.000000 girder-oauth-3.2.3.dev7/setup.py
```

### Comparing `girder-oauth-3.2.3.dev5/PKG-INFO` & `girder-oauth-3.2.3.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/__init__.py` & `girder-oauth-3.2.3.dev7/girder_oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/base.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/base.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/bitbucket.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/bitbucket.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/box.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/box.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/github.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/github.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/globus.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/globus.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/google.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/google.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/linkedin.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/linkedin.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/providers/microsoft.py` & `girder-oauth-3.2.3.dev7/girder_oauth/providers/microsoft.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/rest.py` & `girder-oauth-3.2.3.dev7/girder_oauth/rest.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/settings.py` & `girder-oauth-3.2.3.dev7/girder_oauth/settings.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/main.js` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/main.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/package.json` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/stylesheets/oauthLoginView.styl` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/stylesheets/oauthLoginView.styl`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/templates/configView.pug` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/ConfigView.js` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/OAuthLoginView.js` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/OAuthLoginView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth/web_client/views/RegisterView.js` & `girder-oauth-3.2.3.dev7/girder_oauth/web_client/views/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth.egg-info/PKG-INFO` & `girder-oauth-3.2.3.dev7/girder_oauth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-oauth-3.2.3.dev5/girder_oauth.egg-info/SOURCES.txt` & `girder-oauth-3.2.3.dev7/girder_oauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/plugin_tests/oauth_test.py` & `girder-oauth-3.2.3.dev7/plugin_tests/oauth_test.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.3.dev5/setup.py` & `girder-oauth-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

