# Comparing `tmp/sajjad-1.2.tar.gz` & `tmp/sajjad-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.2.tar", last modified: Mon Apr  1 20:16:17 2024, max compression
+gzip compressed data, was "sajjad-1.3.tar", last modified: Mon Apr  1 20:22:25 2024, max compression
```

## Comparing `sajjad-1.2.tar` & `sajjad-1.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:16:17.074070 sajjad-1.2/
--rw-rw-rw-   0        0        0      445 2024-04-01 20:16:17.074070 sajjad-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 20:16:17.073071 sajjad-1.2/sajjad.egg-info/
--rw-rw-rw-   0        0        0      445 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 20:16:16.000000 sajjad-1.2/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.2/sajjad.py
--rw-rw-rw-   0        0        0       42 2024-04-01 20:16:17.075073 sajjad-1.2/setup.cfg
--rw-rw-rw-   0        0        0      548 2024-04-01 20:16:04.000000 sajjad-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.537597 sajjad-1.3/
+-rw-rw-rw-   0        0        0      441 2024-04-01 20:22:25.535596 sajjad-1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.519176 sajjad-1.3/sajjad/
+-rw-rw-rw-   0        0        0        0 2024-04-01 20:21:50.000000 sajjad-1.3/sajjad/__init__.py
+-rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.3/sajjad/sajjad.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.534625 sajjad-1.3/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:22:25.537597 sajjad-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      562 2024-04-01 20:21:06.000000 sajjad-1.3/setup.py
```

### Comparing `sajjad-1.2/setup.py` & `sajjad-1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='sajjad',
-    version='1.2',
-    py_modules=['sajjad'],
-    description='A simple python library',
+    version='1.3',
+    packages=find_packages(),
+    description='sajjad created that',
     author='sajjad seyedi',
     author_email='sajjad.seyedi.88@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
```

