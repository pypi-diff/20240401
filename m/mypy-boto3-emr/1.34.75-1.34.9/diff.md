# Comparing `tmp/mypy-boto3-emr-1.34.75.tar.gz` & `tmp/mypy-boto3-emr-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.34.75.tar", last modified: Mon Apr  1 20:08:27 2024, max compression
+gzip compressed data, was "mypy-boto3-emr-1.34.9.tar", last modified: Wed Dec 27 20:32:17 2023, max compression
```

## Comparing `mypy-boto3-emr-1.34.75.tar` & `mypy-boto3-emr-1.34.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.289738 mypy-boto3-emr-1.34.75/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-01 20:08:27.285738 mypy-boto3-emr-1.34.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12962 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.285738 mypy-boto3-emr-1.34.75/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45656 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45653 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    75067 2024-04-01 20:08:09.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    75067 2024-04-01 20:08:09.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-01 20:08:07.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:27.285738 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 20:08:27.000000 mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:08:27.289738 mypy-boto3-emr-1.34.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-01 20:08:06.000000 mypy-boto3-emr-1.34.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.875782 mypy-boto3-emr-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2023-12-27 20:32:17.875782 mypy-boto3-emr-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.871782 mypy-boto3-emr-1.34.9/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45001 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44998 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16456 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    74627 2023-12-27 20:32:06.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74627 2023-12-27 20:32:06.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2023-12-27 20:32:05.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.871782 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-27 20:32:17.000000 mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:17.875782 mypy-boto3-emr-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-27 20:32:04.000000 mypy-boto3-emr-1.34.9/setup.py
```

### Comparing `mypy-boto3-emr-1.34.75/LICENSE` & `mypy-boto3-emr-1.34.9/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-emr-1.34.75/PKG-INFO` & `mypy-boto3-emr-1.34.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.34.75
-Summary: Type annotations for boto3.EMR 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.9
+Summary: Type annotations for boto3.EMR 1.34.9 service generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,38 +25,37 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.34.75/README.md` & `mypy-boto3-emr-1.34.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,26 +793,14 @@
         the event of a job-flow
         error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_termination_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_termination_protection)
         """
 
-    def set_unhealthy_node_replacement(
-        self, *, JobFlowIds: Sequence[str], UnhealthyNodeReplacement: bool
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Specify whether to enable unhealthy node replacement, which lets Amazon EMR
-        gracefully replace core nodes on a cluster if any nodes become
-        unhealthy.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_unhealthy_node_replacement)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_unhealthy_node_replacement)
-        """
-
     def set_visible_to_all_users(
         self, *, JobFlowIds: Sequence[str], VisibleToAllUsers: bool
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_visible_to_all_users)
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -790,26 +790,14 @@
         the event of a job-flow
         error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_termination_protection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_termination_protection)
         """
 
-    def set_unhealthy_node_replacement(
-        self, *, JobFlowIds: Sequence[str], UnhealthyNodeReplacement: bool
-    ) -> EmptyResponseMetadataTypeDef:
-        """
-        Specify whether to enable unhealthy node replacement, which lets Amazon EMR
-        gracefully replace core nodes on a cluster if any nodes become
-        unhealthy.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_unhealthy_node_replacement)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/client/#set_unhealthy_node_replacement)
-        """
-
     def set_visible_to_all_users(
         self, *, JobFlowIds: Sequence[str], VisibleToAllUsers: bool
     ) -> EmptyResponseMetadataTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.set_visible_to_all_users)
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -285,15 +284,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -311,15 +309,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -342,15 +339,14 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -411,14 +407,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -592,21 +589,19 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
-    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -285,15 +284,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -311,15 +309,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -342,15 +339,14 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -411,14 +407,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -592,21 +589,19 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
-    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "SupportedProductConfigTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetKeepJobFlowAliveWhenNoStepsInputRequestTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
-    "SetUnhealthyNodeReplacementInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
@@ -292,18 +291,18 @@
     "RunJobFlowInputRequestTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": NotRequired[str],
         "Value": NotRequired[str],
@@ -1002,21 +1001,14 @@
 SetTerminationProtectionInputRequestTypeDef = TypedDict(
     "SetTerminationProtectionInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "TerminationProtected": bool,
     },
 )
-SetUnhealthyNodeReplacementInputRequestTypeDef = TypedDict(
-    "SetUnhealthyNodeReplacementInputRequestTypeDef",
-    {
-        "JobFlowIds": Sequence[str],
-        "UnhealthyNodeReplacement": bool,
-    },
-)
 SetVisibleToAllUsersInputRequestTypeDef = TypedDict(
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
@@ -1458,15 +1450,14 @@
         "InstanceGroups": NotRequired[List[InstanceGroupDetailTypeDef]],
         "NormalizedInstanceHours": NotRequired[int],
         "Ec2KeyName": NotRequired[str],
         "Ec2SubnetId": NotRequired[str],
         "Placement": NotRequired[PlacementTypeTypeDef],
         "KeepJobFlowAliveWhenNoSteps": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "HadoopVersion": NotRequired[str],
     },
 )
 ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "ClusterId": str,
@@ -1724,15 +1715,14 @@
         "LogUri": NotRequired[str],
         "LogEncryptionKmsKeyId": NotRequired[str],
         "RequestedAmiVersion": NotRequired[str],
         "RunningAmiVersion": NotRequired[str],
         "ReleaseLabel": NotRequired[str],
         "AutoTerminate": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "VisibleToAllUsers": NotRequired[bool],
         "Applications": NotRequired[List[ApplicationTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "ServiceRole": NotRequired[str],
         "NormalizedInstanceHours": NotRequired[int],
         "MasterPublicDnsName": NotRequired[str],
         "Configurations": NotRequired[List["ConfigurationTypeDef"]],
@@ -2219,15 +2209,14 @@
         "InstanceCount": NotRequired[int],
         "InstanceGroups": NotRequired[Sequence[InstanceGroupConfigTypeDef]],
         "InstanceFleets": NotRequired[Sequence[InstanceFleetConfigTypeDef]],
         "Ec2KeyName": NotRequired[str],
         "Placement": NotRequired[PlacementTypeTypeDef],
         "KeepJobFlowAliveWhenNoSteps": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "HadoopVersion": NotRequired[str],
         "Ec2SubnetId": NotRequired[str],
         "Ec2SubnetIds": NotRequired[Sequence[str]],
         "EmrManagedMasterSecurityGroup": NotRequired[str],
         "EmrManagedSlaveSecurityGroup": NotRequired[str],
         "ServiceAccessSecurityGroup": NotRequired[str],
         "AdditionalMasterSecurityGroups": NotRequired[Sequence[str]],
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
     "SupportedProductConfigTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetKeepJobFlowAliveWhenNoStepsInputRequestTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
-    "SetUnhealthyNodeReplacementInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
@@ -292,18 +291,18 @@
     "RunJobFlowInputRequestTypeDef",
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": NotRequired[str],
         "Value": NotRequired[str],
@@ -1002,21 +1001,14 @@
 SetTerminationProtectionInputRequestTypeDef = TypedDict(
     "SetTerminationProtectionInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "TerminationProtected": bool,
     },
 )
-SetUnhealthyNodeReplacementInputRequestTypeDef = TypedDict(
-    "SetUnhealthyNodeReplacementInputRequestTypeDef",
-    {
-        "JobFlowIds": Sequence[str],
-        "UnhealthyNodeReplacement": bool,
-    },
-)
 SetVisibleToAllUsersInputRequestTypeDef = TypedDict(
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
@@ -1458,15 +1450,14 @@
         "InstanceGroups": NotRequired[List[InstanceGroupDetailTypeDef]],
         "NormalizedInstanceHours": NotRequired[int],
         "Ec2KeyName": NotRequired[str],
         "Ec2SubnetId": NotRequired[str],
         "Placement": NotRequired[PlacementTypeTypeDef],
         "KeepJobFlowAliveWhenNoSteps": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "HadoopVersion": NotRequired[str],
     },
 )
 ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     {
         "ClusterId": str,
@@ -1724,15 +1715,14 @@
         "LogUri": NotRequired[str],
         "LogEncryptionKmsKeyId": NotRequired[str],
         "RequestedAmiVersion": NotRequired[str],
         "RunningAmiVersion": NotRequired[str],
         "ReleaseLabel": NotRequired[str],
         "AutoTerminate": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "VisibleToAllUsers": NotRequired[bool],
         "Applications": NotRequired[List[ApplicationTypeDef]],
         "Tags": NotRequired[List[TagTypeDef]],
         "ServiceRole": NotRequired[str],
         "NormalizedInstanceHours": NotRequired[int],
         "MasterPublicDnsName": NotRequired[str],
         "Configurations": NotRequired[List["ConfigurationTypeDef"]],
@@ -2219,15 +2209,14 @@
         "InstanceCount": NotRequired[int],
         "InstanceGroups": NotRequired[Sequence[InstanceGroupConfigTypeDef]],
         "InstanceFleets": NotRequired[Sequence[InstanceFleetConfigTypeDef]],
         "Ec2KeyName": NotRequired[str],
         "Placement": NotRequired[PlacementTypeTypeDef],
         "KeepJobFlowAliveWhenNoSteps": NotRequired[bool],
         "TerminationProtected": NotRequired[bool],
-        "UnhealthyNodeReplacement": NotRequired[bool],
         "HadoopVersion": NotRequired[str],
         "Ec2SubnetId": NotRequired[str],
         "Ec2SubnetIds": NotRequired[Sequence[str]],
         "EmrManagedMasterSecurityGroup": NotRequired[str],
         "EmrManagedSlaveSecurityGroup": NotRequired[str],
         "ServiceAccessSecurityGroup": NotRequired[str],
         "AdditionalMasterSecurityGroups": NotRequired[Sequence[str]],
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.34.75
-Summary: Type annotations for boto3.EMR 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.9
+Summary: Type annotations for boto3.EMR 1.34.9 service generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,38 +25,37 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-emr"></a>
 
 # mypy-boto3-emr
 
 [![PyPI - mypy-boto3-emr](https://img.shields.io/pypi/v/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-emr-1.34.75/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.34.9/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.34.75/setup.py` & `mypy-boto3-emr-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.34.75",
+    version="1.34.9",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EMR 1.34.75 service generated with mypy-boto3-builder 7.23.2",
+    description=(
+        "Type annotations for boto3.EMR 1.34.9 service generated with mypy-boto3-builder 7.23.0"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

