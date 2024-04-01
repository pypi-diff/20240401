# Comparing `tmp/timeoutcall-1.0.tar.gz` & `tmp/timeoutcall-1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeoutcall-1.0.tar", last modified: Mon Apr  1 15:03:49 2024, max compression
+gzip compressed data, was "timeoutcall-1.0rc2.tar", last modified: Sat Mar 30 14:23:02 2024, max compression
```

## Comparing `timeoutcall-1.0.tar` & `timeoutcall-1.0rc2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-01 15:03:49.951413 timeoutcall-1.0/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-04-01 15:01:28.000000 timeoutcall-1.0/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2037 2024-04-01 15:03:49.951413 timeoutcall-1.0/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1292 2024-04-01 14:59:57.000000 timeoutcall-1.0/README.md
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-01 15:03:49.951413 timeoutcall-1.0/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)      999 2024-04-01 14:09:07.000000 timeoutcall-1.0/setup.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-01 15:03:49.951413 timeoutcall-1.0/timeoutcall/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2070 2024-04-01 15:03:34.000000 timeoutcall-1.0/timeoutcall/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1725 2024-04-01 13:47:57.000000 timeoutcall-1.0/timeoutcall/test.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      773 2024-04-01 14:05:35.000000 timeoutcall-1.0/timeoutcall/testcall.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-01 15:03:49.951413 timeoutcall-1.0/timeoutcall.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2037 2024-04-01 15:03:49.000000 timeoutcall-1.0/timeoutcall.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      234 2024-04-01 15:03:49.000000 timeoutcall-1.0/timeoutcall.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-01 15:03:49.000000 timeoutcall-1.0/timeoutcall.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-04-01 15:03:49.000000 timeoutcall-1.0/timeoutcall.egg-info/top_level.txt
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-30 14:23:02.721583 timeoutcall-1.0rc2/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1260 2024-03-30 14:23:02.721583 timeoutcall-1.0rc2/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      573 2024-03-30 14:06:10.000000 timeoutcall-1.0rc2/README.md
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-03-30 14:23:02.721583 timeoutcall-1.0rc2/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      904 2024-03-30 14:16:10.000000 timeoutcall-1.0rc2/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-30 14:23:02.720583 timeoutcall-1.0rc2/timeoutcall/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      947 2024-03-30 14:22:16.000000 timeoutcall-1.0rc2/timeoutcall/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      882 2024-03-30 14:21:50.000000 timeoutcall-1.0rc2/timeoutcall/test.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-03-30 14:23:02.721583 timeoutcall-1.0rc2/timeoutcall.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1260 2024-03-30 14:23:02.000000 timeoutcall-1.0rc2/timeoutcall.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      202 2024-03-30 14:23:02.000000 timeoutcall-1.0rc2/timeoutcall.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-03-30 14:23:02.000000 timeoutcall-1.0rc2/timeoutcall.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-03-30 14:23:02.000000 timeoutcall-1.0rc2/timeoutcall.egg-info/top_level.txt
```

### Comparing `timeoutcall-1.0/setup.py` & `timeoutcall-1.0rc2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,15 +22,9 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Intended Audience :: Developers",
     ],
     python_requires=">=3.8",
-    keywords=[
-        "timeout",
-        "sleep",
-        "wait",
-        "decorator",
-    ],
     license="MIT",
 )
```

