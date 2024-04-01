# Comparing `tmp/pystow-0.5.3.tar.gz` & `tmp/pystow-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystow-0.5.3.tar", last modified: Thu Feb 22 11:57:00 2024, max compression
+gzip compressed data, was "pystow-0.5.4.tar", last modified: Mon Apr  1 19:38:31 2024, max compression
```

## Comparing `pystow-0.5.3.tar` & `pystow-0.5.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.046947 pystow-0.5.3/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-10-30 21:20:45.000000 pystow-0.5.3/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      414 2023-10-30 21:20:45.000000 pystow-0.5.3/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     8918 2024-02-22 11:57:00.046868 pystow-0.5.3/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     7089 2023-11-07 07:55:13.000000 pystow-0.5.3/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.038669 pystow-0.5.3/docs/
--rw-r--r--   0 cthoyt     (501) staff       (20)      605 2023-10-30 21:20:45.000000 pystow-0.5.3/docs/Makefile
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.039815 pystow-0.5.3/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      211 2023-10-30 21:20:45.000000 pystow-0.5.3/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     6946 2024-02-22 11:56:59.000000 pystow-0.5.3/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2275 2023-10-30 21:20:45.000000 pystow-0.5.3/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     2714 2023-11-07 07:55:13.000000 pystow-0.5.3/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      252 2023-10-30 21:20:45.000000 pystow-0.5.3/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      113 2023-10-30 21:20:45.000000 pystow-0.5.3/docs/source/utils.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      367 2023-11-07 07:55:13.000000 pystow-0.5.3/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2241 2024-02-22 11:57:00.047281 pystow-0.5.3/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.037618 pystow-0.5.3/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.042844 pystow-0.5.3/src/pystow/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1019 2023-11-07 07:55:13.000000 pystow-0.5.3/src/pystow/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-10-30 21:20:45.000000 pystow-0.5.3/src/pystow/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    56435 2023-11-07 07:55:13.000000 pystow-0.5.3/src/pystow/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5837 2023-10-30 21:20:45.000000 pystow-0.5.3/src/pystow/cache.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1128 2023-10-30 21:20:45.000000 pystow-0.5.3/src/pystow/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     6148 2023-11-07 07:55:13.000000 pystow-0.5.3/src/pystow/config_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2116 2023-10-30 21:20:45.000000 pystow-0.5.3/src/pystow/constants.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    58026 2023-11-07 07:55:13.000000 pystow-0.5.3/src/pystow/impl.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:55:27.000000 pystow-0.5.3/src/pystow/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)    35905 2024-01-29 09:44:31.000000 pystow-0.5.3/src/pystow/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-02-22 11:56:59.000000 pystow-0.5.3/src/pystow/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.046192 pystow-0.5.3/src/pystow.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     8918 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1011 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       43 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-11-07 07:55:50.000000 pystow-0.5.3/src/pystow.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      238 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2024-02-22 11:57:00.000000 pystow-0.5.3/src/pystow.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.044851 pystow-0.5.3/tests/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:57:00.046024 pystow-0.5.3/tests/resources/
--rw-r--r--   0 cthoyt     (501) staff       (20)       20 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       32 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test.txt.md5
--rw-r--r--   0 cthoyt     (501) staff       (20)       42 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_1.csv
--rw-r--r--   0 cthoyt     (501) staff       (20)       20 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_1.json
--rw-r--r--   0 cthoyt     (501) staff       (20)       79 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_1.pkl
--rw-r--r--   0 cthoyt     (501) staff       (20)       39 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_1.tsv
--rw-r--r--   0 cthoyt     (501) staff       (20)       46 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_verbose.txt.md5
--rw-r--r--   0 cthoyt     (501) staff       (20)        4 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/resources/test_wrong.txt.md5
--rw-r--r--   0 cthoyt     (501) staff       (20)     3763 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2611 2023-10-30 21:20:45.000000 pystow-0.5.3/tests/test_caching.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4195 2023-11-07 07:55:13.000000 pystow-0.5.3/tests/test_config.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11495 2023-11-07 07:55:13.000000 pystow-0.5.3/tests/test_module.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    12949 2023-11-07 07:55:13.000000 pystow-0.5.3/tests/test_utils.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.865736 pystow-0.5.4/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-10-30 21:20:45.000000 pystow-0.5.4/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      414 2023-10-30 21:20:45.000000 pystow-0.5.4/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8919 2024-04-01 19:38:31.865659 pystow-0.5.4/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7089 2023-11-07 07:55:13.000000 pystow-0.5.4/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.857766 pystow-0.5.4/docs/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      605 2023-10-30 21:20:45.000000 pystow-0.5.4/docs/Makefile
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.858795 pystow-0.5.4/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      211 2023-10-30 21:20:45.000000 pystow-0.5.4/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6946 2024-04-01 19:38:31.000000 pystow-0.5.4/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2275 2023-10-30 21:20:45.000000 pystow-0.5.4/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2714 2023-11-07 07:55:13.000000 pystow-0.5.4/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      252 2023-10-30 21:20:45.000000 pystow-0.5.4/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      113 2023-10-30 21:20:45.000000 pystow-0.5.4/docs/source/utils.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      368 2024-03-28 09:57:50.000000 pystow-0.5.4/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2188 2024-04-01 19:38:31.866220 pystow-0.5.4/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.856973 pystow-0.5.4/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.861829 pystow-0.5.4/src/pystow/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1032 2024-03-28 09:57:48.000000 pystow-0.5.4/src/pystow/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-10-30 21:20:45.000000 pystow-0.5.4/src/pystow/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    56435 2023-11-07 07:55:13.000000 pystow-0.5.4/src/pystow/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5837 2023-10-30 21:20:45.000000 pystow-0.5.4/src/pystow/cache.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1447 2024-03-28 09:57:48.000000 pystow-0.5.4/src/pystow/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7119 2024-03-28 09:57:56.000000 pystow-0.5.4/src/pystow/config_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2116 2023-10-30 21:20:45.000000 pystow-0.5.4/src/pystow/constants.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    58026 2023-11-07 07:55:13.000000 pystow-0.5.4/src/pystow/impl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2024-02-22 11:55:27.000000 pystow-0.5.4/src/pystow/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)    35918 2024-03-28 09:58:16.000000 pystow-0.5.4/src/pystow/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.865047 pystow-0.5.4/src/pystow.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8919 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1011 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       43 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-11-07 07:55:50.000000 pystow-0.5.4/src/pystow.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      238 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2024-04-01 19:38:31.000000 pystow-0.5.4/src/pystow.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.863747 pystow-0.5.4/tests/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-01 19:38:31.864859 pystow-0.5.4/tests/resources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       20 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       32 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test.txt.md5
+-rw-r--r--   0 cthoyt     (501) staff       (20)       42 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_1.csv
+-rw-r--r--   0 cthoyt     (501) staff       (20)       20 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_1.json
+-rw-r--r--   0 cthoyt     (501) staff       (20)       79 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_1.pkl
+-rw-r--r--   0 cthoyt     (501) staff       (20)       39 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_1.tsv
+-rw-r--r--   0 cthoyt     (501) staff       (20)       46 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_verbose.txt.md5
+-rw-r--r--   0 cthoyt     (501) staff       (20)        4 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/resources/test_wrong.txt.md5
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3763 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2611 2023-10-30 21:20:45.000000 pystow-0.5.4/tests/test_caching.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4195 2023-11-07 07:55:13.000000 pystow-0.5.4/tests/test_config.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11495 2023-11-07 07:55:13.000000 pystow-0.5.4/tests/test_module.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    12949 2023-11-07 07:55:13.000000 pystow-0.5.4/tests/test_utils.py
```

### Comparing `pystow-0.5.3/LICENSE` & `pystow-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/PKG-INFO` & `pystow-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystow
-Version: 0.5.3
+Version: 0.5.4
 Summary: Easily pick a place to store data for your python package.
 Home-page: https://github.com/cthoyt/pystow
 Download-URL: https://github.com/cthoyt/pystow/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -12,19 +12,19 @@
 Project-URL: Bug Tracker, https://github.com/cthoyt/pystow/issues
 Keywords: caching,file management
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pickle5; python_version < "3.8"
 Requires-Dist: click
 Requires-Dist: requests
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pystow Version: 0.5.3 Summary: Easily pick a place
+Metadata-Version: 2.1 Name: pystow Version: 0.5.4 Summary: Easily pick a place
 to store data for your python package. Home-page: https://github.com/cthoyt/
 pystow Download-URL: https://github.com/cthoyt/pystow/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/pystow/issues Keywords: caching,file management
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pickle5; python_version < "3.8" Requires-Dist: click
 Requires-Dist: requests Requires-Dist: tqdm Provides-Extra: rdf Requires-Dist:
 rdflib; extra == "rdf" Provides-Extra: xml Requires-Dist: lxml; extra == "xml"
 Provides-Extra: pandas Requires-Dist: pandas; extra == "pandas" Provides-Extra:
 aws Requires-Dist: boto3; extra == "aws" Provides-Extra: tests Requires-Dist:
 coverage; extra == "tests" Requires-Dist: pytest; extra == "tests" Requires-
