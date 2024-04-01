# Comparing `tmp/authwa-0.3.8.tar.gz` & `tmp/authwa-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authwa-0.3.8.tar", max compression
+gzip compressed data, was "authwa-0.3.9.tar", max compression
```

## Comparing `authwa-0.3.8.tar` & `authwa-0.3.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     8233 2024-03-06 20:58:43.038304 authwa-0.3.8/authWA.py
--rw-r--r--   0        0        0      814 2024-03-06 20:59:02.589052 authwa-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    15359 2024-02-13 03:04:12.192685 authwa-0.3.8/README.md
--rw-r--r--   0        0        0    15603 1970-01-01 00:00:00.000000 authwa-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     8233 2024-03-06 20:58:43.038304 authwa-0.3.9/authWA.py
+-rw-r--r--   0        0        0      816 2024-03-06 21:02:44.102562 authwa-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    15359 2024-02-13 03:04:12.192685 authwa-0.3.9/README.md
+-rw-r--r--   0        0        0    15603 1970-01-01 00:00:00.000000 authwa-0.3.9/PKG-INFO
```

### Comparing `authwa-0.3.8/authWA.py` & `authwa-0.3.9/authWA.py`

 * *Files identical despite different names*

### Comparing `authwa-0.3.8/pyproject.toml` & `authwa-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "authwa"
-version = "0.3.8"
+version = "0.3.9"
 description = "Automações WhatsApp"
 authors = ["Guilherme Breve <64221923+foxtec198@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "authWA.py"}]
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
     "Natural Language :: Portuguese (Brazilian)",
     "Intended Audience :: Developers",
 ]   
 
-[tool.poetry.urls]
+[tool.poetry.urls]  
 "Documentação" = "https://authwa.readthedocs.io"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `authwa-0.3.8/README.md` & `authwa-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `authwa-0.3.8/PKG-INFO` & `authwa-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authwa
-Version: 0.3.8
+Version: 0.3.9
 Summary: Automações WhatsApp
 Author: Guilherme Breve
 Author-email: 64221923+foxtec198@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

