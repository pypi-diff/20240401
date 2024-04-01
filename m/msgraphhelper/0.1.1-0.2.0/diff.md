# Comparing `tmp/msgraphhelper-0.1.1.tar.gz` & `tmp/msgraphhelper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphhelper-0.1.1.tar", last modified: Mon Apr  1 00:10:50 2024, max compression
+gzip compressed data, was "msgraphhelper-0.2.0.tar", last modified: Mon Apr  1 17:23:10 2024, max compression
```

## Comparing `msgraphhelper-0.1.1.tar` & `msgraphhelper-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:10:50.833532 msgraphhelper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-04-01 00:10:50.829532 msgraphhelper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:10:50.829532 msgraphhelper-0.1.1/msgraphhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/msgraphhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/msgraphhelper/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/msgraphhelper/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/msgraphhelper/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:10:50.829532 msgraphhelper-0.1.1/msgraphhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-04-01 00:10:50.000000 msgraphhelper-0.1.1/msgraphhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-01 00:10:50.000000 msgraphhelper-0.1.1/msgraphhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:10:50.000000 msgraphhelper-0.1.1/msgraphhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 00:10:50.000000 msgraphhelper-0.1.1/msgraphhelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 00:10:50.000000 msgraphhelper-0.1.1/msgraphhelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:10:50.833532 msgraphhelper-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:10:50.829532 msgraphhelper-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 00:10:43.000000 msgraphhelper-0.1.1/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.438072 msgraphhelper-0.2.0/msgraphhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/msgraphhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/test/test_odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/test/test_url.py
```

### Comparing `msgraphhelper-0.1.1/LICENSE` & `msgraphhelper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.1.1/PKG-INFO` & `msgraphhelper-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphhelper
-Version: 0.1.1
+Version: 0.2.0
 Summary: Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 Author-email: Giles Antonio Radford <moof@metamoof.net>
 Project-URL: Homepage, https://github.com/metamoof/msgraphhelper
 Project-URL: Issues, https://github.com/metamoof/msgraphhelper/issues
 Keywords: azure-functions,ms-graph,graph,suscription,Webhooks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,14 +19,15 @@
 Requires-Dist: azure-functions
 Requires-Dist: azure-identity
 Requires-Dist: azure-data-tables
 Requires-Dist: azure-functions-durable
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: requests_mock; extra == "dev"
 
 # MSGraphHelper - Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 
 Handling Change Notifications in Microsoft Graph, along with its subscriptions and lifecycle notifications is quite complex, but it's all repetitive boilerplate. This library deals with many of the standard complexities, making it easy to just create functions that will handle specific change notifications, with just a decorator that indicates what they should subscribe to.
 
 This is a library for use in Azure Functions Python v2 applications. Currently Azure functions Python v1 is not supported.
```

### Comparing `msgraphhelper-0.1.1/README.md` & `msgraphhelper-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.1.1/msgraphhelper/session.py` & `msgraphhelper-0.2.0/msgraphhelper/session.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.1.1/msgraphhelper/subscriptions.py` & `msgraphhelper-0.2.0/msgraphhelper/subscriptions.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.1.1/msgraphhelper/url.py` & `msgraphhelper-0.2.0/msgraphhelper/url.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.1.1/msgraphhelper.egg-info/PKG-INFO` & `msgraphhelper-0.2.0/msgraphhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphhelper
-Version: 0.1.1
+Version: 0.2.0
 Summary: Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 Author-email: Giles Antonio Radford <moof@metamoof.net>
 Project-URL: Homepage, https://github.com/metamoof/msgraphhelper
 Project-URL: Issues, https://github.com/metamoof/msgraphhelper/issues
 Keywords: azure-functions,ms-graph,graph,suscription,Webhooks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -19,14 +19,15 @@
 Requires-Dist: azure-functions
 Requires-Dist: azure-identity
 Requires-Dist: azure-data-tables
 Requires-Dist: azure-functions-durable
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
+Requires-Dist: requests_mock; extra == "dev"
 
 # MSGraphHelper - Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 
 Handling Change Notifications in Microsoft Graph, along with its subscriptions and lifecycle notifications is quite complex, but it's all repetitive boilerplate. This library deals with many of the standard complexities, making it easy to just create functions that will handle specific change notifications, with just a decorator that indicates what they should subscribe to.
 
 This is a library for use in Azure Functions Python v2 applications. Currently Azure functions Python v1 is not supported.
```

### Comparing `msgraphhelper-0.1.1/pyproject.toml` & `msgraphhelper-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgraphhelper"
-version = "0.1.1"
+version = "0.2.0"
 description = "Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions"
 readme = "README.md"
 authors = [{ name = "Giles Antonio Radford", email = "moof@metamoof.net" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -23,12 +23,12 @@
     "azure-identity",
     "azure-data-tables",
     "azure-functions-durable",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["pytest", "black"]
+dev = ["pytest", "black", "requests_mock"]
 
 [project.urls]
 Homepage = "https://github.com/metamoof/msgraphhelper"
 Issues = "https://github.com/metamoof/msgraphhelper/issues"
```

### Comparing `msgraphhelper-0.1.1/test/test_url.py` & `msgraphhelper-0.2.0/test/test_url.py`

 * *Files identical despite different names*

