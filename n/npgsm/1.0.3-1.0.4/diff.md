# Comparing `tmp/npgsm-1.0.3.tar.gz` & `tmp/npgsm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npgsm-1.0.3.tar", last modified: Wed Nov 30 08:06:32 2022, max compression
+gzip compressed data, was "npgsm-1.0.4.tar", last modified: Mon Apr  1 12:20:42 2024, max compression
```

## Comparing `npgsm-1.0.3.tar` & `npgsm-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2022-11-30 08:06:32.119966 npgsm-1.0.3/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1062 2022-11-22 09:12:45.000000 npgsm-1.0.3/LICENSE
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1249 2022-11-30 08:06:32.119966 npgsm-1.0.3/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      322 2022-11-30 08:04:51.000000 npgsm-1.0.3/README.md
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2022-11-30 08:06:32.119966 npgsm-1.0.3/npgsm/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      621 2022-11-22 09:13:58.000000 npgsm-1.0.3/npgsm/__init__.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2022-11-30 08:06:32.119966 npgsm-1.0.3/npgsm/core/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2022-11-22 09:12:30.000000 npgsm-1.0.3/npgsm/core/__init__.py
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     3910 2022-11-30 08:04:02.000000 npgsm-1.0.3/npgsm/core/tools.py
-drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2022-11-30 08:06:32.119966 npgsm-1.0.3/npgsm.egg-info/
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1249 2022-11-30 08:06:32.000000 npgsm-1.0.3/npgsm.egg-info/PKG-INFO
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      231 2022-11-30 08:06:32.000000 npgsm-1.0.3/npgsm.egg-info/SOURCES.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        1 2022-11-30 08:06:32.000000 npgsm-1.0.3/npgsm.egg-info/dependency_links.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)      103 2022-11-30 08:06:32.000000 npgsm-1.0.3/npgsm.egg-info/requires.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)        6 2022-11-30 08:06:32.000000 npgsm-1.0.3/npgsm.egg-info/top_level.txt
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)       38 2022-11-30 08:06:32.119966 npgsm-1.0.3/setup.cfg
--rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1474 2022-11-30 08:04:10.000000 npgsm-1.0.3/setup.py
+drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1062 2023-12-12 02:21:56.000000 npgsm-1.0.4/LICENSE
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1449 2024-04-01 12:20:42.146693 npgsm-1.0.4/PKG-INFO
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      341 2024-04-01 12:20:30.000000 npgsm-1.0.4/README.md
+drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm/
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      621 2023-12-12 02:21:56.000000 npgsm-1.0.4/npgsm/__init__.py
+drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm/core/
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)        0 2023-12-12 02:21:56.000000 npgsm-1.0.4/npgsm/core/__init__.py
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     5400 2024-04-01 12:08:49.000000 npgsm-1.0.4/npgsm/core/tools.py
+drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/npgsm.egg-info/
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1449 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/PKG-INFO
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      373 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/SOURCES.txt
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)        1 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/dependency_links.txt
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      103 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/requires.txt
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)        6 2024-04-01 12:20:42.000000 npgsm-1.0.4/npgsm.egg-info/top_level.txt
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)       38 2024-04-01 12:20:42.146693 npgsm-1.0.4/setup.cfg
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     1474 2024-04-01 12:19:56.000000 npgsm-1.0.4/setup.py
+drwxr-xr-x   0 nnopp     (1000) nnopp     (1000)        0 2024-04-01 12:20:42.146693 npgsm-1.0.4/tests/
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      576 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_create_delete.py
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      470 2024-04-01 12:13:15.000000 npgsm-1.0.4/tests/test_disable_secret.py
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      447 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_list_secret.py
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)      357 2024-04-01 12:15:24.000000 npgsm-1.0.4/tests/test_list_versions.py
+-rw-r--r--   0 nnopp     (1000) nnopp     (1000)     3099 2023-12-12 02:21:56.000000 npgsm-1.0.4/tests/test_remove_oldsecret.py
```

### Comparing `npgsm-1.0.3/LICENSE` & `npgsm-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `npgsm-1.0.3/PKG-INFO` & `npgsm-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgsm
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package that could help you manage your secrets in Google Secret Manager
 Home-page: https://github.com/noppGithub/npgsm
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,20 +15,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: google-cloud-secret-manager>=2.12.6
+Requires-Dist: google-cloud-logging>=3.2.5
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # NPGSM
 A helper package to work with Google Secret Manager
 This module is able to create, update, read and delete secrets in Google Secret Manager.
 
 ### Change log
 - 1.0.1: Added method to delete secret
 - 1.0.2: Updated the method to create new secret
 - 1.0.3: Added return to both success and failed of creating secret
+- 1.0.4: Bug fixes
```

