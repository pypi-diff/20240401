# Comparing `tmp/psl-2024.3.4.tar.gz` & `tmp/psl-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2024.3.4.tar", last modified: Mon Mar  4 13:16:46 2024, max compression
+gzip compressed data, was "psl-2024.4.1.tar", last modified: Mon Apr  1 13:04:08 2024, max compression
```

## Comparing `psl-2024.3.4.tar` & `psl-2024.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:16:46.804989 psl-2024.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-04 13:16:15.000000 psl-2024.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-04 13:16:15.000000 psl-2024.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-04 13:16:46.804989 psl-2024.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-04 13:16:15.000000 psl-2024.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:16:46.800989 psl-2024.3.4/psl/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-04 13:16:23.000000 psl-2024.3.4/psl/__init__.py
--rw-------   0 runner    (1001) docker     (127)   131365 2024-03-04 13:16:23.000000 psl-2024.3.4/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 13:16:15.000000 psl-2024.3.4/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:16:46.804989 psl-2024.3.4/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-04 13:16:46.000000 psl-2024.3.4/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-04 13:16:46.000000 psl-2024.3.4/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:16:46.000000 psl-2024.3.4/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:16:35.000000 psl-2024.3.4/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-04 13:16:46.000000 psl-2024.3.4/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 13:16:46.804989 psl-2024.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-04 13:16:15.000000 psl-2024.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.543650 psl-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 13:03:41.000000 psl-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 13:03:41.000000 psl-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-01 13:04:08.539650 psl-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 13:03:41.000000 psl-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.539650 psl-2024.4.1/psl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-01 13:03:47.000000 psl-2024.4.1/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   131396 2024-04-01 13:03:47.000000 psl-2024.4.1/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 13:03:41.000000 psl-2024.4.1/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:04:08.539650 psl-2024.4.1/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:03:58.000000 psl-2024.4.1/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 13:04:08.000000 psl-2024.4.1/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:04:08.543650 psl-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 13:03:41.000000 psl-2024.4.1/setup.py
```

### Comparing `psl-2024.3.4/LICENSE` & `psl-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2024.3.4/PKG-INFO` & `psl-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.3.4
+Version: 2024.4.1
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.3.4/README.md` & `psl-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `psl-2024.3.4/psl/__init__.py` & `psl-2024.4.1/psl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2024.3.4"
-__checksum__ = "23df8ce725d8ecbe9aa0f6c8f7bbd86369e16105"
+__version__ = "2024.4.1"
+__checksum__ = "102474c3ad6504ddf1366a07954c09c67ff40ebf"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2024.3.4/psl/psl.txt` & `psl-2024.4.1/psl/psl.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6157,15 +6157,14 @@
 grainger
 graphics
 gratis
 green
 gripe
 grocery
 group
-guardian
 gucci
 guge
 guide
 guitars
 guru
 hair
 hamburg
@@ -8480,14 +8479,15 @@
 versus.jp
 vivian.jp
 watson.jp
 weblike.jp
 whitesnow.jp
 zombie.jp
 heteml.net
+graphic.design
 cloudapps.digital
 london.cloudapps.digital
 pymnt.uk
 ro.im
 goip.de
 *.run.app
 web.app
@@ -8674,14 +8674,15 @@
 se.leg.br
 sp.leg.br
 to.leg.br
 pixolino.com
 na4u.ru
 iopsys.se
 ipifony.net
+ir.md
 iservschule.de
 mein-iserv.de
 schulplattform.de
 schulserver.de
 test-iserv.de
 iserv.dev
 iobb.net
@@ -8877,15 +8878,15 @@
 custom.metacentrum.cz
 flt.cloud.muni.cz
 usr.cloud.muni.cz
 meteorapp.com
 eu.meteorapp.com
 co.pl
 *.azurecontainer.io
-*.cloudapp.azure.com
+cloudapp.azure.com
 azure-api.net
 azureedge.net
 azurefd.net
 azurewebsites.net
 azure-mobile.net
 azurestaticapps.net
 1.azurestaticapps.net
@@ -8943,14 +8944,15 @@
 sa.ngrok.io
 us.ngrok.io
 ngrok.pizza
 ngrok.pro
 torun.pl
 nh-serv.co.uk
 nfshost.com
+ipfs.nftstorage.link
 *.developer.app
 noop.app
 *.northflank.app
 *.build.run
 *.code.run
 *.database.run
 *.migration.run
```

### Comparing `psl-2024.3.4/psl.egg-info/PKG-INFO` & `psl-2024.4.1/psl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.3.4
+Version: 2024.4.1
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.3.4/setup.py` & `psl-2024.4.1/setup.py`

 * *Files identical despite different names*

