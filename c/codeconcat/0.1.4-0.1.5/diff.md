# Comparing `tmp/codeconcat-0.1.4.tar.gz` & `tmp/codeconcat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeconcat-0.1.4.tar", last modified: Sat Mar  9 18:58:35 2024, max compression
+gzip compressed data, was "codeconcat-0.1.5.tar", last modified: Mon Apr  1 17:35:34 2024, max compression
```

## Comparing `codeconcat-0.1.4.tar` & `codeconcat-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:58:35.846706 codeconcat-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-09 18:58:35.842706 codeconcat-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-09 18:58:31.000000 codeconcat-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:58:35.842706 codeconcat-0.1.4/codeconcat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 18:58:31.000000 codeconcat-0.1.4/codeconcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-09 18:58:31.000000 codeconcat-0.1.4/codeconcat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 18:58:35.842706 codeconcat-0.1.4/codeconcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-09 18:58:35.000000 codeconcat-0.1.4/codeconcat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 18:58:35.846706 codeconcat-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-09 18:58:31.000000 codeconcat-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 17:35:34.695770 codeconcat-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 17:35:28.000000 codeconcat-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/codeconcat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:28.000000 codeconcat-0.1.5/codeconcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-01 17:35:28.000000 codeconcat-0.1.5/codeconcat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:35:34.695770 codeconcat-0.1.5/codeconcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 17:35:34.000000 codeconcat-0.1.5/codeconcat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:35:34.695770 codeconcat-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-01 17:35:28.000000 codeconcat-0.1.5/setup.py
```

### Comparing `codeconcat-0.1.4/PKG-INFO` & `codeconcat-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeconcat
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to concatenate a folders into a single text file
 Home-page: https://github.com/lguibr/CodeConcat
 Author: Luis Guilherme
 Author-email: lgpelin92@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lguibr/CodeConcat/issues
 Project-URL: Documentation, https://github.com/lguibr/CodeConcat/blob/main/README.md
```

### Comparing `codeconcat-0.1.4/README.md` & `codeconcat-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `codeconcat-0.1.4/codeconcat.egg-info/PKG-INFO` & `codeconcat-0.1.5/codeconcat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeconcat
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool to concatenate a folders into a single text file
 Home-page: https://github.com/lguibr/CodeConcat
 Author: Luis Guilherme
 Author-email: lgpelin92@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lguibr/CodeConcat/issues
 Project-URL: Documentation, https://github.com/lguibr/CodeConcat/blob/main/README.md
```

### Comparing `codeconcat-0.1.4/setup.py` & `codeconcat-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 url = "https://github.com/lguibr/CodeConcat"
 
 setup(
     name="codeconcat",
-    version="0.1.4",
+    version="0.1.5",
     author="Luis Guilherme",
     author_email="lgpelin92@gmail.com",
     description="A tool to concatenate a folders into a single text file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url=url,
```

