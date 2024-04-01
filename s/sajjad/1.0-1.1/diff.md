# Comparing `tmp/sajjad-1.0.tar.gz` & `tmp/sajjad-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.0.tar", last modified: Mon Apr  1 19:08:54 2024, max compression
+gzip compressed data, was "sajjad-1.1.tar", last modified: Mon Apr  1 19:56:55 2024, max compression
```

## Comparing `sajjad-1.0.tar` & `sajjad-1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 19:08:54.442749 sajjad-1.0/
--rw-rw-rw-   0        0        0      437 2024-04-01 19:08:54.441054 sajjad-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 19:08:54.440054 sajjad-1.0/sajjad.egg-info/
--rw-rw-rw-   0        0        0      437 2024-04-01 19:08:53.000000 sajjad-1.0/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      128 2024-04-01 19:08:53.000000 sajjad-1.0/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:08:53.000000 sajjad-1.0/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 19:08:53.000000 sajjad-1.0/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 19:08:54.442749 sajjad-1.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-01 19:08:29.000000 sajjad-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:56:55.478526 sajjad-1.1/
+-rw-rw-rw-   0        0        0      437 2024-04-01 19:56:55.477526 sajjad-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 19:56:55.476527 sajjad-1.1/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      437 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 19:56:55.000000 sajjad-1.1/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.1/sajjad.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:56:55.478526 sajjad-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-01 19:56:18.000000 sajjad-1.1/setup.py
```

### Comparing `sajjad-1.0/setup.py` & `sajjad-1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name='sajjad',
-    version='1.0',
-    packages=find_packages(),
+    version='1.1',
+    py_modules=['sajjad'],
     description='A simple python library',
     author='Your Name',
     author_email='your.email@example.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

