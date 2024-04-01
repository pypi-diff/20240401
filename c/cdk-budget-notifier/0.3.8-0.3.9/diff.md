# Comparing `tmp/cdk-budget-notifier-0.3.8.tar.gz` & `tmp/cdk-budget-notifier-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-budget-notifier/cdk-budget-notifier/dist/python/cdk-budget-notifier-0.3.8.tar", last modified: Mon Sep 13 15:57:10 2021, max compression
+gzip compressed data, was "/__w/cdk-budget-notifier/cdk-budget-notifier/dist/python/cdk-budget-notifier-0.3.9.tar", last modified: Sat Sep 25 18:31:42 2021, max compression
```

## Comparing `cdk-budget-notifier-0.3.8.tar` & `cdk-budget-notifier-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2853 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1910 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1900 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/
--rw-r--r--   0 root         (0) root         (0)    12162 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/_jsii/
--rw-r--r--   0 root         (0) root         (0)      480 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20099 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/_jsii/aws_budget_notifier@0.3.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-13 15:57:05.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2853 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-09-13 15:57:10.000000 cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2853 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1910 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1900 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/
+-rw-r--r--   0 root         (0) root         (0)    12162 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      480 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20102 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/_jsii/aws_budget_notifier@0.3.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-25 18:31:37.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2853 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      463 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-09-25 18:31:41.000000 cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/top_level.txt
```

### Comparing `cdk-budget-notifier-0.3.8/LICENSE` & `cdk-budget-notifier-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-budget-notifier-0.3.8/PKG-INFO` & `cdk-budget-notifier-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budget-notifier
-Version: 0.3.8
+Version: 0.3.9
 Summary: A simple AWS budget notifier.
 Home-page: https://github.com/stefan.freitag/projen-budget-notifier.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefan.freitag/projen-budget-notifier.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdk-budget-notifier Version: 0.3.8 Summary: A
+Metadata-Version: 2.1 Name: cdk-budget-notifier Version: 0.3.9 Summary: A
 simple AWS budget notifier. Home-page: https://github.com/stefan.freitag/
 projen-budget-notifier.git Author: Stefan Freitag
 udo.edu> License: Apache-2.0 Project-URL: Source, https://github.com/
 stefan.freitag/projen-budget-notifier.git Platform: UNKNOWN Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cdk-budget-notifier-0.3.8/README.md` & `cdk-budget-notifier-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-budget-notifier-0.3.8/setup.py` & `cdk-budget-notifier-0.3.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-budget-notifier",
-    "version": "0.3.8",
+    "version": "0.3.9",
     "description": "A simple AWS budget notifier.",
     "license": "Apache-2.0",
     "url": "https://github.com/stefan.freitag/projen-budget-notifier.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_budget_notifier",
         "cdk_budget_notifier._jsii"
     ],
     "package_data": {
         "cdk_budget_notifier._jsii": [
-            "aws_budget_notifier@0.3.8.jsii.tgz"
+            "aws_budget_notifier@0.3.9.jsii.tgz"
         ],
         "cdk_budget_notifier": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `cdk-budget-notifier-0.3.8/src/cdk_budget_notifier/__init__.py` & `cdk-budget-notifier-0.3.9/src/cdk_budget_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-budget-notifier-0.3.8/src/cdk_budget_notifier.egg-info/PKG-INFO` & `cdk-budget-notifier-0.3.9/src/cdk_budget_notifier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-budget-notifier
-Version: 0.3.8
+Version: 0.3.9
 Summary: A simple AWS budget notifier.
 Home-page: https://github.com/stefan.freitag/projen-budget-notifier.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefan.freitag/projen-budget-notifier.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdk-budget-notifier Version: 0.3.8 Summary: A
+Metadata-Version: 2.1 Name: cdk-budget-notifier Version: 0.3.9 Summary: A
 simple AWS budget notifier. Home-page: https://github.com/stefan.freitag/
 projen-budget-notifier.git Author: Stefan Freitag
 udo.edu> License: Apache-2.0 Project-URL: Source, https://github.com/
 stefan.freitag/projen-budget-notifier.git Platform: UNKNOWN Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.6
```