```

### Comparing `pystow-0.5.3/README.md` & `pystow-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/docs/Makefile` & `pystow-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/docs/source/conf.py` & `pystow-0.5.4/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'pystow'
 copyright = f'{date.today().year}, Charles Tapley Hoyt'
 author = 'Charles Tapley Hoyt'
 
 # The full version, including alpha/beta/rc tags.
-release = '0.5.3'
+release = '0.5.4'
 
 # The short X.Y version.
 parsed_version = re.match(
     '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
     release,
 )
 version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
```

### Comparing `pystow-0.5.3/docs/source/index.rst` & `pystow-0.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/docs/source/installation.rst` & `pystow-0.5.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/setup.cfg` & `pystow-0.5.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pystow
-version = 0.5.3
+version = 0.5.4
 description = Easily pick a place to store data for your python package.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/pystow
 download_url = https://github.com/cthoyt/pystow/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/pystow/issues
@@ -16,19 +16,19 @@
 license_file = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3 :: Only
 keywords = 
 	caching
 	file management
 
 [options]
 install_requires = 
@@ -94,17 +94,17 @@
 
 [darglint]
 docstring_style = sphinx
 strictness = full
 
 [flake8]
 ignore = 
-	S403 # pickle
-	S301 # pickle
-	W503 # line break before binary operator
+	S403
+	S301
+	W503
 	S410
 	S320
 exclude = 
 	.tox,
 	.git,
 	__pycache__,
 	docs/source/conf.py,
