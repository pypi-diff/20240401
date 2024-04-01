# Comparing `tmp/pre5g-0.8.tar.gz` & `tmp/pre5g-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.8.tar", last modified: Mon Apr  1 11:29:47 2024, max compression
+gzip compressed data, was "dist/pre5g-0.9.tar", last modified: Mon Apr  1 11:30:48 2024, max compression
```

## Comparing `pre5g-0.8.tar` & `pre5g-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:29:47.858564 pre5g-0.8/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.8/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:29:47.857564 pre5g-0.8/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.8/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:29:47.856564 pre5g-0.8/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-01 11:29:32.000000 pre5g-0.8/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1330 2024-04-01 11:28:19.000000 pre5g-0.8/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2687 2024-04-01 11:28:46.000000 pre5g-0.8/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1318 2024-04-01 11:26:36.000000 pre5g-0.8/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.8/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3143 2024-04-01 11:29:20.000000 pre5g-0.8/pre5g/standardization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:29:47.857564 pre5g-0.8/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:29:47.000000 pre5g-0.8/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-01 11:29:47.000000 pre5g-0.8/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-01 11:29:47.000000 pre5g-0.8/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-01 11:29:47.000000 pre5g-0.8/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-01 11:29:47.858564 pre5g-0.8/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      601 2024-03-28 04:29:48.000000 pre5g-0.8/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.087291 pre5g-0.9/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.9/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:30:48.087291 pre5g-0.9/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.9/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.086291 pre5g-0.9/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      650 2024-04-01 11:29:32.000000 pre5g-0.9/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1330 2024-04-01 11:28:19.000000 pre5g-0.9/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2687 2024-04-01 11:28:46.000000 pre5g-0.9/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1318 2024-04-01 11:26:36.000000 pre5g-0.9/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.9/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3143 2024-04-01 11:29:20.000000 pre5g-0.9/pre5g/standardization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-01 11:30:48.087291 pre5g-0.9/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      265 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-01 11:30:48.000000 pre5g-0.9/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-01 11:30:48.087291 pre5g-0.9/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      601 2024-04-01 11:30:41.000000 pre5g-0.9/setup.py
```

### Comparing `pre5g-0.8/LICENSE` & `pre5g-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/__init__.py` & `pre5g-0.9/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/labelen.py` & `pre5g-0.9/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/normalization.py` & `pre5g-0.9/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/onehoten.py` & `pre5g-0.9/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/robustscaler.py` & `pre5g-0.9/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/pre5g/standardization.py` & `pre5g-0.9/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.8/setup.py` & `pre5g-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

