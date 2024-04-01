# Comparing `tmp/otpcr-3.tar.gz` & `tmp/otpcr-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpcr-3.tar", last modified: Wed Mar 27 12:23:21 2024, max compression
+gzip compressed data, was "otpcr-4.tar", last modified: Mon Apr  1 12:02:52 2024, max compression
```

## Comparing `otpcr-3.tar` & `otpcr-4.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 12:23:21.231817 otpcr-3/
--rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-03-27 12:23:21.231817 otpcr-3/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1848 2024-03-26 06:20:35.000000 otpcr-3/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 12:23:21.231817 otpcr-3/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-03-26 06:20:35.000000 otpcr-3/files/verbatim2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 12:23:21.231817 otpcr-3/otpcr/
--rw-r--r--   0 bart      (1000) bart      (1000)       67 2024-03-27 12:16:27.000000 otpcr-3/otpcr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3952 2024-03-27 12:17:25.000000 otpcr-3/otpcr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-03-26 15:31:07.000000 otpcr-3/otpcr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-03-26 09:07:31.000000 otpcr-3/otpcr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-03-26 15:33:49.000000 otpcr-3/otpcr/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 12:23:21.231817 otpcr-3/otpcr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-03-26 09:24:59.000000 otpcr-3/otpcr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-03-26 09:18:34.000000 otpcr-3/otpcr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-03-26 09:18:50.000000 otpcr-3/otpcr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-03-26 09:19:05.000000 otpcr-3/otpcr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      741 2024-03-26 09:23:52.000000 otpcr-3/otpcr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17673 2024-03-26 09:19:27.000000 otpcr-3/otpcr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-03-26 09:19:39.000000 otpcr-3/otpcr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-03-26 09:19:53.000000 otpcr-3/otpcr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2398 2024-03-26 09:20:04.000000 otpcr-3/otpcr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-03-26 09:20:22.000000 otpcr-3/otpcr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1118 2024-03-26 09:20:51.000000 otpcr-3/otpcr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-03-26 09:21:04.000000 otpcr-3/otpcr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5020 2024-03-26 09:21:20.000000 otpcr-3/otpcr/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-03-26 09:07:31.000000 otpcr-3/otpcr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-03-26 09:29:16.000000 otpcr-3/otpcr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-03-26 09:13:10.000000 otpcr-3/otpcr/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 12:23:21.231817 otpcr-3/otpcr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      638 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-27 12:23:21.000000 otpcr-3/otpcr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-03-27 12:10:48.000000 otpcr-3/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-03-27 12:23:21.231817 otpcr-3/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-26 06:20:35.000000 otpcr-3/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-04-01 12:02:52.250407 otpcr-4/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1848 2024-03-27 18:21:46.000000 otpcr-4/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.246407 otpcr-4/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-03-27 18:21:46.000000 otpcr-4/files/verbatim2.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr/
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-03-27 18:21:46.000000 otpcr-4/otpcr/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3952 2024-04-01 12:02:08.000000 otpcr-4/otpcr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-03-27 18:21:46.000000 otpcr-4/otpcr/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-03-27 18:21:46.000000 otpcr-4/otpcr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-03-27 18:21:46.000000 otpcr-4/otpcr/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17673 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3485 2024-04-01 10:39:35.000000 otpcr-4/otpcr/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2398 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2737 2024-04-01 10:39:57.000000 otpcr-4/otpcr/modules/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1118 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5020 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2913 2024-04-01 10:40:14.000000 otpcr-4/otpcr/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-03-27 18:21:46.000000 otpcr-4/otpcr/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-03-27 18:21:46.000000 otpcr-4/otpcr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-03-27 18:21:46.000000 otpcr-4/otpcr/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      701 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-01 12:01:55.000000 otpcr-4/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-01 12:02:52.250407 otpcr-4/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-27 18:21:46.000000 otpcr-4/setup.py
```

### Comparing `otpcr-3/PKG-INFO` & `otpcr-4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 3
+Version: 4
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `otpcr-3/README.rst` & `otpcr-4/README.rst`

 * *Files identical despite different names*

### Comparing `otpcr-3/files/verbatim2.png` & `otpcr-4/files/verbatim2.png`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/__main__.py` & `otpcr-4/otpcr/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .errors  import Errors
 from .persist import Workdir
 
 
 Cfg         = Default()
 Cfg.mod     = "cmd,mod"
 Cfg.name    = "otpcr"
-Cfg.version = "3"
+Cfg.version = "4"
 Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
 Workdir.wd = Cfg.wd
 
 
 from . import modules
```

### Comparing `otpcr-3/otpcr/broker.py` & `otpcr-4/otpcr/broker.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/errors.py` & `otpcr-4/otpcr/errors.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/handler.py` & `otpcr-4/otpcr/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402,E1102
 
 
-"event hsndler"
+"event handler"
 
 
 import queue
 import threading
 import _thread
```

### Comparing `otpcr-3/otpcr/modules/err.py` & `otpcr-4/otpcr/modules/err.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/fnd.py` & `otpcr-4/otpcr/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/irc.py` & `otpcr-4/otpcr/modules/irc.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/log.py` & `otpcr-4/otpcr/modules/log.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/req.py` & `otpcr-4/otpcr/modules/req.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/rss.py` & `otpcr-4/otpcr/modules/rss.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/tdo.py` & `otpcr-4/otpcr/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/thr.py` & `otpcr-4/otpcr/modules/thr.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/modules/tmr.py` & `otpcr-4/otpcr/modules/tmr.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/object.py` & `otpcr-4/otpcr/object.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/persist.py` & `otpcr-4/otpcr/persist.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr/thread.py` & `otpcr-4/otpcr/thread.py`

 * *Files identical despite different names*

### Comparing `otpcr-3/otpcr.egg-info/PKG-INFO` & `otpcr-4/otpcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 3
+Version: 4
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `otpcr-3/otpcr.egg-info/SOURCES.txt` & `otpcr-4/otpcr.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,13 +19,16 @@
 otpcr/modules/__init__.py
 otpcr/modules/cmd.py
 otpcr/modules/err.py
 otpcr/modules/flt.py
 otpcr/modules/fnd.py
 otpcr/modules/irc.py
 otpcr/modules/log.py
+otpcr/modules/mbx.py
 otpcr/modules/mod.py
 otpcr/modules/req.py
 otpcr/modules/rss.py
+otpcr/modules/rst.py
 otpcr/modules/tdo.py
 otpcr/modules/thr.py
-otpcr/modules/tmr.py
+otpcr/modules/tmr.py
+otpcr/modules/udp.py
```

### Comparing `otpcr-3/pyproject.toml` & `otpcr-4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otpcr"
 description = "OTP-CR-117/19"
-version = "3"
+version = "4"
 authors = [
     {name = "xobjectz", email = "objx@proton.me"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

