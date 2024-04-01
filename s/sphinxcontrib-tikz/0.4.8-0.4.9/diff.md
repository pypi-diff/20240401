# Comparing `tmp/sphinxcontrib-tikz-0.4.8.tar.gz` & `tmp/sphinxcontrib-tikz-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-tikz-0.4.8.tar", last modified: Sat Aug 24 15:22:33 2019, max compression
+gzip compressed data, was "dist/sphinxcontrib-tikz-0.4.9.tar", last modified: Sun Jul  5 12:30:09 2020, max compression
```

## Comparing `sphinxcontrib-tikz-0.4.8.tar` & `sphinxcontrib-tikz-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/
-drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/doc/
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      823 2017-03-28 09:40:30.000000 sphinxcontrib-tikz-0.4.8/doc/make.bat
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      400 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.8/doc/index.rst
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      616 2017-03-28 09:40:30.000000 sphinxcontrib-tikz-0.4.8/doc/Makefile
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     5278 2019-04-14 12:46:30.000000 sphinxcontrib-tikz-0.4.8/doc/conf.py
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      161 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.8/MANIFEST.in
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     9595 2019-08-24 14:57:18.000000 sphinxcontrib-tikz-0.4.8/README.rst
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      111 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/setup.cfg
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     1309 2019-04-14 12:46:22.000000 sphinxcontrib-tikz-0.4.8/LICENSE
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     1804 2019-08-24 14:57:37.000000 sphinxcontrib-tikz-0.4.8/setup.py
-drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/
--rw-rw-r--   0 christoph  (1000) christoph  (1000)        1 2017-03-28 19:58:28.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/not-zip-safe
--rw-rw-r--   0 christoph  (1000) christoph  (1000)        7 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/requires.txt
--rw-rw-r--   0 christoph  (1000) christoph  (1000)       14 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/namespace_packages.txt
--rw-rw-r--   0 christoph  (1000) christoph  (1000)       14 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/top_level.txt
--rw-rw-r--   0 christoph  (1000) christoph  (1000)        1 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/dependency_links.txt
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/PKG-INFO
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2019-04-14 12:53:07.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/PKG-INFO~
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      488 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/SOURCES.txt
--rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/PKG-INFO
-drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2019-08-24 15:22:33.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib/
--rw-rw-r--   0 christoph  (1000) christoph  (1000)    15383 2019-08-24 14:58:07.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib/tikz.py
--rw-rw-r--   0 christoph  (1000) christoph  (1000)      366 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.8/sphinxcontrib/__init__.py
+drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/
+drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/doc/
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      823 2017-03-28 09:40:30.000000 sphinxcontrib-tikz-0.4.9/doc/make.bat
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      400 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.9/doc/index.rst
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      616 2017-03-28 09:40:30.000000 sphinxcontrib-tikz-0.4.9/doc/Makefile
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     5278 2019-04-14 12:46:30.000000 sphinxcontrib-tikz-0.4.9/doc/conf.py
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      161 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.9/MANIFEST.in
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     9595 2020-07-05 12:13:04.000000 sphinxcontrib-tikz-0.4.9/README.rst
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      111 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/setup.cfg
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     1308 2020-07-05 12:11:39.000000 sphinxcontrib-tikz-0.4.9/LICENSE
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     1804 2020-07-05 12:12:55.000000 sphinxcontrib-tikz-0.4.9/setup.py
+drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)        1 2017-03-28 19:58:28.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/not-zip-safe
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)        7 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/requires.txt
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)       14 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/namespace_packages.txt
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)       14 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/top_level.txt
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)        1 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/dependency_links.txt
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/PKG-INFO
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2019-04-14 12:53:07.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/PKG-INFO~
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      488 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/SOURCES.txt
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)     1032 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/PKG-INFO
+drwxrwxr-x   0 christoph  (1000) christoph  (1000)        0 2020-07-05 12:30:09.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib/
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)    15383 2020-07-05 12:13:43.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib/tikz.py
+-rw-rw-r--   0 christoph  (1000) christoph  (1000)      366 2013-10-15 12:22:28.000000 sphinxcontrib-tikz-0.4.9/sphinxcontrib/__init__.py
```

### Comparing `sphinxcontrib-tikz-0.4.8/doc/make.bat` & `sphinxcontrib-tikz-0.4.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-tikz-0.4.8/doc/Makefile` & `sphinxcontrib-tikz-0.4.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-tikz-0.4.8/doc/conf.py` & `sphinxcontrib-tikz-0.4.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-tikz-0.4.8/README.rst` & `sphinxcontrib-tikz-0.4.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 <http://www.ctan.org/tex-archive/graphics/pgf/contrib/pgfplots/>`__.)
 
 Use the extension at your own risk.  Anything might change in future versions
 without further notice.
 
 ----
 
