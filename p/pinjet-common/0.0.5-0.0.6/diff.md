# Comparing `tmp/pinjet-common-0.0.5.tar.gz` & `tmp/pinjet-common-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinjet-common-0.0.5.tar", last modified: Mon Apr  1 18:34:24 2024, max compression
+gzip compressed data, was "dist/pinjet-common-0.0.6.tar", last modified: Mon Apr  1 18:38:11 2024, max compression
```

## Comparing `pinjet-common-0.0.5.tar` & `pinjet-common-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/
--rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-0.0.5/LICENSE
--rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-0.0.5/README.md
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.5/pinjet/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet/common/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.5/pinjet/common/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet/common/constants/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.5/pinjet/common/constants/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-0.0.5/pinjet/common/constants/constants.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet/common/io_constants/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.5/pinjet/common/io_constants/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      279 2024-04-01 16:55:14.000000 pinjet-common-0.0.5/pinjet/common/io_constants/io_constants.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet_common.egg-info/
--rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet_common.egg-info/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)      374 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet_common.egg-info/SOURCES.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet_common.egg-info/dependency_links.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/pinjet_common.egg-info/top_level.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-01 18:34:24.000000 pinjet-common-0.0.5/setup.cfg
--rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 18:34:12.000000 pinjet-common-0.0.5/setup.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/
+-rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-0.0.6/LICENSE
+-rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-0.0.6/README.md
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.6/pinjet/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet/common/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.6/pinjet/common/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet/common/constants/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.6/pinjet/common/constants/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-0.0.6/pinjet/common/constants/constants.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet/common/io_constants/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.6/pinjet/common/io_constants/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      279 2024-04-01 16:55:14.000000 pinjet-common-0.0.6/pinjet/common/io_constants/io_constants.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet_common.egg-info/
+-rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet_common.egg-info/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)      374 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet_common.egg-info/SOURCES.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet_common.egg-info/dependency_links.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/pinjet_common.egg-info/top_level.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-01 18:38:11.000000 pinjet-common-0.0.6/setup.cfg
+-rw-r--r--   0 abetrack3   (501) staff       (20)      427 2024-04-01 18:38:01.000000 pinjet-common-0.0.6/setup.py
```

### Comparing `pinjet-common-0.0.5/LICENSE` & `pinjet-common-0.0.6/LICENSE`

 * *Files identical despite different names*

