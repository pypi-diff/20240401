# Comparing `tmp/boto3-stubs-lite-1.34.8.tar.gz` & `tmp/boto3-stubs-lite-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-lite-1.34.8.tar", last modified: Tue Dec 26 20:32:09 2023, max compression
+gzip compressed data, was "boto3-stubs-lite-1.34.9.tar", last modified: Wed Dec 27 20:32:17 2023, max compression
```

## Comparing `boto3-stubs-lite-1.34.8.tar` & `boto3-stubs-lite-1.34.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-26 20:31:52.000000 boto3-stubs-lite-1.34.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    70270 2023-12-26 20:31:52.000000 boto3-stubs-lite-1.34.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.096579 boto3-stubs-lite-1.34.8/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/crt.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.096579 boto3-stubs-lite-1.34.8/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.096579 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:52.000000 boto3-stubs-lite-1.34.8/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/s3/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    35996 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-26 20:32:09.000000 boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 20:32:09.100579 boto3-stubs-lite-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    49544 2023-12-26 20:31:51.000000 boto3-stubs-lite-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    70270 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/crt.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:04.000000 boto3-stubs-lite-1.34.9/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.255780 boto3-stubs-lite-1.34.9/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    82528 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    35996 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-27 20:32:17.000000 boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:17.259780 boto3-stubs-lite-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    49544 2023-12-27 20:32:03.000000 boto3-stubs-lite-1.34.9/setup.py
```

### Comparing `boto3-stubs-lite-1.34.8/LICENSE` & `boto3-stubs-lite-1.34.9/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/PKG-INFO` & `boto3-stubs-lite-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
-Version: 1.34.8
-Summary: Type annotations for boto3 1.34.8 generated with mypy-boto3-builder 7.23.0
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -417,15 +417,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-lite-1.34.8/README.md` & `boto3-stubs-lite-1.34.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/__init__.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/crt.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/crt.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/docs/utils.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/conditions.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/table.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/transform.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/dynamodb/types.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/exceptions.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/action.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/base.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/collection.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/model.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/params.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/resources/response.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/s3/inject.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/s3/transfer.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/session.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3-stubs/utils.pyi` & `boto3-stubs-lite-1.34.9/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/PKG-INFO` & `boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
-Version: 1.34.8
-Summary: Type annotations for boto3 1.34.8 generated with mypy-boto3-builder 7.23.0
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -417,15 +417,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs-lite.svg?color=blue)](https://pypi.org/project/boto3-stubs-lite)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/boto3-stubs-lite)](https://pepy.tech/project/boto3-stubs-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/SOURCES.txt` & `boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.34.8/boto3_stubs_lite.egg-info/requires.txt` & `boto3-stubs-lite-1.34.9/boto3_stubs_lite.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -499,16 +499,16 @@
 [bedrock-runtime]
 mypy-boto3-bedrock-runtime<1.35.0,>=1.34.0
 
 [billingconductor]
 mypy-boto3-billingconductor<1.35.0,>=1.34.0
 
 [boto3]
-boto3==1.34.8
-botocore==1.34.8
+boto3==1.34.9
+botocore==1.34.9
 
 [braket]
 mypy-boto3-braket<1.35.0,>=1.34.0
 
 [budgets]
 mypy-boto3-budgets<1.35.0,>=1.34.0
```

### Comparing `boto3-stubs-lite-1.34.8/setup.py` & `boto3-stubs-lite-1.34.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs-lite",
-    version="1.34.8",
+    version="1.34.9",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.8 generated with mypy-boto3-builder 7.23.0",
+    description="Type annotations for boto3 1.34.9 generated with mypy-boto3-builder 7.23.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -435,15 +435,15 @@
             "mypy-boto3-dynamodb>=1.34.0, <1.35.0",
             "mypy-boto3-ec2>=1.34.0, <1.35.0",
             "mypy-boto3-lambda>=1.34.0, <1.35.0",
             "mypy-boto3-rds>=1.34.0, <1.35.0",
             "mypy-boto3-s3>=1.34.0, <1.35.0",
             "mypy-boto3-sqs>=1.34.0, <1.35.0",
         ],
-        "boto3": ["boto3==1.34.8", "botocore==1.34.8"],
+        "boto3": ["boto3==1.34.9", "botocore==1.34.9"],
         "accessanalyzer": ["mypy-boto3-accessanalyzer>=1.34.0, <1.35.0"],
         "account": ["mypy-boto3-account>=1.34.0, <1.35.0"],
         "acm": ["mypy-boto3-acm>=1.34.0, <1.35.0"],
         "acm-pca": ["mypy-boto3-acm-pca>=1.34.0, <1.35.0"],
         "alexaforbusiness": ["mypy-boto3-alexaforbusiness>=1.34.0, <1.35.0"],
         "amp": ["mypy-boto3-amp>=1.34.0, <1.35.0"],
         "amplify": ["mypy-boto3-amplify>=1.34.0, <1.35.0"],
```

