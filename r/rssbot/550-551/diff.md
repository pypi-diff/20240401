# Comparing `tmp/rssbot-550.tar.gz` & `tmp/rssbot-551.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-550.tar", last modified: Wed Mar 27 22:07:47 2024, max compression
+gzip compressed data, was "rssbot-551.tar", last modified: Mon Apr  1 11:21:49 2024, max compression
```

## Comparing `rssbot-550.tar` & `rssbot-551.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 22:07:47.485855 rssbot-550/
--rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-03-27 22:07:47.485855 rssbot-550/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1785 2024-03-27 20:57:59.000000 rssbot-550/README.rst
--rw-r--r--   0 bart      (1000) bart      (1000)     1006 2024-03-27 20:04:23.000000 rssbot-550/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 22:07:47.481855 rssbot-550/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-03-27 18:22:17.000000 rssbot-550/rssbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4021 2024-03-27 20:56:27.000000 rssbot-550/rssbot/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-03-27 18:22:17.000000 rssbot-550/rssbot/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-03-27 18:22:17.000000 rssbot-550/rssbot/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-03-27 18:22:17.000000 rssbot-550/rssbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 22:07:47.485855 rssbot-550/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      311 2024-03-27 18:28:42.000000 rssbot-550/rssbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17674 2024-03-27 18:27:36.000000 rssbot-550/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-03-27 18:22:23.000000 rssbot-550/rssbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-03-27 18:22:17.000000 rssbot-550/rssbot/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-03-27 18:22:17.000000 rssbot-550/rssbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-03-27 18:22:17.000000 rssbot-550/rssbot/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-27 22:07:47.481855 rssbot-550/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-03-27 22:07:47.000000 rssbot-550/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      510 2024-03-27 22:07:47.000000 rssbot-550/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-27 22:07:47.000000 rssbot-550/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       86 2024-03-27 22:07:47.000000 rssbot-550/rssbot.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-03-27 22:07:47.000000 rssbot-550/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-03-27 22:07:47.485855 rssbot-550/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-27 16:57:23.000000 rssbot-550/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 11:21:49.858303 rssbot-551/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-04-01 11:21:49.854303 rssbot-551/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1785 2024-03-27 20:57:59.000000 rssbot-551/README.rst
+-rw-r--r--   0 bart      (1000) bart      (1000)     1135 2024-04-01 10:47:19.000000 rssbot-551/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 11:21:49.854303 rssbot-551/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-03-27 18:22:17.000000 rssbot-551/rssbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3867 2024-04-01 10:48:31.000000 rssbot-551/rssbot/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-03-27 18:22:17.000000 rssbot-551/rssbot/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-03-27 18:22:17.000000 rssbot-551/rssbot/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-03-27 18:22:17.000000 rssbot-551/rssbot/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 11:21:49.854303 rssbot-551/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      271 2024-03-30 12:22:27.000000 rssbot-551/rssbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-03-27 18:22:23.000000 rssbot-551/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-03-27 18:22:23.000000 rssbot-551/rssbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17674 2024-03-27 18:27:36.000000 rssbot-551/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-03-27 18:22:23.000000 rssbot-551/rssbot/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    10240 2024-04-01 02:11:09.000000 rssbot-551/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-03-27 18:22:17.000000 rssbot-551/rssbot/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-03-27 18:22:17.000000 rssbot-551/rssbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-03-27 18:22:17.000000 rssbot-551/rssbot/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 11:21:49.854303 rssbot-551/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2322 2024-04-01 11:21:49.000000 rssbot-551/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      466 2024-04-01 11:21:49.000000 rssbot-551/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-01 11:21:49.000000 rssbot-551/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       86 2024-04-01 11:21:49.000000 rssbot-551/rssbot.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2024-04-01 11:21:49.000000 rssbot-551/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-01 11:21:49.858303 rssbot-551/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-27 16:57:23.000000 rssbot-551/setup.py
```

### Comparing `rssbot-550/PKG-INFO` & `rssbot-551/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 550
+Version: 551
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rssbot-550/README.rst` & `rssbot-551/README.rst`

 * *Files identical despite different names*

### Comparing `rssbot-550/pyproject.toml` & `rssbot-551/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rssbot"
 description = "24/7 feed fetcher"
-version = "550"
+version = "551"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
@@ -42,13 +42,20 @@
 
 
 [tool.setuptools.data-files]
 "share/doc/rssbot" = [
     "README.rst"
 ]
 
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["rssbot*"]
+exclude = ["tests*", "files*", "mods*"]
+namespaces = false
+
+
 [tool.setuptools.exclude-package-data]
 "*" = [
        "env*",
        "html*",
        "test*"
       ]
```

### Comparing `rssbot-550/rssbot/__main__.py` & `rssbot-551/rssbot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
 # pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
 # ruff: noqa: E402
 
 
 "main"
