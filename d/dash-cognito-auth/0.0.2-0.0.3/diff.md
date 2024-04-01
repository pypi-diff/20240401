# Comparing `tmp/dash-cognito-auth-0.0.2.tar.gz` & `tmp/dash-cognito-auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-cognito-auth-0.0.2.tar", last modified: Sun Mar 31 15:44:42 2024, max compression
+gzip compressed data, was "dash-cognito-auth-0.0.3.tar", last modified: Mon Apr  1 15:00:24 2024, max compression
```

## Comparing `dash-cognito-auth-0.0.2.tar` & `dash-cognito-auth-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.950935 dash-cognito-auth-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/dash_cognito_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/dash_cognito_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/dash_cognito_auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/dash_cognito_auth/cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/dash_cognito_auth/cognito_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-31 15:44:42.000000 dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:42.954935 dash-cognito-auth-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/tests/test_auth_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-31 15:44:37.000000 dash-cognito-auth-0.0.2/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.440144 dash-cognito-auth-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/dash_cognito_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/dash_cognito_auth/cognito_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 15:00:24.000000 dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:24.444144 dash-cognito-auth-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_auth_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 15:00:19.000000 dash-cognito-auth-0.0.3/tests/test_import.py
```

### Comparing `dash-cognito-auth-0.0.2/.github/workflows/build.yml` & `dash-cognito-auth-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/.github/workflows/python-publish.yml` & `dash-cognito-auth-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/.gitignore` & `dash-cognito-auth-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/LICENSE.md` & `dash-cognito-auth-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/PKG-INFO` & `dash-cognito-auth-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cognito-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dash Cognito Auth
 Home-page: https://github.com/fspijkerman/dash-cognito-auth
 Author: Frank Spijkerman
 Author-email: frank@jeito.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -106,11 +106,7 @@
 
 # Connection between the app and the user pool
 COGNITO_DOMAIN=<just-the-prefix>
 COGNITO_REGION=<aws-region-of-the-cognito-userpool>
 COGNITO_OAUTH_CLIENT_ID=<app-client-id>
 COGNITO_OAUTH_CLIENT_SECRET=<app-client-secret>
 ```
-
-## Known Limitations
-
-- Fully Custom Cognito Domains aren't supported at the moment
```

### Comparing `dash-cognito-auth-0.0.2/README.md` & `dash-cognito-auth-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,8 @@
 COGNITO_PASSWORD=<password>
 
 # Connection between the app and the user pool
 COGNITO_DOMAIN=<just-the-prefix>
 COGNITO_REGION=<aws-region-of-the-cognito-userpool>
 COGNITO_OAUTH_CLIENT_ID=<app-client-id>
 COGNITO_OAUTH_CLIENT_SECRET=<app-client-secret>
-```
-
-## Known Limitations
-
-- Fully Custom Cognito Domains aren't supported at the moment
+```
```

### Comparing `dash-cognito-auth-0.0.2/app.py` & `dash-cognito-auth-0.0.3/app.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/dash_cognito_auth/auth.py` & `dash-cognito-auth-0.0.3/dash_cognito_auth/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from __future__ import absolute_import
 from abc import ABCMeta, abstractmethod
 from six import iteritems, add_metaclass
 
 
 @add_metaclass(ABCMeta)
 class Auth(object):
     def __init__(self, app):
         self.app = app
-        self._index_view_name = app.config['routes_pathname_prefix']
+        self._index_view_name = app.config["routes_pathname_prefix"]
         self._overwrite_index()
         self._protect_views()
-        self._index_view_name = app.config['routes_pathname_prefix']
+        self._index_view_name = app.config["routes_pathname_prefix"]
 
     def _overwrite_index(self):
         original_index = self.app.server.view_functions[self._index_view_name]
 
-        self.app.server.view_functions[self._index_view_name] = \
-            self.index_auth_wrapper(original_index)
+        self.app.server.view_functions[self._index_view_name] = self.index_auth_wrapper(
+            original_index
+        )
 
     def _protect_views(self):
         # require auth wrapper for all views
