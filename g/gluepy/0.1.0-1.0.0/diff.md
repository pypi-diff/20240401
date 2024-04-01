# Comparing `tmp/gluepy-0.1.0.tar.gz` & `tmp/gluepy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gluepy-0.1.0.tar", last modified: Wed Apr  1 21:22:26 2020, max compression
+gzip compressed data, was "gluepy-1.0.0.tar", last modified: Mon Apr  1 09:32:48 2024, max compression
```

## Comparing `gluepy-0.1.0.tar` & `gluepy-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-01 21:22:26.823002 gluepy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-04-01 21:22:20.000000 gluepy-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)      457 2020-04-01 21:22:26.823002 gluepy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-04-01 21:22:20.000000 gluepy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-01 21:22:26.823002 gluepy-0.1.0/gluepy/
--rw-r--r--   0 runner    (1001) docker     (115)       18 2020-04-01 21:22:20.000000 gluepy-0.1.0/gluepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-01 21:22:26.823002 gluepy-0.1.0/gluepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)      457 2020-04-01 21:22:26.000000 gluepy-0.1.0/gluepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      169 2020-04-01 21:22:26.000000 gluepy-0.1.0/gluepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-04-01 21:22:26.000000 gluepy-0.1.0/gluepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)        7 2020-04-01 21:22:26.000000 gluepy-0.1.0/gluepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-04-01 21:22:26.823002 gluepy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      802 2020-04-01 21:22:20.000000 gluepy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:32:40.000000 gluepy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:32:48.064003 gluepy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 09:32:40.000000 gluepy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.056003 gluepy-1.0.0/gluepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.056003 gluepy-1.0.0/gluepy/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/bin/gluepy-cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/gluepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/startmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/startproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/commands/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/exec/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/data/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/files/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/files/storages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.060003 gluepy-1.0.0/gluepy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-01 09:32:40.000000 gluepy-1.0.0/gluepy/utils/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/gluepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 09:32:48.000000 gluepy-1.0.0/gluepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:32:48.064003 gluepy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-01 09:32:40.000000 gluepy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:32:48.064003 gluepy-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 09:32:40.000000 gluepy-1.0.0/tests/test_sample.py
```

