# Comparing `tmp/bota-4.0.8.tar.gz` & `tmp/bota-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bota-4.0.8.tar", last modified: Wed Mar 20 08:31:27 2024, max compression
+gzip compressed data, was "bota-4.0.9.tar", last modified: Wed Mar 20 08:37:09 2024, max compression
```

## Comparing `bota-4.0.8.tar` & `bota-4.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 08:31:27.239005 bota-4.0.8/
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 bota-4.0.8/LICENSE
--rw-rw-rw-   0        0        0     1352 2024-03-20 08:31:27.235992 bota-4.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-03-20 08:20:45.000000 bota-4.0.8/README.md
--rw-rw-rw-   0        0        0       86 2024-03-20 08:31:27.245667 bota-4.0.8/setup.cfg
--rw-rw-rw-   0        0        0     8371 2024-03-20 08:31:26.000000 bota-4.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:31:27.179552 bota-4.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-20 08:31:27.200800 bota-4.0.8/src/bota/
--rw-rw-rw-   0        0        0        0 2024-03-20 08:25:56.000000 bota-4.0.8/src/bota/__init__.py
--rw-rw-rw-   0        0        0    23901 2024-03-20 08:31:09.000000 bota-4.0.8/src/bota/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 08:31:27.234486 bota-4.0.8/src/bota.egg-info/
--rw-rw-rw-   0        0        0     1352 2024-03-20 08:31:26.000000 bota-4.0.8/src/bota.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-03-20 08:31:27.000000 bota-4.0.8/src/bota.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 08:31:26.000000 bota-4.0.8/src/bota.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-20 08:31:26.000000 bota-4.0.8/src/bota.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-20 08:31:26.000000 bota-4.0.8/src/bota.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-20 08:37:09.145220 bota-4.0.9/
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 bota-4.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1352 2024-03-20 08:37:09.145220 bota-4.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-03-20 08:20:45.000000 bota-4.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2024-03-20 08:37:09.151492 bota-4.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     8181 2024-03-20 08:37:08.000000 bota-4.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-20 08:37:09.110512 bota-4.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-03-20 08:37:09.122346 bota-4.0.9/src/bota/
+-rw-rw-rw-   0        0        0        0 2024-03-20 08:25:56.000000 bota-4.0.9/src/bota/__init__.py
+-rw-rw-rw-   0        0        0    23901 2024-03-20 08:31:09.000000 bota-4.0.9/src/bota/__main__.py
+drwxrwxrwx   0        0        0        0 2024-03-20 08:37:09.145220 bota-4.0.9/src/bota.egg-info/
+-rw-rw-rw-   0        0        0     1352 2024-03-20 08:37:08.000000 bota-4.0.9/src/bota.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-03-20 08:37:08.000000 bota-4.0.9/src/bota.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-20 08:37:08.000000 bota-4.0.9/src/bota.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-03-20 08:37:08.000000 bota-4.0.9/src/bota.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-20 08:37:08.000000 bota-4.0.9/src/bota.egg-info/top_level.txt
```

### Comparing `bota-4.0.8/LICENSE` & `bota-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bota-4.0.8/PKG-INFO` & `bota-4.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bota
-Version: 4.0.8
+Version: 4.0.9
 Summary: CLI for botasaurus.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Bug Reports, https://github.com/omkarcloud/botasaurus/issues
 Project-URL: Say Thanks!, https://github.com/omkarcloud/botasaurus
```

### Comparing `bota-4.0.8/setup.py` & `bota-4.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-
 
 __author__ = "Chetan Jain <chetan@omkar.cloud>"
 
-# Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
-
 
 install_requires = [
     "click",
 ]
 
 
 def get_description():
@@ -57,15 +49,15 @@
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
-    version='4.0.8',
+    version='4.0.9',
     author="Chetan Jain",
     author_email="chetan@omkar.cloud",
     description="CLI for botasaurus.",
     license="MIT",
     keywords=["seleniumwire proxy authentication", "proxy authentication"],
     url="https://github.com/omkarcloud/botasaurus-proxy-authentication",
     long_description_content_type="text/markdown",
```

### Comparing `bota-4.0.8/src/bota/__main__.py` & `bota-4.0.9/src/bota/__main__.py`

 * *Files identical despite different names*

### Comparing `bota-4.0.8/src/bota.egg-info/PKG-INFO` & `bota-4.0.9/src/bota.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bota
-Version: 4.0.8
+Version: 4.0.9
 Summary: CLI for botasaurus.
 Home-page: https://github.com/omkarcloud/botasaurus-proxy-authentication
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Bug Reports, https://github.com/omkarcloud/botasaurus/issues
 Project-URL: Say Thanks!, https://github.com/omkarcloud/botasaurus
```

