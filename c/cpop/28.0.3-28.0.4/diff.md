# Comparing `tmp/cpop-28.0.3.tar.gz` & `tmp/cpop-28.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.0.3.tar", last modified: Mon Apr  1 20:56:05 2024, max compression
+gzip compressed data, was "cpop-28.0.4.tar", last modified: Mon Apr  1 21:00:43 2024, max compression
```

## Comparing `cpop-28.0.3.tar` & `cpop-28.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.3/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      104 2024-04-01 20:54:49.000000 cpop-28.0.3/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:56:05.666188 cpop-28.0.3/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.3/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/cpop.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      535 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       13 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.3/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.3/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.3/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.3/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.662188 cpop-28.0.3/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.3/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.3/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.3/pop/mods/pop/test.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 20:55:26.000000 cpop-28.0.3/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.3/pop/pop.data.pyx
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.3/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1372 2024-04-01 20:55:06.000000 cpop-28.0.3/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 20:56:05.666188 cpop-28.0.3/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      149 2024-04-01 19:06:55.000000 cpop-28.0.3/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.327643 cpop-28.0.4/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.4/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      104 2024-04-01 20:54:49.000000 cpop-28.0.4/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:00:43.327643 cpop-28.0.4/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.4/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      535 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        4 2024-04-01 21:00:43.000000 cpop-28.0.4/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.4/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.4/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.4/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.4/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.323643 cpop-28.0.4/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/log/async.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/log/init.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.319643 cpop-28.0.4/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 21:00:43.327643 cpop-28.0.4/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.4/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.4/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.4/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.4/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 20:59:35.000000 cpop-28.0.4/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.4/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.4/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.4/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1315 2024-04-01 21:00:35.000000 cpop-28.0.4/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 21:00:43.327643 cpop-28.0.4/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1257 2024-04-01 20:59:31.000000 cpop-28.0.4/setup.py
```

### Comparing `cpop-28.0.3/LICENSE` & `cpop-28.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/PKG-INFO` & `cpop-28.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.3
+Version: 28.0.4
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.3/README.rst` & `cpop-28.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/cpop.egg-info/PKG-INFO` & `cpop-28.0.4/cpop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.3
+Version: 28.0.4
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.3/cpop.egg-info/SOURCES.txt` & `cpop-28.0.4/cpop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/hub/__main__.py` & `cpop-28.0.4/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/contract.py` & `cpop-28.0.4/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/dirs.py` & `cpop-28.0.4/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/exc.py` & `cpop-28.0.4/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/hub.py` & `cpop-28.0.4/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/loader.py` & `cpop-28.0.4/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/log/async.py` & `cpop-28.0.4/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/mods/pop/config.py` & `cpop-28.0.4/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/mods/pop/contract.py` & `cpop-28.0.4/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/mods/pop/sub.py` & `cpop-28.0.4/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/mods/pop/test.py` & `cpop-28.0.4/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/pop.data.c` & `cpop-28.0.4/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/pop.data.pyx` & `cpop-28.0.4/pop/pop.data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/ref.py` & `cpop-28.0.4/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/scanner.py` & `cpop-28.0.4/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pop/verify.py` & `cpop-28.0.4/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.3/pyproject.toml` & `cpop-28.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.0.3"
+version = "28.0.4"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
@@ -42,18 +42,14 @@
   "wheel",
   "twine",
 ]
 
 [project.scripts]
 hub = "hub.__main__:main"
 
-
-[tool.setuptools.packages.find]
-where = ["pop", "hub"]
-
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
```