```

### Comparing `pystow-0.5.3/src/pystow/__init__.py` & `pystow-0.5.4/src/pystow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,12 +42,12 @@
     load_pickle_gz,
     load_rdf,
     load_xml,
     module,
     open,
     open_gz,
 )
-from .config_api import get_config, write_config  # noqa
+from .config_api import ConfigError, get_config, write_config  # noqa
 from .impl import Module  # noqa
 from .utils import ensure_readme  # noqa
 
 ensure_readme()
```

### Comparing `pystow-0.5.3/src/pystow/api.py` & `pystow-0.5.4/src/pystow/api.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/src/pystow/cache.py` & `pystow-0.5.4/src/pystow/cache.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/src/pystow/cli.py` & `pystow-0.5.4/src/pystow/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,50 +4,65 @@
 """Command line interface for PyStow."""
 
 import os
 from typing import Optional, Sequence
 
 import click
 
-from . import api
-
 
 @click.group()
 def main():
     """Run the PyStow CLI."""
 
 
 @main.command()
 @click.argument("keys", nargs=-1)
 @click.option("--name")
 def join(keys: Sequence[str], name: Optional[str]):
     """List a directory."""
+    from . import api
+
     click.echo(api.join(*keys, name=name))
 
 
 @main.command()
 @click.argument("keys", nargs=-1)
 def ls(keys: Sequence[str]):
     """List a directory."""
+    from . import api
+
     directory = api.join(*keys)
     _ls(directory)
 
 
 @main.command()
 @click.argument("keys", nargs=-1)
 @click.option("--url", required=True)
 @click.option("--name")
 @click.option("--force", is_flag=True)
 def ensure(keys: Sequence[str], url: str, name: Optional[str], force: bool):
     """Ensure a file is downloaded."""
+    from . import api
+
     path = api.ensure(*keys, url=url, name=name, force=force)
     _ls(path.parent)
 
 
 def _ls(directory):
     command = f"ls -al {directory}"
     click.secho(f"[pystow] {command}", fg="cyan", bold=True)
     os.system(command)  # noqa:S605
 
 
