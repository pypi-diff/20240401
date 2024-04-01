# Comparing `tmp/utils_huna-0.1.4.tar.gz` & `tmp/utils_huna-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_huna-0.1.4.tar", last modified: Mon Apr  1 16:56:14 2024, max compression
+gzip compressed data, was "utils_huna-0.1.5.tar", last modified: Mon Apr  1 17:01:09 2024, max compression
```

## Comparing `utils_huna-0.1.4.tar` & `utils_huna-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:56:14.528825 utils_huna-0.1.4/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.4/README.md
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-01 16:56:14.528825 utils_huna-0.1.4/setup.cfg
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-01 16:52:38.000000 utils_huna-0.1.4/setup.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/utils_huna/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       44 2024-04-01 16:51:08.000000 utils_huna-0.1.4/utils_huna/__init__.py
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      395 2024-04-01 14:22:15.000000 utils_huna-0.1.4/utils_huna/utils_huna.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/utils_huna.egg-info/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      202 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 17:01:09.327642 utils_huna-0.1.5/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 17:01:09.327642 utils_huna-0.1.5/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.5/README.md
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-01 17:01:09.327642 utils_huna-0.1.5/setup.cfg
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-01 17:00:49.000000 utils_huna-0.1.5/setup.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 17:01:09.327642 utils_huna-0.1.5/utils_huna/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       17 2024-04-01 17:00:32.000000 utils_huna-0.1.5/utils_huna/__init__.py
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      395 2024-04-01 14:22:15.000000 utils_huna-0.1.5/utils_huna/utils_huna.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 17:01:09.327642 utils_huna-0.1.5/utils_huna.egg-info/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 17:01:09.000000 utils_huna-0.1.5/utils_huna.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      202 2024-04-01 17:01:09.000000 utils_huna-0.1.5/utils_huna.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 17:01:09.000000 utils_huna-0.1.5/utils_huna.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-01 17:01:09.000000 utils_huna-0.1.5/utils_huna.egg-info/top_level.txt
```

