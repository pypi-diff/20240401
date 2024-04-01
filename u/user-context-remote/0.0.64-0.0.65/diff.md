# Comparing `tmp/user-context-remote-0.0.64.tar.gz` & `tmp/user-context-remote-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-context-remote-0.0.64.tar", last modified: Sat Mar  2 21:54:26 2024, max compression
+gzip compressed data, was "user-context-remote-0.0.65.tar", last modified: Mon Apr  1 19:52:34 2024, max compression
```

## Comparing `user-context-remote-0.0.64.tar` & `user-context-remote-0.0.65.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-02 21:54:02.000000 user-context-remote-0.0.64/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-02 21:54:02.000000 user-context-remote-0.0.64/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-02 21:54:02.000000 user-context-remote-0.0.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 21:54:02.000000 user-context-remote-0.0.64/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18973 2024-03-02 21:54:02.000000 user-context-remote-0.0.64/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 21:54:26.436376 user-context-remote-0.0.64/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-02 21:54:26.000000 user-context-remote-0.0.64/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-02 21:54:26.000000 user-context-remote-0.0.64/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 21:54:26.000000 user-context-remote-0.0.64/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-02 21:54:26.000000 user-context-remote-0.0.64/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-02 21:54:26.000000 user-context-remote-0.0.64/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.440853 user-context-remote-0.0.65/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-01 19:52:16.000000 user-context-remote-0.0.65/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:52:34.444853 user-context-remote-0.0.65/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 19:52:34.000000 user-context-remote-0.0.65/user_context_remote.egg-info/top_level.txt
```

### Comparing `user-context-remote-0.0.64/PKG-INFO` & `user-context-remote-0.0.65/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.64
+Version: 0.0.65
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: language-local>=0.0.6
+Requires-Dist: language-remote>=0.0.15
 Requires-Dist: url-remote>=0.0.15
 Requires-Dist: requests>=2.31.0
 Requires-Dist: python-sdk-remote>=0.0.44
 
 This is a package for sharing common user-context-remote functions used in different repositories
```

### Comparing `user-context-remote-0.0.64/README.md` & `user-context-remote-0.0.65/README.md`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.64/pyproject.toml` & `user-context-remote-0.0.65/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.64/setup.py` & `user-context-remote-0.0.65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.64',  # https://pypi.org/project/user-context-remote/
+    version='0.0.65',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
@@ -17,13 +17,13 @@
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'language-local>=0.0.6',
+        'language-remote>=0.0.15',
         'url-remote>=0.0.15',
         'requests>=2.31.0',
         'python-sdk-remote>=0.0.44',
     ],
 )
```

### Comparing `user-context-remote-0.0.64/user_context_remote/src/user_context.py` & `user-context-remote-0.0.65/user_context_remote/src/user_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 from http import HTTPStatus
 
-# TODO Shall we use authentication-remote-python-package and not directly authentication-local-restapi-typescript?
-
 import requests
 from language_remote.lang_code import LangCode
 from python_sdk_remote.mini_logger import MiniLogger
 from python_sdk_remote.utilities import our_get_env, create_return_http_headers
 from url_remote import action_name_enum, component_name_enum, entity_name_enum
 from url_remote.url_circlez import OurUrl
 
+# TODO Shall we use authentication-remote-python-package and not directly authentication-local-restapi-typescript?
+
 BRAND_NAME = our_get_env("BRAND_NAME")
 ENVIORNMENT_NAME = our_get_env("ENVIRONMENT_NAME")
 
 # TODO How about using AUTHENTICATION_API_VERSION_DICT per environment_name in url-local-python-package?
 AUTHENTICATION_API_VERSION = 1
 DEFAULT_LANG_CODE = LangCode.ENGLISH
 
@@ -46,15 +46,15 @@
         else:
             # TODO identification or identifier?
             user_identifier = user_identifier or our_get_env("PRODUCT_USER_IDENTIFIER")
             password = password or our_get_env("PRODUCT_PASSWORD")
             user_context = self._authenticate_by_user_identification_and_password(
                 user_identifier=user_identifier, password=password)
         # Populate the private data members with data we received from Authentication Local REST-API https://github.com/circles-zone/authentication-local-restapi-typescript-serverless-com/edit/dev/auth-restapi-serverless-com/src/services/auth-service/auth-service-impl.ts
-        #TODO shall we change the parameter name to user_context=user_context?
+        # TODO shall we change the parameter name to user_context=user_context?
         self.__get_user_data_login_response(validate_user_jwt_response=user_context)
 
     @staticmethod
     # Does it support no parameters? Yes
     def login_using_user_identification_and_password(user_identifier: str = None, password: str = None):
         # LOGIN_USING_USER_IDENTIFICATION_AND_PASSWORD_METHOD_NAME = "login_using_user_identification_and_password"
         # TODO Why commented? Shall we add if (DebugMode)
@@ -212,22 +212,23 @@
                 data=json.dumps(authentication_login_request_json, separators=(",", ":")), headers=headers
             )
             if authentication_login_response_json.status_code != HTTPStatus.OK:
                 MiniLogger.error(_AUTHENTICATE_BY_USER_IDENTIFICATION_AND_PASSWORD_METHOD_NAME +
                                  " authentication_login_response_json.status_code != HTTPStatus.OK " + authentication_login_response_json.text)
                 raise Exception(authentication_login_response_json.text)
             # Maybe there is no "data"
-            MiniLogger.info("authentication_login_response_json.json()"+ str(authentication_login_response_json))
-            MiniLogger.info("authentication_login_response_json.json() with json()"+ str(authentication_login_response_json.json()) )
-            #TODO Put this in try/except as there might be no "data" or no "userJwt"
+            MiniLogger.info("authentication_login_response_json.json()" + str(authentication_login_response_json))
+            MiniLogger.info("authentication_login_response_json.json() with json()" + str(
+                authentication_login_response_json.json()))
+            # TODO Put this in try/except as there might be no "data" or no "userJwt"
             self.user_jwt = authentication_login_response_json.json()["data"]["userJwt"]
             MiniLogger.end(_AUTHENTICATE_BY_USER_IDENTIFICATION_AND_PASSWORD_METHOD_NAME, object={
                 "user_jwt": self.user_jwt})
             return authentication_login_response_json
-        #TODO Catch KeyError: 'data'
+        # TODO Catch KeyError: 'data'
         except Exception as exception:
             MiniLogger.exception(
                 "Error(Exception): user-context-remote-python _authenticate() " + str(exception))
             MiniLogger.end(_AUTHENTICATE_BY_USER_IDENTIFICATION_AND_PASSWORD_METHOD_NAME)
             raise
 
     def _authenticate_by_user_jwt(self, user_jwt: str) -> requests.Response:
```

### Comparing `user-context-remote-0.0.64/user_context_remote.egg-info/PKG-INFO` & `user-context-remote-0.0.65/user_context_remote.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.64
+Version: 0.0.65
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: language-local>=0.0.6
+Requires-Dist: language-remote>=0.0.15
 Requires-Dist: url-remote>=0.0.15
 Requires-Dist: requests>=2.31.0
 Requires-Dist: python-sdk-remote>=0.0.44
 
 This is a package for sharing common user-context-remote functions used in different repositories
```