@@ -22,32 +21,26 @@
 from .handler import Client, Event, cmnd, parse_cmd
 from .object  import Default, cdir, spl
 from .errors  import Errors
 from .persist import Workdir
 
 
 Cfg         = Default()
-Cfg.mod     = "cmd,mod"
+Cfg.mod     = "cmd,irc,mod,rss"
 Cfg.opts    = ""
 Cfg.name    = "rssbot"
-Cfg.version = "550"
+Cfg.version = "551"
 Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
 Workdir.wd = Cfg.wd
 
 
 from . import modules
 
 
-if os.path.exists("mods"):
-    import mods
-else:
-    mods = None
-
-
 dte = time.ctime(time.time()).replace("  ", " ")
 
 
 class Console(Client):
 
     def __init__(self):
         Client.__init__(self)
@@ -137,16 +130,15 @@
 
 def main():
     Workdir.skel()
     Errors.enable(print)
     Client.add(ver)
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
     if 'a' in Cfg.opts:
-        Cfg.mod = ",".join(mods.__dir__())
-        Cfg.mod += "," + ",".join(modules.__dir__())
+        Cfg.mod = "," + ",".join(modules.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
         return
     if "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
@@ -155,15 +147,14 @@
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
         return
     if "c" in Cfg.opts:
         init(modules, Cfg.mod)
-        init(mods, Cfg.mod)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
         return
     if Cfg.otxt:
         return cmnd(Cfg.otxt, print)
```

### Comparing `rssbot-550/rssbot/broker.py` & `rssbot-551/rssbot/broker.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/errors.py` & `rssbot-551/rssbot/errors.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/handler.py` & `rssbot-551/rssbot/handler.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/modules/err.py` & `rssbot-551/rssbot/modules/err.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/modules/irc.py` & `rssbot-551/rssbot/modules/irc.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/modules/rss.py` & `rssbot-551/rssbot/modules/rss.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,18 +137,18 @@
 
 
 class Parser:
 
     @staticmethod
     def getvalue(line, attr):
         lne = ''
-        index1 = line.find(f' {attr}="')
+        index1 = line.find(f'{attr}="')
         if index1 == -1:
             return lne
-        index1 += len(attr) + 3
+        index1 += len(attr) + 2
         index2 = line.find('"', index1)
         if index2 == -1:
             index2 = line.find('"/>', index1)
         if index2 == -1:
             return lne
         lne = line[index1:index2]
         if 'CDATA' in lne:
@@ -189,15 +189,15 @@
 
     @staticmethod
     def getitems(text, token):
         index = 0
         result = []
         stop = False
         while not stop:
-            index1 = text.find(f'<{token}>', index)
+            index1 = text.find(f'<{token}', index)
             if index1 == -1:
                 break
             index1 += len(token) + 2
             index2 = text.find(f'</{token}>', index1)
             if index2 == -1:
                 break
             lne = text[index1:index2]
@@ -215,15 +215,15 @@
                 val = Parser.getitem(line, itm)
                 if val:
                     val = unescape(val.strip())
                     val = val.replace("\n", "")
                     val = striphtml(val)
                     setattr(obj, itm, val)
                 else:
-                    att = Parser.getattrs(line, itm)
+                    att = Parser.getattrs(line, toke)
                     if att:
                         if itm == "link":
                             itm = "href"
                         val = Parser.getvalue(att, itm)
                         if val:
                             if itm == "href":
                                 itm = "link"
@@ -301,14 +301,30 @@
             sync(feed)
     event.reply('ok')
 
 
 Client.add(dpl)
 
 
+def exp(event):
+    event.reply(TEMPLATE)
+    nr = 0
+    for fnm, obj in find("rss"):
+        nr += 1
+        name = obj.name or f"url{nr}"
+        txt = f'<outline name={name} display_list={obj.display_list} xmlUrl="{obj.rss}"/>'
+        event.reply(" "*12 + txt)
+    event.reply(" "*8 + "</outline>")
+    event.reply("    <body>")
+    event.reply("</opml>")
+
+
+Client.add(exp)
+
+
 def nme(event):
     if len(event.args) != 2:
         event.reply('nme <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector):
         if feed:
@@ -372,7 +388,15 @@
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
 
 
 Client.add(rss)
+
+
+TEMPLATE = """<opml version="1.0">
+    <head>
+        <title>rssbot opml</title>
+    </head>
+    <body>
+        <outline title="rssbot opml" text="24/7 feed fetcher">"""
```

### Comparing `rssbot-550/rssbot/object.py` & `rssbot-551/rssbot/object.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/persist.py` & `rssbot-551/rssbot/persist.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot/thread.py` & `rssbot-551/rssbot/thread.py`

 * *Files identical despite different names*

### Comparing `rssbot-550/rssbot.egg-info/PKG-INFO` & `rssbot-551/rssbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 550
+Version: 551
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
```

