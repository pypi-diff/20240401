# Comparing `tmp/bioomics-0.1.7.tar.gz` & `tmp/bioomics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.1.7.tar", last modified: Mon Apr  1 16:34:07 2024, max compression
+gzip compressed data, was "bioomics-0.1.9.tar", last modified: Mon Apr  1 19:10:36 2024, max compression
```

## Comparing `bioomics-0.1.7.tar` & `bioomics-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 16:34:03.000000 bioomics-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 16:34:07.020427 bioomics-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 16:34:03.000000 bioomics-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:34:07.020427 bioomics-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-01 16:34:03.000000 bioomics-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.016427 bioomics-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.016427 bioomics-0.1.7/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 16:34:03.000000 bioomics-0.1.7/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 16:34:07.000000 bioomics-0.1.7/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:34:07.020427 bioomics-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 16:34:03.000000 bioomics-0.1.7/tests/test_rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:10:36.364621 bioomics-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 19:10:32.000000 bioomics-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 19:10:36.364621 bioomics-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 19:10:32.000000 bioomics-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:10:36.364621 bioomics-0.1.9/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 19:10:36.000000 bioomics-0.1.9/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-01 19:10:36.000000 bioomics-0.1.9/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:10:36.000000 bioomics-0.1.9/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 19:10:36.000000 bioomics-0.1.9/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:10:36.000000 bioomics-0.1.9/bioomics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:10:36.364621 bioomics-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 19:10:32.000000 bioomics-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:10:36.364621 bioomics-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 19:10:32.000000 bioomics-0.1.9/tests/test_rnacentral.py
```

### Comparing `bioomics-0.1.7/LICENSE` & `bioomics-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/PKG-INFO` & `bioomics-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.1.7
+Version: 0.1.9
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.1.7/setup.py` & `bioomics-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.1.7',
+    version='0.1.9',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=['bioomics'],
-    package_dir={'': 'src'},
+    packages=find_packages(include=['bioomics']),
     install_requires=[
         "Bio",
         "biosequtils",
         "lxml",
         "redis",
         "sh",
     ],
```

### Comparing `bioomics-0.1.7/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.1.9/bioomics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.1.7
+Version: 0.1.9
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.1.7/tests/test_conn_ftp.py` & `bioomics-0.1.9/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/tests/test_conn_ftplib.py` & `bioomics-0.1.9/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/tests/test_conn_redis.py` & `bioomics-0.1.9/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/tests/test_mirbase.py` & `bioomics-0.1.9/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/tests/test_ncbi.py` & `bioomics-0.1.9/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.1.7/tests/test_rnacentral.py` & `bioomics-0.1.9/tests/test_rnacentral.py`

 * *Files identical despite different names*

