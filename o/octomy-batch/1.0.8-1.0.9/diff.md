# Comparing `tmp/octomy-batch-1.0.8.tar.gz` & `tmp/octomy-batch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-1.0.8.tar", last modified: Tue Jan 19 02:56:38 2021, max compression
+gzip compressed data, was "octomy-batch-1.0.9.tar", last modified: Tue Jan 19 03:35:36 2021, max compression
```

## Comparing `octomy-batch-1.0.8.tar` & `octomy-batch-1.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      489 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/.gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      804 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/.gitlab/ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4982 2021-01-18 00:10:57.000000 octomy-batch-1.0.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      718 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2021-01-19 02:56:32.000000 octomy-batch-1.0.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/bin/
--rwxrwxrwx   0 root         (0) root         (0)     1936 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/bin/octomy-batch
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/code_quality/
--rw-rw-rw-   0 root         (0) root         (0)      136 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/code_quality/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1919 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/code_quality/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/code_quality/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    11867 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/code_quality/pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     2574 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/design/
--rw-rw-rw-   0 root         (0) root         (0)    71853 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/design/logo-1024.png
--rw-rw-rw-   0 root         (0) root         (0)     7666 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/design/logo-1024.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.023694 octomy-batch-1.0.8/fk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/fk/batch/
--rw-rw-rw-   0 root         (0) root         (0)    12257 2021-01-19 02:11:54.000000 octomy-batch-1.0.8/fk/batch/BatchProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk/batch/Server.py
--rw-rw-rw-   0 root         (0) root         (0)     5374 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk/batch/WebsiteIO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk/batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13149 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk/batch/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.023694 octomy-batch-1.0.8/fk_batch_filters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.027694 octomy-batch-1.0.8/fk_batch_filters/default/
--rw-rw-rw-   0 root         (0) root         (0)        2 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk_batch_filters/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/fk_batch_filters/default/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/octomy_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1077 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       35 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 02:56:37.000000 octomy-batch-1.0.8/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       35 2021-01-18 00:10:57.000000 octomy-batch-1.0.8/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      776 2021-01-19 02:56:32.000000 octomy-batch-1.0.8/requirements/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      215 2021-01-18 00:10:57.000000 octomy-batch-1.0.8/requirements/test_requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     2907 2021-01-18 00:10:57.000000 octomy-batch-1.0.8/requirements/test_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2021-01-19 02:56:38.035694 octomy-batch-1.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     5190 2021-01-19 02:56:32.000000 octomy-batch-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/Makefile
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/integration/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/tests/load/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/load/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/load/test_load.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/tests/regressions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/regressions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/regressions/test_regressions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 02:56:38.031694 octomy-batch-1.0.8/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:34.000000 octomy-batch-1.0.8/tests/unit/test_unit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      489 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/.gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/.gitlab/ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4982 2021-01-18 00:11:01.000000 octomy-batch-1.0.9/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      718 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     1936 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/bin/octomy-batch
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/code_quality/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      117 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/design/
+-rw-rw-rw-   0 root         (0) root         (0)    71853 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/design/logo-1024.png
+-rw-rw-rw-   0 root         (0) root         (0)     7666 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/design/logo-1024.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.774476 octomy-batch-1.0.9/fk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/fk/batch/
+-rw-rw-rw-   0 root         (0) root         (0)    12257 2021-01-19 02:56:17.000000 octomy-batch-1.0.9/fk/batch/BatchProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/Server.py
+-rw-rw-rw-   0 root         (0) root         (0)     5374 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/WebsiteIO.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13149 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.774476 octomy-batch-1.0.9/fk_batch_filters/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/fk_batch_filters/default/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk_batch_filters/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk_batch_filters/default/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/octomy_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1077 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      776 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      215 2021-01-18 00:11:01.000000 octomy-batch-1.0.9/requirements/test_requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     2907 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/test_requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     5190 2021-01-19 02:56:17.000000 octomy-batch-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/integration/test_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/load/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/load/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/load/test_load.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/regressions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/regressions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/regressions/test_regressions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/unit/test_unit.py
```

### Comparing `octomy-batch-1.0.8/.gitlab/ci.yaml` & `octomy-batch-1.0.9/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/Makefile` & `octomy-batch-1.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/PKG-INFO` & `octomy-batch-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 1.0.8
+Version: 1.0.9
 Summary: OctoMY scheduler
 Home-page: https://gitlab.com/octomy/batch
 Author: Lennart Rolland
 Author-email: lennart@octomy.org
 Maintainer: Lennart Rolland
 Maintainer-email: lennart@octomy.org
 License: GPL-3 LGPL-3 MIT
```

### Comparing `octomy-batch-1.0.8/README.md` & `octomy-batch-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/bin/octomy-batch` & `octomy-batch-1.0.9/bin/octomy-batch`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/code_quality/Makefile` & `octomy-batch-1.0.9/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/code_quality/pylintrc` & `octomy-batch-1.0.9/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/config.json` & `octomy-batch-1.0.9/config.json`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/design/logo-1024.png` & `octomy-batch-1.0.9/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/design/logo-1024.svg` & `octomy-batch-1.0.9/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/fk/batch/BatchProcessor.py` & `octomy-batch-1.0.9/fk/batch/BatchProcessor.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/fk/batch/WebsiteIO.py` & `octomy-batch-1.0.9/fk/batch/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/fk/batch/db.py` & `octomy-batch-1.0.9/fk/batch/db.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/fk_batch_filters/default/test.py` & `octomy-batch-1.0.9/fk_batch_filters/default/test.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/octomy_batch.egg-info/PKG-INFO` & `octomy-batch-1.0.9/octomy_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 1.0.8
+Version: 1.0.9
 Summary: OctoMY scheduler
 Home-page: https://gitlab.com/octomy/batch
 Author: Lennart Rolland
 Author-email: lennart@octomy.org
 Maintainer: Lennart Rolland
 Maintainer-email: lennart@octomy.org
 License: GPL-3 LGPL-3 MIT
```

### Comparing `octomy-batch-1.0.8/octomy_batch.egg-info/SOURCES.txt` & `octomy-batch-1.0.9/octomy_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/requirements/requirements.txt` & `octomy-batch-1.0.9/requirements/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     # via requests
 colored-traceback==0.3.0
     # via octomy-common
 colorlog==4.1.0
     # via octomy-common
 idna==2.10
     # via requests
-octomy-common==1.0.13
+octomy-common==1.0.14
     # via -r temporary_requirements.in
 psycopg2==2.8.6
     # via octomy-common
 py3dns==3.2.1
     # via octomy-common
 pygments==2.7.4
     # via colored-traceback
```

### Comparing `octomy-batch-1.0.8/requirements/test_requirements.txt` & `octomy-batch-1.0.9/requirements/test_requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     #   black
     #   mypy
 mypy==0.790
     # via
     #   -r temporary_requirements.in
     #   pytest-mypy
     #   sqlalchemy-stubs
-octomy-common==1.0.13
+octomy-common==1.0.14
     # via -r temporary_requirements.in
 packaging==20.8
     # via pytest
 pathspec==0.8.1
     # via black
 pip-tools==5.5.0
     # via -r temporary_requirements.in
```

### Comparing `octomy-batch-1.0.8/setup.py` & `octomy-batch-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.8/tests/Makefile` & `octomy-batch-1.0.9/tests/Makefile`

 * *Files identical despite different names*

