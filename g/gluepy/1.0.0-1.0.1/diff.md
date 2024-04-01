# Comparing `tmp/gluepy-1.0.0.tar.gz` & `tmp/gluepy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluepy-1.0.0.tar", last modified: Mon Apr  1 09:32:48 2024, max compression
+gzip compressed data, was "gluepy-1.0.1.tar", last modified: Mon Apr  1 09:46:02 2024, max compression
```

## Comparing `gluepy-1.0.0.tar` & `gluepy-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:32:40.000000 gluepy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:32:48.064003 gluepy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 09:32:40.000000 gluepy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.056003 gluepy-1.0.0/gluepy/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.056003 gluepy-1.0.0/gluepy/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/bin/gluepy-cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/gluepy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/startmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/startproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/boot.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/data/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/gluepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:32:48.064003 gluepy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-01 09:32:40.000000 gluepy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 09:32:40.000000 gluepy-1.0.0/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.030297 gluepy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:45:53.000000 gluepy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:46:02.030297 gluepy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 09:45:53.000000 gluepy-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.022297 gluepy-1.0.1/gluepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.022297 gluepy-1.0.1/gluepy/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/bin/gluepy-cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/gluepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/startmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/startproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/commands/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/conf/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/exec/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/exec/dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/exec/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/files/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/data/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.026297 gluepy-1.0.1/gluepy/files/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/files/storages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.030297 gluepy-1.0.1/gluepy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-01 09:45:53.000000 gluepy-1.0.1/gluepy/utils/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.030297 gluepy-1.0.1/gluepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 09:46:01.000000 gluepy-1.0.1/gluepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:46:02.030297 gluepy-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-01 09:45:53.000000 gluepy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:46:02.030297 gluepy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 09:45:53.000000 gluepy-1.0.1/tests/test_sample.py
```

### Comparing `gluepy-1.0.0/LICENSE` & `gluepy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/PKG-INFO` & `gluepy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.0.0/gluepy/commands/airflow.py` & `gluepy-1.0.1/gluepy/commands/airflow.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/commands/base.py` & `gluepy-1.0.1/gluepy/commands/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/commands/dag.py` & `gluepy-1.0.1/gluepy/commands/dag.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/commands/gluepy.py` & `gluepy-1.0.1/gluepy/commands/gluepy.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/commands/task.py` & `gluepy-1.0.1/gluepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/conf/context.py` & `gluepy-1.0.1/gluepy/conf/context.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/exec/dags.py` & `gluepy-1.0.1/gluepy/exec/dags.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/exec/tasks.py` & `gluepy-1.0.1/gluepy/exec/tasks.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/files/data/pandas.py` & `gluepy-1.0.1/gluepy/files/data/pandas.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/files/storages/base.py` & `gluepy-1.0.1/gluepy/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/files/storages/google.py` & `gluepy-1.0.1/gluepy/files/storages/google.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/files/storages/local.py` & `gluepy-1.0.1/gluepy/files/storages/local.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/files/storages/s3.py` & `gluepy-1.0.1/gluepy/files/storages/s3.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/utils/dict.py` & `gluepy-1.0.1/gluepy/utils/dict.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy/utils/loading.py` & `gluepy-1.0.1/gluepy/utils/loading.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/gluepy.egg-info/PKG-INFO` & `gluepy-1.0.1/gluepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.0.0/gluepy.egg-info/SOURCES.txt` & `gluepy-1.0.1/gluepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gluepy-1.0.0/setup.py` & `gluepy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     extra_require={
         "all": (requirements_base + requirements_dev + requirements_digitalocean),
         "digitalocean": (requirements_base + requirements_digitalocean),
         "gcp": (requirements_base + requirements_gcp),
     },
     entry_points="""
         [console_scripts]
-        gluepy=gluepy.commands.gluepy:cli
+        gluepy-cli=gluepy.commands.gluepy:cli
     """,
 )
```

