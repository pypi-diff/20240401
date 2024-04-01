# Comparing `tmp/reflex-google-auth-0.0.3.tar.gz` & `tmp/reflex-google-auth-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-google-auth-0.0.3.tar", last modified: Wed Mar 20 00:58:23 2024, max compression
+gzip compressed data, was "reflex-google-auth-0.0.4.tar", last modified: Mon Apr  1 19:16:19 2024, max compression
```

## Comparing `reflex-google-auth-0.0.3.tar` & `reflex-google-auth-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-20 00:58:23.675748 reflex-google-auth-0.0.3/
--rw-r--r--   0 masen      (502) staff       (20)      668 2024-03-20 00:58:23.675537 reflex-google-auth-0.0.3/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)      114 2024-03-18 23:19:27.000000 reflex-google-auth-0.0.3/README.md
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-20 00:58:23.672599 reflex-google-auth-0.0.3/custom_components/
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-20 00:58:23.674180 reflex-google-auth-0.0.3/custom_components/reflex_google_auth/
--rw-r--r--   0 masen      (502) staff       (20)      291 2024-03-20 00:51:35.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth/__init__.py
--rw-r--r--   0 masen      (502) staff       (20)      594 2024-03-18 23:49:05.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth/decorator.py
--rw-r--r--   0 masen      (502) staff       (20)      826 2024-03-20 00:51:27.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth/google_auth.py
--rw-r--r--   0 masen      (502) staff       (20)     1486 2024-03-20 00:54:30.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth/state.py
-drwxr-xr-x   0 masen      (502) staff       (20)        0 2024-03-20 00:58:23.675175 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/
--rw-r--r--   0 masen      (502) staff       (20)      668 2024-03-20 00:58:23.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/PKG-INFO
--rw-r--r--   0 masen      (502) staff       (20)      520 2024-03-20 00:58:23.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 masen      (502) staff       (20)        1 2024-03-20 00:58:23.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 masen      (502) staff       (20)       55 2024-03-20 00:58:23.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/requires.txt
--rw-r--r--   0 masen      (502) staff       (20)       19 2024-03-20 00:58:23.000000 reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/top_level.txt
--rw-r--r--   0 masen      (502) staff       (20)      739 2024-03-20 00:57:05.000000 reflex-google-auth-0.0.3/pyproject.toml
--rw-r--r--   0 masen      (502) staff       (20)       38 2024-03-20 00:58:23.675792 reflex-google-auth-0.0.3/setup.cfg
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.348198 reflex-google-auth-0.0.4/
+-rw-r--r--   0 masenf     (501) staff       (20)      669 2024-04-01 19:16:19.347998 reflex-google-auth-0.0.4/PKG-INFO
+-rw-r--r--   0 masenf     (501) staff       (20)      114 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/README.md
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.345464 reflex-google-auth-0.0.4/custom_components/
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.346831 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/
+-rw-r--r--   0 masenf     (501) staff       (20)      291 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/__init__.py
+-rw-r--r--   0 masenf     (501) staff       (20)      594 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/decorator.py
+-rw-r--r--   0 masenf     (501) staff       (20)      794 2024-04-01 19:11:51.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.py
+-rw-r--r--   0 masenf     (501) staff       (20)     3800 2024-04-01 19:16:18.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.pyi
+-rw-r--r--   0 masenf     (501) staff       (20)     1486 2024-04-01 19:11:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth/state.py
+drwxr-xr-x   0 masenf     (501) staff       (20)        0 2024-04-01 19:16:19.347697 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/
+-rw-r--r--   0 masenf     (501) staff       (20)      669 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 masenf     (501) staff       (20)      573 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 masenf     (501) staff       (20)        1 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 masenf     (501) staff       (20)       56 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/requires.txt
+-rw-r--r--   0 masenf     (501) staff       (20)       19 2024-04-01 19:16:19.000000 reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/top_level.txt
+-rw-r--r--   0 masenf     (501) staff       (20)      740 2024-04-01 19:15:08.000000 reflex-google-auth-0.0.4/pyproject.toml
+-rw-r--r--   0 masenf     (501) staff       (20)       38 2024-04-01 19:16:19.348236 reflex-google-auth-0.0.4/setup.cfg
```

### Comparing `reflex-google-auth-0.0.3/PKG-INFO` & `reflex-google-auth-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-google-auth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reflex custom component google-auth
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/martinxu9/reflex-google-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: reflex>=0.4.6a
 Requires-Dist: google-auth[requests]
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # google-auth
```

### Comparing `reflex-google-auth-0.0.3/custom_components/reflex_google_auth/decorator.py` & `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/decorator.py`

 * *Files identical despite different names*

### Comparing `reflex-google-auth-0.0.3/custom_components/reflex_google_auth/google_auth.py` & `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/google_auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 google_oauth_provider = GoogleOAuthProvider.create
 
 
 class GoogleLogin(rx.Component):
     library = "@react-oauth/google"
     tag = "GoogleLogin"
 
-    def get_event_triggers(self):
-        return {"on_success": lambda data: [data]}
+    on_success: rx.EventHandler[lambda data: [data]]
 
     @classmethod
     def create(cls, **props) -> "GoogleLogin":
         props.setdefault("on_success", GoogleAuthState.on_success)
         return super().create(**props)
```

### Comparing `reflex-google-auth-0.0.3/custom_components/reflex_google_auth/state.py` & `reflex-google-auth-0.0.4/custom_components/reflex_google_auth/state.py`

 * *Files identical despite different names*

### Comparing `reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/PKG-INFO` & `reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-google-auth
-Version: 0.0.3
+Version: 0.0.4
 Summary: Reflex custom component google-auth
 Author-email: Masen Furer <m_github@0x26.net>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/martinxu9/reflex-google-auth
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: reflex>=0.4.2
+Requires-Dist: reflex>=0.4.6a
 Requires-Dist: google-auth[requests]
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # google-auth
```

### Comparing `reflex-google-auth-0.0.3/custom_components/reflex_google_auth.egg-info/SOURCES.txt` & `reflex-google-auth-0.0.4/custom_components/reflex_google_auth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 custom_components/reflex_google_auth/__init__.py
 custom_components/reflex_google_auth/decorator.py
 custom_components/reflex_google_auth/google_auth.py
+custom_components/reflex_google_auth/google_auth.pyi
 custom_components/reflex_google_auth/state.py
 custom_components/reflex_google_auth.egg-info/PKG-INFO
 custom_components/reflex_google_auth.egg-info/SOURCES.txt
 custom_components/reflex_google_auth.egg-info/dependency_links.txt
 custom_components/reflex_google_auth.egg-info/requires.txt
 custom_components/reflex_google_auth.egg-info/top_level.txt
```

### Comparing `reflex-google-auth-0.0.3/pyproject.toml` & `reflex-google-auth-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-google-auth"
-version = "0.0.3"
+version = "0.0.4"
 description = "Reflex custom component google-auth"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "Masen Furer", email = "m_github@0x26.net" }]
 keywords = [
     "reflex",
     "reflex-custom-components"]
 
 dependencies = [
-    "reflex>=0.4.2",
+    "reflex>=0.4.6a",
     "google-auth[requests]",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
 ]
```

