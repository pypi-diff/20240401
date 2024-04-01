# Comparing `tmp/jinny-1.9.3.tar.gz` & `tmp/jinny-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinny-1.9.3.tar", last modified: Sun Jan  7 20:28:18 2024, max compression
+gzip compressed data, was "jinny-1.9.4.tar", last modified: Sat Mar 30 21:36:42 2024, max compression
```

## Comparing `jinny-1.9.3.tar` & `jinny-1.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:28:18.870399 jinny-1.9.3/
--rw-r--r--   0 root         (0) root         (0)    35148 2024-01-07 20:28:16.000000 jinny-1.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3442 2024-01-07 20:28:18.870399 jinny-1.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2825 2024-01-07 20:28:16.000000 jinny-1.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-07 20:28:16.000000 jinny-1.9.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-07 20:28:18.874399 jinny-1.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1379 2024-01-07 20:28:16.000000 jinny-1.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:28:18.866399 jinny-1.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:28:18.870399 jinny-1.9.3/src/jinny/
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:28:18.870399 jinny-1.9.3/src/jinny/imports/
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/imports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3876 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/imports/filter_extensions.py
--rw-r--r--   0 root         (0) root         (0)     2205 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/imports/global_extensions.py
--rwxr-xr-x   0 root         (0) root         (0)    27700 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/jinny.py
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-07 20:28:16.000000 jinny-1.9.3/src/jinny/version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-07 20:28:18.870399 jinny-1.9.3/src/jinny.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3442 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-01-07 20:28:18.000000 jinny-1.9.3/src/jinny.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 21:36:42.401114 jinny-1.9.4/
+-rw-r--r--   0 root         (0) root         (0)    35148 2024-03-30 21:36:40.000000 jinny-1.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-03-30 21:36:42.401114 jinny-1.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2825 2024-03-30 21:36:40.000000 jinny-1.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-30 21:36:40.000000 jinny-1.9.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-30 21:36:42.401114 jinny-1.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-03-30 21:36:40.000000 jinny-1.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 21:36:42.393114 jinny-1.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 21:36:42.397114 jinny-1.9.4/src/jinny/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 21:36:42.401114 jinny-1.9.4/src/jinny/imports/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/imports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/imports/filter_extensions.py
+-rw-r--r--   0 root         (0) root         (0)     2205 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/imports/global_extensions.py
+-rwxr-xr-x   0 root         (0) root         (0)    27700 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/jinny.py
+-rw-r--r--   0 root         (0) root         (0)        6 2024-03-30 21:36:40.000000 jinny-1.9.4/src/jinny/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 21:36:42.397114 jinny-1.9.4/src/jinny.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-03-30 21:36:42.000000 jinny-1.9.4/src/jinny.egg-info/top_level.txt
```

### Comparing `jinny-1.9.3/LICENSE` & `jinny-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jinny-1.9.3/PKG-INFO` & `jinny-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinny
-Version: 1.9.3
+Version: 1.9.4
 Summary: A practical templating tool for Jinja templates
 Home-page: 
 Author: smasherofallthings
 Author-email: bots@trulydigital.net
 License: GPLv3
 Project-URL: Github, https://github.com/smashthings/jinny
 Project-URL: Gitlab, https://gitlab.com/scripteddog/jinny
```

### Comparing `jinny-1.9.3/README.md` & `jinny-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `jinny-1.9.3/setup.py` & `jinny-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `jinny-1.9.3/src/jinny/imports/filter_extensions.py` & `jinny-1.9.4/src/jinny/imports/filter_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,7 +126,10 @@
 
 def removeext(s: str):
   root, ext = os.path.splitext(s)
   if not root:
     raise Exception(f"jinny.filter_extenions.removeext(): The provided path '{s}' did not result in a usable path via os.path.splitext(). Please check the documentation!")
   return root
 
+def newlinetr(s:str, v:str='<br />'):
+  return s.replace("\n", v)
+
```

### Comparing `jinny-1.9.3/src/jinny/imports/global_extensions.py` & `jinny-1.9.4/src/jinny/imports/global_extensions.py`

 * *Files identical despite different names*

### Comparing `jinny-1.9.3/src/jinny/jinny.py` & `jinny-1.9.4/src/jinny/jinny.py`

 * *Files identical despite different names*

### Comparing `jinny-1.9.3/src/jinny.egg-info/PKG-INFO` & `jinny-1.9.4/src/jinny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinny
-Version: 1.9.3
+Version: 1.9.4
 Summary: A practical templating tool for Jinja templates
 Home-page: 
 Author: smasherofallthings
 Author-email: bots@trulydigital.net
 License: GPLv3
 Project-URL: Github, https://github.com/smashthings/jinny
 Project-URL: Gitlab, https://gitlab.com/scripteddog/jinny
```

