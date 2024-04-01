# Comparing `tmp/large-image-source-rasterio-1.27.5.dev63.tar.gz` & `tmp/large-image-source-rasterio-1.27.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.27.5.dev63.tar", last modified: Mon Apr  1 15:31:41 2024, max compression
+gzip compressed data, was "large-image-source-rasterio-1.27.5.dev8.tar", last modified: Thu Mar 21 13:12:40 2024, max compression
```

## Comparing `large-image-source-rasterio-1.27.5.dev63.tar` & `large-image-source-rasterio-1.27.5.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:31:41.992834 large-image-source-rasterio-1.27.5.dev63/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      897 2024-04-01 15:31:41.992834 large-image-source-rasterio-1.27.5.dev63/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:31:41.988834 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43791 2024-04-01 15:27:06.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-04-01 15:27:06.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:31:41.992834 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      897 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      110 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-01 15:31:41.000000 large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-01 15:27:06.000000 large-image-source-rasterio-1.27.5.dev63/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-01 15:31:41.992834 large-image-source-rasterio-1.27.5.dev63/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-04-01 15:27:06.000000 large-image-source-rasterio-1.27.5.dev63/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:12:40.472526 large-image-source-rasterio-1.27.5.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      896 2024-03-21 13:12:40.472526 large-image-source-rasterio-1.27.5.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:12:40.468526 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43337 2024-03-21 13:08:10.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2024-03-21 13:08:10.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:12:40.472526 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      896 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-03-21 13:12:40.000000 large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-21 13:08:10.000000 large-image-source-rasterio-1.27.5.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-21 13:12:40.472526 large-image-source-rasterio-1.27.5.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2636 2024-03-21 13:08:10.000000 large-image-source-rasterio-1.27.5.dev8/setup.py
```

### Comparing `large-image-source-rasterio-1.27.5.dev63/LICENSE` & `large-image-source-rasterio-1.27.5.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev63/PKG-INFO` & `large-image-source-rasterio-1.27.5.dev8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.27.5.dev63/README.rst` & `large-image-source-rasterio-1.27.5.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from rasterio import warp
 from rasterio.enums import ColorInterp, Resampling
 from rasterio.errors import RasterioIOError
 
 import large_image
 from large_image.cache_util import LruCacheMetaclass, methodcache
 from large_image.constants import (TILE_FORMAT_IMAGE, TILE_FORMAT_NUMPY,
-                                   TILE_FORMAT_PIL, SourcePriority,
-                                   TileInputUnits, TileOutputMimeTypes)
+                                   TILE_FORMAT_PIL, TileInputUnits,
+                                   TileOutputMimeTypes)
 from large_image.exceptions import (TileSourceError,
                                     TileSourceFileNotFoundError,
                                     TileSourceInefficientError)
 from large_image.tilesource.geo import (GDALBaseFileTileSource,
                                         ProjUnitsAcrossLevel0,
                                         ProjUnitsAcrossLevel0_MaxSize)
 from large_image.tilesource.utilities import JSONDict
@@ -83,15 +83,14 @@
             which is the distance between (-180,0) and (180,0) in EPSG:4326 converted to the
             projection divided by the tile size. crs projections that are not latlong
             (is_geographic is False) must specify unitsPerPixel.
 
         """
         # init the object
         super().__init__(path, **kwargs)
-        self.addKnownExtensions()
 
         # create a thread lock
         self._getDatasetLock = threading.RLock()
 
         if isinstance(path, rio.io.MemoryFile):
             path = path.open(mode='r')
 
@@ -1028,25 +1027,14 @@
                 return False
         if ds.crs or (ds.transform and ds.transform != rio.Affine(1, 0, 0, 0, 1, 0)):
             return True
         if len(ds.gcps[0]) and ds.gcps[1]:
             return True
         return False
 
-    @classmethod
-    def addKnownExtensions(cls):
-        import rasterio.drivers
-
-        if not hasattr(cls, '_addedExtensions'):
-            cls._addedExtensions = True
-            cls.extensions = cls.extensions.copy()
-            for ext in rasterio.drivers.raster_driver_extensions():
-                if ext not in cls.extensions:
-                    cls.extensions[ext] = SourcePriority.IMPLICIT
-
 
 def open(*args, **kwargs):
     """Create an instance of the module class."""
     return RasterioFileTileSource(*args, **kwargs)
 
 
 def canRead(*args, **kwargs):
```

### Comparing `large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.27.5.dev63/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.27.5.dev8/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.27.5.dev63/setup.py` & `large-image-source-rasterio-1.27.5.dev8/setup.py`

 * *Files identical despite different names*

