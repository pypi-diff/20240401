# Comparing `tmp/payze-pkg-2.1.tar.gz` & `tmp/payze-pkg-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payze-pkg-2.1.tar", last modified: Mon Apr  1 05:22:09 2024, max compression
+gzip compressed data, was "payze-pkg-2.2.tar", last modified: Mon Apr  1 09:57:52 2024, max compression
```

## Comparing `payze-pkg-2.1.tar` & `payze-pkg-2.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.939979 payze-pkg-2.1/
--rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 05:22:09.939892 payze-pkg-2.1/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)      857 2024-04-01 04:25:57.000000 payze-pkg-2.1/README.md
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.935428 payze-pkg-2.1/payze/
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.936025 payze-pkg-2.1/payze/param/
--rw-r--r--   0 muhammadali   (501) staff       (20)      141 2024-04-01 04:17:05.000000 payze-pkg-2.1/payze/param/__init__.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.936503 payze-pkg-2.1/payze/param/ops/
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-03-30 20:13:36.000000 payze-pkg-2.1/payze/param/ops/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      407 2024-04-01 04:19:11.000000 payze-pkg-2.1/payze/param/ops/client.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.937350 payze-pkg-2.1/payze/param/request/
--rw-r--r--   0 muhammadali   (501) staff       (20)       76 2024-04-01 04:06:02.000000 payze-pkg-2.1/payze/param/request/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      507 2024-04-01 04:05:59.000000 payze-pkg-2.1/payze/param/request/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      689 2024-04-01 04:26:58.000000 payze-pkg-2.1/payze/param/request/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.938100 payze-pkg-2.1/payze/param/response/
--rw-r--r--   0 muhammadali   (501) staff       (20)       60 2024-04-01 04:06:00.000000 payze-pkg-2.1/payze/param/response/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     2076 2024-04-01 03:57:51.000000 payze-pkg-2.1/payze/param/response/base.py
--rw-r--r--   0 muhammadali   (501) staff       (20)      200 2024-04-01 04:19:43.000000 payze-pkg-2.1/payze/param/response/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.938869 payze-pkg-2.1/payze/param/webhook/
--rw-r--r--   0 muhammadali   (501) staff       (20)        0 2024-04-01 04:04:42.000000 payze-pkg-2.1/payze/param/webhook/__init__.py
--rw-r--r--   0 muhammadali   (501) staff       (20)     1533 2024-04-01 04:05:58.000000 payze-pkg-2.1/payze/param/webhook/just_pay.py
-drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 05:22:09.939631 payze-pkg-2.1/payze/payze_pkg.egg-info/
--rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 05:22:09.000000 payze-pkg-2.1/payze/payze_pkg.egg-info/PKG-INFO
--rw-r--r--   0 muhammadali   (501) staff       (20)      551 2024-04-01 05:22:09.000000 payze-pkg-2.1/payze/payze_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        1 2024-04-01 05:22:09.000000 payze-pkg-2.1/payze/payze_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-04-01 05:22:09.000000 payze-pkg-2.1/payze/payze_pkg.egg-info/requires.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)        6 2024-04-01 05:22:09.000000 payze-pkg-2.1/payze/payze_pkg.egg-info/top_level.txt
--rw-r--r--   0 muhammadali   (501) staff       (20)      107 2024-04-01 05:22:09.940230 payze-pkg-2.1/setup.cfg
--rw-r--r--   0 muhammadali   (501) staff       (20)      535 2024-04-01 05:21:58.000000 payze-pkg-2.1/setup.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.678645 payze-pkg-2.2/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 09:57:52.678555 payze-pkg-2.2/PKG-INFO
+-rw-r--r--   0 muhammadali   (501) staff       (20)      857 2024-04-01 04:25:57.000000 payze-pkg-2.2/README.md
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.675669 payze-pkg-2.2/payze/
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676374 payze-pkg-2.2/payze/payze/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       48 2024-04-01 09:56:33.000000 payze-pkg-2.2/payze/payze/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     1785 2024-04-01 09:56:55.000000 payze-pkg-2.2/payze/payze/client.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676480 payze-pkg-2.2/payze/payze/param/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      141 2024-04-01 04:17:05.000000 payze-pkg-2.2/payze/payze/param/__init__.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.676737 payze-pkg-2.2/payze/payze/param/ops/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-03-30 20:13:36.000000 payze-pkg-2.2/payze/payze/param/ops/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      407 2024-04-01 04:19:11.000000 payze-pkg-2.2/payze/payze/param/ops/client.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677110 payze-pkg-2.2/payze/payze/param/request/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       76 2024-04-01 04:06:02.000000 payze-pkg-2.2/payze/payze/param/request/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      507 2024-04-01 04:05:59.000000 payze-pkg-2.2/payze/payze/param/request/base.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      689 2024-04-01 04:26:58.000000 payze-pkg-2.2/payze/payze/param/request/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677460 payze-pkg-2.2/payze/payze/param/response/
+-rw-r--r--   0 muhammadali   (501) staff       (20)       60 2024-04-01 04:06:00.000000 payze-pkg-2.2/payze/payze/param/response/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     2076 2024-04-01 03:57:51.000000 payze-pkg-2.2/payze/payze/param/response/base.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)      200 2024-04-01 04:19:43.000000 payze-pkg-2.2/payze/payze/param/response/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.677693 payze-pkg-2.2/payze/payze/param/webhook/
+-rw-r--r--   0 muhammadali   (501) staff       (20)        0 2024-04-01 04:04:42.000000 payze-pkg-2.2/payze/payze/param/webhook/__init__.py
+-rw-r--r--   0 muhammadali   (501) staff       (20)     1533 2024-04-01 04:05:58.000000 payze-pkg-2.2/payze/payze/param/webhook/just_pay.py
+drwxr-xr-x   0 muhammadali   (501) staff       (20)        0 2024-04-01 09:57:52.678312 payze-pkg-2.2/payze/payze_pkg.egg-info/
+-rw-r--r--   0 muhammadali   (501) staff       (20)      328 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadali   (501) staff       (20)      663 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)        1 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)       47 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/requires.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)        6 2024-04-01 09:57:52.000000 payze-pkg-2.2/payze/payze_pkg.egg-info/top_level.txt
+-rw-r--r--   0 muhammadali   (501) staff       (20)      107 2024-04-01 09:57:52.678937 payze-pkg-2.2/setup.cfg
+-rw-r--r--   0 muhammadali   (501) staff       (20)      535 2024-04-01 09:57:36.000000 payze-pkg-2.2/setup.py
```

### Comparing `payze-pkg-2.1/README.md` & `payze-pkg-2.2/README.md`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.1/payze/param/request/just_pay.py` & `payze-pkg-2.2/payze/payze/param/request/just_pay.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.1/payze/param/response/base.py` & `payze-pkg-2.2/payze/payze/param/response/base.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.1/payze/param/webhook/just_pay.py` & `payze-pkg-2.2/payze/payze/param/webhook/just_pay.py`

 * *Files identical despite different names*

