# Comparing `tmp/nellie-0.1.3.tar.gz` & `tmp/nellie-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nellie-0.1.3.tar", last modified: Sat Mar 23 03:57:40 2024, max compression
+gzip compressed data, was "nellie-0.1.4.tar", last modified: Mon Apr  1 17:26:18 2024, max compression
```

## Comparing `nellie-0.1.3.tar` & `nellie-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.995728 nellie-0.1.3/
--rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.3/LICENSE
--rw-r--r--   0 austin     (501) staff       (20)    11211 2024-03-23 03:57:40.995388 nellie-0.1.3/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.3/README.md
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.983506 nellie-0.1.3/nellie/
--rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.984995 nellie-0.1.3/nellie/feature_extraction/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/feature_extraction/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    54372 2024-03-23 03:46:37.000000 nellie-0.1.3/nellie/feature_extraction/hierarchical.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.985356 nellie-0.1.3/nellie/im_info/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/im_info/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    15773 2024-03-23 03:34:32.000000 nellie-0.1.3/nellie/im_info/im_info.py
--rw-r--r--   0 austin     (501) staff       (20)     1778 2024-03-23 03:17:20.000000 nellie-0.1.3/nellie/run.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.986502 nellie-0.1.3/nellie/segmentation/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/segmentation/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)    11578 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/segmentation/filtering.py
--rw-r--r--   0 austin     (501) staff       (20)     6487 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/segmentation/labelling.py
--rw-r--r--   0 austin     (501) staff       (20)     9709 2024-03-23 03:45:34.000000 nellie-0.1.3/nellie/segmentation/mocap_marking.py
--rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/segmentation/networking.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.987643 nellie-0.1.3/nellie/tracking/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/tracking/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     4743 2024-03-23 00:41:03.000000 nellie-0.1.3/nellie/tracking/all_tracks_for_label.py
--rw-r--r--   0 austin     (501) staff       (20)    11441 2024-03-23 03:00:09.000000 nellie-0.1.3/nellie/tracking/flow_interpolation.py
--rw-r--r--   0 austin     (501) staff       (20)    17974 2024-03-23 02:58:51.000000 nellie-0.1.3/nellie/tracking/hu_tracking.py
--rw-r--r--   0 austin     (501) staff       (20)    19639 2024-03-23 02:59:11.000000 nellie-0.1.3/nellie/tracking/voxel_reassignment.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.989004 nellie-0.1.3/nellie/utils/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/utils/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/utils/base_logger.py
--rw-r--r--   0 austin     (501) staff       (20)     1572 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/utils/general.py
--rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.3/nellie/utils/gpu_functions.py
--rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.3/nellie/utils/torch_xp.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.995042 nellie-0.1.3/nellie.egg-info/
--rw-r--r--   0 austin     (501) staff       (20)    11211 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/PKG-INFO
--rw-r--r--   0 austin     (501) staff       (20)     1253 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/SOURCES.txt
--rw-r--r--   0 austin     (501) staff       (20)        1 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/dependency_links.txt
--rw-r--r--   0 austin     (501) staff       (20)       53 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/entry_points.txt
--rw-r--r--   0 austin     (501) staff       (20)      121 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/requires.txt
--rw-r--r--   0 austin     (501) staff       (20)       27 2024-03-23 03:57:40.000000 nellie-0.1.3/nellie.egg-info/top_level.txt
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.991708 nellie-0.1.3/nellie_napari/
--rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.3/nellie_napari/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.3/nellie_napari/batch_mode.py
--rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.3/nellie_napari/home.py
--rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.3/nellie_napari/logo.png
--rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.3/nellie_napari/napari.yaml
--rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.3/nellie_napari/nellie_analysis.py
--rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.3/nellie_napari/nellie_fileselect.py
--rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.3/nellie_napari/nellie_loader.py
--rw-r--r--   0 austin     (501) staff       (20)    15621 2024-03-23 03:54:43.000000 nellie-0.1.3/nellie_napari/nellie_processor.py
--rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.3/nellie_napari/visualizer.py
--rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.3/pyproject.toml
--rw-r--r--   0 austin     (501) staff       (20)      816 2024-03-23 03:57:40.996079 nellie-0.1.3/setup.cfg
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.992204 nellie-0.1.3/tests/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/tests/__init__.py
-drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-03-23 03:57:40.994528 nellie-0.1.3/tests/unit/
--rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.3/tests/unit/__init__.py
--rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.3/tests/unit/test_frangi_filter.py
--rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.3/tests/unit/test_im_info.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.212382 nellie-0.1.4/
+-rw-r--r--   0 austin     (501) staff       (20)    18826 2024-03-19 19:14:37.000000 nellie-0.1.4/LICENSE
+-rw-r--r--   0 austin     (501) staff       (20)    11211 2024-04-01 17:26:18.212260 nellie-0.1.4/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)    10555 2024-03-23 00:41:03.000000 nellie-0.1.4/README.md
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.200919 nellie-0.1.4/nellie/
+-rw-r--r--   0 austin     (501) staff       (20)     1421 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.202123 nellie-0.1.4/nellie/feature_extraction/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/feature_extraction/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    54372 2024-04-01 16:16:45.000000 nellie-0.1.4/nellie/feature_extraction/hierarchical.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.202427 nellie-0.1.4/nellie/im_info/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/im_info/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    16095 2024-04-01 17:07:15.000000 nellie-0.1.4/nellie/im_info/im_info.py
+-rw-r--r--   0 austin     (501) staff       (20)     1774 2024-04-01 17:14:11.000000 nellie-0.1.4/nellie/run.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.203447 nellie-0.1.4/nellie/segmentation/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/segmentation/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)    11578 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/segmentation/filtering.py
+-rw-r--r--   0 austin     (501) staff       (20)     6487 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/segmentation/labelling.py
+-rw-r--r--   0 austin     (501) staff       (20)     9769 2024-04-01 16:59:42.000000 nellie-0.1.4/nellie/segmentation/mocap_marking.py
+-rw-r--r--   0 austin     (501) staff       (20)    16823 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/segmentation/networking.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.205248 nellie-0.1.4/nellie/tracking/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/tracking/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     4743 2024-03-23 00:41:03.000000 nellie-0.1.4/nellie/tracking/all_tracks_for_label.py
+-rw-r--r--   0 austin     (501) staff       (20)    11441 2024-04-01 16:16:45.000000 nellie-0.1.4/nellie/tracking/flow_interpolation.py
+-rw-r--r--   0 austin     (501) staff       (20)    17974 2024-04-01 16:16:45.000000 nellie-0.1.4/nellie/tracking/hu_tracking.py
+-rw-r--r--   0 austin     (501) staff       (20)    19639 2024-04-01 16:16:45.000000 nellie-0.1.4/nellie/tracking/voxel_reassignment.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.206595 nellie-0.1.4/nellie/utils/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/utils/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)      275 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/utils/base_logger.py
+-rw-r--r--   0 austin     (501) staff       (20)     1572 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/utils/general.py
+-rw-r--r--   0 austin     (501) staff       (20)     2594 2024-03-15 22:18:53.000000 nellie-0.1.4/nellie/utils/gpu_functions.py
+-rw-r--r--   0 austin     (501) staff       (20)     5892 2024-03-15 22:13:16.000000 nellie-0.1.4/nellie/utils/torch_xp.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.211918 nellie-0.1.4/nellie.egg-info/
+-rw-r--r--   0 austin     (501) staff       (20)    11211 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/PKG-INFO
+-rw-r--r--   0 austin     (501) staff       (20)     1253 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/SOURCES.txt
+-rw-r--r--   0 austin     (501) staff       (20)        1 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/dependency_links.txt
+-rw-r--r--   0 austin     (501) staff       (20)       53 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/entry_points.txt
+-rw-r--r--   0 austin     (501) staff       (20)      121 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/requires.txt
+-rw-r--r--   0 austin     (501) staff       (20)       27 2024-04-01 17:26:18.000000 nellie-0.1.4/nellie.egg-info/top_level.txt
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.210258 nellie-0.1.4/nellie_napari/
+-rw-r--r--   0 austin     (501) staff       (20)      112 2024-03-18 21:13:24.000000 nellie-0.1.4/nellie_napari/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)     8386 2024-03-19 15:37:36.000000 nellie-0.1.4/nellie_napari/batch_mode.py
+-rw-r--r--   0 austin     (501) staff       (20)     3595 2024-03-23 00:44:38.000000 nellie-0.1.4/nellie_napari/home.py
+-rw-r--r--   0 austin     (501) staff       (20)    89016 2024-03-19 16:27:20.000000 nellie-0.1.4/nellie_napari/logo.png
+-rw-r--r--   0 austin     (501) staff       (20)      218 2024-03-15 22:32:30.000000 nellie-0.1.4/nellie_napari/napari.yaml
+-rw-r--r--   0 austin     (501) staff       (20)    20913 2024-03-19 21:11:06.000000 nellie-0.1.4/nellie_napari/nellie_analysis.py
+-rw-r--r--   0 austin     (501) staff       (20)    16190 2024-03-19 18:53:00.000000 nellie-0.1.4/nellie_napari/nellie_fileselect.py
+-rw-r--r--   0 austin     (501) staff       (20)     2719 2024-03-19 01:57:46.000000 nellie-0.1.4/nellie_napari/nellie_loader.py
+-rw-r--r--   0 austin     (501) staff       (20)    15621 2024-04-01 16:16:45.000000 nellie-0.1.4/nellie_napari/nellie_processor.py
+-rw-r--r--   0 austin     (501) staff       (20)    12833 2024-03-19 16:50:50.000000 nellie-0.1.4/nellie_napari/visualizer.py
+-rw-r--r--   0 austin     (501) staff       (20)       90 2024-01-23 18:46:05.000000 nellie-0.1.4/pyproject.toml
+-rw-r--r--   0 austin     (501) staff       (20)      816 2024-04-01 17:26:18.212702 nellie-0.1.4/setup.cfg
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.210730 nellie-0.1.4/tests/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/tests/__init__.py
+drwxr-xr-x   0 austin     (501) staff       (20)        0 2024-04-01 17:26:18.211312 nellie-0.1.4/tests/unit/
+-rw-r--r--   0 austin     (501) staff       (20)        0 2024-03-15 22:13:16.000000 nellie-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0 austin     (501) staff       (20)        6 2024-03-15 22:13:16.000000 nellie-0.1.4/tests/unit/test_frangi_filter.py
+-rw-r--r--   0 austin     (501) staff       (20)     3310 2024-03-15 22:18:53.000000 nellie-0.1.4/tests/unit/test_im_info.py
```

### Comparing `nellie-0.1.3/LICENSE` & `nellie-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/PKG-INFO` & `nellie-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.3/README.md` & `nellie-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/__init__.py` & `nellie-0.1.4/nellie/__init__.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/feature_extraction/hierarchical.py` & `nellie-0.1.4/nellie/feature_extraction/hierarchical.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/im_info/im_info.py` & `nellie-0.1.4/nellie/im_info/im_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,72 +112,85 @@
         if 'Z' in self.axes and self.shape[self.axes.index('Z')] > 1:
             self.no_z = False
         if 'T' in self.axes and self.shape[self.axes.index('T')] > 1:
             self.no_t = False
         if 'C' in self.axes and self.shape[self.axes.index('C')] > 1:
             self.no_c = False
 
