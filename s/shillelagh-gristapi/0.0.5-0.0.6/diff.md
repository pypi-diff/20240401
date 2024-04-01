# Comparing `tmp/shillelagh-gristapi-0.0.5.tar.gz` & `tmp/shillelagh-gristapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-gristapi-0.0.5.tar", last modified: Sun Mar 31 07:03:24 2024, max compression
+gzip compressed data, was "shillelagh-gristapi-0.0.6.tar", last modified: Mon Apr  1 19:14:54 2024, max compression
```

## Comparing `shillelagh-gristapi-0.0.5.tar` & `shillelagh-gristapi-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)    11357 2024-03-30 21:29:03.000000 shillelagh-gristapi-0.0.5/LICENSE.txt
--rw-r--r--   0 qleroy    (1000) qleroy    (1000)     2066 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/PKG-INFO
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     1445 2024-03-31 06:42:39.000000 shillelagh-gristapi-0.0.5/README.md
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      870 2024-03-31 07:03:18.000000 shillelagh-gristapi-0.0.5/pyproject.toml
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       38 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/setup.cfg
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.095742 shillelagh-gristapi-0.0.5/src/
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.095742 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        0 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__init__.py
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      175 2024-03-23 08:32:37.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     6995 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8234 2024-03-31 03:49:10.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8992 2024-03-31 03:49:05.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/grist.py
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/
--rw-r--r--   0 qleroy    (1000) qleroy    (1000)     2066 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/PKG-INFO
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      588 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/SOURCES.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        1 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/dependency_links.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       67 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/entry_points.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       35 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/requires.txt
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       20 2024-03-31 07:03:24.000000 shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/top_level.txt
-drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-03-31 07:03:24.099742 shillelagh-gristapi-0.0.5/tests/
--rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     1515 2024-03-31 03:27:06.000000 shillelagh-gristapi-0.0.5/tests/test_grist.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)    11357 2024-03-30 21:29:03.000000 shillelagh-gristapi-0.0.6/LICENSE.txt
+-rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/PKG-INFO
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     2819 2024-04-01 19:09:33.000000 shillelagh-gristapi-0.0.6/README.md
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      870 2024-04-01 19:14:29.000000 shillelagh-gristapi-0.0.6/pyproject.toml
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       38 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/setup.cfg
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.136668 shillelagh-gristapi-0.0.6/src/
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.140668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        0 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__init__.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      175 2024-03-23 08:32:37.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     6995 2024-03-23 05:41:01.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8234 2024-03-31 03:49:10.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     8992 2024-03-31 03:49:05.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/grist.py
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/
+-rw-r--r--   0 qleroy    (1000) qleroy    (1000)     3441 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/PKG-INFO
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)      588 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)        1 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       67 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/entry_points.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       35 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/requires.txt
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)       20 2024-04-01 19:14:54.000000 shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/top_level.txt
+drwxrwxr-x   0 qleroy    (1000) qleroy    (1000)        0 2024-04-01 19:14:54.144668 shillelagh-gristapi-0.0.6/tests/
+-rw-rw-r--   0 qleroy    (1000) qleroy    (1000)     1515 2024-03-31 03:27:06.000000 shillelagh-gristapi-0.0.6/tests/test_grist.py
```

### Comparing `shillelagh-gristapi-0.0.5/LICENSE.txt` & `shillelagh-gristapi-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.5/pyproject.toml` & `shillelagh-gristapi-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shillelagh-gristapi"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = ["requests >=2.31.0", "shillelagh >=1.2.6"]
 authors = [{ name = "Quentin Leroy", email = "quentin.n.leroy@gmail.com" }]
 description = "Shillelagh adapter for querying Grist Documents."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc` & `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/govinfo.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc` & `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/__pycache__/grist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.5/src/shillelagh_gristapi/grist.py` & `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi/grist.py`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.5/src/shillelagh_gristapi.egg-info/SOURCES.txt` & `shillelagh-gristapi-0.0.6/src/shillelagh_gristapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-gristapi-0.0.5/tests/test_grist.py` & `shillelagh-gristapi-0.0.6/tests/test_grist.py`

 * *Files identical despite different names*

