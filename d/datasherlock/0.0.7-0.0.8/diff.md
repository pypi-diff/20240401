# Comparing `tmp/datasherlock-0.0.7.tar.gz` & `tmp/datasherlock-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasherlock-0.0.7.tar", last modified: Mon Sep 18 13:08:40 2023, max compression
+gzip compressed data, was "datasherlock-0.0.8.tar", last modified: Wed Dec 27 16:48:27 2023, max compression
```

## Comparing `datasherlock-0.0.7.tar` & `datasherlock-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-09-18 13:08:40.880234 datasherlock-0.0.7/
--rw-r--r--   0 runner    (1000) runner    (1000)     1125 2023-09-18 13:08:40.880234 datasherlock-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-09-18 13:08:12.000000 datasherlock-0.0.7/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-09-18 13:08:40.880234 datasherlock-0.0.7/datasherlock.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1125 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      232 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)      147 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-09-18 13:08:40.000000 datasherlock-0.0.7/datasherlock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-09-18 13:08:40.880234 datasherlock-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1558 2023-09-18 13:08:12.000000 datasherlock-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-12-27 16:48:27.530387 datasherlock-0.0.8/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1125 2023-12-27 16:48:27.526387 datasherlock-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      489 2023-12-27 16:48:24.000000 datasherlock-0.0.8/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-12-27 16:48:27.526387 datasherlock-0.0.8/datasherlock.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1125 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      232 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)      147 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-12-27 16:48:27.000000 datasherlock-0.0.8/datasherlock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-12-27 16:48:27.530387 datasherlock-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1558 2023-12-27 16:48:24.000000 datasherlock-0.0.8/setup.py
```

### Comparing `datasherlock-0.0.7/PKG-INFO` & `datasherlock-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: datasherlock
-Version: 0.0.7
+Version: 0.0.8
 Summary: datasherlock
 Home-page: http://datasherlocks.io
 Author: datasherlock
 Author-email: founder@textquery.dev
 License: UNKNOWN
 Description: Sherlock
         ==========================
```

### Comparing `datasherlock-0.0.7/datasherlock.egg-info/PKG-INFO` & `datasherlock-0.0.8/datasherlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: datasherlock
-Version: 0.0.7
+Version: 0.0.8
 Summary: datasherlock
 Home-page: http://datasherlocks.io
 Author: datasherlock
 Author-email: founder@textquery.dev
 License: UNKNOWN
 Description: Sherlock
         ==========================
```

### Comparing `datasherlock-0.0.7/setup.py` & `datasherlock-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 setuptools.setup(name='datasherlock',
                  version=__version__,
                  description='datasherlock',
                  long_description=open('README.md').read().strip(),
                  author='datasherlock',
                  author_email='founder@textquery.dev',
```

