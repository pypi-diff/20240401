# Comparing `tmp/strapp-0.3.8.tar.gz` & `tmp/strapp-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strapp-0.3.8.tar", max compression
+gzip compressed data, was "strapp-0.3.9.tar", max compression
```

## Comparing `strapp-0.3.8.tar` & `strapp-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1053 2022-01-18 15:55:26.361868 strapp-0.3.8/LICENSE
--rw-r--r--   0        0        0     1930 2022-04-07 13:03:50.789959 strapp-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-18 15:55:26.367496 strapp-0.3.8/src/strapp/__init__.py
--rw-r--r--   0        0        0      319 2022-01-18 15:55:32.772665 strapp-0.3.8/src/strapp/click/__init__.py
--rw-r--r--   0        0        0     4157 2022-01-18 15:55:26.368287 strapp-0.3.8/src/strapp/click/resolver.py
--rw-r--r--   0        0        0     3277 2022-01-18 15:55:32.773036 strapp-0.3.8/src/strapp/click/testing.py
--rw-r--r--   0        0        0     1859 2022-01-18 19:51:07.119360 strapp-0.3.8/src/strapp/datadog.py
--rw-r--r--   0        0        0      424 2022-01-18 15:55:26.369050 strapp-0.3.8/src/strapp/flask/__init__.py
--rw-r--r--   0        0        0     3643 2022-01-18 15:55:26.369400 strapp-0.3.8/src/strapp/flask/base.py
--rw-r--r--   0        0        0     1405 2022-01-18 15:55:26.369728 strapp-0.3.8/src/strapp/flask/database.py
--rw-r--r--   0        0        0     4688 2022-01-18 15:55:26.370108 strapp-0.3.8/src/strapp/flask/decorators.py
--rw-r--r--   0        0        0     3107 2022-01-18 15:55:26.370445 strapp-0.3.8/src/strapp/flask/error.py
--rw-r--r--   0        0        0     1485 2022-01-18 15:55:26.370767 strapp-0.3.8/src/strapp/flask/route.py
--rw-r--r--   0        0        0     4589 2022-01-18 15:54:13.086758 strapp-0.3.8/src/strapp/http/client.py
--rw-r--r--   0        0        0     6200 2022-04-07 13:03:50.796196 strapp-0.3.8/src/strapp/http/request.py
--rw-r--r--   0        0        0     2210 2022-01-18 15:55:26.371094 strapp-0.3.8/src/strapp/logging.py
--rw-r--r--   0        0        0        0 2022-01-18 15:55:26.371221 strapp-0.3.8/src/strapp/py.typed
--rw-r--r--   0        0        0     2705 2022-01-18 15:55:26.371592 strapp-0.3.8/src/strapp/sentry.py
--rw-r--r--   0        0        0      320 2022-01-18 15:55:26.372012 strapp-0.3.8/src/strapp/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4838 2022-03-16 16:08:26.535616 strapp-0.3.8/src/strapp/sqlalchemy/model_base.py
--rw-r--r--   0        0        0     3632 2022-03-15 16:00:42.262090 strapp-0.3.8/src/strapp/sqlalchemy/mypy.py
--rw-r--r--   0        0        0     2314 2022-01-18 15:55:26.372658 strapp-0.3.8/src/strapp/sqlalchemy/session.py
--rw-r--r--   0        0        0     2090 2022-01-18 15:55:26.372961 strapp-0.3.8/src/strapp/sqlalchemy/testing.py
--rw-r--r--   0        0        0     1045 2022-04-07 13:04:01.508634 strapp-0.3.8/setup.py
--rw-r--r--   0        0        0     1139 2022-04-07 13:04:01.509054 strapp-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1053 2022-01-18 15:55:26.361868 strapp-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1930 2022-04-27 17:04:09.490799 strapp-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-01-18 15:55:26.367496 strapp-0.3.9/src/strapp/__init__.py
+-rw-r--r--   0        0        0      319 2022-01-18 15:55:32.772665 strapp-0.3.9/src/strapp/click/__init__.py
+-rw-r--r--   0        0        0     4157 2022-01-18 15:55:26.368287 strapp-0.3.9/src/strapp/click/resolver.py
+-rw-r--r--   0        0        0     3277 2022-01-18 15:55:32.773036 strapp-0.3.9/src/strapp/click/testing.py
+-rw-r--r--   0        0        0     1859 2022-01-18 19:51:07.119360 strapp-0.3.9/src/strapp/datadog.py
+-rw-r--r--   0        0        0      424 2022-01-18 15:55:26.369050 strapp-0.3.9/src/strapp/flask/__init__.py
+-rw-r--r--   0        0        0     3643 2022-01-18 15:55:26.369400 strapp-0.3.9/src/strapp/flask/base.py
+-rw-r--r--   0        0        0     1405 2022-01-18 15:55:26.369728 strapp-0.3.9/src/strapp/flask/database.py
+-rw-r--r--   0        0        0     4688 2022-01-18 15:55:26.370108 strapp-0.3.9/src/strapp/flask/decorators.py
+-rw-r--r--   0        0        0     3107 2022-01-18 15:55:26.370445 strapp-0.3.9/src/strapp/flask/error.py
+-rw-r--r--   0        0        0     1485 2022-01-18 15:55:26.370767 strapp-0.3.9/src/strapp/flask/route.py
+-rw-r--r--   0        0        0     4589 2022-01-18 15:54:13.086758 strapp-0.3.9/src/strapp/http/client.py
+-rw-r--r--   0        0        0     6200 2022-04-07 13:03:50.796196 strapp-0.3.9/src/strapp/http/request.py
+-rw-r--r--   0        0        0     2210 2022-01-18 15:55:26.371094 strapp-0.3.9/src/strapp/logging.py
+-rw-r--r--   0        0        0        0 2022-01-18 15:55:26.371221 strapp-0.3.9/src/strapp/py.typed
+-rw-r--r--   0        0        0     5450 2022-04-27 17:04:09.495518 strapp-0.3.9/src/strapp/sentry.py
+-rw-r--r--   0        0        0      320 2022-01-18 15:55:26.372012 strapp-0.3.9/src/strapp/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4838 2022-03-16 16:08:26.535616 strapp-0.3.9/src/strapp/sqlalchemy/model_base.py
+-rw-r--r--   0        0        0     3632 2022-03-15 16:00:42.262090 strapp-0.3.9/src/strapp/sqlalchemy/mypy.py
+-rw-r--r--   0        0        0     2314 2022-01-18 15:55:26.372658 strapp-0.3.9/src/strapp/sqlalchemy/session.py
+-rw-r--r--   0        0        0     2090 2022-01-18 15:55:26.372961 strapp-0.3.9/src/strapp/sqlalchemy/testing.py
+-rw-r--r--   0        0        0     1045 2022-04-27 17:04:31.802785 strapp-0.3.9/setup.py
+-rw-r--r--   0        0        0     1139 2022-04-27 17:04:31.803107 strapp-0.3.9/PKG-INFO
```

### Comparing `strapp-0.3.8/LICENSE` & `strapp-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/pyproject.toml` & `strapp-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strapp"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = []
 packages = [
     { include = "strapp", from = "src" },
 ]
 include = ["src/strapp/py.typed"]
