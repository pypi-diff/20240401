# Comparing `tmp/python-return-youtube-dislike-1.1.4.tar.gz` & `tmp/python-return-youtube-dislike-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-return-youtube-dislike-1.1.4.tar", last modified: Sun Mar 31 04:31:58 2024, max compression
+gzip compressed data, was "python-return-youtube-dislike-1.1.5.tar", last modified: Mon Apr  1 21:24:55 2024, max compression
```

## Comparing `python-return-youtube-dislike-1.1.4.tar` & `python-return-youtube-dislike-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 04:31:58.869967 python-return-youtube-dislike-1.1.4/
--rw-rw-rw-   0        0        0     1093 2024-03-31 03:02:53.000000 python-return-youtube-dislike-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      708 2024-03-31 04:31:58.868281 python-return-youtube-dislike-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      101 2024-03-30 23:28:49.000000 python-return-youtube-dislike-1.1.4/README.md
--rw-rw-rw-   0        0        0      570 2024-03-31 04:31:44.000000 python-return-youtube-dislike-1.1.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-31 04:31:58.868281 python-return-youtube-dislike-1.1.4/python_return_youtube_dislike.egg-info/
--rw-rw-rw-   0        0        0      708 2024-03-31 04:31:58.000000 python-return-youtube-dislike-1.1.4/python_return_youtube_dislike.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-03-31 04:31:58.000000 python-return-youtube-dislike-1.1.4/python_return_youtube_dislike.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 04:31:58.000000 python-return-youtube-dislike-1.1.4/python_return_youtube_dislike.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-31 04:31:58.000000 python-return-youtube-dislike-1.1.4/python_return_youtube_dislike.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1646 2024-03-31 03:14:37.000000 python-return-youtube-dislike-1.1.4/pythonryd.py
--rw-rw-rw-   0        0        0       42 2024-03-31 04:31:58.869967 python-return-youtube-dislike-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      957 2024-03-31 04:31:10.000000 python-return-youtube-dislike-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 21:24:55.676788 python-return-youtube-dislike-1.1.5/
+-rw-rw-rw-   0        0        0     1093 2024-03-31 03:02:53.000000 python-return-youtube-dislike-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2719 2024-04-01 21:24:55.675788 python-return-youtube-dislike-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2114 2024-03-31 16:10:35.000000 python-return-youtube-dislike-1.1.5/README.md
+-rw-rw-rw-   0        0        0      570 2024-04-01 21:23:32.000000 python-return-youtube-dislike-1.1.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-01 21:24:55.674788 python-return-youtube-dislike-1.1.5/python_return_youtube_dislike.egg-info/
+-rw-rw-rw-   0        0        0     2719 2024-04-01 21:24:55.000000 python-return-youtube-dislike-1.1.5/python_return_youtube_dislike.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-01 21:24:55.000000 python-return-youtube-dislike-1.1.5/python_return_youtube_dislike.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 21:24:55.000000 python-return-youtube-dislike-1.1.5/python_return_youtube_dislike.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 21:24:55.000000 python-return-youtube-dislike-1.1.5/python_return_youtube_dislike.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1646 2024-03-31 03:14:37.000000 python-return-youtube-dislike-1.1.5/pythonryd.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 21:24:55.676788 python-return-youtube-dislike-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      957 2024-04-01 21:23:38.000000 python-return-youtube-dislike-1.1.5/setup.py
```

### Comparing `python-return-youtube-dislike-1.1.4/LICENSE` & `python-return-youtube-dislike-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-return-youtube-dislike-1.1.4/pyproject.toml` & `python-return-youtube-dislike-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-return-youtube-dislike"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Sean-e", email="seane410@gmail.com" },
 ]
 description = "A simple Python library to interact with the Return YouTube Dislike API"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `python-return-youtube-dislike-1.1.4/pythonryd.py` & `python-return-youtube-dislike-1.1.5/pythonryd.py`

 * *Files identical despite different names*

### Comparing `python-return-youtube-dislike-1.1.4/setup.py` & `python-return-youtube-dislike-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.3' 
+VERSION = '1.1.5' 
 DESCRIPTION = 'A simple Python library to interact with the Return YouTube Dislike API'
 LONG_DESCRIPTION = 'A simple Python library to interact with the Return YouTube Dislike API'
 
 # Setting up
 setup(
     name="pythonpyd", 
     version=VERSION,
```

