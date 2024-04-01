# Comparing `tmp/utils_huna-0.1.3.tar.gz` & `tmp/utils_huna-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_huna-0.1.3.tar", last modified: Mon Apr  1 16:46:39 2024, max compression
+gzip compressed data, was "utils_huna-0.1.4.tar", last modified: Mon Apr  1 16:56:14 2024, max compression
```

## Comparing `utils_huna-0.1.3.tar` & `utils_huna-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,13 @@
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:46:39.428509 utils_huna-0.1.3/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:46:39.428509 utils_huna-0.1.3/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.3/README.md
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-01 16:46:39.428509 utils_huna-0.1.3/setup.cfg
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-01 16:46:19.000000 utils_huna-0.1.3/setup.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:46:39.428509 utils_huna-0.1.3/utils_huna/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       44 2024-04-01 16:45:52.000000 utils_huna-0.1.3/utils_huna/__init__.py
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      395 2024-04-01 14:22:15.000000 utils_huna-0.1.3/utils_huna/utils.py
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:46:39.428509 utils_huna-0.1.3/utils_huna.egg-info/
-drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:46:39.428509 utils_huna-0.1.3/utils_huna.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 14:36:32.000000 utils_huna-0.1.3/utils_huna.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      154 2024-04-01 14:36:32.000000 utils_huna-0.1.3/utils_huna.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 14:36:32.000000 utils_huna-0.1.3/utils_huna.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 14:36:32.000000 utils_huna-0.1.3/utils_huna.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:46:39.000000 utils_huna-0.1.3/utils_huna.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)      453 2024-04-01 16:46:39.000000 utils_huna-0.1.3/utils_huna.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 16:46:39.000000 utils_huna-0.1.3/utils_huna.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-01 16:46:39.000000 utils_huna-0.1.3/utils_huna.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:56:14.528825 utils_huna-0.1.4/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      326 2024-03-18 14:37:13.000000 utils_huna-0.1.4/README.md
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       38 2024-04-01 16:56:14.528825 utils_huna-0.1.4/setup.cfg
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      204 2024-04-01 16:52:38.000000 utils_huna-0.1.4/setup.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/utils_huna/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       44 2024-04-01 16:51:08.000000 utils_huna-0.1.4/utils_huna/__init__.py
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      395 2024-04-01 14:22:15.000000 utils_huna-0.1.4/utils_huna/utils_huna.py
+drwxr-xr-x   0 jupyter   (1005) jupyter   (1006)        0 2024-04-01 16:56:14.528825 utils_huna-0.1.4/utils_huna.egg-info/
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       98 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)      202 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)        1 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1005) jupyter   (1006)       11 2024-04-01 16:56:14.000000 utils_huna-0.1.4/utils_huna.egg-info/top_level.txt
```

