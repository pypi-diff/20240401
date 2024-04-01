# Comparing `tmp/cdklabs.generative-ai-cdk-constructs-0.1.98.tar.gz` & `tmp/cdklabs.generative-ai-cdk-constructs-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.generative-ai-cdk-constructs-0.1.98.tar", last modified: Thu Mar 21 23:49:24 2024, max compression
+gzip compressed data, was "cdklabs.generative-ai-cdk-constructs-0.1.99.tar", last modified: Fri Mar 22 15:08:28 2024, max compression
```

## Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98.tar` & `cdklabs.generative-ai-cdk-constructs-0.1.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.511872 cdklabs.generative-ai-cdk-constructs-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-03-21 23:49:24.511872 cdklabs.generative-ai-cdk-constructs-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 23:49:24.511872 cdklabs.generative-ai-cdk-constructs-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.503872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.503872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.507872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (127)   997192 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.507872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   584087 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/_jsii/generative-ai-cdk-constructs@0.1.98.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.507872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/bedrock/
--rw-r--r--   0 runner    (1001) docker     (127)   129509 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/bedrock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.507872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/
--rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.511872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 23:49:14.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:49:24.507872 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-03-21 23:49:24.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-21 23:49:24.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 23:49:24.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-21 23:49:24.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 23:49:24.000000 cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.139750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.139750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.143750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   997192 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   584081 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/_jsii/generative-ai-cdk-constructs@0.1.99.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/bedrock/
+-rw-r--r--   0 runner    (1001) docker     (127)   129509 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/bedrock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/
+-rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.147750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:08:17.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 15:08:28.143750 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-03-22 15:08:28.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-22 15:08:28.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 15:08:28.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-22 15:08:28.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 15:08:28.000000 cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/LICENSE` & `cdklabs.generative-ai-cdk-constructs-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/PKG-INFO` & `cdklabs.generative-ai-cdk-constructs-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.generative-ai-cdk-constructs
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS Generative AI CDK Constructs is a library for well-architected generative AI patterns.
 Home-page: https://github.com/awslabs/generative-ai-cdk-constructs
 Author: Amazon Web Services - Prototyping and Cloud Engineering
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/generative-ai-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/README.md` & `cdklabs.generative-ai-cdk-constructs-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/setup.py` & `cdklabs.generative-ai-cdk-constructs-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.generative-ai-cdk-constructs",
-    "version": "0.1.98",
+    "version": "0.1.99",
     "description": "AWS Generative AI CDK Constructs is a library for well-architected generative AI patterns.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/generative-ai-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services - Prototyping and Cloud Engineering",
     "bdist_wheel": {
         "universal": true
@@ -25,24 +25,24 @@
         "cdklabs.generative_ai_cdk_constructs._jsii",
         "cdklabs.generative_ai_cdk_constructs.bedrock",
         "cdklabs.generative_ai_cdk_constructs.opensearch_vectorindex",
         "cdklabs.generative_ai_cdk_constructs.opensearchserverless"
     ],
     "package_data": {
         "cdklabs.generative_ai_cdk_constructs._jsii": [
-            "generative-ai-cdk-constructs@0.1.98.jsii.tgz"
+            "generative-ai-cdk-constructs@0.1.99.jsii.tgz"
         ],
         "cdklabs.generative_ai_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.122.0, <3.0.0",
-        "cdk-nag>=2.28.69, <3.0.0",
+        "cdk-nag>=2.28.70, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/__init__.py` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/bedrock/__init__.py` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/__init__.py` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/__init__.py` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/PKG-INFO` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.generative-ai-cdk-constructs
-Version: 0.1.98
+Version: 0.1.99
 Summary: AWS Generative AI CDK Constructs is a library for well-architected generative AI patterns.
 Home-page: https://github.com/awslabs/generative-ai-cdk-constructs
 Author: Amazon Web Services - Prototyping and Cloud Engineering
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/generative-ai-cdk-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.generative-ai-cdk-constructs-0.1.98/src/cdklabs.generative_ai_cdk_constructs.egg-info/SOURCES.txt` & `cdklabs.generative-ai-cdk-constructs-0.1.99/src/cdklabs.generative_ai_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 src/cdklabs.generative_ai_cdk_constructs.egg-info/SOURCES.txt
 src/cdklabs.generative_ai_cdk_constructs.egg-info/dependency_links.txt
 src/cdklabs.generative_ai_cdk_constructs.egg-info/requires.txt
 src/cdklabs.generative_ai_cdk_constructs.egg-info/top_level.txt
 src/cdklabs/generative_ai_cdk_constructs/__init__.py
 src/cdklabs/generative_ai_cdk_constructs/py.typed
 src/cdklabs/generative_ai_cdk_constructs/_jsii/__init__.py
-src/cdklabs/generative_ai_cdk_constructs/_jsii/generative-ai-cdk-constructs@0.1.98.jsii.tgz
+src/cdklabs/generative_ai_cdk_constructs/_jsii/generative-ai-cdk-constructs@0.1.99.jsii.tgz
 src/cdklabs/generative_ai_cdk_constructs/bedrock/__init__.py
 src/cdklabs/generative_ai_cdk_constructs/opensearch_vectorindex/__init__.py
 src/cdklabs/generative_ai_cdk_constructs/opensearchserverless/__init__.py
```

