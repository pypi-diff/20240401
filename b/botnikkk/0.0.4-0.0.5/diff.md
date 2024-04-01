# Comparing `tmp/botnikkk-0.0.4.tar.gz` & `tmp/botnikkk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botnikkk-0.0.4.tar", last modified: Sun Mar 31 11:14:28 2024, max compression
+gzip compressed data, was "botnikkk-0.0.5.tar", last modified: Mon Apr  1 12:43:28 2024, max compression
```

## Comparing `botnikkk-0.0.4.tar` & `botnikkk-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 11:14:28.910163 botnikkk-0.0.4/
--rw-rw-rw-   0        0        0      559 2024-03-31 11:14:28.907183 botnikkk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-03-30 21:04:38.000000 botnikkk-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 11:14:28.892162 botnikkk-0.0.4/botnikkk/
--rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.4/botnikkk/__init__.py
--rw-rw-rw-   0        0        0     2448 2024-03-31 11:10:51.000000 botnikkk-0.0.4/botnikkk/formatting.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:14:28.905168 botnikkk-0.0.4/botnikkk.egg-info/
--rw-rw-rw-   0        0        0      559 2024-03-31 11:14:28.000000 botnikkk-0.0.4/botnikkk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-03-31 11:14:28.000000 botnikkk-0.0.4/botnikkk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 11:14:28.000000 botnikkk-0.0.4/botnikkk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-31 11:14:28.000000 botnikkk-0.0.4/botnikkk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 11:14:28.000000 botnikkk-0.0.4/botnikkk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 11:14:28.910163 botnikkk-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      961 2024-03-31 11:14:13.000000 botnikkk-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.076300 botnikkk-0.0.5/
+-rw-rw-rw-   0        0        0      559 2024-04-01 12:43:28.072298 botnikkk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-03-30 21:04:38.000000 botnikkk-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.058299 botnikkk-0.0.5/botnikkk/
+-rw-rw-rw-   0        0        0      172 2024-03-31 09:55:49.000000 botnikkk-0.0.5/botnikkk/__init__.py
+-rw-rw-rw-   0        0        0     2453 2024-04-01 12:42:28.000000 botnikkk-0.0.5/botnikkk/formatting.py
+drwxrwxrwx   0        0        0        0 2024-04-01 12:43:28.071298 botnikkk-0.0.5/botnikkk.egg-info/
+-rw-rw-rw-   0        0        0      559 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-01 12:43:27.000000 botnikkk-0.0.5/botnikkk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 12:43:28.076300 botnikkk-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      961 2024-04-01 12:43:10.000000 botnikkk-0.0.5/setup.py
```

### Comparing `botnikkk-0.0.4/PKG-INFO` & `botnikkk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.4
+Version: 0.0.5
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botnikkk-0.0.4/botnikkk/formatting.py` & `botnikkk-0.0.5/botnikkk/formatting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import screeninfo
 import asyncio
 
 screen_width = screeninfo.get_monitors()[0].width
-middle = " "*int(((screen_width/10)-128)/2)
+middle = " "*int(((screen_width/9)-128)/2)
 
 def centre(title,symbol=" ",str_end="\n") :
     #aligns the title in centre with symbols around it
     gap = str(symbol)*(64-int((len(title)/2)))
     gap2 = str(symbol)*(128- len(title) - len(gap))
     if str_end != '\r' :
         print(( middle + "|" + gap + title + gap2 + "|" + "\n" + middle + "|" + 128*" " + "|"),end=str_end)
@@ -62,8 +62,10 @@
         symbol = " "
         gap = str(symbol)*(64-int((len(title)/2)))
         gap2 = str(symbol)*(128- len(title) - len(gap))
         print(( middle + "|" + gap + title + gap2 + "|"),end='\r') 
         await asyncio.sleep(1) 
 
 async def redirect(redirect='UNKNOWN'):
-    await redirect_function(redirect)
+    await redirect_function(redirect)
+
+
```

### Comparing `botnikkk-0.0.4/botnikkk.egg-info/PKG-INFO` & `botnikkk-0.0.5/botnikkk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botnikkk
-Version: 0.0.4
+Version: 0.0.5
 Summary: a personal package
 Author: BotNikkk
 Author-email: <nikhi.ace.chd@gmail.com>
 Keywords: python,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `botnikkk-0.0.4/setup.py` & `botnikkk-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'a personal package'
 
 # Setting up
 setup(
     name="botnikkk",
     version=VERSION,
     author="BotNikkk",
```

