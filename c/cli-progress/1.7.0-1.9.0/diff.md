# Comparing `tmp/cli_progress-1.7.0.tar.gz` & `tmp/cli_progress-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_progress-1.7.0.tar", last modified: Sat Jan 27 09:53:52 2024, max compression
+gzip compressed data, was "cli_progress-1.9.0.tar", last modified: Mon Apr  1 15:09:06 2024, max compression
```

## Comparing `cli_progress-1.7.0.tar` & `cli_progress-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:52.764369 cli_progress-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-27 09:53:42.000000 cli_progress-1.7.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-27 09:53:42.000000 cli_progress-1.7.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-27 09:53:42.000000 cli_progress-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-27 09:53:42.000000 cli_progress-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-27 09:53:52.764369 cli_progress-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-01-27 09:53:42.000000 cli_progress-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:52.764369 cli_progress-1.7.0/cli_progress/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/ANSIWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/BackgroundWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/LogListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-01-27 09:53:42.000000 cli_progress-1.7.0/cli_progress/progress_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:52.764369 cli_progress-1.7.0/cli_progress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-27 09:53:52.000000 cli_progress-1.7.0/cli_progress.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 09:53:52.764369 cli_progress-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-01-27 09:53:42.000000 cli_progress-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:52.764369 cli_progress-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 09:53:42.000000 cli_progress-1.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-27 09:53:42.000000 cli_progress-1.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-27 09:53:42.000000 cli_progress-1.7.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.225836 cli_progress-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 15:08:54.000000 cli_progress-1.9.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 15:08:54.000000 cli_progress-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 15:08:54.000000 cli_progress-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-01 15:09:06.225836 cli_progress-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-01 15:08:54.000000 cli_progress-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/cli_progress/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/ANSIWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/BackgroundWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/LogListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-01 15:08:54.000000 cli_progress-1.9.0/cli_progress/progress_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/cli_progress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:09:06.000000 cli_progress-1.9.0/cli_progress.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:09:06.225836 cli_progress-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-01 15:08:54.000000 cli_progress-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:09:06.221836 cli_progress-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 15:08:54.000000 cli_progress-1.9.0/tests/test_base.py
```

### Comparing `cli_progress-1.7.0/LICENSE` & `cli_progress-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/PKG-INFO` & `cli_progress-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cli_progress
-Version: 1.7.0
+Version: 1.9.0
 Summary: Awesome cli_progress created by hiddify
 Home-page: https://github.com/hiddify/cli_progress/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urwid==2.4.1
-Requires-Dist: twisted==23.10.0
-Requires-Dist: pyOpenSSL==23.3.0
-Requires-Dist: service_identity==24.1.0
+Requires-Dist: urwid==2.6.10
+Requires-Dist: Twisted==24.3.0
+Requires-Dist: pyOpenSSL==24.1.0
+Requires-Dist: service-identity==24.1.0
 Requires-Dist: argparse==1.4.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
```

### Comparing `cli_progress-1.7.0/README.md` & `cli_progress-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress/ANSIWidget.py` & `cli_progress-1.9.0/cli_progress/ANSIWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress/BackgroundWidget.py` & `cli_progress-1.9.0/cli_progress/BackgroundWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress/LogListWidget.py` & `cli_progress-1.9.0/cli_progress/LogListWidget.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress/__main__.py` & `cli_progress-1.9.0/cli_progress/__main__.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress/progress_ui.py` & `cli_progress-1.9.0/cli_progress/progress_ui.py`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/cli_progress.egg-info/PKG-INFO` & `cli_progress-1.9.0/cli_progress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: cli_progress
-Version: 1.7.0
+Version: 1.9.0
 Summary: Awesome cli_progress created by hiddify
 Home-page: https://github.com/hiddify/cli_progress/
 Author: hiddify
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urwid==2.4.1
-Requires-Dist: twisted==23.10.0
-Requires-Dist: pyOpenSSL==23.3.0
-Requires-Dist: service_identity==24.1.0
+Requires-Dist: urwid==2.6.10
+Requires-Dist: Twisted==24.3.0
+Requires-Dist: pyOpenSSL==24.1.0
+Requires-Dist: service-identity==24.1.0
 Requires-Dist: argparse==1.4.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
```

### Comparing `cli_progress-1.7.0/cli_progress.egg-info/SOURCES.txt` & `cli_progress-1.9.0/cli_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_progress-1.7.0/setup.py` & `cli_progress-1.9.0/setup.py`

 * *Files identical despite different names*