-        for view_name, view_method in iteritems(
-                self.app.server.view_functions):
+        for view_name, view_method in iteritems(self.app.server.view_functions):
             if view_name != self._index_view_name:
-                self.app.server.view_functions[view_name] = \
-                    self.auth_wrapper(view_method)
+                self.app.server.view_functions[view_name] = self.auth_wrapper(
+                    view_method
+                )
 
     @abstractmethod
     def is_authorized(self):
         pass
 
     @abstractmethod
     def auth_wrapper(self, f):
```

### Comparing `dash-cognito-auth-0.0.2/dash_cognito_auth/cognito.py` & `dash-cognito-auth-0.0.3/dash_cognito_auth/cognito.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 from flask_dance.consumer import OAuth2ConsumerBlueprint
 from flask.globals import LocalProxy
 from flask import g
 
 
 __maintainer__ = "Frank Spijkerman <frank@jeito.nl>"
 
@@ -15,15 +13,15 @@
     redirect_url=None,
     redirect_to=None,
     login_url=None,
     authorized_url=None,
     session_class=None,
     storage=None,
     domain=None,
-    region="eu-west-1",
+    region=None,
 ):
     """
     Make a blueprint for authenticating with Cognito using OAuth 2. This requires
     a client ID and client secret from Cognito. You should either pass them to
     this constructor, or make sure that your Flask application config defines
     them, using the variables :envvar:`COGNITO_OAUTH_CLIENT_ID` and
     :envvar:`COGNITO_OAUTH_CLIENT_SECRET`.
@@ -45,29 +43,41 @@
             Requests session. Defaults to
             :class:`~flask_dance.consumer.requests.OAuth2Session`.
         storage: A token storage class, or an instance of a token storage
                 class, to use for this blueprint. Defaults to
                 :class:`~flask_dance.consumer.storage.session.SessionStorage`.
         domain (str): The domain configured in Cognito
         region (str): The region of AWS
-            Defaults to ``eu-west-1``.
 
     :rtype: :class:`~flask_dance.consumer.OAuth2ConsumerBlueprint`
     :returns: A :ref:`blueprint <flask:blueprints>` to attach to your Flask app.
     """
+
+    # There are more sophisticated checks, but for our purposes it should
+    # strike a balance between accuracy and readability. The value of domain
+    # is either just a prefix in Cognito or a FQDN.
+    custom_domain = "." in domain
+
+    if not custom_domain and region is None:
+        raise ValueError("The region parameter must be set if 'domain' is not a FQDN.")
+
+    hostname = (
+        f"{domain}.auth.{region}.amazoncognito.com" if region is not None else domain
+    )
+
     scope = scope or ["openid", "email", "phone", "profile"]
     cognito_bp = OAuth2ConsumerBlueprint(
         "cognito",
         __name__,
         client_id=client_id,
         client_secret=client_secret,
         scope=scope,
-        base_url=f"https://{domain}.auth.{region}.amazoncognito.com",
-        authorization_url=f"https://{domain}.auth.{region}.amazoncognito.com/oauth2/authorize",
-        token_url=f"https://{domain}.auth.{region}.amazoncognito.com/oauth2/token",
+        base_url=f"https://{hostname}",
+        authorization_url=f"https://{hostname}/oauth2/authorize",
+        token_url=f"https://{hostname}/oauth2/token",
         redirect_url=redirect_url,
         redirect_to=redirect_to,
         login_url=login_url,
         authorized_url=authorized_url,
         session_class=session_class,
         storage=storage,
     )
```

### Comparing `dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/PKG-INFO` & `dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cognito-auth
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dash Cognito Auth
 Home-page: https://github.com/fspijkerman/dash-cognito-auth
 Author: Frank Spijkerman
 Author-email: frank@jeito.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -106,11 +106,7 @@
 
 # Connection between the app and the user pool
 COGNITO_DOMAIN=<just-the-prefix>
 COGNITO_REGION=<aws-region-of-the-cognito-userpool>
 COGNITO_OAUTH_CLIENT_ID=<app-client-id>
 COGNITO_OAUTH_CLIENT_SECRET=<app-client-secret>
 ```
-
-## Known Limitations
-
-- Fully Custom Cognito Domains aren't supported at the moment
```

