# Comparing `tmp/justogres-3.0.8.tar.gz` & `tmp/justogres-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justogres-3.0.8.tar", last modified: Mon Mar 25 15:48:07 2024, max compression
+gzip compressed data, was "justogres-3.0.9.tar", last modified: Mon Mar 25 19:57:16 2024, max compression
```

## Comparing `justogres-3.0.8.tar` & `justogres-3.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 15:48:07.468527 justogres-3.0.8/
--rw-r--r--   0 joseizam   (502) staff       (20)     1067 2022-03-24 13:45:23.000000 justogres-3.0.8/LICENSE
--rw-r--r--   0 joseizam   (502) staff       (20)     3610 2024-03-25 15:48:07.468100 justogres-3.0.8/PKG-INFO
--rw-r--r--   0 joseizam   (502) staff       (20)     2829 2023-12-14 14:35:36.000000 justogres-3.0.8/README.md
--rw-r--r--   0 joseizam   (502) staff       (20)       84 2022-03-25 21:47:06.000000 justogres-3.0.8/pyproject.toml
--rw-r--r--   0 joseizam   (502) staff       (20)      828 2024-03-25 15:48:07.471498 justogres-3.0.8/setup.cfg
-drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 15:48:07.455564 justogres-3.0.8/src/
-drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 15:48:07.459655 justogres-3.0.8/src/dftopo/
--rw-r--r--   0 joseizam   (502) staff       (20)       57 2022-03-24 13:45:23.000000 justogres-3.0.8/src/dftopo/__init__.py
--rw-r--r--   0 joseizam   (502) staff       (20)      642 2022-03-24 13:45:23.000000 justogres-3.0.8/src/dftopo/dfps.py
-drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 15:48:07.462528 justogres-3.0.8/src/justogres/
--rw-r--r--   0 joseizam   (502) staff       (20)      644 2024-03-25 15:43:46.000000 justogres-3.0.8/src/justogres/Mongo.py
--rw-r--r--   0 joseizam   (502) staff       (20)       91 2024-03-25 15:47:42.000000 justogres-3.0.8/src/justogres/__init__.py
--rw-r--r--   0 joseizam   (502) staff       (20)     4171 2023-02-14 15:24:04.000000 justogres-3.0.8/src/justogres/db.py
--rw-r--r--   0 joseizam   (502) staff       (20)     3732 2024-01-03 19:44:59.000000 justogres-3.0.8/src/justogres/spreadsheets.py
--rw-r--r--   0 joseizam   (502) staff       (20)      716 2022-12-15 17:40:04.000000 justogres-3.0.8/src/justogres/utils.py
-drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 15:48:07.466758 justogres-3.0.8/src/justogres.egg-info/
--rw-r--r--   0 joseizam   (502) staff       (20)     3610 2024-03-25 15:48:07.000000 justogres-3.0.8/src/justogres.egg-info/PKG-INFO
--rw-r--r--   0 joseizam   (502) staff       (20)      390 2024-03-25 15:48:07.000000 justogres-3.0.8/src/justogres.egg-info/SOURCES.txt
--rw-r--r--   0 joseizam   (502) staff       (20)        1 2024-03-25 15:48:07.000000 justogres-3.0.8/src/justogres.egg-info/dependency_links.txt
--rw-r--r--   0 joseizam   (502) staff       (20)       85 2024-03-25 15:48:07.000000 justogres-3.0.8/src/justogres.egg-info/requires.txt
--rw-r--r--   0 joseizam   (502) staff       (20)       17 2024-03-25 15:48:07.000000 justogres-3.0.8/src/justogres.egg-info/top_level.txt
+drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 19:57:16.276330 justogres-3.0.9/
+-rw-r--r--   0 joseizam   (502) staff       (20)     1067 2022-03-24 13:45:23.000000 justogres-3.0.9/LICENSE
+-rw-r--r--   0 joseizam   (502) staff       (20)     3610 2024-03-25 19:57:16.276105 justogres-3.0.9/PKG-INFO
+-rw-r--r--   0 joseizam   (502) staff       (20)     2829 2023-12-14 14:35:36.000000 justogres-3.0.9/README.md
+-rw-r--r--   0 joseizam   (502) staff       (20)       84 2022-03-25 21:47:06.000000 justogres-3.0.9/pyproject.toml
+-rw-r--r--   0 joseizam   (502) staff       (20)      828 2024-03-25 19:57:16.278379 justogres-3.0.9/setup.cfg
+drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 19:57:16.259649 justogres-3.0.9/src/
+drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 19:57:16.264048 justogres-3.0.9/src/dftopo/
+-rw-r--r--   0 joseizam   (502) staff       (20)       57 2022-03-24 13:45:23.000000 justogres-3.0.9/src/dftopo/__init__.py
+-rw-r--r--   0 joseizam   (502) staff       (20)      642 2022-03-24 13:45:23.000000 justogres-3.0.9/src/dftopo/dfps.py
+drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 19:57:16.269026 justogres-3.0.9/src/justogres/
+-rw-r--r--   0 joseizam   (502) staff       (20)      362 2024-03-25 19:56:46.000000 justogres-3.0.9/src/justogres/Mongo.py
+-rw-r--r--   0 joseizam   (502) staff       (20)       91 2024-03-25 15:47:42.000000 justogres-3.0.9/src/justogres/__init__.py
+-rw-r--r--   0 joseizam   (502) staff       (20)     4171 2023-02-14 15:24:04.000000 justogres-3.0.9/src/justogres/db.py
+-rw-r--r--   0 joseizam   (502) staff       (20)     3732 2024-01-03 19:44:59.000000 justogres-3.0.9/src/justogres/spreadsheets.py
+-rw-r--r--   0 joseizam   (502) staff       (20)      716 2022-12-15 17:40:04.000000 justogres-3.0.9/src/justogres/utils.py
+drwxr-xr-x   0 joseizam   (502) staff       (20)        0 2024-03-25 19:57:16.275207 justogres-3.0.9/src/justogres.egg-info/
+-rw-r--r--   0 joseizam   (502) staff       (20)     3610 2024-03-25 19:57:16.000000 justogres-3.0.9/src/justogres.egg-info/PKG-INFO
+-rw-r--r--   0 joseizam   (502) staff       (20)      390 2024-03-25 19:57:16.000000 justogres-3.0.9/src/justogres.egg-info/SOURCES.txt
+-rw-r--r--   0 joseizam   (502) staff       (20)        1 2024-03-25 19:57:16.000000 justogres-3.0.9/src/justogres.egg-info/dependency_links.txt
+-rw-r--r--   0 joseizam   (502) staff       (20)       85 2024-03-25 19:57:16.000000 justogres-3.0.9/src/justogres.egg-info/requires.txt
+-rw-r--r--   0 joseizam   (502) staff       (20)       17 2024-03-25 19:57:16.000000 justogres-3.0.9/src/justogres.egg-info/top_level.txt
```

### Comparing `justogres-3.0.8/LICENSE` & `justogres-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/PKG-INFO` & `justogres-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justogres
-Version: 3.0.8
+Version: 3.0.9
 Summary: This library is used to read or write data in Postgres, MongoDB (Only read) or Google Sheets
 Home-page: https://github.com/justo-bi/justogres
 Author: Jose Izam, Daniel Taiba
 Author-email: jose.izam99@gmail.com, danielt.dtr@gmail.com
 Project-URL: Bug Tracker, https://github.com/justo-bi/justogres
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `justogres-3.0.8/README.md` & `justogres-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/setup.cfg` & `justogres-3.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = justogres
-version = 3.0.8
+version = 3.0.9
 author = Jose Izam, Daniel Taiba
 author_email = jose.izam99@gmail.com, danielt.dtr@gmail.com
 description = This library is used to read or write data in Postgres, MongoDB (Only read) or Google Sheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/justo-bi/justogres
 project_urls =
```

### Comparing `justogres-3.0.8/src/dftopo/dfps.py` & `justogres-3.0.9/src/dftopo/dfps.py`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/src/justogres/db.py` & `justogres-3.0.9/src/justogres/db.py`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/src/justogres/spreadsheets.py` & `justogres-3.0.9/src/justogres/spreadsheets.py`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/src/justogres/utils.py` & `justogres-3.0.9/src/justogres/utils.py`

 * *Files identical despite different names*

### Comparing `justogres-3.0.8/src/justogres.egg-info/PKG-INFO` & `justogres-3.0.9/src/justogres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justogres
-Version: 3.0.8
+Version: 3.0.9
 Summary: This library is used to read or write data in Postgres, MongoDB (Only read) or Google Sheets
 Home-page: https://github.com/justo-bi/justogres
 Author: Jose Izam, Daniel Taiba
 Author-email: jose.izam99@gmail.com, danielt.dtr@gmail.com
 Project-URL: Bug Tracker, https://github.com/justo-bi/justogres
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

