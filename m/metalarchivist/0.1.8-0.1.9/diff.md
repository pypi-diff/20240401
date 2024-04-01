# Comparing `tmp/metalarchivist-0.1.8.tar.gz` & `tmp/metalarchivist-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.1.8.tar", last modified: Sat Nov 25 15:45:42 2023, max compression
+gzip compressed data, was "metalarchivist-0.1.9.tar", last modified: Sat Nov 25 16:46:12 2023, max compression
```

## Comparing `metalarchivist-0.1.8.tar` & `metalarchivist-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.267549 metalarchivist-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      651 2023-11-25 15:45:42.266548 metalarchivist-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-25 15:45:42.267549 metalarchivist-0.1.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.262549 metalarchivist-0.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.263549 metalarchivist-0.1.8/src/metalarchivist/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.265549 metalarchivist-0.1.8/src/metalarchivist/export/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/export/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6601 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/export/album.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.265549 metalarchivist-0.1.8/src/metalarchivist/interface/
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/interface/album.py
--rw-rw-rw-   0 root         (0) root         (0)    12838 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.266548 metalarchivist-0.1.8/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-11-25 15:45:42.000000 metalarchivist-0.1.8/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2023-11-25 15:45:42.000000 metalarchivist-0.1.8/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-25 15:45:42.000000 metalarchivist-0.1.8/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-11-25 15:45:42.000000 metalarchivist-0.1.8/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-11-25 15:45:42.000000 metalarchivist-0.1.8/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 15:45:42.266548 metalarchivist-0.1.8/src/test/
--rw-rw-rw-   0 root         (0) root         (0)     9712 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/test/test_albums.py
--rw-rw-rw-   0 root         (0) root         (0)     5963 2023-11-25 15:45:27.000000 metalarchivist-0.1.8/src/test/test_band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.957296 metalarchivist-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      693 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      674 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-25 16:46:12.957296 metalarchivist-0.1.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.952296 metalarchivist-0.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.953296 metalarchivist-0.1.9/src/metalarchivist/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.955296 metalarchivist-0.1.9/src/metalarchivist/export/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6601 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/album.py
+-rw-rw-rw-   0 root         (0) root         (0)     3716 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/metalarchivist/interface/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7054 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/album.py
+-rw-rw-rw-   0 root         (0) root         (0)    12838 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      674 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-11-25 16:46:12.000000 metalarchivist-0.1.9/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-25 16:46:12.956296 metalarchivist-0.1.9/src/test/
+-rw-rw-rw-   0 root         (0) root         (0)     9712 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/test/test_albums.py
+-rw-rw-rw-   0 root         (0) root         (0)     5963 2023-11-25 16:45:57.000000 metalarchivist-0.1.9/src/test/test_band.py
```

### Comparing `metalarchivist-0.1.8/LICENSE` & `metalarchivist-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/PKG-INFO` & `metalarchivist-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: lxml
+Requires-Dist: urllib3
 
 # MetalArchivist
 
 A Python package for extracting data from [Encyclopaedia Metallum](https://metal-archives.com)
```

### Comparing `metalarchivist-0.1.8/pyproject.toml` & `metalarchivist-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "metalarchivist"
-version = "0.1.8"
+version = "0.1.9"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
-dependencies = [ "rich", "lxml" ]
+dependencies = [ "rich", "lxml", "urllib3" ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `metalarchivist-0.1.8/src/metalarchivist/export/album.py` & `metalarchivist-0.1.9/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/metalarchivist/export/band.py` & `metalarchivist-0.1.9/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/metalarchivist/interface/album.py` & `metalarchivist-0.1.9/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/metalarchivist/interface/band.py` & `metalarchivist-0.1.9/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/metalarchivist/report.py` & `metalarchivist-0.1.9/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.1.9/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich
 Requires-Dist: lxml
+Requires-Dist: urllib3
 
 # MetalArchivist
 
 A Python package for extracting data from [Encyclopaedia Metallum](https://metal-archives.com)
```

### Comparing `metalarchivist-0.1.8/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.1.9/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/test/test_albums.py` & `metalarchivist-0.1.9/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.1.8/src/test/test_band.py` & `metalarchivist-0.1.9/src/test/test_band.py`

 * *Files identical despite different names*