### Comparing `payze-pkg-2.1/payze/payze_pkg.egg-info/SOURCES.txt` & `payze-pkg-2.2/payze/payze_pkg.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.md
 setup.cfg
 setup.py
-payze/param/__init__.py
-payze/param/ops/__init__.py
-payze/param/ops/client.py
-payze/param/request/__init__.py
-payze/param/request/base.py
-payze/param/request/just_pay.py
-payze/param/response/__init__.py
-payze/param/response/base.py
-payze/param/response/just_pay.py
-payze/param/webhook/__init__.py
-payze/param/webhook/just_pay.py
+payze/payze/__init__.py
+payze/payze/client.py
+payze/payze/param/__init__.py
+payze/payze/param/ops/__init__.py
+payze/payze/param/ops/client.py
+payze/payze/param/request/__init__.py
+payze/payze/param/request/base.py
+payze/payze/param/request/just_pay.py
+payze/payze/param/response/__init__.py
+payze/payze/param/response/base.py
+payze/payze/param/response/just_pay.py
+payze/payze/param/webhook/__init__.py
+payze/payze/param/webhook/just_pay.py
 payze/payze_pkg.egg-info/PKG-INFO
 payze/payze_pkg.egg-info/SOURCES.txt
 payze/payze_pkg.egg-info/dependency_links.txt
 payze/payze_pkg.egg-info/requires.txt
 payze/payze_pkg.egg-info/top_level.txt
```

### Comparing `payze-pkg-2.1/setup.py` & `payze-pkg-2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
     name='payze-pkg',
-    version='2.1',
+    version='2.2',
     license='MIT',
     author="paytechuz",
     author_email='paytechuz@gmail.com',
     packages=find_packages('payze'),
     package_dir={'': 'payze'},
     url='https://github.com/PayTechUz/payze-pkg',
     keywords='payze-merchant payze-uz payze-pkg payze-python payze-github',
```

