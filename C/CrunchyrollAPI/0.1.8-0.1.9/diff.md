# Comparing `tmp/CrunchyrollAPI-0.1.8.tar.gz` & `tmp/CrunchyrollAPI-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CrunchyrollAPI-0.1.8.tar", last modified: Sun Mar 31 21:56:34 2024, max compression
+gzip compressed data, was "CrunchyrollAPI-0.1.9.tar", last modified: Sun Mar 31 22:14:28 2024, max compression
```

## Comparing `CrunchyrollAPI-0.1.8.tar` & `CrunchyrollAPI-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:56:34.580646 CrunchyrollAPI-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33914 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/crunchyrollapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/crunchyrollentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-03-31 21:56:34.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-31 21:56:34.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 21:56:34.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 21:56:34.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-31 21:56:34.000000 CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 21:56:34.584646 CrunchyrollAPI-0.1.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-03-31 21:56:28.000000 CrunchyrollAPI-0.1.8/test/test_crunchyrollapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:14:28.445188 CrunchyrollAPI-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-03-31 22:14:28.445188 CrunchyrollAPI-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 22:14:28.445188 CrunchyrollAPI-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:14:28.441187 CrunchyrollAPI-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:14:28.441187 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33961 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/crunchyrollapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/crunchyrollentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:14:28.441187 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41988 2024-03-31 22:14:28.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-31 22:14:28.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 22:14:28.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 22:14:28.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-31 22:14:28.000000 CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 22:14:28.441187 CrunchyrollAPI-0.1.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-03-31 22:14:24.000000 CrunchyrollAPI-0.1.9/test/test_crunchyrollapi.py
```

### Comparing `CrunchyrollAPI-0.1.8/LICENSE.txt` & `CrunchyrollAPI-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CrunchyrollAPI-0.1.8/PKG-INFO` & `CrunchyrollAPI-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrunchyrollAPI
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crunchyroll API Python interface
 Author-email: jbsky <webmaster@jbsky.fr>
 Maintainer-email: jbsky <webmaster@jbsky.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `CrunchyrollAPI-0.1.8/README.md` & `CrunchyrollAPI-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `CrunchyrollAPI-0.1.8/pyproject.toml` & `CrunchyrollAPI-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CrunchyrollAPI"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
   'requests'
 ]
 requires-python = ">=3.8"
 authors = [
   {name = "jbsky", email = "webmaster@jbsky.fr" },
 ]
```

### Comparing `CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/__init__.py` & `CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/crunchyrollapi.py` & `CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/crunchyrollapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,28 +46,24 @@
     session_restart = False
 
     def __init__(self):
         """Initialize arguments object
         Hold also references to the addon which can't be kept at module level.
         """
         if not hasattr(self, "crunchyroll_username"):
-            utils.crunchy_err(self, "No crunchyroll username")
-            exit(11)
+            utils.crunchy_warn(self, "No crunchyroll username")
 
         if not hasattr(self, "crunchyroll_password"):
-            utils.crunchy_err(self, "No crunchyroll password")
-            exit(12)
+            utils.crunchy_warn(self, "No crunchyroll password")
 
         if not hasattr(self, "subtitle"):
-            utils.crunchy_err(self, "No subtitle defined")
-            exit(13)
+            utils.crunchy_warn(self, "No subtitle defined in enUS enGB esLA esES ptBR ptPT frFR deDE arME itIT ruRU")
 
         if not hasattr(self, "subtitle_fallback"):
-            utils.crunchy_err(self, "subtitle_fallback")
-            exit(13)
+            utils.crunchy_warn(self, "No subtitle_fallback defined in enUS enGB esLA esES ptBR ptPT frFR deDE arME itIT ruRU")
 
         if not self.device_id:
             char_set = "0123456789abcdefghijklmnopqrstuvwxyz0123456789"
             self.device_id = (
                     "".join(random.sample(char_set, 8)) +
                     "-" +
                     "".join(self.name[0:4]) +
```

### Comparing `CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/crunchyrollentity.py` & `CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/crunchyrollentity.py`

 * *Files identical despite different names*

### Comparing `CrunchyrollAPI-0.1.8/src/CrunchyrollAPI/utils.py` & `CrunchyrollAPI-0.1.9/src/CrunchyrollAPI/utils.py`

 * *Files identical despite different names*

### Comparing `CrunchyrollAPI-0.1.8/src/CrunchyrollAPI.egg-info/PKG-INFO` & `CrunchyrollAPI-0.1.9/src/CrunchyrollAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CrunchyrollAPI
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crunchyroll API Python interface
 Author-email: jbsky <webmaster@jbsky.fr>
 Maintainer-email: jbsky <webmaster@jbsky.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `CrunchyrollAPI-0.1.8/test/test_crunchyrollapi.py` & `CrunchyrollAPI-0.1.9/test/test_crunchyrollapi.py`

 * *Files identical despite different names*

