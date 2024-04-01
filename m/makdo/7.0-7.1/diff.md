# Comparing `tmp/makdo-7.0.tar.gz` & `tmp/makdo-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makdo-7.0.tar", last modified: Mon Apr  1 17:36:51 2024, max compression
+gzip compressed data, was "makdo-7.1.tar", last modified: Mon Apr  1 18:32:34 2024, max compression
```

## Comparing `makdo-7.0.tar` & `makdo-7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 17:36:51.040522 makdo-7.0/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 17:36:51.040522 makdo-7.0/PKG-INFO
--rw-------   0 say       (1000) say       (1000)    17888 2024-04-01 17:36:31.000000 makdo-7.0/README.txt
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 17:36:51.036522 makdo-7.0/makdo/
--rw-------   0 say       (1000) say       (1000)      137 2024-04-01 17:36:31.000000 makdo-7.0/makdo/__init__.py
--rwx------   0 say       (1000) say       (1000)   262507 2024-04-01 17:36:31.000000 makdo-7.0/makdo/makdo_docx2md.py
--rwx------   0 say       (1000) say       (1000)     3994 2024-04-01 17:36:31.000000 makdo-7.0/makdo/makdo_gui.py
--rwx------   0 say       (1000) say       (1000)   237782 2024-04-01 17:36:31.000000 makdo-7.0/makdo/makdo_md2docx.py
-drwx------   0 say       (1000) say       (1000)        0 2024-04-01 17:36:51.040522 makdo-7.0/makdo.egg-info/
--rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 17:36:50.000000 makdo-7.0/makdo.egg-info/PKG-INFO
--rw-------   0 say       (1000) say       (1000)      246 2024-04-01 17:36:51.000000 makdo-7.0/makdo.egg-info/SOURCES.txt
--rw-------   0 say       (1000) say       (1000)        1 2024-04-01 17:36:50.000000 makdo-7.0/makdo.egg-info/dependency_links.txt
--rw-------   0 say       (1000) say       (1000)       32 2024-04-01 17:36:50.000000 makdo-7.0/makdo.egg-info/requires.txt
--rw-------   0 say       (1000) say       (1000)        6 2024-04-01 17:36:50.000000 makdo-7.0/makdo.egg-info/top_level.txt
--rw-------   0 say       (1000) say       (1000)       38 2024-04-01 17:36:51.040522 makdo-7.0/setup.cfg
--rw-------   0 say       (1000) say       (1000)      567 2024-04-01 17:36:31.000000 makdo-7.0/setup.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/
+-rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 18:32:34.030760 makdo-7.1/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)    17888 2024-04-01 18:32:06.000000 makdo-7.1/README.txt
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/makdo/
+-rw-------   0 say       (1000) say       (1000)      137 2024-04-01 18:32:06.000000 makdo-7.1/makdo/__init__.py
+-rwx------   0 say       (1000) say       (1000)   262576 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_docx2md.py
+-rwx------   0 say       (1000) say       (1000)     4000 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_gui.py
+-rwx------   0 say       (1000) say       (1000)   237782 2024-04-01 18:32:06.000000 makdo-7.1/makdo/makdo_md2docx.py
+drwx------   0 say       (1000) say       (1000)        0 2024-04-01 18:32:34.030760 makdo-7.1/makdo.egg-info/
+-rw-------   0 say       (1000) say       (1000)    21832 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)      246 2024-04-01 18:32:34.000000 makdo-7.1/makdo.egg-info/SOURCES.txt
+-rw-------   0 say       (1000) say       (1000)        1 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/dependency_links.txt
+-rw-------   0 say       (1000) say       (1000)       32 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/requires.txt
+-rw-------   0 say       (1000) say       (1000)        6 2024-04-01 18:32:33.000000 makdo-7.1/makdo.egg-info/top_level.txt
+-rw-------   0 say       (1000) say       (1000)       38 2024-04-01 18:32:34.030760 makdo-7.1/setup.cfg
+-rw-------   0 say       (1000) say       (1000)      567 2024-04-01 18:32:06.000000 makdo-7.1/setup.py
```

### Comparing `makdo-7.0/PKG-INFO` & `makdo-7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.0
+Version: 7.1
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
```

### Comparing `makdo-7.0/README.txt` & `makdo-7.1/README.txt`

 * *Files identical despite different names*

### Comparing `makdo-7.0/makdo/makdo_docx2md.py` & `makdo-7.1/makdo/makdo_docx2md.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         docx2md.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-01:54:21-JST>
+# Time-stamp:   <2024.04.02-03:19:19-JST>
 
 # docx2md.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -6121,15 +6121,18 @@
         longest_row = 0
         max_length = 0
         for i, row in enumerate(tab):
             if len(row) > max_length:
                 max_length = len(row)
                 longest_row = i
         # GET CONFIGURE ROW
-        half_row = int(len(tab) / 2) + (len(tab) % 2)
+        if len(tab) == 1:
+            half_row = 0
+        else:
+            half_row = int(len(tab) / 2) + (len(tab) % 2)
         conf_row = half_row
         if longest_row > 0:
             conf_row = longest_row
         # GET NIL OR DOUBLE LINE (ROW)
         row_line = []
         for i in range(len(tab)):
             for tag in tab[i][0]:
```

### Comparing `makdo-7.0/makdo/makdo_gui.py` & `makdo-7.1/makdo/makdo_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         makdo-gui.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-02:08:33-JST>
+# Time-stamp:   <2024.04.02-03:25:09-JST>
 
 # makdo-gui.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -26,15 +26,15 @@
 # 2023.01.07 v04 Mitaki
 # 2023.03.16 v05 Aki-Nagatsuka
 # 2023.06.07 v06 Shimo-Gion
 # 2024.04.02 v07 Furuichibashi
 
 
 # USAGE
-# from makdo_gui import Makdo
+# from makdo.makdo_gui import Makdo
 # Makdo()
 
 
 import tkinter as tk
 from tkinter import ttk
 from tkinterdnd2 import TkinterDnD, DND_FILES
 import sys
```

### Comparing `makdo-7.0/makdo/makdo_md2docx.py` & `makdo-7.1/makdo/makdo_md2docx.py`

 * *Files identical despite different names*

### Comparing `makdo-7.0/makdo.egg-info/PKG-INFO` & `makdo-7.1/makdo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.0
+Version: 7.1
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Description: <!-- Time-stamp:   <2024.04.02-01:49:42-JST> -->
```

### Comparing `makdo-7.0/setup.py` & `makdo-7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='makdo',
-    version='07.00',
+    version='07.01',
     description='日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Seiichiro HATA',
     author_email='hata48915b@post.nifty.jp',
     url='https://github.com/hata48915b/makdo/',
     license='GPLv3+',
```

