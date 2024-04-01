# Comparing `tmp/gammarer.aws-waf-geo-restriction-rule-group-1.3.1.tar.gz` & `tmp/gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-waf-geo-restriction-rule-group-1.3.1.tar", last modified: Mon Mar 18 19:21:30 2024, max compression
+gzip compressed data, was "gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar", last modified: Mon Apr  1 19:24:10 2024, max compression
```

## Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1.tar` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27038 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:21:19.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:21:30.761076 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-18 19:21:30.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-18 19:21:30.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:21:30.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-18 19:21:30.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 19:21:30.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.182466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.182466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27037 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:23:59.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:24:10.186466 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 19:24:10.000000 gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/LICENSE` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/PKG-INFO` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-geo-restriction-rule-group
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/README.md` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/setup.py` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-waf-geo-restriction-rule-group",
-    "version": "1.3.1",
+    "version": "1.3.2",
     "description": "This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_waf_geo_restriction_rule_group",
         "gammarer.aws_waf_geo_restriction_rule_group._jsii"
     ],
     "package_data": {
         "gammarer.aws_waf_geo_restriction_rule_group._jsii": [
-            "aws-waf-geo-restriction-rule-group@1.3.1.jsii.tgz"
+            "aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz"
         ],
         "gammarer.aws_waf_geo_restriction_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-waf-geo-restriction-rule-group
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-waf-geo-restriction-rule-group-1.3.1/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt` & `gammarer.aws-waf-geo-restriction-rule-group-1.3.2/src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
 src/gammarer.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
 src/gammarer/aws_waf_geo_restriction_rule_group/__init__.py
 src/gammarer/aws_waf_geo_restriction_rule_group/py.typed
 src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
-src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.1.jsii.tgz
+src/gammarer/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.3.2.jsii.tgz
```

