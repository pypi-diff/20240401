# Comparing `tmp/large-image-source-vips-1.27.5.dev63.tar.gz` & `tmp/large-image-source-vips-1.27.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.27.5.dev63.tar", last modified: Mon Apr  1 15:32:32 2024, max compression
+gzip compressed data, was "large-image-source-vips-1.27.5.dev8.tar", last modified: Thu Mar 21 13:13:33 2024, max compression
```

## Comparing `large-image-source-vips-1.27.5.dev63.tar` & `large-image-source-vips-1.27.5.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:32.313023 large-image-source-vips-1.27.5.dev63/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2024-04-01 15:32:32.313023 large-image-source-vips-1.27.5.dev63/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:32.309023 large-image-source-vips-1.27.5.dev63/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25419 2024-04-01 15:27:06.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-04-01 15:27:06.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:32.313023 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-01 15:32:32.000000 large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-01 15:27:06.000000 large-image-source-vips-1.27.5.dev63/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-01 15:32:32.313023 large-image-source-vips-1.27.5.dev63/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-04-01 15:27:06.000000 large-image-source-vips-1.27.5.dev63/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:33.288645 large-image-source-vips-1.27.5.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-03-21 13:13:32.000000 large-image-source-vips-1.27.5.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-03-21 13:13:33.288645 large-image-source-vips-1.27.5.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-03-21 13:13:32.000000 large-image-source-vips-1.27.5.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:33.284645 large-image-source-vips-1.27.5.dev8/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24947 2024-03-21 13:08:10.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2024-03-21 13:08:10.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:33.284645 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-03-21 13:13:33.000000 large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-21 13:08:10.000000 large-image-source-vips-1.27.5.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-21 13:13:33.288645 large-image-source-vips-1.27.5.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2024-03-21 13:08:10.000000 large-image-source-vips-1.27.5.dev8/setup.py
```

### Comparing `large-image-source-vips-1.27.5.dev63/LICENSE` & `large-image-source-vips-1.27.5.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.27.5.dev63/PKG-INFO` & `large-image-source-vips-1.27.5.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.27.5.dev63/README.rst` & `large-image-source-vips-1.27.5.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.27.5.dev63/large_image_source_vips/__init__.py` & `large-image-source-vips-1.27.5.dev8/large_image_source_vips/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,25 @@
     name = 'vips'
     extensions = {
         None: SourcePriority.LOW,
     }
     mimeTypes = {
         None: SourcePriority.FALLBACK,
     }
-    newPriority = SourcePriority.MEDIUM
 
     _tileSize = 256
 
     def __init__(self, path, **kwargs):
         """
         Initialize the tile class.  See the base class for other available
         parameters.
 
         :param path: a filesystem path for the tile source.
         """
         super().__init__(path, **kwargs)
-        self.addKnownExtensions()
 
         if str(path).startswith(NEW_IMAGE_PATH_FLAG):
             self._initNew(**kwargs)
             return
         self._largeImagePath = str(self._getLargeImagePath())
         self._editable = False
 
@@ -608,24 +606,14 @@
     @property
     def origin(self):
         if not self._editable:
             return {'x': 0, 'y': 0}
         return {'x': min(0, self._output['minx'] or 0),
                 'y': min(0, self._output['miny'] or 0)}
 
-    @classmethod
-    def addKnownExtensions(cls):
-        if not hasattr(cls, '_addedExtensions'):
-            cls._addedExtensions = True
-            cls.extensions = cls.extensions.copy()
-            for dotext in pyvips.base.get_suffixes():
-                ext = dotext.lstrip('.')
-                if ext not in cls.extensions:
-                    cls.extensions[ext] = SourcePriority.IMPLICIT
-
 
 def open(*args, **kwargs):
     """Create an instance of the module class."""
     return VipsFileTileSource(*args, **kwargs)
 
 
 def canRead(*args, **kwargs):
```

### Comparing `large-image-source-vips-1.27.5.dev63/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.27.5.dev8/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.27.5.dev63/setup.py` & `large-image-source-vips-1.27.5.dev8/setup.py`

 * *Files identical despite different names*

