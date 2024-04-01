# Comparing `tmp/mypy-boto3-1.34.8.tar.gz` & `tmp/mypy-boto3-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-1.34.8.tar", last modified: Tue Dec 26 20:32:06 2023, max compression
+gzip compressed data, was "mypy-boto3-1.34.9.tar", last modified: Wed Dec 27 20:32:14 2023, max compression
```

## Comparing `mypy-boto3-1.34.8.tar` & `mypy-boto3-1.34.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:06.092612 mypy-boto3-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-26 20:32:06.092612 mypy-boto3-1.34.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:06.092612 mypy-boto3-1.34.8/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-26 20:31:43.000000 mypy-boto3-1.34.8/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-26 20:31:43.000000 mypy-boto3-1.34.8/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-26 20:31:44.000000 mypy-boto3-1.34.8/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2023-12-26 20:31:43.000000 mypy-boto3-1.34.8/mypy_boto3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2023-12-26 20:31:44.000000 mypy-boto3-1.34.8/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 20:31:44.000000 mypy-boto3-1.34.8/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   114250 2023-12-26 20:31:43.000000 mypy-boto3-1.34.8/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-26 20:31:43.000000 mypy-boto3-1.34.8/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 20:32:06.092612 mypy-boto3-1.34.8/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-26 20:32:06.000000 mypy-boto3-1.34.8/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 20:32:06.092612 mypy-boto3-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-26 20:31:42.000000 mypy-boto3-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.351771 mypy-boto3-1.34.9/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   114250 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/setup.py
```

### Comparing `mypy-boto3-1.34.8/LICENSE` & `mypy-boto3-1.34.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/PKG-INFO` & `mypy-boto3-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.8
-Summary: Type annotations for boto3 1.34.8 master module generated with mypy-boto3-builder 7.23.0
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.34.8/README.md` & `mypy-boto3-1.34.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.34.8/mypy_boto3/boto3_init_stub.py` & `mypy-boto3-1.34.9/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/mypy_boto3/boto3_session_stub.py` & `mypy-boto3-1.34.9/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/mypy_boto3/literals.py` & `mypy-boto3-1.34.9/mypy_boto3/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/mypy_boto3/main.py` & `mypy-boto3-1.34.9/mypy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/mypy_boto3/submodules.py` & `mypy-boto3-1.34.9/mypy_boto3/submodules.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.8/mypy_boto3.egg-info/PKG-INFO` & `mypy-boto3-1.34.9/mypy_boto3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.8
-Summary: Type annotations for boto3 1.34.8 master module generated with mypy-boto3-builder 7.23.0
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.8](https://boto3.amazonaws.com/v1/documentation/api/1.34.8/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
 [mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
```

### Comparing `mypy-boto3-1.34.8/setup.py` & `mypy-boto3-1.34.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.34.8",
+    version="1.34.9",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3 1.34.8 master module generated with mypy-boto3-builder 7.23.0"
+        "Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

