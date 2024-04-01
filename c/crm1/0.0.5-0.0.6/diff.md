# Comparing `tmp/crm1-0.0.5.tar.gz` & `tmp/crm1-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.0.5.tar", max compression
+gzip compressed data, was "crm1-0.0.6.tar", max compression
```

## Comparing `crm1-0.0.5.tar` & `crm1-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      158 2024-04-01 19:41:03.227788 crm1-0.0.5/crm1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.5/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.5/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     6947 2024-04-01 19:42:38.977440 crm1-0.0.5/crm1/helpers/versions.py
--rw-r--r--   0        0        0      182 2024-04-01 19:40:39.007960 crm1-0.0.5/crm1/spec/__init__.py
--rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.5/crm1/spec/dependency.py
--rw-r--r--   0        0        0      978 2024-04-01 20:26:21.932441 crm1-0.0.5/crm1/spec/mod.py
--rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.5/crm1/spec/repository.py
--rw-r--r--   0        0        0     1692 2024-04-01 20:21:17.411767 crm1-0.0.5/crm1/spec/unsafe_modext.py
--rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.5/crm1/types/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-01 19:38:40.277289 crm1-0.0.5/crm1/types/dependency.py
--rw-r--r--   0        0        0     1221 2024-04-01 19:41:25.588271 crm1-0.0.5/crm1/types/mod.py
--rw-r--r--   0        0        0     1933 2024-04-01 19:41:34.284778 crm1-0.0.5/crm1/types/repository.py
--rw-r--r--   0        0        0     2709 2024-04-01 19:42:47.392723 crm1-0.0.5/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      595 2024-04-01 20:25:30.948258 crm1-0.0.5/crm1/utils.py
--rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.5/LICENSE
--rw-r--r--   0        0        0      397 2024-04-01 19:57:15.478309 crm1-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3855 2024-04-01 19:43:56.788453 crm1-0.0.5/README.md
--rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 crm1-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      158 2024-04-01 19:41:03.227788 crm1-0.0.6/crm1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:13:19.201078 crm1-0.0.6/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:48:13.428536 crm1-0.0.6/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     7032 2024-04-01 20:37:10.726323 crm1-0.0.6/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      182 2024-04-01 19:40:39.007960 crm1-0.0.6/crm1/spec/__init__.py
+-rw-r--r--   0        0        0      486 2024-04-01 17:35:21.364549 crm1-0.0.6/crm1/spec/dependency.py
+-rw-r--r--   0        0        0      978 2024-04-01 20:26:21.932441 crm1-0.0.6/crm1/spec/mod.py
+-rw-r--r--   0        0        0      606 2024-04-01 17:35:16.918527 crm1-0.0.6/crm1/spec/repository.py
+-rw-r--r--   0        0        0     1692 2024-04-01 20:21:17.411767 crm1-0.0.6/crm1/spec/unsafe_modext.py
+-rw-r--r--   0        0        0      158 2024-04-01 18:09:31.539707 crm1-0.0.6/crm1/types/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-01 19:38:40.277289 crm1-0.0.6/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1221 2024-04-01 19:41:25.588271 crm1-0.0.6/crm1/types/mod.py
+-rw-r--r--   0        0        0     1933 2024-04-01 19:41:34.284778 crm1-0.0.6/crm1/types/repository.py
+-rw-r--r--   0        0        0     2709 2024-04-01 19:42:47.392723 crm1-0.0.6/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      595 2024-04-01 20:25:30.948258 crm1-0.0.6/crm1/utils.py
+-rw-r--r--   0        0        0     1085 2024-04-01 17:50:55.501196 crm1-0.0.6/LICENSE
+-rw-r--r--   0        0        0      397 2024-04-01 20:38:31.299144 crm1-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3855 2024-04-01 19:43:56.788453 crm1-0.0.6/README.md
+-rw-r--r--   0        0        0     4299 1970-01-01 00:00:00.000000 crm1-0.0.6/PKG-INFO
```

### Comparing `crm1-0.0.5/crm1/helpers/versions.py` & `crm1-0.0.6/crm1/helpers/versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,16 @@
 
     def __str__(self) -> str:
         return self.to_string()
 
 
 def range_from_maven_string(version: str):
     """Create a VersionRange object from a Maven version string."""
+    if version == "*":
+        return VersionRange(None, DONTCARE, None, DONTCARE)
     if version.startswith(">="):
         lower_mode = VersionEndMode.INCLUSIVE
         lower = Version.from_string(version[2:])
         upper = None
         upper_mode = DONTCARE
     elif version.startswith(">"):
         lower_mode = VersionEndMode.EXCLUSIVE
```

### Comparing `crm1-0.0.5/crm1/spec/mod.py` & `crm1-0.0.6/crm1/spec/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/spec/repository.py` & `crm1-0.0.6/crm1/spec/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/spec/unsafe_modext.py` & `crm1-0.0.6/crm1/spec/unsafe_modext.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/types/dependency.py` & `crm1-0.0.6/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/types/mod.py` & `crm1-0.0.6/crm1/types/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/types/repository.py` & `crm1-0.0.6/crm1/types/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/types/repository_pool.py` & `crm1-0.0.6/crm1/types/repository_pool.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/crm1/utils.py` & `crm1-0.0.6/crm1/utils.py`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/LICENSE` & `crm1-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/README.md` & `crm1-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.0.5/PKG-INFO` & `crm1-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.0.5
+Version: 0.0.6
 Summary: A CRM-1 repository exploration package
 License: MIT
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

