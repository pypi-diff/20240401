# Comparing `tmp/cdk8s-awscdk-resolver-0.0.8.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.8.tar", last modified: Mon Oct  9 06:15:32 2023, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.9.tar", last modified: Mon Oct  9 12:16:32 2023, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.8.tar` & `cdk8s-awscdk-resolver-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:15:32.345283 cdk8s-awscdk-resolver-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   804437 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 06:15:17.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 06:15:32.349283 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 06:15:32.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-10-09 06:15:32.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 06:15:32.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-09 06:15:32.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-09 06:15:32.000000 cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   804432 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.8/LICENSE` & `cdk8s-awscdk-resolver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.8/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.8
+Version: 0.0.9
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-awscdk-resolver-0.0.8/README.md` & `cdk8s-awscdk-resolver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.8/setup.py` & `cdk8s-awscdk-resolver-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.8",
+    "version": "0.0.9",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.8.jsii.tgz"
+            "awscdk-resolver@0.0.9.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.8/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.8
+Version: 0.0.9
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

