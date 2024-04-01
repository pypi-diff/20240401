# Comparing `tmp/phone_email_auth-0.4.tar.gz` & `tmp/phone_email_auth-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_email_auth-0.4.tar", last modified: Mon Apr  1 11:13:47 2024, max compression
+gzip compressed data, was "phone_email_auth-0.5.tar", last modified: Mon Apr  1 11:17:09 2024, max compression
```

## Comparing `phone_email_auth-0.4.tar` & `phone_email_auth-0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 11:13:47.109252 phone_email_auth-0.4/
--rw-rw-rw-   0        0        0     1542 2024-04-01 09:14:40.000000 phone_email_auth-0.4/LICENSE
--rw-rw-rw-   0        0        0       61 2024-04-01 09:14:40.000000 phone_email_auth-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1950 2024-04-01 11:13:47.105239 phone_email_auth-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2024-04-01 09:14:40.000000 phone_email_auth-0.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-01 11:13:47.097603 phone_email_auth-0.4/phone_email_auth/
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/admin.py
--rw-rw-rw-   0        0        0      201 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/apps.py
--rw-rw-rw-   0        0        0      390 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/config.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:13:47.105239 phone_email_auth-0.4/phone_email_auth/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/models.py
--rw-rw-rw-   0        0        0       63 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/tests.py
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/urls.py
--rw-rw-rw-   0        0        0      853 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/utils.py
--rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.4/phone_email_auth/views.py
-drwxrwxrwx   0        0        0        0 2024-04-01 11:13:47.105239 phone_email_auth-0.4/phone_email_auth.egg-info/
--rw-rw-rw-   0        0        0     1950 2024-04-01 11:13:46.000000 phone_email_auth-0.4/phone_email_auth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-04-01 11:13:47.000000 phone_email_auth-0.4/phone_email_auth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 11:13:46.000000 phone_email_auth-0.4/phone_email_auth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 11:13:46.000000 phone_email_auth-0.4/phone_email_auth.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 11:13:46.000000 phone_email_auth-0.4/phone_email_auth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2024-04-01 11:13:47.110683 phone_email_auth-0.4/setup.cfg
--rw-rw-rw-   0        0        0      205 2024-04-01 11:13:35.000000 phone_email_auth-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:17:09.245469 phone_email_auth-0.5/
+-rw-rw-rw-   0        0        0     1542 2024-04-01 09:14:40.000000 phone_email_auth-0.5/LICENSE
+-rw-rw-rw-   0        0        0       61 2024-04-01 09:14:40.000000 phone_email_auth-0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1953 2024-04-01 11:17:09.245469 phone_email_auth-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2024-04-01 11:16:46.000000 phone_email_auth-0.5/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-01 11:17:09.239463 phone_email_auth-0.5/phone_email_auth/
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/admin.py
+-rw-rw-rw-   0        0        0      201 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/apps.py
+-rw-rw-rw-   0        0        0      390 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/config.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:17:09.245469 phone_email_auth-0.5/phone_email_auth/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/models.py
+-rw-rw-rw-   0        0        0       63 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/tests.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/urls.py
+-rw-rw-rw-   0        0        0      853 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 09:14:40.000000 phone_email_auth-0.5/phone_email_auth/views.py
+drwxrwxrwx   0        0        0        0 2024-04-01 11:17:09.245469 phone_email_auth-0.5/phone_email_auth.egg-info/
+-rw-rw-rw-   0        0        0     1953 2024-04-01 11:17:09.000000 phone_email_auth-0.5/phone_email_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-01 11:17:09.000000 phone_email_auth-0.5/phone_email_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 11:17:09.000000 phone_email_auth-0.5/phone_email_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 11:17:09.000000 phone_email_auth-0.5/phone_email_auth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-01 11:17:09.000000 phone_email_auth-0.5/phone_email_auth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2024-04-01 11:17:09.250678 phone_email_auth-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      205 2024-04-01 11:17:00.000000 phone_email_auth-0.5/setup.py
```

### Comparing `phone_email_auth-0.4/LICENSE` & `phone_email_auth-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.4/PKG-INFO` & `phone_email_auth-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_email_auth
-Version: 0.4
+Version: 0.5
 Summary: A Django app to use services of phone.email.
 Home-page: https://www.phone.email/
 Author: Phone Email
 Author-email: mg@phone.email
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -26,34 +26,34 @@
 Installation
 ------------
 
 You can install One Tap Sign In using pip:
 
 .. code-block:: bash
 
