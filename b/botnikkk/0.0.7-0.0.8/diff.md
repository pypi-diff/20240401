# Comparing `tmp/botnikkk-0.0.7.tar.gz` & `tmp/botnikkk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.0.7.tar", last modified: Mon Apr  1 16:12:02 2024, max compression
+gzip compressed data, was "botnikkk-0.0.8.tar", last modified: Mon Apr  1 17:51:16 2024, max compression
```

## Comparing `botnikkk-0.0.7.tar` & `botnikkk-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:12:02.010647 botnikkk-0.0.7/
--rw-rw-rw-   0        0        0     2181 2024-04-01 16:12:02.007647 botnikkk-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1543 2024-04-01 16:11:21.000000 botnikkk-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 16:12:01.995499 botnikkk-0.0.7/botnikkk/
--rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.7/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.7/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:12:02.004655 botnikkk-0.0.7/botnikkk.egg-info/
--rw-rw-rw-   0        0        0     2181 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 16:12:01.000000 botnikkk-0.0.7/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 16:12:02.011647 botnikkk-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1000 2024-04-01 16:11:50.000000 botnikkk-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:51:16.672402 botnikkk-0.0.8/
+-rw-rw-rw-   0        0        0     2297 2024-04-01 17:51:16.668403 botnikkk-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1652 2024-04-01 17:49:44.000000 botnikkk-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 17:51:16.655401 botnikkk-0.0.8/botnikkk/
+-rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.8/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     2619 2024-04-01 16:02:27.000000 botnikkk-0.0.8/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:51:16.667401 botnikkk-0.0.8/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0     2297 2024-04-01 17:51:16.000000 botnikkk-0.0.8/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-01 17:51:16.000000 botnikkk-0.0.8/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 17:51:16.000000 botnikkk-0.0.8/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-01 17:51:16.000000 botnikkk-0.0.8/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 17:51:16.000000 botnikkk-0.0.8/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 17:51:16.672402 botnikkk-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2024-04-01 17:51:10.000000 botnikkk-0.0.8/setup.py
```

### Comparing `botnikkk-0.0.7/PKG-INFO` & `botnikkk-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.7
+Version: 0.0.8
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -81,12 +81,19 @@
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
+import asyncio
 
-await botnikkk.redirect("screen_name")
+async def function():
+
+    #some code
+    await botnikkk.redirect("screen_name")
+    #some more code
+
+asyncio.run(function())
 ```
 
 check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.7/README.md` & `botnikkk-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -63,12 +63,19 @@
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
+import asyncio
 
-await botnikkk.redirect("screen_name")
+async def function():
+
+    #some code
+    await botnikkk.redirect("screen_name")
+    #some more code
+
+asyncio.run(function())
 ```
 
 check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.7/botnikkk/formatting.py` & `botnikkk-0.0.8/botnikkk/formatting.py`

 * *Files identical despite different names*

### Comparing `botnikkk-0.0.7/botnikkk.egg-info/PKG-INFO` & `botnikkk-0.0.8/botnikkk.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.7
+Version: 0.0.8
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -81,12 +81,19 @@
 
 ## 4. redirect() function
 
 Usage = takes a input string as screen name and redirects the user to the said screen in a countdown of 3 seconds. Can only be used in async functions due it's await nature.
 
 ```python
 import botnikkk
+import asyncio
 
-await botnikkk.redirect("screen_name")
+async def function():
+
+    #some code
+    await botnikkk.redirect("screen_name")
+    #some more code
+
+asyncio.run(function())
 ```
 
 check out : https://botnikkk.github.io
```

### Comparing `botnikkk-0.0.7/setup.py` & `botnikkk-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

