# Comparing `tmp/cryptoowl-0.0.8.tar.gz` & `tmp/cryptoowl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptoowl-0.0.8.tar", last modified: Sun Jun 25 08:21:25 2023, max compression
+gzip compressed data, was "cryptoowl-0.0.9.tar", last modified: Sun Jun 25 21:26:23 2023, max compression
```

## Comparing `cryptoowl-0.0.8.tar` & `cryptoowl-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/cryptoowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-25 08:21:25.000000 cryptoowl-0.0.8/cryptoowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 08:21:25.000000 cryptoowl-0.0.8/cryptoowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:21:25.000000 cryptoowl-0.0.8/cryptoowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 08:21:25.000000 cryptoowl-0.0.8/cryptoowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 08:21:25.000000 cryptoowl-0.0.8/cryptoowl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/database/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 08:21:25.375017 cryptoowl-0.0.8/social/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-25 08:21:17.000000 cryptoowl-0.0.8/social/kitty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/cryptoowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-25 21:26:23.000000 cryptoowl-0.0.9/cryptoowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 21:26:23.000000 cryptoowl-0.0.9/cryptoowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:26:23.000000 cryptoowl-0.0.9/cryptoowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 21:26:23.000000 cryptoowl-0.0.9/cryptoowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 21:26:23.000000 cryptoowl-0.0.9/cryptoowl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/database/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:26:23.299803 cryptoowl-0.0.9/social/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-25 21:26:18.000000 cryptoowl-0.0.9/social/kitty.py
```

### Comparing `cryptoowl-0.0.8/LICENSE` & `cryptoowl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptoowl-0.0.8/database/constants.py` & `cryptoowl-0.0.9/database/constants.py`

 * *Files identical despite different names*

