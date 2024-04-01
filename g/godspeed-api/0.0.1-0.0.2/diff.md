# Comparing `tmp/godspeed_api-0.0.1.tar.gz` & `tmp/godspeed_api-0.0.2.tar.gz`

## Comparing `godspeed_api-0.0.1.tar` & `godspeed_api-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/src/godspeed_api/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/src/godspeed_api/api.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/LICENSE
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/README.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 godspeed_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/src/godspeed_api/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/src/godspeed_api/api.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/LICENSE
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/README.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 godspeed_api-0.0.2/PKG-INFO
```

### Comparing `godspeed_api-0.0.1/LICENSE` & `godspeed_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `godspeed_api-0.0.1/pyproject.toml` & `godspeed_api-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "godspeed_api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Artem Trubacheev", email="almaz5200@gmail.com" },
 ]
 description = "A Godspeed task manager API wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `godspeed_api-0.0.1/PKG-INFO` & `godspeed_api-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: godspeed_api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Godspeed task manager API wrapper
 Project-URL: Homepage, https://github.com/almaz5200/godspeed
 Project-URL: Issues, https://github.com/almaz5200/godspeed/issues
 Author-email: Artem Trubacheev <almaz5200@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

