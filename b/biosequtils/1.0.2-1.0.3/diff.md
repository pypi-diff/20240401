# Comparing `tmp/biosequtils-1.0.2.tar.gz` & `tmp/biosequtils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosequtils-1.0.2.tar", last modified: Tue Mar 26 01:34:42 2024, max compression
+gzip compressed data, was "biosequtils-1.0.3.tar", last modified: Mon Apr  1 16:04:07 2024, max compression
```

## Comparing `biosequtils-1.0.2.tar` & `biosequtils-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:34:42.040007 biosequtils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 01:34:37.000000 biosequtils-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-26 01:34:42.040007 biosequtils-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-26 01:34:37.000000 biosequtils-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:34:42.040007 biosequtils-1.0.2/biosequtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-26 01:34:42.000000 biosequtils-1.0.2/biosequtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-26 01:34:42.000000 biosequtils-1.0.2/biosequtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 01:34:42.000000 biosequtils-1.0.2/biosequtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-26 01:34:42.000000 biosequtils-1.0.2/biosequtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 01:34:42.000000 biosequtils-1.0.2/biosequtils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 01:34:42.040007 biosequtils-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-26 01:34:37.000000 biosequtils-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 01:34:42.040007 biosequtils-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_handle_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_jtxt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-26 01:34:37.000000 biosequtils-1.0.2/tests/test_key_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:07.117835 biosequtils-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 16:03:55.000000 biosequtils-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-01 16:04:07.117835 biosequtils-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 16:03:55.000000 biosequtils-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:04:07.117835 biosequtils-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-01 16:03:55.000000 biosequtils-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:07.113835 biosequtils-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:07.117835 biosequtils-1.0.3/src/biosequtils/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/handle_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/jtxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 16:03:55.000000 biosequtils-1.0.3/src/biosequtils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:07.117835 biosequtils-1.0.3/src/biosequtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-01 16:04:07.000000 biosequtils-1.0.3/src/biosequtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 16:04:07.000000 biosequtils-1.0.3/src/biosequtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:04:07.000000 biosequtils-1.0.3/src/biosequtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-01 16:04:07.000000 biosequtils-1.0.3/src/biosequtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 16:04:07.000000 biosequtils-1.0.3/src/biosequtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:07.117835 biosequtils-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_handle_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_jtxt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-01 16:03:55.000000 biosequtils-1.0.3/tests/test_key_value.py
```

### Comparing `biosequtils-1.0.2/LICENSE` & `biosequtils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/PKG-INFO` & `biosequtils-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosequtils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provide methods on hand for bioinformatics coding work
 Home-page: https://github.com/Tiezhengyuan/bio_utils
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `biosequtils-1.0.2/biosequtils.egg-info/PKG-INFO` & `biosequtils-1.0.3/src/biosequtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosequtils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provide methods on hand for bioinformatics coding work
 Home-page: https://github.com/Tiezhengyuan/bio_utils
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `biosequtils-1.0.2/setup.py` & `biosequtils-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="biosequtils",
-    version='1.0.2',
+    version='1.0.3',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Provide methods on hand for bioinformatics coding work",
     url = "https://github.com/Tiezhengyuan/bio_utils",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(),
+    packages=['biosequtils'],
+    package_dir={'': 'src'},
     install_requires=['Bio', 'numpy', 'pandas'],
     keywords=['pypi', 'cicd', 'python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

### Comparing `biosequtils-1.0.2/tests/test_dir.py` & `biosequtils-1.0.3/tests/test_dir.py`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/tests/test_file.py` & `biosequtils-1.0.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/tests/test_handle_json.py` & `biosequtils-1.0.3/tests/test_handle_json.py`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/tests/test_iterator.py` & `biosequtils-1.0.3/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/tests/test_jtxt.py` & `biosequtils-1.0.3/tests/test_jtxt.py`

 * *Files identical despite different names*

### Comparing `biosequtils-1.0.2/tests/test_key_value.py` & `biosequtils-1.0.3/tests/test_key_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
         [{}, '', 1, {}],
         [{}, '-', 1, {}],
         [{}, None, 1, {}],
         [{'a':[]}, 'a', 1, {'a':[1,]}],
         [{'a':[1,]}, 'a', 1, {'a':[1,]}],
         [{'a':[0,]}, 'a', 1, {'a':[0,1,]}],
         [{'a':[1,]}, 'b', 2, {'a':[1,],'b':[2,]}],
+        # value is not list
+        [{'a':1}, 'a', [1,2], {'a':[1,2]}],
         # val is list
         [{}, 'a', [1,2], {'a':[1,2]}],
         [{'a':[1]}, 'a', [1,2], {'a':[1,2]}],
     )
     @unpack
     def test_update_dict(self, input, key, val, expect):
         KeyValue.update_dict(input, key, val)
```