+@main.command(name="set")
+@click.argument("module")
+@click.argument("key")
+@click.argument("value")
+def set_config(module: str, key: str, value: str):
+    """Set a configuration value."""
+    from .config_api import write_config
+
+    write_config(module, key, value)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `pystow-0.5.3/src/pystow/config_api.py` & `pystow-0.5.4/src/pystow/config_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,21 +32,43 @@
         :param module: Name of the module, e.g., ``bioportal``
         :param key: Name of the key inside the module, e.g., ``api_key``
         """
         self.module = module
         self.key = key
 
     def __str__(self) -> str:
+        path = get_home().joinpath(self.module).with_suffix(".ini")
         return dedent(
             f"""\
-        Could not look up {self.module}/{self.key} and no default given
+        Could not look up {self.module}/{self.key} and no default given.
 
-        1. Set the {self.module.upper()}_{self.key.upper()}
-        2. Create a file in {get_home()}/{self.module}.ini, create a section inside it
-           called [{self.module}] and set a value for {self.key} = ...
+        This can be solved with one of the following:
+
+        1. Set the {self.module.upper()}_{self.key.upper()} environment variable
+
+           - Windows, via GUI: https://www.computerhope.com/issues/ch000549.htm
+           - Windows, via CLI: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/set_1
+           - Mac OS: https://apple.stackexchange.com/questions/106778/how-do-i-set-environment-variables-on-os-x
+           - Linux: https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/
+
+        2. Use the PyStow CLI from the command line to
+           set the configuration like so:
+
+           $ pystow set {self.module} {self.key} <value>
+
+           This creates an INI file in {path}
+           with the configuration in the right place.
+
+        3. Create/edit an INI file in {path} and manually
+           fill it in by 1) creating a section inside it called [{self.module}]
+           and 2) setting a value for {self.key} = <value> that looks like:
+
+           # {path}
+           [{self.module}]
+           {self.key} = <value>
 
         See https://github.com/cthoyt/pystow#%EF%B8%8F%EF%B8%8F-configuration for more information.
         """
         )
 
 
 def get_name() -> str:
@@ -65,15 +87,15 @@
     :param ensure_exists: If true, ensures the directory is created
     :returns: A path object representing the pystow home directory, as one of:
 
         1. :data:`CONFIG_HOME_ENVVAR` environment variable or
         2. The default directory constructed in the user's home directory plus what's
            returned by :func:`get_name`.
     """
-    default = Path.home() / get_name()
+    default = Path.home().joinpath(get_name()).expanduser()
     return getenv_path(CONFIG_HOME_ENVVAR, default, ensure_exists=ensure_exists)
 
 
 @lru_cache(maxsize=1)
 def _get_cfp(module: str) -> ConfigParser:
     cfp = ConfigParser()
     directory = get_home()
```

### Comparing `pystow-0.5.3/src/pystow/constants.py` & `pystow-0.5.4/src/pystow/constants.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/src/pystow/impl.py` & `pystow-0.5.4/src/pystow/impl.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/src/pystow/utils.py` & `pystow-0.5.4/src/pystow/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
     """Get an environment variable representing a path, or use the default.
 
     :param envvar: The environmental variable name to check
     :param default: The default path to return if the environmental variable is not set
     :param ensure_exists: Should the directories leading to the path be created if they don't already exist?
     :return: A path either specified by the environmental variable or by the default.
     """
-    rv = Path(os.getenv(envvar, default=default))
+    rv = Path(os.getenv(envvar, default=default)).expanduser()
     mkdir(rv, ensure_exists=ensure_exists)
     return rv
 
 
 def n() -> str:
     """Get a random string for testing.
```

### Comparing `pystow-0.5.3/src/pystow.egg-info/PKG-INFO` & `pystow-0.5.4/src/pystow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystow
-Version: 0.5.3
+Version: 0.5.4
 Summary: Easily pick a place to store data for your python package.
 Home-page: https://github.com/cthoyt/pystow
 Download-URL: https://github.com/cthoyt/pystow/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -12,19 +12,19 @@
 Project-URL: Bug Tracker, https://github.com/cthoyt/pystow/issues
 Keywords: caching,file management
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pickle5; python_version < "3.8"
 Requires-Dist: click
 Requires-Dist: requests
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: pystow Version: 0.5.3 Summary: Easily pick a place
+Metadata-Version: 2.1 Name: pystow Version: 0.5.4 Summary: Easily pick a place
 to store data for your python package. Home-page: https://github.com/cthoyt/
 pystow Download-URL: https://github.com/cthoyt/pystow/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/pystow/issues Keywords: caching,file management
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pickle5; python_version < "3.8" Requires-Dist: click
 Requires-Dist: requests Requires-Dist: tqdm Provides-Extra: rdf Requires-Dist:
 rdflib; extra == "rdf" Provides-Extra: xml Requires-Dist: lxml; extra == "xml"
 Provides-Extra: pandas Requires-Dist: pandas; extra == "pandas" Provides-Extra:
 aws Requires-Dist: boto3; extra == "aws" Provides-Extra: tests Requires-Dist:
 coverage; extra == "tests" Requires-Dist: pytest; extra == "tests" Requires-
```

### Comparing `pystow-0.5.3/src/pystow.egg-info/SOURCES.txt` & `pystow-0.5.4/src/pystow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/tests/test_api.py` & `pystow-0.5.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/tests/test_caching.py` & `pystow-0.5.4/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/tests/test_config.py` & `pystow-0.5.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/tests/test_module.py` & `pystow-0.5.4/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `pystow-0.5.3/tests/test_utils.py` & `pystow-0.5.4/tests/test_utils.py`

 * *Files identical despite different names*

