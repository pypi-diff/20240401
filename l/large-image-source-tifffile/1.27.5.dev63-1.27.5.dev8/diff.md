# Comparing `tmp/large-image-source-tifffile-1.27.5.dev63.tar.gz` & `tmp/large-image-source-tifffile-1.27.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.27.5.dev63.tar", last modified: Mon Apr  1 15:32:20 2024, max compression
+gzip compressed data, was "large-image-source-tifffile-1.27.5.dev8.tar", last modified: Thu Mar 21 13:13:20 2024, max compression
```

## Comparing `large-image-source-tifffile-1.27.5.dev63.tar` & `large-image-source-tifffile-1.27.5.dev8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:20.452978 large-image-source-tifffile-1.27.5.dev63/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2024-04-01 15:32:20.452978 large-image-source-tifffile-1.27.5.dev63/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:20.452978 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25085 2024-04-01 15:27:06.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-01 15:27:06.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-01 15:32:20.452978 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      100 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-01 15:32:20.000000 large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-01 15:27:06.000000 large-image-source-tifffile-1.27.5.dev63/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-01 15:32:20.456978 large-image-source-tifffile-1.27.5.dev63/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-01 15:27:06.000000 large-image-source-tifffile-1.27.5.dev63/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:20.508620 large-image-source-tifffile-1.27.5.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      876 2024-03-21 13:13:20.508620 large-image-source-tifffile-1.27.5.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:20.508620 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-03-21 13:08:10.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-03-21 13:08:10.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-21 13:13:20.508620 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      876 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-03-21 13:13:20.000000 large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-03-21 13:08:10.000000 large-image-source-tifffile-1.27.5.dev8/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-21 13:13:20.508620 large-image-source-tifffile-1.27.5.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-03-21 13:08:10.000000 large-image-source-tifffile-1.27.5.dev8/setup.py
```

### Comparing `large-image-source-tifffile-1.27.5.dev63/LICENSE` & `large-image-source-tifffile-1.27.5.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.27.5.dev63/PKG-INFO` & `large-image-source-tifffile-1.27.5.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.27.5.dev63/README.rst` & `large-image-source-tifffile-1.27.5.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         :param path: a filesystem path for the tile source.
         """
         super().__init__(path, **kwargs)
 
         self._largeImagePath = str(self._getLargeImagePath())
 
         _lazyImport()
-        self.addKnownExtensions()
         try:
             self._tf = tifffile.TiffFile(self._largeImagePath)
         except Exception:
             if not os.path.isfile(self._largeImagePath):
                 raise TileSourceFileNotFoundError(self._largeImagePath) from None
             msg = 'File cannot be opened via tifffile.'
             raise TileSourceError(msg)
@@ -555,24 +554,14 @@
             # rotate
             if baxis not in {'YXS', 'YX'}:
                 tile = np.moveaxis(
                     tile, [baxis.index(a) for a in 'YXS' if a in baxis], range(len(baxis)))
         return self._outputTile(tile, TILE_FORMAT_NUMPY, x, y, z,
                                 pilImageAllowed, numpyAllowed, **kwargs)
 
-    @classmethod
-    def addKnownExtensions(cls):
-        if not hasattr(cls, '_addedExtensions'):
-            _lazyImport()
-            cls._addedExtensions = True
-            cls.extensions = cls.extensions.copy()
-            for ext in tifffile.TIFF.FILE_EXTENSIONS:
-                if ext not in cls.extensions:
-                    cls.extensions[ext] = SourcePriority.IMPLICIT
-
 
 def open(*args, **kwargs):
     """
     Create an instance of the module class.
     """
     return TifffileFileTileSource(*args, **kwargs)
```

### Comparing `large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.27.5.dev63/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.27.5.dev8/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.27.5.dev63
+Version: 1.27.5.dev8
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-tifffile-1.27.5.dev63/setup.py` & `large-image-source-tifffile-1.27.5.dev8/setup.py`

 * *Files identical despite different names*