+    def _get_tif_tag_metadata(self, metadata):
+        tag_names = {tag_value.name: tag_code for tag_code, tag_value in metadata.items()}
+
+        if 'XResolution' in tag_names:
+            self.dim_sizes['X'] = metadata[tag_names['XResolution']].value[1] \
+                                  / metadata[tag_names['XResolution']].value[0]
+        else:
+            logger.warning('No XResolution tag found.')
+            self.dim_sizes['X'] = None
+
+        if 'YResolution' in tag_names:
+            self.dim_sizes['Y'] = metadata[tag_names['YResolution']].value[1] \
+                                  / metadata[tag_names['YResolution']].value[0]
+        else:
+            logger.warning('No YResolution tag found.')
+            self.dim_sizes['Y'] = None
+
+        if 'ResolutionUnit' in tag_names:
+            if metadata[tag_names['ResolutionUnit']].value == tifffile.TIFF.RESUNIT.CENTIMETER:
+                self.dim_sizes['X'] *= 1E-2 * 1E6
+                self.dim_sizes['Y'] *= 1E-2 * 1E6
+        if 'Z' in self.axes:
+            if 'ZResolution' in tag_names:
+                self.dim_sizes['Z'] = 1 / metadata[tag_names['ZResolution']].value[0]
+            else:
+                logger.warning('No ZResolution tag found.')
+                self.dim_sizes['Z'] = None
+        else:
+            logger.warning('No ZResolution tag found.')
+            self.dim_sizes['Z'] = None
+
+        if 'T' in self.axes:
+            if 'FrameRate' in tag_names:
+                self.dim_sizes['T'] = 1 / metadata[tag_names['FrameRate']].value[0]
+        else:
+            logger.warning('No FrameRate tag found.')
+            self.dim_sizes['T'] = None
+
+    def _get_imagej_metadata(self, metadata):
+        if 'physicalsizex' in metadata:
+            self.dim_sizes['X'] = metadata['physicalsizex']
+        if 'physicalsizey' in metadata:
+            self.dim_sizes['Y'] = metadata['physicalsizey']
+        if 'spacing' in metadata:
+            self.dim_sizes['Z'] = metadata['spacing']
+        if 'finterval' in metadata:
+            self.dim_sizes['T'] = metadata['finterval']
+
     def _set_dim_sizes(self):
         if self.dim_sizes is not None:
             return
         try:
             self.dim_sizes = {'X': None, 'Y': None, 'Z': None, 'T': None}
             if self.metadata_type == 'imagej':
