# Comparing `tmp/girder-user-quota-3.2.3.dev5.tar.gz` & `tmp/girder-user-quota-3.2.3.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-user-quota-3.2.3.dev5.tar", last modified: Wed Feb 14 15:49:49 2024, max compression
+gzip compressed data, was "girder-user-quota-3.2.3.dev7.tar", last modified: Wed Feb 14 18:48:15 2024, max compression
```

## Comparing `girder-user-quota-3.2.3.dev5.tar` & `girder-user-quota-3.2.3.dev7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.955314 girder-user-quota-3.2.3.dev5/girder_user_quota/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.955314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.955314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/models/extendModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.955314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/extendView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1424 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 15:49:49.000000 girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 15:49:49.959314 girder-user-quota-3.2.3.dev5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-02-14 15:48:27.000000 girder-user-quota-3.2.3.dev5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.369375 girder-user-quota-3.2.3.dev7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 18:48:15.369375 girder-user-quota-3.2.3.dev7/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.361374 girder-user-quota-3.2.3.dev7/girder_user_quota/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/quota.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/main.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/models/extendModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/stylesheets/userQuota.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/utilities/Conversions.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/CollectionView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/UploadWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/UserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/extendView.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1424 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-02-14 18:48:15.000000 girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:48:15.365375 girder-user-quota-3.2.3.dev7/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/plugin_tests/userQuotaSpec.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/plugin_tests/user_quota_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-14 18:48:15.369375 girder-user-quota-3.2.3.dev7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-02-14 18:46:47.000000 girder-user-quota-3.2.3.dev7/setup.py
```

### Comparing `girder-user-quota-3.2.3.dev5/PKG-INFO` & `girder-user-quota-3.2.3.dev7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/__init__.py` & `girder-user-quota-3.2.3.dev7/girder_user_quota/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/quota.py` & `girder-user-quota-3.2.3.dev7/girder_user_quota/quota.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/settings.py` & `girder-user-quota-3.2.3.dev7/girder_user_quota/settings.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/models/extendModel.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/models/extendModel.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/package.json` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/configView.pug` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/utilities/Conversions.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/utilities/Conversions.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/ConfigView.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/QuotaPoliciesWidget.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/QuotaPoliciesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/UploadWidget.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota/web_client/views/extendView.js` & `girder-user-quota-3.2.3.dev7/girder_user_quota/web_client/views/extendView.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/PKG-INFO` & `girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.2.3.dev5
+Version: 3.2.3.dev7
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-user-quota-3.2.3.dev5/girder_user_quota.egg-info/SOURCES.txt` & `girder-user-quota-3.2.3.dev7/girder_user_quota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/plugin_tests/userQuotaSpec.js` & `girder-user-quota-3.2.3.dev7/plugin_tests/userQuotaSpec.js`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/plugin_tests/user_quota_test.py` & `girder-user-quota-3.2.3.dev7/plugin_tests/user_quota_test.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.3.dev5/setup.py` & `girder-user-quota-3.2.3.dev7/setup.py`

 * *Files identical despite different names*

