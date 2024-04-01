# Comparing `tmp/britive-2.8.1.tar.gz` & `tmp/britive-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "britive-2.8.1.tar", last modified: Thu Sep 22 18:11:03 2022, max compression
+gzip compressed data, was "britive-2.9.0.tar", last modified: Fri Sep 30 13:18:03 2022, max compression
```

## Comparing `britive-2.8.1.tar` & `britive-2.9.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:11:03.577378 britive-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-22 18:10:51.000000 britive-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-09-22 18:11:03.577378 britive-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6955 2022-09-22 18:10:51.000000 britive-2.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-22 18:10:51.000000 britive-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-22 18:11:03.577378 britive-2.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:11:03.569378 britive-2.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:11:03.573378 britive-2.8.1/src/britive/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8003 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/api_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     6834 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/applications.py
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14426 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/britive.py
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/environment_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     5301 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/environments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/identity_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/identity_providers.py
--rw-r--r--   0 runner    (1001) docker     (121)    26314 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/my_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     7148 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/my_secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5646 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    30563 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/saml.py
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/scans.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/security_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     7104 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/service_identities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/service_identity_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     4744 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/task_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8425 2022-09-22 18:10:51.000000 britive-2.8.1/src/britive/users.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 18:11:03.577378 britive-2.8.1/src/britive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-09-22 18:11:03.000000 britive-2.8.1/src/britive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-09-22 18:11:03.000000 britive-2.8.1/src/britive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 18:11:03.000000 britive-2.8.1/src/britive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-22 18:11:03.000000 britive-2.8.1/src/britive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:18:03.138455 britive-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-30 13:17:53.000000 britive-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-09-30 13:18:03.138455 britive-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6955 2022-09-30 13:17:53.000000 britive-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-30 13:17:53.000000 britive-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-30 13:18:03.138455 britive-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:18:03.134455 britive-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:18:03.138455 britive-2.9.0/src/britive/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8003 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/api_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6834 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/applications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3004 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14643 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/britive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/environment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5301 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/environments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/identity_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/identity_providers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26314 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/my_access.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7148 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/my_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5646 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30563 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/saml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/scans.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7104 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/service_identities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/service_identity_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4744 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/task_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8425 2022-09-30 13:17:53.000000 britive-2.9.0/src/britive/users.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 13:18:03.138455 britive-2.9.0/src/britive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-09-30 13:18:03.000000 britive-2.9.0/src/britive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-09-30 13:18:03.000000 britive-2.9.0/src/britive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 13:18:03.000000 britive-2.9.0/src/britive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-30 13:18:03.000000 britive-2.9.0/src/britive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-30 13:18:03.000000 britive-2.9.0/src/britive.egg-info/top_level.txt
```

### Comparing `britive-2.8.1/LICENSE` & `britive-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/PKG-INFO` & `britive-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: britive
-Version: 2.8.1
+Version: 2.9.0
 Summary: A pure Python SDK for the Britive API
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `britive-2.8.1/README.md` & `britive-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/setup.cfg` & `britive-2.9.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = britive
-version = 2.8.1
+version = 2.9.0
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python SDK for the Britive API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers = 
@@ -13,14 +13,16 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
+install_requires = 
+	requests
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `britive-2.8.1/src/britive/accounts.py` & `britive-2.9.0/src/britive/accounts.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/api_tokens.py` & `britive-2.9.0/src/britive/api_tokens.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/applications.py` & `britive-2.9.0/src/britive/applications.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/audit_logs.py` & `britive-2.9.0/src/britive/audit_logs.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/britive.py` & `britive-2.9.0/src/britive/britive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import requests
+from requests.adapters import HTTPAdapter, Retry
 import json as native_json
 import pkg_resources
 from .users import Users
 from .service_identity_tokens import ServiceIdentityTokens
 from .service_identities import ServiceIdentities
 from .exceptions import TenantMissingError, TokenMissingError, RootEnvironmentGroupNotFound, allowed_exceptions
 from .tags import Tags