-                if 'physicalsizex' in self.metadata:
-                    self.dim_sizes['X'] = self.metadata['physicalsizex']
-                if 'physicalsizey' in self.metadata:
-                    self.dim_sizes['Y'] = self.metadata['physicalsizey']
-                if 'spacing' in self.metadata:
-                    self.dim_sizes['Z'] = self.metadata['spacing']
-                if 'finterval' in self.metadata:
-                    self.dim_sizes['T'] = self.metadata['finterval']
+                self._get_imagej_metadata(self.metadata)
+
             elif self.metadata_type == 'ome':
                 self.dim_sizes['X'] = self.metadata.images[0].pixels.physical_size_x
                 self.dim_sizes['Y'] = self.metadata.images[0].pixels.physical_size_y
                 self.dim_sizes['Z'] = self.metadata.images[0].pixels.physical_size_z
                 self.dim_sizes['T'] = self.metadata.images[0].pixels.time_increment
-            elif self.metadata_type is None:
-                tag_names = {tag_value.name: tag_code for tag_code, tag_value in self.metadata.items()}
-
-                if 'XResolution' in tag_names:
-                    self.dim_sizes['X'] = self.metadata[tag_names['XResolution']].value[1] \
-                                          / self.metadata[tag_names['XResolution']].value[0]
-                else:
-                    logger.warning('No XResolution tag found.')
-                    self.dim_sizes['X'] = None
-
-                if 'YResolution' in tag_names:
-                    self.dim_sizes['Y'] = self.metadata[tag_names['YResolution']].value[1] \
-                                          / self.metadata[tag_names['YResolution']].value[0]
-                else:
-                    logger.warning('No YResolution tag found.')
-                    self.dim_sizes['Y'] = None
-
-                if 'ResolutionUnit' in tag_names:
-                    if self.metadata[tag_names['ResolutionUnit']].value == tifffile.TIFF.RESUNIT.CENTIMETER:
-                        self.dim_sizes['X'] *= 1E-2 * 1E6
-                        self.dim_sizes['Y'] *= 1E-2 * 1E6
-                if 'Z' in self.axes:
-                    if 'ZResolution' in tag_names:
-                        self.dim_sizes['Z'] = 1 / self.metadata[tag_names['ZResolution']].value[0]
-                    else:
-                        logger.warning('No ZResolution tag found.')
-                        self.dim_sizes['Z'] = None
-                else:
-                    logger.warning('No ZResolution tag found.')
-                    self.dim_sizes['Z'] = None
-
-                if 'T' in self.axes:
-                    if 'FrameRate' in tag_names:
-                        self.dim_sizes['T'] = 1 / self.metadata[tag_names['FrameRate']].value[0]
-                else:
-                    logger.warning('No FrameRate tag found.')
-                    self.dim_sizes['T'] = None
+            elif self.metadata_type == 'imagej_tif_tags':
+                self._get_tif_tag_metadata(self.metadata[1])
+                self._get_imagej_metadata(self.metadata[0])
+                logger.warning(f'File is an ImageJ type, but has weird metadata, '
+                               f'found dimension sizes: {self.dim_sizes}')
 
