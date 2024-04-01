# Comparing `tmp/lineup-lang-0.1.1.tar.gz` & `tmp/lineup-lang-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineup-lang-0.1.1.tar", last modified: Mon Apr  1 13:30:34 2024, max compression
+gzip compressed data, was "lineup-lang-0.1.2.tar", last modified: Mon Apr  1 13:33:21 2024, max compression
```

## Comparing `lineup-lang-0.1.1.tar` & `lineup-lang-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:30:34.209533 lineup-lang-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 13:30:34.209533 lineup-lang-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:30:34.205533 lineup-lang-0.1.1/lineup-lang/
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:30:34.205533 lineup-lang-0.1.1/lineup-lang/core/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/core/var_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:30:34.205533 lineup-lang-0.1.1/lineup-lang/executor/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/executor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/executor/jump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/lineup-lang/language_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:30:34.209533 lineup-lang-0.1.1/lineup_lang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 13:30:34.000000 lineup-lang-0.1.1/lineup_lang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 13:30:34.000000 lineup-lang-0.1.1/lineup_lang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:30:34.000000 lineup-lang-0.1.1/lineup_lang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 13:30:34.000000 lineup-lang-0.1.1/lineup_lang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:30:34.209533 lineup-lang-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-01 13:30:30.000000 lineup-lang-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:33:21.729595 lineup-lang-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 13:33:21.729595 lineup-lang-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:33:21.725595 lineup-lang-0.1.2/lineup_lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:33:21.725595 lineup-lang-0.1.2/lineup_lang/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/core/var_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:33:21.729595 lineup-lang-0.1.2/lineup_lang/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/executor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/executor/jump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/lineup_lang/language_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:33:21.729595 lineup-lang-0.1.2/lineup_lang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 13:33:21.000000 lineup-lang-0.1.2/lineup_lang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-01 13:33:21.000000 lineup-lang-0.1.2/lineup_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:33:21.000000 lineup-lang-0.1.2/lineup_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 13:33:21.000000 lineup-lang-0.1.2/lineup_lang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:33:21.729595 lineup-lang-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-01 13:33:16.000000 lineup-lang-0.1.2/setup.py
```

### Comparing `lineup-lang-0.1.1/LICENSE` & `lineup-lang-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/PKG-INFO` & `lineup-lang-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineup-lang
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pseudo language interpreter for Python
 Home-page: https://github.com/alex-bouget/Lineup
 Author: alex-bouget
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lineup-lang-0.1.1/lineup-lang/__init__.py` & `lineup-lang-0.1.2/lineup_lang/__init__.py`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/lineup-lang/core/var_object.py` & `lineup-lang-0.1.2/lineup_lang/core/var_object.py`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/lineup-lang/executor/default.py` & `lineup-lang-0.1.2/lineup_lang/executor/default.py`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/lineup-lang/executor/jump.py` & `lineup-lang-0.1.2/lineup_lang/executor/jump.py`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/lineup-lang/language_object.py` & `lineup-lang-0.1.2/lineup_lang/language_object.py`

 * *Files identical despite different names*

### Comparing `lineup-lang-0.1.1/lineup_lang.egg-info/PKG-INFO` & `lineup-lang-0.1.2/lineup_lang.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineup-lang
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pseudo language interpreter for Python
 Home-page: https://github.com/alex-bouget/Lineup
 Author: alex-bouget
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lineup-lang-0.1.1/setup.py` & `lineup-lang-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name="lineup-lang",
-    version="0.1.1",
+    version="0.1.2",
     description="Pseudo language interpreter for Python",
     long_description=Path(__file__).parent.joinpath("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/alex-bouget/Lineup",
     author="alex-bouget",
-    packages=["lineup-lang", "lineup-lang.core", "lineup-lang.executor"],
+    packages=["lineup_lang", "lineup_lang.core", "lineup_lang.executor"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Interpreters",
```