@@ -97,14 +98,16 @@
             raise TokenMissingError(
                 'Token not explicitly provided and could not be sourced '
                 f'from environment variable {BRITIVE_TOKEN_ENV_NAME}'
             )
 
         self.base_url = f'https://{self.tenant}.britive-app.com/api'
         self.session = requests.Session()
+        retries = Retry(total=5, backoff_factor=1, status_forcelist=[429, 500, 502, 503, 504])
+        self.session.mount('https://', HTTPAdapter(max_retries=retries))
 
         token_type = 'TOKEN' if len(self.__token) < 50 else 'Bearer'
 
         try:
             version = pkg_resources.get_distribution('britive').version
         except Exception:
             version = 'unknown'
```

### Comparing `britive-2.8.1/src/britive/environment_groups.py` & `britive-2.9.0/src/britive/environment_groups.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/environments.py` & `britive-2.9.0/src/britive/environments.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/exceptions.py` & `britive-2.9.0/src/britive/exceptions.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/groups.py` & `britive-2.9.0/src/britive/groups.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/identity_attributes.py` & `britive-2.9.0/src/britive/identity_attributes.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/identity_providers.py` & `britive-2.9.0/src/britive/identity_providers.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/my_access.py` & `britive-2.9.0/src/britive/my_access.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/my_secrets.py` & `britive-2.9.0/src/britive/my_secrets.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/notifications.py` & `britive-2.9.0/src/britive/notifications.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/permissions.py` & `britive-2.9.0/src/britive/permissions.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/policies.py` & `britive-2.9.0/src/britive/policies.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/profiles.py` & `britive-2.9.0/src/britive/profiles.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/reports.py` & `britive-2.9.0/src/britive/reports.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,25 +23,30 @@
         """
 
         params = {
             'type': 'report'
         }
         return self.britive.get(self.base_url, params=params)
 
-    def run(self, report_id: str, csv: bool = False) -> any:
+    def run(self, report_id: str, csv: bool = False, filter_expression: str = None) -> any:
         """
         Run a report.
 
         :param report_id: The ID of the report.
         :param csv: If True the result will be returned as a CSV string. If False (default) the result will be returned
             as a list where each time in the list is a dict representing the row of data.
+        :param filter_expression: The filter to apply to the report. It is left to the caller to provide a syntactically
+            correct filter expression string.
         :return: CSV string or list.
         """
 
-        csv_results = self.britive.get(f'{self.base_url}/{report_id}/csv')
+        params = {}
+        if filter_expression:
+            params['filter'] = filter_expression
+        csv_results = self.britive.get(f'{self.base_url}/{report_id}/csv', params=params)
 
         # convert csv to json - issue is that JSON response has max of 1k records returned so have to use CSV
         # as the base and convert to dict if the client asked for dict
         if csv:
             return csv_results
         else:
             dict_results = []
```

### Comparing `britive-2.8.1/src/britive/saml.py` & `britive-2.9.0/src/britive/saml.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/scans.py` & `britive-2.9.0/src/britive/scans.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/security_policies.py` & `britive-2.9.0/src/britive/security_policies.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/service_identities.py` & `britive-2.9.0/src/britive/service_identities.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/service_identity_tokens.py` & `britive-2.9.0/src/britive/service_identity_tokens.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/tags.py` & `britive-2.9.0/src/britive/tags.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/task_services.py` & `britive-2.9.0/src/britive/task_services.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/tasks.py` & `britive-2.9.0/src/britive/tasks.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive/users.py` & `britive-2.9.0/src/britive/users.py`

 * *Files identical despite different names*

### Comparing `britive-2.8.1/src/britive.egg-info/PKG-INFO` & `britive-2.9.0/src/britive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: britive
-Version: 2.8.1
+Version: 2.9.0
 Summary: A pure Python SDK for the Britive API
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `britive-2.8.1/src/britive.egg-info/SOURCES.txt` & `britive-2.9.0/src/britive.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 src/britive/tags.py
 src/britive/task_services.py
 src/britive/tasks.py
 src/britive/users.py
 src/britive.egg-info/PKG-INFO
 src/britive.egg-info/SOURCES.txt
 src/britive.egg-info/dependency_links.txt
+src/britive.egg-info/requires.txt
 src/britive.egg-info/top_level.txt
```