```

### Comparing `strapp-0.3.8/src/strapp/click/resolver.py` & `strapp-0.3.9/src/strapp/click/resolver.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/click/testing.py` & `strapp-0.3.9/src/strapp/click/testing.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/datadog.py` & `strapp-0.3.9/src/strapp/datadog.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/flask/base.py` & `strapp-0.3.9/src/strapp/flask/base.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/flask/database.py` & `strapp-0.3.9/src/strapp/flask/database.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/flask/decorators.py` & `strapp-0.3.9/src/strapp/flask/decorators.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/flask/error.py` & `strapp-0.3.9/src/strapp/flask/error.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/flask/route.py` & `strapp-0.3.9/src/strapp/flask/route.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/http/client.py` & `strapp-0.3.9/src/strapp/http/client.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/http/request.py` & `strapp-0.3.9/src/strapp/http/request.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/logging.py` & `strapp-0.3.9/src/strapp/logging.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/sqlalchemy/model_base.py` & `strapp-0.3.9/src/strapp/sqlalchemy/model_base.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/sqlalchemy/mypy.py` & `strapp-0.3.9/src/strapp/sqlalchemy/mypy.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/sqlalchemy/session.py` & `strapp-0.3.9/src/strapp/sqlalchemy/session.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/src/strapp/sqlalchemy/testing.py` & `strapp-0.3.9/src/strapp/sqlalchemy/testing.py`

 * *Files identical despite different names*

### Comparing `strapp-0.3.8/setup.py` & `strapp-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'flask': ['flask', 'flask_reverse_proxy'],
  'http': ['setuplog>=0.2.2', 'backoff>=1.11.1,<2.0.0'],
  'sentry': ['sentry-sdk'],
  'sqlalchemy': ['sqlalchemy']}
 
 setup_kwargs = {
     'name': 'strapp',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '',
     'long_description': None,
     'author': None,
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `strapp-0.3.8/PKG-INFO` & `strapp-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strapp
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

