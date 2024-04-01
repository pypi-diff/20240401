# Comparing `tmp/better_bing_image_downloader-1.1.0.tar.gz` & `tmp/better_bing_image_downloader-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_bing_image_downloader-1.1.0.tar", last modified: Sat Mar  2 12:26:04 2024, max compression
+gzip compressed data, was "better_bing_image_downloader-1.1.1.tar", last modified: Mon Apr  1 16:25:55 2024, max compression
```

## Comparing `better_bing_image_downloader-1.1.0.tar` & `better_bing_image_downloader-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 krishnatejaswis  (1000) krishnatejaswis  (1001)        0 2024-03-02 12:26:04.262869 better_bing_image_downloader-1.1.0/
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     1073 2024-02-15 13:33:11.000000 better_bing_image_downloader-1.1.0/LICENSE
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     2941 2024-03-02 12:26:04.262869 better_bing_image_downloader-1.1.0/PKG-INFO
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     2375 2024-02-16 14:39:12.000000 better_bing_image_downloader-1.1.0/README.md
-drwxr-xr-x   0 krishnatejaswis  (1000) krishnatejaswis  (1001)        0 2024-03-02 12:26:04.262869 better_bing_image_downloader-1.1.0/better_bing_image_downloader/
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)       55 2024-02-16 14:36:31.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader/__init__.py
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     8684 2024-03-02 12:15:11.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader/bing.py
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     3820 2024-03-02 12:15:11.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader/download.py
-drwxr-xr-x   0 krishnatejaswis  (1000) krishnatejaswis  (1001)        0 2024-03-02 12:26:04.262869 better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)     2941 2024-03-02 12:26:04.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/PKG-INFO
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)      353 2024-03-02 12:26:04.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)        1 2024-03-02 12:26:04.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)       29 2024-03-02 12:26:04.000000 better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/top_level.txt
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)       38 2024-03-02 12:26:04.262869 better_bing_image_downloader-1.1.0/setup.cfg
--rw-r--r--   0 krishnatejaswis  (1000) krishnatejaswis  (1001)      806 2024-03-02 12:17:43.000000 better_bing_image_downloader-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.885739 better_bing_image_downloader-1.1.1/better_bing_image_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 16:25:55.000000 better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:55.889739 better_bing_image_downloader-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/tests/test_bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:25:51.000000 better_bing_image_downloader-1.1.1/tests/test_download.py
```

### Comparing `better_bing_image_downloader-1.1.0/LICENSE` & `better_bing_image_downloader-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `better_bing_image_downloader-1.1.0/PKG-INFO` & `better_bing_image_downloader-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better_bing_image_downloader
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package is built on top of bing-image-downloader by gaurav singh
 Home-page: https://github.com/KTS-o7/better_bing_image_downloader
 Author: Krishnatejaswi S
 Author-email: shentharkrishnatejaswi@gmail.com
 Keywords: bing,images,scraping,image download,bulk image downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,16 @@
 ![GitHub](https://img.shields.io/github/license/KTS-o7/better-bing-image-downloader)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FKTS-o7%2Fbetter_bing_image_downloader&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 ### Installation <br />
 
 ```bash
 git clone https://github.com/KTS-o7better_bing_image_downloader
+python -m venv ./env
+source env/bin/activate
 cd better_bing_image_downloader
 pip install .
 ```
 
 or
 
 ```bash
```

### Comparing `better_bing_image_downloader-1.1.0/README.md` & `better_bing_image_downloader-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ![GitHub](https://img.shields.io/github/license/KTS-o7/better-bing-image-downloader)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FKTS-o7%2Fbetter_bing_image_downloader&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 ### Installation <br />
 
 ```bash
 git clone https://github.com/KTS-o7better_bing_image_downloader
+python -m venv ./env
+source env/bin/activate
 cd better_bing_image_downloader
 pip install .
 ```
 
 or
 
 ```bash
```

### Comparing `better_bing_image_downloader-1.1.0/better_bing_image_downloader/bing.py` & `better_bing_image_downloader-1.1.1/better_bing_image_downloader/bing.py`

 * *Files identical despite different names*

### Comparing `better_bing_image_downloader-1.1.0/better_bing_image_downloader/download.py` & `better_bing_image_downloader-1.1.1/better_bing_image_downloader/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import shutil
 import argparse
 import logging
 from pathlib import Path
-from bing import Bing
+from .bing import Bing
 from tqdm import tqdm
 from math import ceil
 
 
 def downloader(query, limit=100, output_dir='dataset', adult_filter_off=True,
             force_replace=False, timeout=60, filter="", verbose=True, badsites=[], name='Image'):
     """
```

### Comparing `better_bing_image_downloader-1.1.0/better_bing_image_downloader.egg-info/PKG-INFO` & `better_bing_image_downloader-1.1.1/better_bing_image_downloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: better-bing-image-downloader
-Version: 1.1.0
+Name: better_bing_image_downloader
+Version: 1.1.1
 Summary: This package is built on top of bing-image-downloader by gaurav singh
 Home-page: https://github.com/KTS-o7/better_bing_image_downloader
 Author: Krishnatejaswi S
 Author-email: shentharkrishnatejaswi@gmail.com
 Keywords: bing,images,scraping,image download,bulk image downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -31,14 +31,16 @@
 ![GitHub](https://img.shields.io/github/license/KTS-o7/better-bing-image-downloader)
 [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FKTS-o7%2Fbetter_bing_image_downloader&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 ### Installation <br />
 
 ```bash
 git clone https://github.com/KTS-o7better_bing_image_downloader
+python -m venv ./env
+source env/bin/activate
 cd better_bing_image_downloader
 pip install .
 ```
 
 or
 
 ```bash
```

### Comparing `better_bing_image_downloader-1.1.0/setup.py` & `better_bing_image_downloader-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="better_bing_image_downloader",
-    version="1.1.0",
+    version="1.1.1",
     author="Krishnatejaswi S",
     author_email="shentharkrishnatejaswi@gmail.com",
     description="This package is built on top of bing-image-downloader by gaurav singh",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KTS-o7/better_bing_image_downloader",
     keywords=['bing', 'images', 'scraping', 'image download', 'bulk image downloader',],
```

