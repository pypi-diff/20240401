# Comparing `tmp/pinjet-common-0.0.2.tar.gz` & `tmp/pinjet-common-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinjet-common-0.0.2.tar", last modified: Mon Apr  1 18:12:29 2024, max compression
+gzip compressed data, was "dist/pinjet-common-0.0.3.tar", last modified: Mon Apr  1 18:28:55 2024, max compression
```

## Comparing `pinjet-common-0.0.2.tar` & `pinjet-common-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/
--rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-0.0.2/LICENSE
--rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-0.0.2/README.md
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet/
--rw-r--r--   0 abetrack3   (501) staff       (20)       14 2024-04-01 18:06:10.000000 pinjet-common-0.0.2/pinjet/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet/common/
--rw-r--r--   0 abetrack3   (501) staff       (20)       37 2024-04-01 18:06:10.000000 pinjet-common-0.0.2/pinjet/common/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet/common/constants/
--rw-r--r--   0 abetrack3   (501) staff       (20)       87 2024-04-01 16:53:34.000000 pinjet-common-0.0.2/pinjet/common/constants/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-0.0.2/pinjet/common/constants/constants.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet/common/io_constants/
--rw-r--r--   0 abetrack3   (501) staff       (20)      143 2024-04-01 16:55:14.000000 pinjet-common-0.0.2/pinjet/common/io_constants/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      279 2024-04-01 16:55:14.000000 pinjet-common-0.0.2/pinjet/common/io_constants/io_constants.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet_common.egg-info/
--rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet_common.egg-info/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)      374 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet_common.egg-info/SOURCES.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet_common.egg-info/dependency_links.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/pinjet_common.egg-info/top_level.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-01 18:12:29.000000 pinjet-common-0.0.2/setup.cfg
--rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 18:07:50.000000 pinjet-common-0.0.2/setup.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/
+-rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-0.0.3/LICENSE
+-rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-0.0.3/README.md
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.3/pinjet/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet/common/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.3/pinjet/common/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet/common/constants/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.3/pinjet/common/constants/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-0.0.3/pinjet/common/constants/constants.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet/common/io_constants/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-0.0.3/pinjet/common/io_constants/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      279 2024-04-01 16:55:14.000000 pinjet-common-0.0.3/pinjet/common/io_constants/io_constants.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet_common.egg-info/
+-rw-r--r--   0 abetrack3   (501) staff       (20)      240 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet_common.egg-info/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)      374 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet_common.egg-info/SOURCES.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet_common.egg-info/dependency_links.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/pinjet_common.egg-info/top_level.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-01 18:28:55.000000 pinjet-common-0.0.3/setup.cfg
+-rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 18:28:37.000000 pinjet-common-0.0.3/setup.py
```

### Comparing `pinjet-common-0.0.2/LICENSE` & `pinjet-common-0.0.3/LICENSE`

 * *Files identical despite different names*