+            elif self.metadata_type is None:
+                self._get_tif_tag_metadata(self.metadata)
                 logger.warning(f'File is not an ImageJ or OME type, found dimension sizes: {self.dim_sizes}')
+
             elif self.metadata_type == 'nd2':
                 try:
                     timestamps = self.metadata.recorded_data['Time [s]']
                     self.dim_sizes['T'] = timestamps[-1] / len(timestamps)
                 except KeyError:
                     logger.warning('No time data found in ND2 file.')
                     self.dim_sizes['T'] = None
@@ -207,14 +220,17 @@
                 ome_xml = tifffile.tiffcomment(self.im_path)
                 ome = ome_types.from_xml(ome_xml, parser="lxml")
                 self.metadata = ome
                 self.metadata_type = 'ome'
             elif tif.is_imagej:
                 self.metadata = tif.imagej_metadata
                 self.metadata_type = 'imagej'
+                if 'physicalsizex' not in self.metadata:
+                    self.metadata_type = 'imagej_tif_tags'
+                    self.metadata = [self.metadata, tif.pages[0].tags._dict]
             else:
                 self.metadata = tif.pages[0].tags._dict
                 self.metadata_type = None
                 if 'C' in self.axes:
                     logger.error('Multichannel TIFF files must have ImageJ or OME metadata. Resubmit the'
                                  'file either with correct metadata or the single channel of interest.')
             if self.axes == '':