-:Version: 0.4.8
+:Version: 0.4.9
 :Author: Christoph Reller ``christoph.reller@gmail.com``
 :License: `BSD License <http://opensource.org/licenses/bsd-license.html>`__
 :Git Repository: https://bitbucket.org/philexander/tikz
 :PyPI Package: http://pypi.python.org/pypi/sphinxcontrib-tikz
 :Documentation: http://sphinxcontrib-tikz.readthedocs.io
 
 Prerequisites and Configuration
```

### Comparing `sphinxcontrib-tikz-0.4.8/LICENSE` & `sphinxcontrib-tikz-0.4.9/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 License
 =======
 
-Copyright (c) 2011-2019 by Christoph Reller. All rights reserved.
+Copyright (c) 2011-2020 by Christoph Reller. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
@@ -21,8 +21,7 @@
 EVENT SHALL CHRISTOPH RELLER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
 EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
```

### Comparing `sphinxcontrib-tikz-0.4.8/setup.py` & `sphinxcontrib-tikz-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 '''
 This package contains the tikz Sphinx extension, which enables the use
 of the PGF/TikZ LaTeX package to draw nice pictures.
 '''
 
 NAME         = 'sphinxcontrib-tikz'
 DESCRIPTION  = 'TikZ extension for Sphinx'
-VERSION      = '0.4.8'
+VERSION      = '0.4.9'
 AUTHOR       = 'Christoph Reller'
 AUTHOR_EMAIL = 'christoph.reller@gmail.com'
 URL          = 'https://bitbucket.org/philexander/tikz'
 DOWNLOAD     = 'http://pypi.python.org/pypi/sphinxcontrib-tikz'
 LICENSE      = 'BSD'
 REQUIRES     = ['Sphinx']
 CLASSIFIERS  = [
```

### Comparing `sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/PKG-INFO` & `sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-tikz
-Version: 0.4.8
+Version: 0.4.9
 Summary: TikZ extension for Sphinx
 Home-page: https://bitbucket.org/philexander/tikz
 Author: Christoph Reller
 Author-email: christoph.reller@gmail.com
 License: BSD
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-tikz
 Description:
```

### Comparing `sphinxcontrib-tikz-0.4.8/sphinxcontrib_tikz.egg-info/PKG-INFO~` & `sphinxcontrib-tikz-0.4.9/sphinxcontrib_tikz.egg-info/PKG-INFO~`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-tikz-0.4.8/PKG-INFO` & `sphinxcontrib-tikz-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-tikz
-Version: 0.4.8
+Version: 0.4.9
 Summary: TikZ extension for Sphinx
 Home-page: https://bitbucket.org/philexander/tikz
 Author: Christoph Reller
 Author-email: christoph.reller@gmail.com
 License: BSD
 Download-URL: http://pypi.python.org/pypi/sphinxcontrib-tikz
 Description:
```

### Comparing `sphinxcontrib-tikz-0.4.8/sphinxcontrib/tikz.py` & `sphinxcontrib-tikz-0.4.9/sphinxcontrib/tikz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2012-2019 by Christoph Reller. All rights reserved.
+# Copyright (c) 2012-2020 by Christoph Reller. All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 
 #    1. Redistributions of source code must retain the above copyright notice,
 #       this list of conditions and the following disclaimer.
 
@@ -34,15 +34,15 @@
     Draw pictures with the TikZ/PGF LaTeX package.
 
     See README.rst file for details
 
     Author: Christoph Reller <christoph.reller@gmail.com>
 """
 
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 
 import contextlib
 import tempfile
 import posixpath
 import shutil
 import sys
 import codecs
@@ -387,20 +387,20 @@
         sty_path = os.path.join(app.builder._tikz_tempdir,
                                 "sphinxcontribtikz.sty")
         sty = open(sty_path, mode="w")
         sty.write(r"\RequirePackage{tikz}" + "\n")
         sty.write(r"\RequirePackage{amsmath}" + "\n")
         sty.write(r"\RequirePackage{amsfonts}" + "\n")
         sty.write(r"\RequirePackage{pgfplots}" + "\n")
-        sty.write(app.builder.config.tikz_latex_preamble + "\n")
         tikzlibs = app.builder.config.tikz_tikzlibraries
         tikzlibs = tikzlibs.replace(' ', '')
         tikzlibs = tikzlibs.replace('\t', '')
         tikzlibs = tikzlibs.strip(', ') + "\n"
         sty.write(r"\usetikzlibrary{%s}" % tikzlibs)
+        sty.write(app.builder.config.tikz_latex_preamble + "\n")
         sty.close()
 
         app.builder.config.latex_additional_files.append(sty_path)
         app.add_latex_package("sphinxcontribtikz")
 
 
 def which(program):
```