### Comparing `npgsm-1.0.3/npgsm/__init__.py` & `npgsm-1.0.4/npgsm/__init__.py`

 * *Files identical despite different names*

### Comparing `npgsm-1.0.3/npgsm/core/tools.py` & `npgsm-1.0.4/npgsm/core/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 import os
 from typing import Optional
 
 import google.cloud.logging
 from google.api_core import exceptions
-from google.cloud import secretmanager
+from google.cloud import secretmanager, secretmanager_v1
 
 _MY_RETRIABLE_TYPES = (
     exceptions.TooManyRequests,  # 429
     exceptions.InternalServerError,  # 500
     exceptions.BadGateway,  # 502
     exceptions.ServiceUnavailable,  # 503
 )
@@ -78,16 +78,52 @@
         name = f"projects/{self.project_id}/secrets/{secret_id}/versions/{version_id}"
         # Access the secret version.
         response = self.client.access_secret_version(name=name)
         # Return the decoded payload.
         payload = response.payload.data.decode("UTF-8")  # type: ignore
         return payload
 
+    def get_versions(self,secret_id):
+        name = f"projects/{self.project_id}/secrets/{secret_id}"
+        request = secretmanager.ListSecretVersionsRequest(parent=name)
+        page_result = self.client.list_secret_versions(request=request)
+        # client.list_secret_versions(request={"parent": parent})
+        # Handle the response
+        versions = [v.name for v in page_result if v.state.name != 'DESTROYED']
+        return versions
+
     def delete_secret(self, secret_id):
         name = self.client.secret_path(self.project_id, secret_id)
         print(f"Deleting Secret: {name}")
         self.client.delete_secret(request={"name": name})
         print(f"Deleted secret {secret_id}")
 
-    # def secret_hash(secret_value):
-    #     # return the sha224 hash of the secret value
-    #     return hashlib.sha224(bytes(secret_value, "utf-8")).hexdigest()
+    def delete_secret_version(self,secret_name,version_id):
+        name = f"projects/{self.project_id}/secrets/{secret_name}/versions/{version_id}"
+        request = secretmanager.DestroySecretVersionRequest(
+            name=name,
+        )
+        response = self.client.destroy_secret_version(request=request)
+        print(response)
+
+    def disable_secret_version(self,secret_name,version_id):
+        name = f"projects/{self.project_id}/secrets/{secret_name}/versions/{version_id}"
+        request = secretmanager.DisableSecretVersionRequest(
+            name=name,
+        )
+        response = self.client.disable_secret_version(request=request)
+        print(response)
+
+    def list_secret(self, parent):
+        # parent = "projects/586562253728"
+        request = secretmanager_v1.ListSecretsRequest(
+            parent=parent,
+        )
+        data = self.client.list_secrets(request)
+        secrets = []
+        for secret in data:
+            secrets.append(secret.name.split("/")[-1])
+        return secrets
+
+    def secret_hash(self, secret_value):
+        # return the sha224 hash of the secret value
+        return hashlib.sha224(bytes(secret_value, "utf-8")).hexdigest()
```

### Comparing `npgsm-1.0.3/npgsm.egg-info/PKG-INFO` & `npgsm-1.0.4/npgsm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npgsm
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package that could help you manage your secrets in Google Secret Manager
 Home-page: https://github.com/noppGithub/npgsm
 Author: Nopporn Phantawee
 Author-email: n.phantawee@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,20 +15,25 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: google-cloud-secret-manager>=2.12.6
+Requires-Dist: google-cloud-logging>=3.2.5
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # NPGSM
 A helper package to work with Google Secret Manager
 This module is able to create, update, read and delete secrets in Google Secret Manager.
 
 ### Change log
 - 1.0.1: Added method to delete secret
 - 1.0.2: Updated the method to create new secret
 - 1.0.3: Added return to both success and failed of creating secret
+- 1.0.4: Bug fixes
```

### Comparing `npgsm-1.0.3/setup.py` & `npgsm-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="npgsm",
-    version="1.0.3",
+    version="1.0.4",
     description="A package that could help you manage your secrets in Google Secret Manager",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Nopporn Phantawee",
     author_email="n.phantawee@gmail.com",
     url="https://github.com/noppGithub/npgsm",
     license="MIT",
```

