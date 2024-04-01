# Comparing `tmp/PyNUTClient-2.8.1.post1.tar.gz` & `tmp/PyNUTClient-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNUTClient-2.8.1.post1.tar", last modified: Mon Nov 20 09:13:36 2023, max compression
+gzip compressed data, was "PyNUTClient-2.8.2.tar", last modified: Mon Apr  1 16:51:42 2024, max compression
```

## Comparing `PyNUTClient-2.8.1.post1.tar` & `PyNUTClient-2.8.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-11-20 09:13:18.627133 PyNUTClient-2.8.1.post1/
--rw-r--r--   0 jim       (1000) jim       (1000)    35068 2022-08-05 10:31:29.000000 PyNUTClient-2.8.1.post1/LICENSE-GPL3
--rw-r--r--   0 jim       (1000) jim       (1000)    12685 2023-11-20 09:13:18.627133 PyNUTClient-2.8.1.post1/PKG-INFO
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-11-20 09:13:18.627133 PyNUTClient-2.8.1.post1/PyNUTClient/
--rw-r--r--   0 jim       (1000) jim       (1000)    18592 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient/PyNUT.py
--rw-r--r--   0 jim       (1000) jim       (1000)       20 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient/__init__.py
--rwxr-xr-x   0 jim       (1000) jim       (1000)     6532 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient/test_nutclient.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2023-11-20 09:13:18.627133 PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/
--rw-r--r--   0 jim       (1000) jim       (1000)    12685 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)      255 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       12 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/top_level.txt
--rw-r--r--   0 jim       (1000) jim       (1000)    11862 2023-11-15 23:24:33.000000 PyNUTClient-2.8.1.post1/README.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       38 2023-11-20 09:13:18.627133 PyNUTClient-2.8.1.post1/setup.cfg
--rw-r--r--   0 jim       (1000) jim       (1000)     1919 2023-11-20 09:13:18.000000 PyNUTClient-2.8.1.post1/setup.py
--rw-r--r--   0 jim       (1000) jim       (1000)      971 2023-11-20 08:14:35.000000 PyNUTClient-2.8.1.post1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:51:42.826144 PyNUTClient-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35068 2024-04-01 16:51:39.000000 PyNUTClient-2.8.2/LICENSE-GPL3
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 16:51:39.000000 PyNUTClient-2.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-01 16:51:42.826144 PyNUTClient-2.8.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:51:42.826144 PyNUTClient-2.8.2/PyNUTClient/
+-rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-04-01 16:51:41.000000 PyNUTClient-2.8.2/PyNUTClient/PyNUT.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 16:51:41.000000 PyNUTClient-2.8.2/PyNUTClient/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6525 2024-04-01 16:51:41.000000 PyNUTClient-2.8.2/PyNUTClient/test_nutclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:51:42.826144 PyNUTClient-2.8.2/PyNUTClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-01 16:51:42.000000 PyNUTClient-2.8.2/PyNUTClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 16:51:42.000000 PyNUTClient-2.8.2/PyNUTClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:51:42.000000 PyNUTClient-2.8.2/PyNUTClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 16:51:42.000000 PyNUTClient-2.8.2/PyNUTClient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-04-01 16:51:39.000000 PyNUTClient-2.8.2/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:51:42.826144 PyNUTClient-2.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-01 16:51:41.000000 PyNUTClient-2.8.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-01 16:51:39.000000 PyNUTClient-2.8.2/tox.ini
```

### Comparing `PyNUTClient-2.8.1.post1/LICENSE-GPL3` & `PyNUTClient-2.8.2/LICENSE-GPL3`

 * *Files identical despite different names*

### Comparing `PyNUTClient-2.8.1.post1/PKG-INFO` & `PyNUTClient-2.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: PyNUTClient
-Version: 2.8.1.post1
+Version: 2.8.2
 Summary: Python client bindings for NUT
 Home-page: https://github.com/networkupstools/nut/tree/master/scripts/python/module
 Author: The Network UPS Tools project
 Author-email: jimklimov+nut@gmail.com
-License: UNKNOWN
 Keywords: pypi,cicd,python,nut,Network UPS Tools
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -145,15 +143,15 @@
 wisdom it has to offer.
 
 
 ver
 ~~~
 
 Sends the `VER` command to the NUT data server and returns its self-reported
-identification such as version, product or distribution it may be bundied with.
+identification such as version, product or distribution it may be bundled with.
 
 Note that the NUT client interactions should not rely on reported versions,
 but follow the protocol as defined.
 
 
 DeviceLogin
 ~~~~~~~~~~~
