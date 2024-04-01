# Comparing `tmp/pylogfile-0.0.1.dev1.tar.gz` & `tmp/pylogfile-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogfile-0.0.1.dev1.tar", last modified: Mon Apr  1 17:26:20 2024, max compression
+gzip compressed data, was "pylogfile-0.0.1.dev2.tar", last modified: Mon Apr  1 17:31:01 2024, max compression
```

## Comparing `pylogfile-0.0.1.dev1.tar` & `pylogfile-0.0.1.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:26:20.728052 pylogfile-0.0.1.dev1/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1503 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev1/LICENSE
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:26:20.727625 pylogfile-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       43 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev1/README.md
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      605 2024-04-01 17:26:02.000000 pylogfile-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       38 2024-04-01 17:26:20.728153 pylogfile-0.0.1.dev1/setup.cfg
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:26:20.724641 pylogfile-0.0.1.dev1/src/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:13:14.000000 pylogfile-0.0.1.dev1/src/__init__.py
-drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:26:20.727254 pylogfile-0.0.1.dev1/src/pylogfile.egg-info/
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:26:20.000000 pylogfile-0.0.1.dev1/src/pylogfile.egg-info/PKG-INFO
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      213 2024-04-01 17:26:20.000000 pylogfile-0.0.1.dev1/src/pylogfile.egg-info/SOURCES.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        1 2024-04-01 17:26:20.000000 pylogfile-0.0.1.dev1/src/pylogfile.egg-info/dependency_links.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       19 2024-04-01 17:26:20.000000 pylogfile-0.0.1.dev1/src/pylogfile.egg-info/top_level.txt
--rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1788 2024-03-28 21:11:23.000000 pylogfile-0.0.1.dev1/src/pylogfile.py
+drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.844353 pylogfile-0.0.1.dev2/
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1503 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev2/LICENSE
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:31:01.843946 pylogfile-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       43 2024-03-28 21:07:52.000000 pylogfile-0.0.1.dev2/README.md
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      605 2024-04-01 17:30:40.000000 pylogfile-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       38 2024-04-01 17:31:01.844446 pylogfile-0.0.1.dev2/setup.cfg
+drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.841484 pylogfile-0.0.1.dev2/src/
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:13:14.000000 pylogfile-0.0.1.dev2/src/__init__.py
+drwxr-xr-x   0 grantgiesbrecht   (501) staff       (20)        0 2024-04-01 17:31:01.843515 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      579 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/PKG-INFO
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)      213 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/SOURCES.txt
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)        1 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/dependency_links.txt
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)       19 2024-04-01 17:31:01.000000 pylogfile-0.0.1.dev2/src/pylogfile.egg-info/top_level.txt
+-rw-r--r--   0 grantgiesbrecht   (501) staff       (20)     1788 2024-03-28 21:11:23.000000 pylogfile-0.0.1.dev2/src/pylogfile.py
```

### Comparing `pylogfile-0.0.1.dev1/LICENSE` & `pylogfile-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogfile-0.0.1.dev1/PKG-INFO` & `pylogfile-0.0.1.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogfile
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Universal log files for Python
 Author-email: Grant Giesbrecht <grant.giesbrecht@colorado.edu>
 Project-URL: Homepage, https://github.com/Grant-Giesbrecht/pylogfile
 Project-URL: Issues, https://github.com/Grant-Giesbrecht/pylogfile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylogfile-0.0.1.dev1/pyproject.toml` & `pylogfile-0.0.1.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylogfile"
-version = "0.0.1.dev1"
+version = "0.0.1.dev2"
 authors = [
   { name="Grant Giesbrecht", email="grant.giesbrecht@colorado.edu" },
 ]
 description = "Universal log files for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pylogfile-0.0.1.dev1/src/pylogfile.egg-info/PKG-INFO` & `pylogfile-0.0.1.dev2/src/pylogfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogfile
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Universal log files for Python
 Author-email: Grant Giesbrecht <grant.giesbrecht@colorado.edu>
 Project-URL: Homepage, https://github.com/Grant-Giesbrecht/pylogfile
 Project-URL: Issues, https://github.com/Grant-Giesbrecht/pylogfile/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylogfile-0.0.1.dev1/src/pylogfile.py` & `pylogfile-0.0.1.dev2/src/pylogfile.py`

 * *Files identical despite different names*