-    $ pip install one-tap-sign-in
+    $ pip install phone-email-auth
 
 Usage
 -----
 
 To configure One Tap Sign In in your Django project, you can set the client ID and access token using the following functions:
 
 .. code-block:: python
     
-    from one_tap_sign_in.config import set_client_id, set_access_token
+    from phone-email-auth.config import set_client_id, set_access_token
 
     set_client_id("your_client_id")
     set_access_token("your_access_token")
 
 Once configured, you can call the `get_verified_phone()` function in your views to retrieve the verified phone number:
 
 .. code-block:: python
 
     # views.py
-    from one_tap_sign_in.utils import get_verified_phone
+    from phone-email-auth.utils import get_verified_phone
 
     def my_view(request):
         # Call the get_verified_phone function
         phone_number = get_verified_phone()
         # Further logic based on the retrieved phone number
 
 License
```

### Comparing `phone_email_auth-0.4/README.rst` & `phone_email_auth-0.5/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 Installation
 ------------
 
 You can install One Tap Sign In using pip:
 
 .. code-block:: bash
 
-    $ pip install one-tap-sign-in
+    $ pip install phone-email-auth
 
 Usage
 -----
 
 To configure One Tap Sign In in your Django project, you can set the client ID and access token using the following functions:
 
 .. code-block:: python
     
-    from one_tap_sign_in.config import set_client_id, set_access_token
+    from phone-email-auth.config import set_client_id, set_access_token
 
     set_client_id("your_client_id")
     set_access_token("your_access_token")
 
 Once configured, you can call the `get_verified_phone()` function in your views to retrieve the verified phone number:
 
 .. code-block:: python
 
     # views.py
-    from one_tap_sign_in.utils import get_verified_phone
+    from phone-email-auth.utils import get_verified_phone
 
     def my_view(request):
         # Call the get_verified_phone function
         phone_number = get_verified_phone()
         # Further logic based on the retrieved phone number
 
 License
```

### Comparing `phone_email_auth-0.4/phone_email_auth/utils.py` & `phone_email_auth-0.5/phone_email_auth/utils.py`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.4/phone_email_auth.egg-info/PKG-INFO` & `phone_email_auth-0.5/phone_email_auth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_email_auth
-Version: 0.4
+Version: 0.5
 Summary: A Django app to use services of phone.email.
 Home-page: https://www.phone.email/
 Author: Phone Email
 Author-email: mg@phone.email
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -26,34 +26,34 @@
 Installation
 ------------
 
 You can install One Tap Sign In using pip:
 
 .. code-block:: bash
 
-    $ pip install one-tap-sign-in
+    $ pip install phone-email-auth
 
 Usage
 -----
 
 To configure One Tap Sign In in your Django project, you can set the client ID and access token using the following functions:
 
 .. code-block:: python
     
-    from one_tap_sign_in.config import set_client_id, set_access_token
+    from phone-email-auth.config import set_client_id, set_access_token
 
     set_client_id("your_client_id")
     set_access_token("your_access_token")
 
 Once configured, you can call the `get_verified_phone()` function in your views to retrieve the verified phone number:
 
 .. code-block:: python
 
     # views.py
-    from one_tap_sign_in.utils import get_verified_phone
+    from phone-email-auth.utils import get_verified_phone
 
     def my_view(request):
         # Call the get_verified_phone function
         phone_number = get_verified_phone()
         # Further logic based on the retrieved phone number
 
 License
```

### Comparing `phone_email_auth-0.4/phone_email_auth.egg-info/SOURCES.txt` & `phone_email_auth-0.5/phone_email_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_email_auth-0.4/setup.cfg` & `phone_email_auth-0.5/setup.cfg`

 * *Files identical despite different names*