@@ -408,9 +406,7 @@
     result = ups.SetRWVar( ups='UPS1', var='battery.date', value='06/17/08' )
     print( result )
 
     >> OK
 -----
 
 See also: `GetRWVars()`
-
-
```

### Comparing `PyNUTClient-2.8.1.post1/PyNUTClient/PyNUT.py` & `PyNUTClient-2.8.2/PyNUTClient/PyNUT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python
+#!@PYTHON@
 # -*- coding: utf-8 -*-
 
 #   Copyright (C) 2008 David Goncalves <david@lestat.st>
 #
 #   This program is free software: you can redistribute it and/or modify
 #   it under the terms of the GNU General Public License as published by
 #   the Free Software Foundation; either version 3 of the License, or
```

### Comparing `PyNUTClient-2.8.1.post1/PyNUTClient/test_nutclient.py` & `PyNUTClient-2.8.2/PyNUTClient/test_nutclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/python
+#!@PYTHON@
 # -*- coding: utf-8 -*-
 
 # This source code is provided for testing/debuging purpose ;)
 
 import PyNUT
 import sys
 import os
```

### Comparing `PyNUTClient-2.8.1.post1/PyNUTClient.egg-info/PKG-INFO` & `PyNUTClient-2.8.2/PyNUTClient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: PyNUTClient
-Version: 2.8.1.post1
+Version: 2.8.2
 Summary: Python client bindings for NUT
 Home-page: https://github.com/networkupstools/nut/tree/master/scripts/python/module
 Author: The Network UPS Tools project
 Author-email: jimklimov+nut@gmail.com
-License: UNKNOWN
 Keywords: pypi,cicd,python,nut,Network UPS Tools
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -145,15 +143,15 @@
 wisdom it has to offer.
 
 
 ver
 ~~~
 
 Sends the `VER` command to the NUT data server and returns its self-reported
-identification such as version, product or distribution it may be bundied with.
+identification such as version, product or distribution it may be bundled with.
 
 Note that the NUT client interactions should not rely on reported versions,
 but follow the protocol as defined.
 
 
 DeviceLogin
 ~~~~~~~~~~~
@@ -408,9 +406,7 @@
     result = ups.SetRWVar( ups='UPS1', var='battery.date', value='06/17/08' )
     print( result )
 
     >> OK
 -----
 
 See also: `GetRWVars()`
-
-
```

### Comparing `PyNUTClient-2.8.1.post1/README.txt` & `PyNUTClient-2.8.2/README.txt`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 wisdom it has to offer.
 
 
 ver
 ~~~
 
 Sends the `VER` command to the NUT data server and returns its self-reported
-identification such as version, product or distribution it may be bundied with.
+identification such as version, product or distribution it may be bundled with.
 
 Note that the NUT client interactions should not rely on reported versions,
 but follow the protocol as defined.
 
 
 DeviceLogin
 ~~~~~~~~~~~
```

### Comparing `PyNUTClient-2.8.1.post1/setup.py` & `PyNUTClient-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 # README.txt appears from README.adoc during package or CI build
 with codecs.open(os.path.join(here, "README.txt"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name =	"PyNUTClient",
-    version =	'2.8.1.post1',
+    version =	'2.8.2',
     author =	"The Network UPS Tools project",
     license_files =	('LICENSE-GPL3',),
     author_email =	"jimklimov+nut@gmail.com",
     description =	"Python client bindings for NUT",
     url =	"https://github.com/networkupstools/nut/tree/master/scripts/python/module",
     long_description_content_type =	"text/plain",	# NOTE: No asciidoc so far, see https://packaging.python.org/en/latest/specifications/core-metadata/
     long_description =	long_description,
     packages   =	find_packages(),
     #py_modules =	['PyNUT'],
     package_dir =	{'PyNUT': 'PyNUTClient'},
-    data_files =	[('', ['tox.ini'])],
+    #data_files =	[('', ['tox.ini'])],
     #scripts    =	['PyNUTClient/test_nutclient.py', 'PyNUTClient/__init__.py'],
     python_requires =	'>=2.6',
     # install_requires =	['telnetlib'],	# NOTE: telnetlib.py is part of Python core for tested 2.x and 3.x versions, not something 'pip' can download
     keywords =	['pypi', 'cicd', 'python', 'nut', 'Network UPS Tools'],
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `PyNUTClient-2.8.1.post1/tox.ini` & `PyNUTClient-2.8.2/tox.ini`

 * *Files identical despite different names*

