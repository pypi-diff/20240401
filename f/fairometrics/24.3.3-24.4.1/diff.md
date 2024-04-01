# Comparing `tmp/fairometrics-24.3.3.tar.gz` & `tmp/fairometrics-24.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairometrics-24.3.3.tar", last modified: Wed Mar 13 17:21:11 2024, max compression
+gzip compressed data, was "fairometrics-24.4.1.tar", last modified: Mon Apr  1 16:11:53 2024, max compression
```

## Comparing `fairometrics-24.3.3.tar` & `fairometrics-24.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:21:11.660618 fairometrics-24.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-13 17:21:11.660618 fairometrics-24.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-13 17:21:08.000000 fairometrics-24.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:21:11.660618 fairometrics-24.3.3/fairometrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 17:21:08.000000 fairometrics-24.3.3/fairometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-03-13 17:21:08.000000 fairometrics-24.3.3/fairometrics/fairness_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    38716 2024-03-13 17:21:08.000000 fairometrics-24.3.3/fairometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-03-13 17:21:08.000000 fairometrics-24.3.3/fairometrics/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:21:11.660618 fairometrics-24.3.3/fairometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-13 17:21:11.000000 fairometrics-24.3.3/fairometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-13 17:21:11.000000 fairometrics-24.3.3/fairometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:21:11.000000 fairometrics-24.3.3/fairometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-13 17:21:11.000000 fairometrics-24.3.3/fairometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 17:21:11.660618 fairometrics-24.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-13 17:21:08.000000 fairometrics-24.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:11:53.181835 fairometrics-24.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-01 16:11:53.181835 fairometrics-24.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-01 16:11:33.000000 fairometrics-24.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:11:53.177835 fairometrics-24.4.1/fairometrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:11:33.000000 fairometrics-24.4.1/fairometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-01 16:11:33.000000 fairometrics-24.4.1/fairometrics/fairness_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38716 2024-04-01 16:11:33.000000 fairometrics-24.4.1/fairometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-01 16:11:33.000000 fairometrics-24.4.1/fairometrics/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:11:53.181835 fairometrics-24.4.1/fairometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-01 16:11:53.000000 fairometrics-24.4.1/fairometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-01 16:11:53.000000 fairometrics-24.4.1/fairometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:11:53.000000 fairometrics-24.4.1/fairometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 16:11:53.000000 fairometrics-24.4.1/fairometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:11:53.181835 fairometrics-24.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 16:11:33.000000 fairometrics-24.4.1/setup.py
```

### Comparing `fairometrics-24.3.3/PKG-INFO` & `fairometrics-24.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairometrics
-Version: 24.3.3
+Version: 24.4.1
 Summary: A collection of pre-certified fairness metrics supported by Fairo.
 Home-page: https://www.fairo.ai
 Author: Fairo Systems, Inc.
 Author-email: support@fairo.ai
 License: Apache-2.0
 Keywords: fairo fairness AI governance metrics
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `fairometrics-24.3.3/README.md` & `fairometrics-24.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fairometrics-24.3.3/fairometrics/fairness_object.py` & `fairometrics-24.4.1/fairometrics/fairness_object.py`

 * *Files identical despite different names*

### Comparing `fairometrics-24.3.3/fairometrics/metrics.py` & `fairometrics-24.4.1/fairometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `fairometrics-24.3.3/fairometrics/test.py` & `fairometrics-24.4.1/fairometrics/test.py`

 * *Files identical despite different names*

### Comparing `fairometrics-24.3.3/fairometrics.egg-info/PKG-INFO` & `fairometrics-24.4.1/fairometrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairometrics
-Version: 24.3.3
+Version: 24.4.1
 Summary: A collection of pre-certified fairness metrics supported by Fairo.
 Home-page: https://www.fairo.ai
 Author: Fairo Systems, Inc.
 Author-email: support@fairo.ai
 License: Apache-2.0
 Keywords: fairo fairness AI governance metrics
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `fairometrics-24.3.3/setup.py` & `fairometrics-24.4.1/setup.py`

 * *Files identical despite different names*

