# Comparing `tmp/girder-ldap-3.2.3.dev5.tar.gz` & `tmp/girder-ldap-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-ldap-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:27 2024, max compression
+gzip compressed data, was "girder-ldap-3.2.3.dev7.tar", last modified: Wed Feb 14 18:47:49 2024, max compression
```

## Comparing `girder-ldap-3.2.3.dev5.tar` & `girder-ldap-3.2.3.dev7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.531200 girder-ldap-3.2.3.dev5/girder_ldap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.531200 girder-ldap-3.2.3.dev5/girder_ldap/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.531200 girder-ldap-3.2.3.dev5/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/girder_ldap/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      716 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 15:49:27.000000 girder-ldap-3.2.3.dev5/girder_ldap.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:27.535199 girder-ldap-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-02-14 15:48:27.000000 girder-ldap-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/stylesheets/configView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/editServerMixin.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/newServerTemplate.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/girder_ldap/web_client/views/ConfigView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      716 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-02-14 18:47:49.000000 girder-ldap-3.2.3.dev7/girder_ldap.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/plugin_tests/ldap_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:47:49.457331 girder-ldap-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-02-14 18:46:47.000000 girder-ldap-3.2.3.dev7/setup.py
```

### Comparing `girder-ldap-3.2.3.dev5/PKG-INFO` & `girder-ldap-3.2.3.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/__init__.py` & `girder-ldap-3.2.3.dev7/girder_ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/settings.py` & `girder-ldap-3.2.3.dev7/girder_ldap/settings.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/web_client/package.json` & `girder-ldap-3.2.3.dev7/girder_ldap/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/configView.pug` & `girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/web_client/templates/editServerMixin.pug` & `girder-ldap-3.2.3.dev7/girder_ldap/web_client/templates/editServerMixin.pug`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap/web_client/views/ConfigView.js` & `girder-ldap-3.2.3.dev7/girder_ldap/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap.egg-info/PKG-INFO` & `girder-ldap-3.2.3.dev7/girder_ldap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-ldap-3.2.3.dev5/girder_ldap.egg-info/SOURCES.txt` & `girder-ldap-3.2.3.dev7/girder_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/plugin_tests/ldap_test.py` & `girder-ldap-3.2.3.dev7/plugin_tests/ldap_test.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.3.dev5/setup.py` & `girder-ldap-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