@@ -274,19 +290,19 @@
         axes = axes.replace('C', '') if 'C' in axes else axes
         if shape is None:
             shape = self.shape
         logger.debug(f'Saving axes as {axes}')
         if 'T' not in axes:
             axes = 'T' + axes
             self.axes = axes
-            if len(axes) != len(shape):
-                shape = (1,) + shape
-                self.shape = shape
-                if data is not None:
-                    data = np.expand_dims(data, axis=0)
+        if len(axes) != len(shape):
+            shape = (1,) + shape
+            self.shape = shape
+            if data is not None:
+                data = np.expand_dims(data, axis=0)
         if data is None:
             assert shape is not None
             tifffile.imwrite(
                 path_im, shape=shape, dtype=dtype, bigtiff=True, metadata={"axes": axes}
             )
         else:
             tifffile.imwrite(
```

### Comparing `nellie-0.1.3/nellie/run.py` & `nellie-0.1.4/nellie/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     hierarchy.run()
 
     return im_info
 
 
 if __name__ == "__main__":
     # Single file run
-    im_path = r"/Users/austin/Downloads/glu.ome.tiff"
+    im_path = r"/Users/austin/Downloads/test.tif"
     im_info = run(im_path, remove_edges=False, ch=0)
 
     # # Directory bactch run
     # import os
     # top_dir = r"D:\test_files\nellie_longer_smorgasbord"
     # ch = 0
     # num_t = None
```

### Comparing `nellie-0.1.3/nellie/segmentation/filtering.py` & `nellie-0.1.4/nellie/segmentation/filtering.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/segmentation/labelling.py` & `nellie-0.1.4/nellie/segmentation/labelling.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/segmentation/mocap_marking.py` & `nellie-0.1.4/nellie/segmentation/mocap_marking.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class Markers:
     def __init__(self, im_info: ImInfo, num_t=None,
                  min_radius_um=0.20, max_radius_um=1, use_im='distance', num_sigma=5):
         self.im_info = im_info
         self.num_t = num_t
-        if num_t is None: # and not self.im_info.no_t:
+        if self.im_info.no_t:
+            self.num_t = 1
+        elif num_t is None:  # and not self.im_info.no_t:
             self.num_t = im_info.shape[im_info.axes.index('T')]
         if not self.im_info.no_z:
             self.z_ratio = self.im_info.dim_sizes['Z'] / self.im_info.dim_sizes['X']
         self.min_radius_um = max(min_radius_um, self.im_info.dim_sizes['X'])
         self.max_radius_um = max_radius_um
 
         self.min_radius_px = self.min_radius_um / self.im_info.dim_sizes['X']
```

### Comparing `nellie-0.1.3/nellie/segmentation/networking.py` & `nellie-0.1.4/nellie/segmentation/networking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/tracking/all_tracks_for_label.py` & `nellie-0.1.4/nellie/tracking/all_tracks_for_label.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/tracking/flow_interpolation.py` & `nellie-0.1.4/nellie/tracking/flow_interpolation.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/tracking/hu_tracking.py` & `nellie-0.1.4/nellie/tracking/hu_tracking.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/tracking/voxel_reassignment.py` & `nellie-0.1.4/nellie/tracking/voxel_reassignment.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/utils/general.py` & `nellie-0.1.4/nellie/utils/general.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/utils/gpu_functions.py` & `nellie-0.1.4/nellie/utils/gpu_functions.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie/utils/torch_xp.py` & `nellie-0.1.4/nellie/utils/torch_xp.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie.egg-info/PKG-INFO` & `nellie-0.1.4/nellie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nellie
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 Home-page: https://github.com/aelefebv/nellie
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre+nellie@gmail.com
 Classifier: Framework :: napari
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `nellie-0.1.3/nellie.egg-info/SOURCES.txt` & `nellie-0.1.4/nellie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/batch_mode.py` & `nellie-0.1.4/nellie_napari/batch_mode.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/home.py` & `nellie-0.1.4/nellie_napari/home.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/logo.png` & `nellie-0.1.4/nellie_napari/logo.png`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/nellie_analysis.py` & `nellie-0.1.4/nellie_napari/nellie_analysis.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/nellie_fileselect.py` & `nellie-0.1.4/nellie_napari/nellie_fileselect.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/nellie_loader.py` & `nellie-0.1.4/nellie_napari/nellie_loader.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/nellie_processor.py` & `nellie-0.1.4/nellie_napari/nellie_processor.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/nellie_napari/visualizer.py` & `nellie-0.1.4/nellie_napari/visualizer.py`

 * *Files identical despite different names*

### Comparing `nellie-0.1.3/setup.cfg` & `nellie-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nellie
-version = 0.1.3
+version = 0.1.4
 description = Automated organelle segmentation, tracking, and hierarchical feature extraction in 2D/3D live-cell microscopy
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Austin E. Y. T. Lefebvre
 author_email = austin.e.lefebvre+nellie@gmail.com
 url = https://github.com/aelefebv/nellie
 classifiers =
```

### Comparing `nellie-0.1.3/tests/unit/test_im_info.py` & `nellie-0.1.4/tests/unit/test_im_info.py`

 * *Files identical despite different names*

