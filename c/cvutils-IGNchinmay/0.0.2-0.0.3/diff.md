# Comparing `tmp/cvutils_IGNchinmay-0.0.2.tar.gz` & `tmp/cvutils_IGNchinmay-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvutils_IGNchinmay-0.0.2.tar", last modified: Mon Apr  1 07:18:06 2024, max compression
+gzip compressed data, was "cvutils_IGNchinmay-0.0.3.tar", last modified: Mon Apr  1 11:25:40 2024, max compression
```

## Comparing `cvutils_IGNchinmay-0.0.2.tar` & `cvutils_IGNchinmay-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,37 @@
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 07:18:06.163614 cvutils_IGNchinmay-0.0.2/
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    11357 2024-04-01 07:09:57.000000 cvutils_IGNchinmay-0.0.2/LICENSE.txt
--rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      855 2024-04-01 07:18:06.163614 cvutils_IGNchinmay-0.0.2/PKG-INFO
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       63 2024-04-01 07:16:41.000000 cvutils_IGNchinmay-0.0.2/README.md
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 07:18:06.163614 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      135 2024-04-01 06:48:03.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/__init__.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     9802 2024-04-01 06:47:18.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/draw_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3062 2024-03-26 11:13:44.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/json_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1756 2024-03-26 11:27:12.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/typehint_utils.py
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 07:18:06.163614 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/
--rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      855 2024-04-01 07:18:06.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/PKG-INFO
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      396 2024-04-01 07:18:06.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/SOURCES.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        1 2024-04-01 07:18:06.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/dependency_links.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      104 2024-04-01 07:18:06.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/requires.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       19 2024-04-01 07:18:06.000000 cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/top_level.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      730 2024-04-01 07:11:20.000000 cvutils_IGNchinmay-0.0.2/pyproject.toml
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      103 2024-04-01 07:08:07.000000 cvutils_IGNchinmay-0.0.2/requirements.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       38 2024-04-01 07:18:06.163614 cvutils_IGNchinmay-0.0.2/setup.cfg
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    11357 2024-04-01 07:09:57.000000 cvutils_IGNchinmay-0.0.3/LICENSE.txt
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1002 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       63 2024-04-01 07:16:41.000000 cvutils_IGNchinmay-0.0.3/README.md
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.893171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      763 2024-04-01 10:53:21.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    37749 2024-04-01 10:33:02.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/contour_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     9802 2024-04-01 06:47:18.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/draw_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    14245 2024-04-01 10:26:00.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/file_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4775 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/geom_utils.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    24718 2024-04-01 10:33:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/img_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3062 2024-03-26 11:13:44.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/json_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5694 2024-04-01 10:33:55.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/labelme_utils.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    20543 2024-04-01 10:26:11.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/mouse_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2094 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/multi_process_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12934 2024-04-01 10:54:37.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/show_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3232 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/system_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    19654 2024-04-01 10:30:03.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/transform_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1756 2024-03-26 11:27:12.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/typehint_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      811 2024-04-01 10:49:44.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2927 2024-04-01 10:24:45.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/dump_frames.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2616 2024-04-01 10:24:54.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/exif_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3760 2024-04-01 10:25:04.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/folder_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3305 2024-04-01 10:25:14.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/play_video.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12840 2024-04-01 10:25:24.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     8359 2024-04-01 10:25:35.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_sync.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4389 2024-04-01 10:25:46.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_writer.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1002 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1114 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        1 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      161 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/requires.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       19 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/top_level.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      730 2024-04-01 10:17:39.000000 cvutils_IGNchinmay-0.0.3/pyproject.toml
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      160 2024-04-01 11:00:55.000000 cvutils_IGNchinmay-0.0.3/requirements.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       38 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/setup.cfg
```

### Comparing `cvutils_IGNchinmay-0.0.2/LICENSE.txt` & `cvutils_IGNchinmay-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.2/PKG-INFO` & `cvutils_IGNchinmay-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: cvutils_IGNchinmay
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/jerinkantony/ignutils
 Project-URL: Issues, https://github.com/jerinkantony/ignutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: docker
+Requires-Dist: easyprocess
+Requires-Dist: fabulous
 Requires-Dist: imgaug
-Requires-Dist: numpy==1.23.0
+Requires-Dist: lsb_release_ex
 Requires-Dist: matplotlib
+Requires-Dist: numpy==1.23.0
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: pandas
+Requires-Dist: pynput
 Requires-Dist: scikit-image
+Requires-Dist: shapely
+Requires-Dist: sympy
 Requires-Dist: termcolor
 Requires-Dist: docker
 
 # cvutils
 Python package for reusable modules including AI, CV
```

### Comparing `cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/draw_utils.py` & `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/draw_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/json_utils.py` & `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay/typehint_utils.py` & `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/typehint_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.2/cvutils_IGNchinmay.egg-info/PKG-INFO` & `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: cvutils_IGNchinmay
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://github.com/jerinkantony/ignutils
 Project-URL: Issues, https://github.com/jerinkantony/ignutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: docker
+Requires-Dist: easyprocess
+Requires-Dist: fabulous
 Requires-Dist: imgaug
-Requires-Dist: numpy==1.23.0
+Requires-Dist: lsb_release_ex
 Requires-Dist: matplotlib
+Requires-Dist: numpy==1.23.0
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: Pillow
 Requires-Dist: pandas
+Requires-Dist: pynput
 Requires-Dist: scikit-image
+Requires-Dist: shapely
+Requires-Dist: sympy
 Requires-Dist: termcolor
 Requires-Dist: docker
 
 # cvutils
 Python package for reusable modules including AI, CV
```

### Comparing `cvutils_IGNchinmay-0.0.2/pyproject.toml` & `cvutils_IGNchinmay-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvutils_IGNchinmay"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

