# Comparing `tmp/large-image-source-multi-1.27.5.dev63.tar.gz` & `tmp/large-image-source-multi-1.27.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.27.5.dev63.tar", last modified: Mon Apr  1 15:30:09 2024, max compression
+gzip compressed data, was "large-image-source-multi-1.27.5.dev8.tar", last modified: Thu Mar 21 13:11:13 2024, max compression
```

## Comparing `large-image-source-multi-1.27.5.dev63.tar` & `large-image-source-multi-1.27.5.dev8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-04-01 15:27:06.000000 large-image-source-multi-1.27.5.dev63/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54069 2024-04-01 15:27:06.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-01 15:27:06.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-01 15:30:09.000000 large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-01 15:27:06.000000 large-image-source-multi-1.27.5.dev63/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-01 15:30:09.504470 large-image-source-multi-1.27.5.dev63/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-04-01 15:27:06.000000 large-image-source-multi-1.27.5.dev63/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      937 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-03-21 13:08:10.000000 large-image-source-multi-1.27.5.dev8/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54069 2024-03-21 13:08:10.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-03-21 13:08:10.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      937 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-03-21 13:11:13.000000 large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-21 13:08:10.000000 large-image-source-multi-1.27.5.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-21 13:11:13.852408 large-image-source-multi-1.27.5.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-03-21 13:08:10.000000 large-image-source-multi-1.27.5.dev8/setup.py
```

### Comparing `large-image-source-multi-1.27.5.dev63/LICENSE` & `large-image-source-multi-1.27.5.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.27.5.dev63/PKG-INFO` & `large-image-source-multi-1.27.5.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.27.5.dev63/README.rst` & `large-image-source-multi-1.27.5.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.27.5.dev63/docs/specification.rst` & `large-image-source-multi-1.27.5.dev8/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.27.5.dev63/large_image_source_multi/__init__.py` & `large-image-source-multi-1.27.5.dev8/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.27.5.dev63/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.27.5.dev8/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.27.5.dev63/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.27.5.dev8/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.27.5.dev63/setup.py` & `large-image-source-multi-1.27.5.dev8/setup.py`

 * *Files identical despite different names*

