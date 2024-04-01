# Comparing `tmp/wheelsmith-0.1.0.tar.gz` & `tmp/wheelsmith-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelsmith-0.1.0.tar", last modified: Mon Apr  1 15:34:13 2024, max compression
+gzip compressed data, was "wheelsmith-0.1.1.tar", last modified: Mon Apr  1 15:48:29 2024, max compression
```

## Comparing `wheelsmith-0.1.0.tar` & `wheelsmith-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:34:13.843073 wheelsmith-0.1.0/
--rw-r--r--   0 choco     (1000) choco     (1000)      638 2024-04-01 15:34:13.843073 wheelsmith-0.1.0/PKG-INFO
--rw-r--r--   0 choco     (1000) choco     (1000)       12 2024-04-01 15:32:16.000000 wheelsmith-0.1.0/README.md
--rw-r--r--   0 choco     (1000) choco     (1000)       38 2024-04-01 15:34:13.843073 wheelsmith-0.1.0/setup.cfg
--rw-r--r--   0 choco     (1000) choco     (1000)     1472 2024-04-01 15:30:53.000000 wheelsmith-0.1.0/setup.py
-drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:34:13.842073 wheelsmith-0.1.0/wheelsmith/
--rw-r--r--   0 choco     (1000) choco     (1000)       28 2024-04-01 15:25:16.000000 wheelsmith-0.1.0/wheelsmith/__init__.py
--rw-r--r--   0 choco     (1000) choco     (1000)       94 2024-04-01 15:24:51.000000 wheelsmith-0.1.0/wheelsmith/__main__.py
--rw-r--r--   0 choco     (1000) choco     (1000)     2293 2024-04-01 15:29:05.000000 wheelsmith-0.1.0/wheelsmith/wheelsmith.py
-drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:34:13.843073 wheelsmith-0.1.0/wheelsmith.egg-info/
--rw-r--r--   0 choco     (1000) choco     (1000)      638 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/PKG-INFO
--rw-r--r--   0 choco     (1000) choco     (1000)      295 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/SOURCES.txt
--rw-r--r--   0 choco     (1000) choco     (1000)        1 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/dependency_links.txt
--rw-r--r--   0 choco     (1000) choco     (1000)       66 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/entry_points.txt
--rw-r--r--   0 choco     (1000) choco     (1000)       17 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/requires.txt
--rw-r--r--   0 choco     (1000) choco     (1000)       11 2024-04-01 15:34:13.000000 wheelsmith-0.1.0/wheelsmith.egg-info/top_level.txt
+drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:48:29.953261 wheelsmith-0.1.1/
+-rw-r--r--   0 choco     (1000) choco     (1000)     3657 2024-04-01 15:48:29.953261 wheelsmith-0.1.1/PKG-INFO
+-rw-r--r--   0 choco     (1000) choco     (1000)     2591 2024-04-01 15:45:13.000000 wheelsmith-0.1.1/README.md
+-rw-r--r--   0 choco     (1000) choco     (1000)       38 2024-04-01 15:48:29.954261 wheelsmith-0.1.1/setup.cfg
+-rw-r--r--   0 choco     (1000) choco     (1000)     1473 2024-04-01 15:48:13.000000 wheelsmith-0.1.1/setup.py
+drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:48:29.952262 wheelsmith-0.1.1/wheelsmith/
+-rw-r--r--   0 choco     (1000) choco     (1000)       28 2024-04-01 15:25:16.000000 wheelsmith-0.1.1/wheelsmith/__init__.py
+-rw-r--r--   0 choco     (1000) choco     (1000)       94 2024-04-01 15:24:51.000000 wheelsmith-0.1.1/wheelsmith/__main__.py
+-rw-r--r--   0 choco     (1000) choco     (1000)     2293 2024-04-01 15:29:05.000000 wheelsmith-0.1.1/wheelsmith/wheelsmith.py
+drwxr-xr-x   0 choco     (1000) choco     (1000)        0 2024-04-01 15:48:29.953261 wheelsmith-0.1.1/wheelsmith.egg-info/
+-rw-r--r--   0 choco     (1000) choco     (1000)     3657 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/PKG-INFO
+-rw-r--r--   0 choco     (1000) choco     (1000)      295 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/SOURCES.txt
+-rw-r--r--   0 choco     (1000) choco     (1000)        1 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/dependency_links.txt
+-rw-r--r--   0 choco     (1000) choco     (1000)       66 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/entry_points.txt
+-rw-r--r--   0 choco     (1000) choco     (1000)       17 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/requires.txt
+-rw-r--r--   0 choco     (1000) choco     (1000)       11 2024-04-01 15:48:29.000000 wheelsmith-0.1.1/wheelsmith.egg-info/top_level.txt
```

### Comparing `wheelsmith-0.1.0/setup.py` & `wheelsmith-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.01'
 DESCRIPTION = 'A utility tool for building and publishing Python packages to PyPI'
 LONG_DESCRIPTION = 'WheelSmith is a command-line tool that simplifies the process of building and publishing Python packages to the Python Package Index (PyPI). It combines the steps of building wheels and uploading them to PyPI into a single command, making it easier for developers to distribute their packages.'
 
 # Setting up
 setup(
     name="wheelsmith",
     version=VERSION,
```

### Comparing `wheelsmith-0.1.0/wheelsmith/wheelsmith.py` & `wheelsmith-0.1.1/wheelsmith/wheelsmith.py`

 * *Files identical despite different names*

