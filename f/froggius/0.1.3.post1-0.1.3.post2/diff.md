# Comparing `tmp/froggius-0.1.3.post1.tar.gz` & `tmp/froggius-0.1.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.3.post1.tar", last modified: Mon Apr  1 09:49:30 2024, max compression
+gzip compressed data, was "froggius-0.1.3.post2.tar", last modified: Mon Apr  1 14:21:41 2024, max compression
```

## Comparing `froggius-0.1.3.post1.tar` & `froggius-0.1.3.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:49:29.996822 froggius-0.1.3.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 09:49:24.000000 froggius-0.1.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-01 09:49:29.996822 froggius-0.1.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 09:49:24.000000 froggius-0.1.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:49:29.992822 froggius-0.1.3.post1/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:49:24.000000 froggius-0.1.3.post1/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-01 09:49:27.000000 froggius-0.1.3.post1/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:49:29.996822 froggius-0.1.3.post1/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-01 09:49:29.000000 froggius-0.1.3.post1/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 09:49:29.000000 froggius-0.1.3.post1/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:49:29.000000 froggius-0.1.3.post1/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 09:49:29.000000 froggius-0.1.3.post1/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:49:29.996822 froggius-0.1.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 09:49:27.000000 froggius-0.1.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:33.000000 froggius-0.1.3.post2/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-01 14:21:39.000000 froggius-0.1.3.post2/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 14:21:41.000000 froggius-0.1.3.post2/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:21:41.890987 froggius-0.1.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 14:21:39.000000 froggius-0.1.3.post2/setup.py
```

### Comparing `froggius-0.1.3.post1/PKG-INFO` & `froggius-0.1.3.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.3.post1
+Version: 0.1.3.post2
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
+License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `froggius-0.1.3.post1/README.md` & `froggius-0.1.3.post2/README.md`

 * *Files identical despite different names*

### Comparing `froggius-0.1.3.post1/froggius/logger.py` & `froggius-0.1.3.post2/froggius/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-"""
-Froggius
-Version: v0.1.4
-License: GPLv3
-
-Author of this file: zlElo
-"""
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
 import datetime
 import sys
 import traceback
 
 
 class Froggius:
```

### Comparing `froggius-0.1.3.post1/froggius.egg-info/PKG-INFO` & `froggius-0.1.3.post2/froggius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.3.post1
+Version: 0.1.3.post2
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
+License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

