# Comparing `tmp/sajjad-1.1.tar.gz` & `tmp/sajjad-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.1.tar", last modified: Mon Apr  1 19:56:55 2024, max compression
+gzip compressed data, was "sajjad-1.2.tar", last modified: Mon Apr  1 20:16:17 2024, max compression
```

## Comparing `sajjad-1.1.tar` & `sajjad-1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 19:56:55.478526 sajjad-1.1/
--rw-rw-rw-   0        0        0      437 2024-04-01 19:56:55.477526 sajjad-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 19:56:55.476527 sajjad-1.1/sajjad.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.1/sajjad.py
--rw-rw-rw-   0        0        0       42 2024-04-01 19:56:55.478526 sajjad-1.1/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-01 19:56:18.000000 sajjad-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:16:17.074070 sajjad-1.2/
+-rw-rw-rw-   0        0        0      445 2024-04-01 20:16:17.074070 sajjad-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 20:16:17.073071 sajjad-1.2/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      445 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.2/sajjad.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:16:17.075073 sajjad-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      548 2024-04-01 20:16:04.000000 sajjad-1.2/setup.py
```

### Comparing `sajjad-1.1/setup.py` & `sajjad-1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='sajjad',
-    version='1.1',
+    version='1.2',
     py_modules=['sajjad'],
     description='A simple python library',
-    author='Your Name',
-    author_email='your.email@example.com',
+    author='sajjad seyedi',
+    author_email='sajjad.seyedi.88@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

