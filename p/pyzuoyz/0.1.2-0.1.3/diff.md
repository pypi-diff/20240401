# Comparing `tmp/pyzuoyz-0.1.2.tar.gz` & `tmp/pyzuoyz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzuoyz-0.1.2.tar", last modified: Mon Apr  1 05:07:36 2024, max compression
+gzip compressed data, was "pyzuoyz-0.1.3.tar", last modified: Mon Apr  1 11:32:57 2024, max compression
```

## Comparing `pyzuoyz-0.1.2.tar` & `pyzuoyz-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 05:07:36.349656 pyzuoyz-0.1.2/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)     1068 2024-04-01 04:24:56.000000 pyzuoyz-0.1.2/LICENSE
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      886 2024-04-01 05:07:36.349460 pyzuoyz-0.1.2/PKG-INFO
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       96 2024-04-01 04:54:26.000000 pyzuoyz-0.1.2/README.rst
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 05:07:36.348527 pyzuoyz-0.1.2/pyzuoyz/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 04:30:18.000000 pyzuoyz-0.1.2/pyzuoyz/__init__.py
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      129 2024-04-01 05:07:13.000000 pyzuoyz-0.1.2/pyzuoyz/help.py
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      427 2024-04-01 04:29:01.000000 pyzuoyz-0.1.2/pyzuoyz/main.py
-drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 05:07:36.349250 pyzuoyz-0.1.2/pyzuoyz.egg-info/
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      886 2024-04-01 05:07:36.000000 pyzuoyz-0.1.2/pyzuoyz.egg-info/PKG-INFO
--rw-r--r--   0 aaazuoyz   (501) staff       (20)      203 2024-04-01 05:07:36.000000 pyzuoyz-0.1.2/pyzuoyz.egg-info/SOURCES.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)        1 2024-04-01 05:07:36.000000 pyzuoyz-0.1.2/pyzuoyz.egg-info/dependency_links.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)        8 2024-04-01 05:07:36.000000 pyzuoyz-0.1.2/pyzuoyz.egg-info/top_level.txt
--rw-r--r--   0 aaazuoyz   (501) staff       (20)       38 2024-04-01 05:07:36.349703 pyzuoyz-0.1.2/setup.cfg
--rw-r--r--   0 aaazuoyz   (501) staff       (20)     4060 2024-04-01 05:07:29.000000 pyzuoyz-0.1.2/setup.py
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:32:57.980228 pyzuoyz-0.1.3/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     1068 2024-04-01 04:24:56.000000 pyzuoyz-0.1.3/LICENSE
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-04-01 11:32:57.980017 pyzuoyz-0.1.3/PKG-INFO
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       96 2024-04-01 04:54:26.000000 pyzuoyz-0.1.3/README.rst
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:32:57.978845 pyzuoyz-0.1.3/pyzuoyz/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 04:30:18.000000 pyzuoyz-0.1.3/pyzuoyz/__init__.py
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      129 2024-04-01 05:07:13.000000 pyzuoyz-0.1.3/pyzuoyz/help.py
+drwxr-xr-x   0 aaazuoyz   (501) staff       (20)        0 2024-04-01 11:32:57.979772 pyzuoyz-0.1.3/pyzuoyz.egg-info/
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      948 2024-04-01 11:32:57.000000 pyzuoyz-0.1.3/pyzuoyz.egg-info/PKG-INFO
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)      217 2024-04-01 11:32:57.000000 pyzuoyz-0.1.3/pyzuoyz.egg-info/SOURCES.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)        1 2024-04-01 11:32:57.000000 pyzuoyz-0.1.3/pyzuoyz.egg-info/dependency_links.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       17 2024-04-01 11:32:57.000000 pyzuoyz-0.1.3/pyzuoyz.egg-info/requires.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)        8 2024-04-01 11:32:57.000000 pyzuoyz-0.1.3/pyzuoyz.egg-info/top_level.txt
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)       38 2024-04-01 11:32:57.980278 pyzuoyz-0.1.3/setup.cfg
+-rw-r--r--   0 aaazuoyz   (501) staff       (20)     4053 2024-04-01 11:32:16.000000 pyzuoyz-0.1.3/setup.py
```

### Comparing `pyzuoyz-0.1.2/LICENSE` & `pyzuoyz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzuoyz-0.1.2/setup.py` & `pyzuoyz-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'pyzuoyz'
 DESCRIPTION = 'Packages for zyz.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'z80179030@163.com'
 AUTHOR = 'Yuezhong Zuo'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    # 'requests', 'maya', 'records',
+    'nltk', 'jieba', 'rouge',
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

