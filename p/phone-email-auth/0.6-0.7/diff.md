# Comparing `tmp/phone_email_auth-0.6.tar.gz` & `tmp/phone_email_auth-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_email_auth-0.6.tar", last modified: Mon Apr  1 11:42:44 2024, max compression
+gzip compressed data, was "phone_email_auth-0.7.tar", last modified: Mon Apr  1 12:36:21 2024, max compression
```

## Comparing `phone_email_auth-0.6.tar` & `phone_email_auth-0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:42:44.487408 phone_email_auth-0.6/
--rw-rw-rw-   0        0        0     1542 2024-04-01 09:14:40.000000 phone_email_auth-0.6/LICENSE
--rw-rw-rw-   0        0        0       61 2024-04-01 09:14:40.000000 phone_email_auth-0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1953 2024-04-01 11:42:44.486382 phone_email_auth-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2024-04-01 11:42:00.000000 phone_email_auth-0.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 11:42:44.476106 phone_email_auth-0.6/phone_email_auth/
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/admin.py
--rw-rw-rw-   0        0        0      201 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/apps.py
--rw-rw-rw-   0        0        0      390 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/config.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:42:44.476106 phone_email_auth-0.6/phone_email_auth/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/models.py
--rw-rw-rw-   0        0        0       63 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/tests.py
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/urls.py
--rw-rw-rw-   0        0        0      853 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/utils.py
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.6/phone_email_auth/views.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:42:44.476106 phone_email_auth-0.6/phone_email_auth.egg-info/
--rw-rw-rw-   0        0        0     1953 2024-04-01 11:42:44.000000 phone_email_auth-0.6/phone_email_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-04-01 11:42:44.000000 phone_email_auth-0.6/phone_email_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:42:44.000000 phone_email_auth-0.6/phone_email_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 11:42:44.000000 phone_email_auth-0.6/phone_email_auth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 11:42:44.000000 phone_email_auth-0.6/phone_email_auth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2024-04-01 11:42:44.489770 phone_email_auth-0.6/setup.cfg
--rw-rw-rw-   0        0        0      205 2024-04-01 11:42:30.000000 phone_email_auth-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:36:21.361533 phone_email_auth-0.7/
+-rw-rw-rw-   0        0        0     1542 2024-04-01 09:14:40.000000 phone_email_auth-0.7/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-04-01 09:14:40.000000 phone_email_auth-0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1953 2024-04-01 12:36:21.360528 phone_email_auth-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2024-04-01 11:42:00.000000 phone_email_auth-0.7/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-01 12:36:21.351016 phone_email_auth-0.7/phone_email_auth/
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/admin.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/apps.py
+-rw-rw-rw-   0        0        0      390 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/config.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:36:21.358014 phone_email_auth-0.7/phone_email_auth/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/models.py
+-rw-rw-rw-   0        0        0       63 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/tests.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/urls.py
+-rw-rw-rw-   0        0        0      874 2024-04-01 12:35:27.000000 phone_email_auth-0.7/phone_email_auth/utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.7/phone_email_auth/views.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:36:21.360016 phone_email_auth-0.7/phone_email_auth.egg-info/
+-rw-rw-rw-   0        0        0     1953 2024-04-01 12:36:21.000000 phone_email_auth-0.7/phone_email_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-01 12:36:21.000000 phone_email_auth-0.7/phone_email_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:36:21.000000 phone_email_auth-0.7/phone_email_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 12:36:21.000000 phone_email_auth-0.7/phone_email_auth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 12:36:21.000000 phone_email_auth-0.7/phone_email_auth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2024-04-01 12:36:21.362533 phone_email_auth-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      205 2024-04-01 12:36:02.000000 phone_email_auth-0.7/setup.py
```

### Comparing `phone_email_auth-0.6/LICENSE` & `phone_email_auth-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.6/PKG-INFO` & `phone_email_auth-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_email_auth
-Version: 0.6
+Version: 0.7
 Summary: A Django app to use services of phone.email.
 Home-page: https://www.phone.email/
 Author: Phone Email
 Author-email: mg@phone.email
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `phone_email_auth-0.6/README.rst` & `phone_email_auth-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.6/phone_email_auth/utils.py` & `phone_email_auth-0.7/phone_email_auth/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.shortcuts import render
-from .config import CLIENT_ID, ACCESS_TOKEN
 # Create your views here.
 import requests
 
-def get_verified_phone():
+def get_verified_phone(ACCESS_TOKEN, CLIENT_ID):
 
     url = "https://eapi.phone.email/getuser"
     if not CLIENT_ID or not ACCESS_TOKEN:
         raise ValueError("Client ID and Access Token must be set")
 
     postData = {
         'access_token': ACCESS_TOKEN,
@@ -17,17 +16,17 @@
     response = requests.post(url, data=postData, verify=True) 
 
     if response.status_code != 200:
         print("Error:", response.text)
         exit()
 
     json_data = response.json()
-
     if json_data['status'] != 200:
-        print("Error:")
-        exit()
+            print("Error:")
+            exit()
 
     country_code = json_data['country_code']
     phone_no = json_data['phone_no']
     ph_email_jwt = json_data['ph_email_jwt']
 
-    print(country_code+phone_no)
+    print(country_code+phone_no)
+    return (country_code, phone_no)
```

### Comparing `phone_email_auth-0.6/phone_email_auth.egg-info/PKG-INFO` & `phone_email_auth-0.7/phone_email_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_email_auth
-Version: 0.6
+Version: 0.7
 Summary: A Django app to use services of phone.email.
 Home-page: https://www.phone.email/
 Author: Phone Email
 Author-email: mg@phone.email
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `phone_email_auth-0.6/phone_email_auth.egg-info/SOURCES.txt` & `phone_email_auth-0.7/phone_email_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.6/setup.cfg` & `phone_email_auth-0.7/setup.cfg`

 * *Files identical despite different names*

