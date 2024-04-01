# Comparing `tmp/cpop-28.0.2.tar.gz` & `tmp/cpop-28.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpop-28.0.2.tar", last modified: Mon Apr  1 20:53:42 2024, max compression
+gzip compressed data, was "cpop-28.0.3.tar", last modified: Mon Apr  1 20:56:05 2024, max compression
```

## Comparing `cpop-28.0.2.tar` & `cpop-28.0.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.717392 cpop-28.0.2/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.2/LICENSE
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       77 2024-04-01 20:39:20.000000 cpop-28.0.2/MANIFEST.in
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:53:42.717392 cpop-28.0.2/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.2/README.rst
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.713391 cpop-28.0.2/cpop.egg-info/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/PKG-INFO
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      518 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/SOURCES.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/dependency_links.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/entry_points.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/requires.txt
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       13 2024-04-01 20:53:42.000000 cpop-28.0.2/cpop.egg-info/top_level.txt
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.713391 cpop-28.0.2/hub/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.2/hub/__init__.py
--rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.2/hub/__main__.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.713391 cpop-28.0.2/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/dirs.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.2/pop/exc.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.2/pop/hub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.2/pop/loader.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.717392 cpop-28.0.2/pop/log/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/log/async.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/log/init.py
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.713391 cpop-28.0.2/pop/mods/
-drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:53:42.717392 cpop-28.0.2/pop/mods/pop/
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.2/pop/mods/pop/config.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/mods/pop/contract.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.2/pop/mods/pop/dyne.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.2/pop/mods/pop/sub.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.2/pop/mods/pop/test.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 20:50:19.000000 cpop-28.0.2/pop/pop.data.c
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.2/pop/ref.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.2/pop/scanner.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.2/pop/verify.py
--rw-rw-r--   0 akmod     (1000) akmod     (1000)     1372 2024-04-01 20:39:25.000000 cpop-28.0.2/pyproject.toml
--rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 20:53:42.717392 cpop-28.0.2/setup.cfg
--rw-rw-r--   0 akmod     (1000) akmod     (1000)      149 2024-04-01 19:06:55.000000 cpop-28.0.2/setup.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11348 2024-03-24 19:08:30.000000 cpop-28.0.3/LICENSE
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      104 2024-04-01 20:54:49.000000 cpop-28.0.3/MANIFEST.in
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:56:05.666188 cpop-28.0.3/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4063 2024-04-01 20:42:25.000000 cpop-28.0.3/README.rst
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/cpop.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4648 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/PKG-INFO
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      535 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/SOURCES.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        1 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/dependency_links.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       42 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/entry_points.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      128 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/requires.txt
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       13 2024-04-01 20:56:05.000000 cpop-28.0.3/cpop.egg-info/top_level.txt
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/hub/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:07:30.000000 cpop-28.0.3/hub/__init__.py
+-rwxrwxr-x   0 akmod     (1000) akmod     (1000)     1979 2024-04-01 18:01:36.000000 cpop-28.0.3/hub/__main__.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    10888 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4379 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/dirs.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1573 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/exc.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    21514 2024-04-01 20:11:42.000000 cpop-28.0.3/pop/hub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)    11789 2024-04-01 17:46:15.000000 cpop-28.0.3/pop/loader.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/log/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     4750 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/log/async.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      491 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/log/init.py
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.662188 cpop-28.0.3/pop/mods/
+drwxrwxr-x   0 akmod     (1000) akmod     (1000)        0 2024-04-01 20:56:05.666188 cpop-28.0.3/pop/mods/pop/
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6077 2024-04-01 20:16:36.000000 cpop-28.0.3/pop/mods/pop/config.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      570 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/mods/pop/contract.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      234 2024-04-01 16:10:17.000000 cpop-28.0.3/pop/mods/pop/dyne.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6985 2024-04-01 17:42:04.000000 cpop-28.0.3/pop/mods/pop/sub.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      861 2024-04-01 19:09:27.000000 cpop-28.0.3/pop/mods/pop/test.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)   878107 2024-04-01 20:55:26.000000 cpop-28.0.3/pop/pop.data.c
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     6101 2024-04-01 19:03:13.000000 cpop-28.0.3/pop/pop.data.pyx
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      555 2024-04-01 17:31:50.000000 cpop-28.0.3/pop/ref.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1321 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/scanner.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     7642 2024-03-24 19:08:30.000000 cpop-28.0.3/pop/verify.py
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)     1372 2024-04-01 20:55:06.000000 cpop-28.0.3/pyproject.toml
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)       38 2024-04-01 20:56:05.666188 cpop-28.0.3/setup.cfg
+-rw-rw-r--   0 akmod     (1000) akmod     (1000)      149 2024-04-01 19:06:55.000000 cpop-28.0.3/setup.py
```

### Comparing `cpop-28.0.2/LICENSE` & `cpop-28.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/PKG-INFO` & `cpop-28.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.2
+Version: 28.0.3
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.2/README.rst` & `cpop-28.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/cpop.egg-info/PKG-INFO` & `cpop-28.0.3/cpop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 28.0.2
+Version: 28.0.3
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cpop-28.0.2/cpop.egg-info/SOURCES.txt` & `cpop-28.0.3/cpop.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 hub/__main__.py
 pop/contract.py
 pop/dirs.py
 pop/exc.py
 pop/hub.py
 pop/loader.py
 pop/pop.data.c
+pop/pop.data.pyx
 pop/ref.py
 pop/scanner.py
 pop/verify.py
 pop/log/async.py
 pop/log/init.py
 pop/mods/pop/config.py
 pop/mods/pop/contract.py
```

### Comparing `cpop-28.0.2/hub/__main__.py` & `cpop-28.0.3/hub/__main__.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/contract.py` & `cpop-28.0.3/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/dirs.py` & `cpop-28.0.3/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/exc.py` & `cpop-28.0.3/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/hub.py` & `cpop-28.0.3/pop/hub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/loader.py` & `cpop-28.0.3/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/log/async.py` & `cpop-28.0.3/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/mods/pop/config.py` & `cpop-28.0.3/pop/mods/pop/config.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/mods/pop/contract.py` & `cpop-28.0.3/pop/mods/pop/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/mods/pop/sub.py` & `cpop-28.0.3/pop/mods/pop/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/mods/pop/test.py` & `cpop-28.0.3/pop/mods/pop/test.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/pop.data.c` & `cpop-28.0.3/pop/pop.data.c`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/ref.py` & `cpop-28.0.3/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/scanner.py` & `cpop-28.0.3/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pop/verify.py` & `cpop-28.0.3/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-28.0.2/pyproject.toml` & `cpop-28.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpop"
-version = "28.0.2"
+version = "28.0.3"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

