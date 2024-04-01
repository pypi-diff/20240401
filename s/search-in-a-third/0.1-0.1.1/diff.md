# Comparing `tmp/search_in_a_third-0.1.tar.gz` & `tmp/search_in_a_third-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search_in_a_third-0.1.tar", last modified: Sat Mar 30 21:32:38 2024, max compression
+gzip compressed data, was "search_in_a_third-0.1.1.tar", last modified: Mon Apr  1 10:37:50 2024, max compression
```

## Comparing `search_in_a_third-0.1.tar` & `search_in_a_third-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 21:32:38.356880 search_in_a_third-0.1/
--rw-rw-rw-   0        0        0     1922 2024-03-30 21:32:38.353330 search_in_a_third-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1136 2024-03-30 21:17:13.000000 search_in_a_third-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 21:32:38.215444 search_in_a_third-0.1/search_in_a_third/
--rw-rw-rw-   0        0        0        0 2024-03-30 21:22:12.000000 search_in_a_third-0.1/search_in_a_third/__init__.py
--rw-rw-rw-   0        0        0    33957 2024-03-29 17:57:50.000000 search_in_a_third-0.1/search_in_a_third/search_in_a_third.py
-drwxrwxrwx   0        0        0        0 2024-03-30 21:32:38.349485 search_in_a_third-0.1/search_in_a_third.egg-info/
--rw-rw-rw-   0        0        0     1922 2024-03-30 21:32:37.000000 search_in_a_third-0.1/search_in_a_third.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-03-30 21:32:38.000000 search_in_a_third-0.1/search_in_a_third.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 21:32:38.000000 search_in_a_third-0.1/search_in_a_third.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-03-30 21:32:38.000000 search_in_a_third-0.1/search_in_a_third.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-30 21:32:38.000000 search_in_a_third-0.1/search_in_a_third.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 21:32:38.357903 search_in_a_third-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1112 2024-03-30 21:19:31.000000 search_in_a_third-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:37:50.350025 search_in_a_third-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2024-03-30 21:51:38.000000 search_in_a_third-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     6646 2024-04-01 10:37:50.349049 search_in_a_third-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5827 2024-04-01 09:20:15.000000 search_in_a_third-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 10:37:50.320548 search_in_a_third-0.1.1/search_in_a_third/
+-rw-rw-rw-   0        0        0        0 2024-03-30 21:43:13.000000 search_in_a_third-0.1.1/search_in_a_third/__init__.py
+-rw-rw-rw-   0        0        0    33957 2024-03-30 21:43:13.000000 search_in_a_third-0.1.1/search_in_a_third/search_in_a_third.py
+drwxrwxrwx   0        0        0        0 2024-04-01 10:37:50.346997 search_in_a_third-0.1.1/search_in_a_third.egg-info/
+-rw-rw-rw-   0        0        0     6646 2024-04-01 10:37:50.000000 search_in_a_third-0.1.1/search_in_a_third.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-04-01 10:37:50.000000 search_in_a_third-0.1.1/search_in_a_third.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 10:37:50.000000 search_in_a_third-0.1.1/search_in_a_third.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-01 10:37:50.000000 search_in_a_third-0.1.1/search_in_a_third.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-01 10:37:50.000000 search_in_a_third-0.1.1/search_in_a_third.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 10:37:50.350025 search_in_a_third-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2024-04-01 10:26:50.000000 search_in_a_third-0.1.1/setup.py
```

### Comparing `search_in_a_third-0.1/search_in_a_third/search_in_a_third.py` & `search_in_a_third-0.1.1/search_in_a_third/search_in_a_third.py`

 * *Files identical despite different names*

### Comparing `search_in_a_third-0.1/setup.py` & `search_in_a_third-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Función para leer las dependencias de requirements.txt
 def read_requirements():
     with open('requirements.txt') as req:
         return req.read().splitlines()
 
 setup(
     name='search_in_a_third',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     description='A Python package for efficient hyperparameter optimization in neural networks, using a greedy algorithm guided by heuristic directions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Diego Larriera',
     author_email='proflarriera@gmail.com',
     url='https://github.com/proflarriera/searchinathird',
```