### Comparing `dash-cognito-auth-0.0.2/dash_cognito_auth.egg-info/SOURCES.txt` & `dash-cognito-auth-0.0.3/dash_cognito_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.2/setup.py` & `dash-cognito-auth-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name="dash-cognito-auth",
     description="Dash Cognito Auth",
-    long_description=open("README.md", "rt").read().strip(),
+    long_description=open("README.md", "rt", encoding="utf-8").read().strip(),
     long_description_content_type="text/markdown",
     author="Frank Spijkerman",
     author_email="frank@jeito.nl",
     url="https://github.com/fspijkerman/dash-cognito-auth",
     license="MIT",
     package="dash_cognito_auth",
     packages=["dash_cognito_auth"],
```

### Comparing `dash-cognito-auth-0.0.2/tests/conftest.py` & `dash-cognito-auth-0.0.3/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+Shared test fixtures.
+"""
+
+# pylint: disable=W0621
+from typing import Iterator
 from unittest.mock import patch
 
 import pytest
 
 from dash import Dash, html
 from dotenv import load_dotenv
 from flask import Flask, redirect
@@ -43,15 +49,70 @@
     auth.app.server.config["COGNITO_OAUTH_CLIENT_ID"] = "testclient"
     auth.app.server.config["COGNITO_OAUTH_CLIENT_SCRET"] = "testsecret"
 
     return auth
 
 
 @pytest.fixture
-def authorized_app(app) -> CognitoOAuth:
+def app_with_url_prefix(name="dash") -> Dash:
+    """
+    Dash App that has only one H1 Tag with the value "Hello World".
+    It uses a Flask server with the secret key just_a_test.
+
+    All URLs should be prefixed with /some/prefix/
+    """
+
+    dash_app = Dash(name, server=Flask(name), url_base_pathname="/some/prefix/")
+    dash_app.layout = html.H1("Hello World")
+    dash_app.server.config.update(
+        {
+            "TESTING": True,
+        }
+    )
+    dash_app.server.secret_key = "just_a_test"
+    return dash_app
+
+
+@pytest.fixture
+def prefixed_app_with_auth(app_with_url_prefix) -> CognitoOAuth:
+    """
+    Dash App wrapped with Cognito Authentication:
+    - Domain name: test
+    - Region: eu-central-1
+    - App Client Id: testclient
+    - App Client Secret: testsecret
+    """
+
+    app = app_with_url_prefix
+
+    auth = CognitoOAuth(app, domain="test", region="eu-central-1")
+    auth.app.server.config["COGNITO_OAUTH_CLIENT_ID"] = "testclient"
+    auth.app.server.config["COGNITO_OAUTH_CLIENT_SCRET"] = "testsecret"
+
+    return auth
+
+
+@pytest.fixture
+def app_with_auth_and_cognito_custom_domain(app) -> CognitoOAuth:
+    """
+    Dash App wrapped with Cognito Authentication
+    - Domain name authentication.example.com
+    - App Client Id: testclient
+    - App Client Secret: testsecret
+    """
+
+    auth = CognitoOAuth(app, domain="authentication.example.com")
+    auth.app.server.config["COGNITO_OAUTH_CLIENT_ID"] = "testclient"
+    auth.app.server.config["COGNITO_OAUTH_CLIENT_SCRET"] = "testsecret"
+
+    return auth
+
+
+@pytest.fixture
+def authorized_app(app) -> Iterator[CognitoOAuth]:
     """
     App with Cognito Based authentication that bypasses the authentication/authorization
     part, i.e. replaced is_authorized and the authorized endpoint.
 
     Intended for tests that
     """
```

### Comparing `dash-cognito-auth-0.0.2/tests/test_end_to_end.py` & `dash-cognito-auth-0.0.3/tests/test_end_to_end.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Integration test that authenticates against a real user pool.
 
 Naturally these are a bit sensitive to the way the Cognito UI is implemented.
 """
 
+# pylint: disable=W0621
+
 import os
 
 from http import HTTPStatus
 
 import requests
 import pytest
```

