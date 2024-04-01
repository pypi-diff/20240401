# Comparing `tmp/Dosepy-0.5.1.tar.gz` & `tmp/Dosepy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dosepy-0.5.1.tar", last modified: Thu Feb 22 04:28:44 2024, max compression
+gzip compressed data, was "Dosepy-0.6.0.tar", last modified: Mon Apr  1 02:12:41 2024, max compression
```

## Comparing `Dosepy-0.5.1.tar` & `Dosepy-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,66 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.759311 Dosepy-0.5.1/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1413 2023-10-19 15:53:23.000000 Dosepy-0.5.1/LICENSE
--rw-rw-r--   0 luis      (1000) luis      (1000)       40 2022-11-02 16:13:29.000000 Dosepy-0.5.1/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)    11247 2024-02-22 04:28:44.759311 Dosepy-0.5.1/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)    10254 2023-10-19 15:53:23.000000 Dosepy-0.5.1/README.md
--rw-rw-r--   0 luis      (1000) luis      (1000)     1392 2024-02-22 03:59:48.000000 Dosepy-0.5.1/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)       38 2024-02-22 04:28:44.759311 Dosepy-0.5.1/setup.cfg
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.751310 Dosepy-0.5.1/src/
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.755310 Dosepy-0.5.1/src/Dosepy/
--rw-rw-r--   0 luis      (1000) luis      (1000)    17582 2024-02-22 03:59:11.000000 Dosepy-0.5.1/src/Dosepy/GUI.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.755310 Dosepy-0.5.1/src/Dosepy/GUILayouts/
--rw-rw-r--   0 luis      (1000) luis      (1000)    12980 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/Bloque_Imagenes.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     7556 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/Bloque_gamma.py
--rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3037 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/about_window.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3457 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/cross_hair_cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      429 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    15578 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/film_to_doseGUI.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4576 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/licencia_window.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4783 2024-02-22 03:42:08.000000 Dosepy-0.5.1/src/Dosepy/GUILayouts/to_do_rendering.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.755310 Dosepy-0.5.1/src/Dosepy/Icon/
--rw-rw-r--   0 luis      (1000) luis      (1000)    14061 2022-11-02 16:13:30.000000 Dosepy-0.5.1/src/Dosepy/Icon/Logo_Dosepy.png
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.5.1/src/Dosepy/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    15468 2023-10-19 15:53:23.000000 Dosepy-0.5.1/src/Dosepy/dose.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.755310 Dosepy-0.5.1/src/Dosepy/scripts/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1034 2024-02-22 03:59:11.000000 Dosepy-0.5.1/src/Dosepy/scripts/test_tutorial.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.759311 Dosepy-0.5.1/src/Dosepy/tools/
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.5.1/src/Dosepy/tools/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3339 2024-02-22 03:59:11.000000 Dosepy-0.5.1/src/Dosepy/tools/calibration.py
--rwxrwxr-x   0 luis      (1000) luis      (1000)     4433 2023-10-19 15:53:23.000000 Dosepy-0.5.1/src/Dosepy/tools/film_to_dose.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     1039 2024-02-22 03:59:11.000000 Dosepy-0.5.1/src/Dosepy/tools/i_o.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    19865 2024-02-22 04:11:55.000000 Dosepy-0.5.1/src/Dosepy/tools/image.py
--rwxrwxr-x   0 luis      (1000) luis      (1000)     4183 2023-10-19 15:53:23.000000 Dosepy-0.5.1/src/Dosepy/tools/resol.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-22 04:28:44.759311 Dosepy-0.5.1/src/Dosepy.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)    11247 2024-02-22 04:28:44.000000 Dosepy-0.5.1/src/Dosepy.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      860 2024-02-22 04:28:44.000000 Dosepy-0.5.1/src/Dosepy.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2024-02-22 04:28:44.000000 Dosepy-0.5.1/src/Dosepy.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)      118 2024-02-22 04:28:44.000000 Dosepy-0.5.1/src/Dosepy.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        7 2024-02-22 04:28:44.000000 Dosepy-0.5.1/src/Dosepy.egg-info/top_level.txt
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.606345 Dosepy-0.6.0/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1413 2023-10-19 15:53:23.000000 Dosepy-0.6.0/LICENSE
+-rw-rw-r--   0 luis      (1000) luis      (1000)       59 2024-03-03 18:37:22.000000 Dosepy-0.6.0/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-04-01 02:12:41.606345 Dosepy-0.6.0/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2658 2024-03-30 15:51:07.000000 Dosepy-0.6.0/README.md
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1416 2024-03-30 13:48:49.000000 Dosepy-0.6.0/pyproject.toml
+-rw-rw-r--   0 luis      (1000) luis      (1000)       38 2024-04-01 02:12:41.606345 Dosepy-0.6.0/setup.cfg
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.594345 Dosepy-0.6.0/src/
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.594345 Dosepy-0.6.0/src/Dosepy/
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.598345 Dosepy-0.6.0/src/Dosepy/Icon/
+-rw-rw-r--   0 luis      (1000) luis      (1000)   568371 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/Icon/Icon.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)    14061 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/Icon/Logo_Dosepy.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)    13444 2023-10-19 15:53:23.000000 Dosepy-0.6.0/src/Dosepy/Icon/cut_icon.png
+-rwxrwxr-x   0 luis      (1000) luis      (1000)    11084 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/Icon/folder.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)     5824 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/Icon/save.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1474 2024-03-28 18:41:08.000000 Dosepy-0.6.0/src/Dosepy/app.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.598345 Dosepy-0.6.0/src/Dosepy/app_components/
+-rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/app_components/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3048 2024-03-05 23:50:08.000000 Dosepy-0.6.0/src/Dosepy/app_components/about_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/
+-rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3457 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      429 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4773 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/dp_multi_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3153 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/draggable rectangle.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      415 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/multi_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4825 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/to_do_rendering.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     5604 2024-03-01 23:24:27.000000 Dosepy-0.6.0/src/Dosepy/app_components/calibration_widget.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2074 2024-03-05 23:43:07.000000 Dosepy-0.6.0/src/Dosepy/app_components/file_dialog.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4587 2024-03-05 23:50:38.000000 Dosepy-0.6.0/src/Dosepy/app_components/licencia_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/app_components/styles/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      240 2024-02-28 23:03:41.000000 Dosepy-0.6.0/src/Dosepy/app_components/styles/styles.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3451 2024-03-02 19:52:33.000000 Dosepy-0.6.0/src/Dosepy/app_components/tiff2dose_widget.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     8674 2024-03-28 18:37:44.000000 Dosepy-0.6.0/src/Dosepy/app_controller.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2817 2024-03-28 17:23:41.000000 Dosepy-0.6.0/src/Dosepy/app_model.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3921 2024-03-03 16:45:32.000000 Dosepy-0.6.0/src/Dosepy/calibration.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/data/
+-rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/data/D_FILM.csv
+-rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/data/D_TPS.csv
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1873 2024-03-31 21:09:27.000000 Dosepy-0.6.0/src/Dosepy/i_o.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    37592 2024-04-01 02:12:01.000000 Dosepy-0.6.0/src/Dosepy/image.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/old/
+-rw-rw-r--   0 luis      (1000) luis      (1000)    17219 2024-03-23 13:31:52.000000 Dosepy-0.6.0/src/Dosepy/old/GUI.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/old/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    15468 2023-10-19 15:53:23.000000 Dosepy-0.6.0/src/Dosepy/old/dose.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/old/gui_components/
+-rw-rw-r--   0 luis      (1000) luis      (1000)    12983 2024-03-05 23:18:39.000000 Dosepy-0.6.0/src/Dosepy/old/gui_components/Bloque_Imagenes.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     7330 2024-03-05 23:21:07.000000 Dosepy-0.6.0/src/Dosepy/old/gui_components/Bloque_gamma.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3042 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/old/gui_components/about_window.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    15764 2024-03-29 16:11:58.000000 Dosepy-0.6.0/src/Dosepy/old/gui_components/film_to_doseGUI.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4581 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/old/gui_components/licencia_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.602345 Dosepy-0.6.0/src/Dosepy/scripts/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1034 2024-02-22 03:59:11.000000 Dosepy-0.6.0/src/Dosepy/scripts/test_tutorial.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.606345 Dosepy-0.6.0/src/Dosepy/tools/
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.0/src/Dosepy/tools/__init__.py
+-rwxrwxr-x   0 luis      (1000) luis      (1000)     4433 2023-10-19 15:53:23.000000 Dosepy-0.6.0/src/Dosepy/tools/film_to_dose.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.606345 Dosepy-0.6.0/src/Dosepy/tools/gui_widgets/
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2024-02-27 19:07:50.000000 Dosepy-0.6.0/src/Dosepy/tools/gui_widgets/__init__.py
+-rwxrwxr-x   0 luis      (1000) luis      (1000)     4243 2024-03-30 02:27:22.000000 Dosepy-0.6.0/src/Dosepy/tools/resol.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 02:12:41.606345 Dosepy-0.6.0/src/Dosepy.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-04-01 02:12:41.000000 Dosepy-0.6.0/src/Dosepy.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1769 2024-04-01 02:12:41.000000 Dosepy-0.6.0/src/Dosepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2024-04-01 02:12:41.000000 Dosepy-0.6.0/src/Dosepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)      133 2024-04-01 02:12:41.000000 Dosepy-0.6.0/src/Dosepy.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        7 2024-04-01 02:12:41.000000 Dosepy-0.6.0/src/Dosepy.egg-info/top_level.txt
```

### Comparing `Dosepy-0.5.1/LICENSE` & `Dosepy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/pyproject.toml` & `Dosepy-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Dosepy"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
-description = "Gamma analysis and film dosimetry for dose distributions in radiotherapy"
+description = "Film dosimetry and gamma analysis for dose distributions in radiotherapy"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
@@ -29,19 +29,20 @@
 dependencies = [
   "numpy >= 1.23.4",
   "pydicom >= 2.3.0",
   "matplotlib >= 3.6.1",
   "tifffile >= 2022.10.10",
   "scipy >= 1.9.3",
   "PyQt6 >= 6.5.1",
-  "relative_dose_1d >= 0.1.7"
+  "relative_dose_1d >= 0.1.7",
+  "PySide6 >= 6.6.1",
 ]
 [project.urls]
 homepage = "https://dosepy.readthedocs.io/en/latest/intro.html"
 repository = "https://pypi.org/project/Dosepy/"
 Bug-Tracker = "https://github.com/LuisOlivaresJ/Dosepy"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-dp_dep = ["*.csv", "*.png"]
+Dosepy = ["*.csv", "*.png"]
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/Bloque_Imagenes.py` & `Dosepy-0.6.0/src/Dosepy/old/gui_components/Bloque_Imagenes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 #   Importaciones
 
 #---------------------------------------------
 
 from matplotlib import patches
 from PyQt6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
 import sys
-import pkg_resources
+from importlib import resources
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import numpy as np
 #from PyQt5.QtGui import QIcon
-import Dosepy.dose as dp
+import Dosepy.old.dose as dp
 
 
 
 #%%
 #########################################################
 #---------------------------------------------
 
@@ -40,16 +40,16 @@
 
 
     def IniciarWidgets(self):
 
 #%%
         #   Widget para imagen de referencia
 
-        file_name_FILM = pkg_resources.resource_filename('Dosepy', 'data/D_FILM.csv')
-        file_name_TPS = pkg_resources.resource_filename('Dosepy', 'data/D_TPS.csv')
+        file_name_FILM = str(resources.files("Dosepy") / "data" / "D_FILM.csv")
+        file_name_TPS = str(resources.files("Dosepy") / "data" / "D_TPS.csv")
 
         self.D_ref = dp.from_csv(file_name_FILM, 1)
         self.D_eval = dp.from_csv(file_name_TPS, 1)
 
         self.Mpl_Izq = Qt_Figure_Imagen()
         self.Mpl_Der = Qt_Figure_Imagen()
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/Bloque_gamma.py` & `Dosepy-0.6.0/src/Dosepy/old/gui_components/Bloque_gamma.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import sys
 from matplotlib.backends.backend_qtagg import FigureCanvas
-from PyQt6.QtWidgets import QApplication, QWidget, QLabel, QPushButton, QFormLayout, QLineEdit, QHBoxLayout, QVBoxLayout, QMessageBox
-from PyQt6.QtWidgets import QFileDialog
+from PyQt6.QtWidgets import (
+    QApplication,
+    QWidget,
+    QLabel,
+    QPushButton,
+    QFormLayout,
+    QLineEdit,
+    QHBoxLayout,
+    QVBoxLayout,
+)
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QIcon
 from matplotlib.figure import Figure
 import numpy as np
-from Dosepy.GUILayouts.Bloque_Imagenes import Qt_Figure_Imagen
+from .Bloque_Imagenes import Qt_Figure_Imagen
+
 #from GUILayouts.Bloque_Imagenes import Qt_Figure_Imagen
-import pkg_resources
-import Dosepy.dose as dp
+from importlib import resources
+
+import Dosepy.old.dose as dp
 
 
 class Bloque_gamma(QWidget):
     """
     Permite mostrar los archivos a cargar, parámetros gamma y resultados.
     """
-    def __init__(self, Us):
+    def __init__(self):
         super().__init__()
-        self.Us = Us
-        self.iniciarUI()
+        self.setup()
 
-    def iniciarUI(self):
-        self.Widgets_Labels()
-        #self.show()
-
-    def Widgets_Labels(self):
+    def setup(self):
 
         # Crear botones para cargar archivos
         #folder_icon = QIcon("Icon/folder.png")
-        file_name_folder = pkg_resources.resource_filename('Dosepy', 'Icon/folder.png')
+        file_name_folder = str(resources.files("Dosepy") / "Icon" / "folder.png")
         folder_icon = QIcon(file_name_folder)
 
+
         self.Refer_button = QPushButton()
         self.Refer_button.setIcon(folder_icon)
         Refer_label = QLabel('D. de referencia')
 
 
         self.Eval_button = QPushButton()
         self.Eval_button.setEnabled(False)
@@ -113,32 +119,30 @@
         archivos_Pre_h_box.addWidget(Refer_label)
         archivos_Pre_h_box.addWidget(self.Refer_button)
 
         archivos_Post_h_box = QHBoxLayout()
         archivos_Post_h_box.addWidget(Eval_label)
         archivos_Post_h_box.addWidget(self.Eval_button)
 
-        if self.Us == 'P':
-            #   Crear FormLayout
-            Parametros_gamma_Layout = QFormLayout()
-            #Parametros_gamma_Layout.setLabelAlignment(Qt.AlignLeft)
-            Parametros_gamma_Layout.setFormAlignment(Qt.AlignmentFlag.AlignRight)
-            Parametros_gamma_Layout.addRow('Toler. en dosis [%]', self.Toler_dosis)
-            Parametros_gamma_Layout.addRow('Toler. en distancia [mm]', self.Toler_dist)
-            Parametros_gamma_Layout.addRow('Umbral de dosis [%]', self.Umbral_dosis)
+        #   Crear FormLayout
+        Parametros_gamma_Layout = QFormLayout()
+        #Parametros_gamma_Layout.setLabelAlignment(Qt.AlignLeft)
+        Parametros_gamma_Layout.setFormAlignment(Qt.AlignmentFlag.AlignRight)
+        Parametros_gamma_Layout.addRow('Toler. en dosis [%]', self.Toler_dosis)
+        Parametros_gamma_Layout.addRow('Toler. en distancia [mm]', self.Toler_dist)
+        Parametros_gamma_Layout.addRow('Umbral de dosis [%]', self.Umbral_dosis)
 
         #   Crear vertical Layout
 
         Padre_Info_V_Layout = QVBoxLayout()
         Padre_Info_V_Layout.addLayout(archivos_Pre_h_box)
         Padre_Info_V_Layout.addLayout(archivos_Post_h_box)
 
-        if self.Us == 'P':
-            Padre_Info_V_Layout.addLayout(Parametros_gamma_Layout)
-            Padre_Info_V_Layout.addStretch()
+        Padre_Info_V_Layout.addLayout(Parametros_gamma_Layout)
+        Padre_Info_V_Layout.addStretch()
         #Padre_Info_V_Layout.addWidget(self.Indice_gamma_maximo_Label)
         #Padre_Info_V_Layout.addWidget(self.Indice_gamma_mediana_Label)
         Padre_Info_V_Layout.addWidget(self.Calcular_Button)
         Padre_Info_V_Layout.addWidget(self.Indice_gamma_porcentaje_Label)
         Padre_Info_V_Layout.addWidget(self.Indice_gamma_promedio_Label)
 
         Padre_Hist_V_Layout = QVBoxLayout()
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/about_window.py` & `Dosepy-0.6.0/src/Dosepy/old/gui_components/about_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Físico Médico en Radioterapia, La Paz, Baja California Sur, México.
 
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 
 """
 
 import sys
-import pkg_resources
+from importlib import resources
 
 from PyQt6.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication
 from PyQt6.QtGui import QPixmap
 from PyQt6.QtCore import Qt
 
 
 class About_Window(QWidget):
@@ -31,15 +31,15 @@
         self.iniciar_ventana()
 
 
     def iniciar_ventana(self):
 
         layout_padre_V = QVBoxLayout()
 
-        file_name_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
+        file_name_logo = str(resources.files("Dosepy") / "Icon" / "Logo_Dosepy.png")
         logo = QPixmap(file_name_logo)
         #logo.scaled(0.5, 0.5) #Qt.KeepAspectRatio)
         label_logo = QLabel(self)
         label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_logo.setPixmap(logo)
         label_logo.setStyleSheet(
             "border-radius: 15px;" +
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/cross_hair_cursor.py` & `Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/film_to_doseGUI.py` & `Dosepy-0.6.0/src/Dosepy/old/gui_components/film_to_doseGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 
 """
 
 #---------------------------------------------
 #   Importaciones
 from Dosepy.tools.film_to_dose import calibracion, cubico
-from Dosepy.tools.resol import match_resolution
-#from ..tools.resol import match_resolution
+from Dosepy.tools.resol import equate_resolution
+#from ..tools.resol import equate_resolution
 
 from PyQt6.QtWidgets import QWidget, QVBoxLayout, QApplication, QHBoxLayout, QMessageBox, QMainWindow, QLabel, QPushButton, QFileDialog, QLayout, QCheckBox, QLineEdit, QFormLayout
 from PyQt6.QtGui import QIcon, QPixmap
 from PyQt6.QtCore import Qt
 
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import tifffile as tiff
 import numpy as np
-import pkg_resources
+from importlib import resources
 import sys
 import os
 
 #---------------------------------------------
 
 class Film_to_Dose_Window(QWidget):
     """
@@ -41,15 +41,15 @@
         self.setWindowTitle('Dosimetría con película')
 
         self.iniciarUI_calibracion()
 
 
     def iniciarUI_calibracion(self):
 
-        file_name_folder = pkg_resources.resource_filename('Dosepy', 'Icon/folder.png')
+        file_name_folder = str(resources.files("Dosepy") / "Icon" / "folder.png")
         folder_icon = QIcon(file_name_folder)
 
         layout_bisabuelo = QVBoxLayout()
 
         layout_abuelo = QHBoxLayout()
         layout_abuelo_2inf = QHBoxLayout()
 
@@ -81,15 +81,15 @@
 
         #   Widget para los perfiles
         self.Qt_Mpl_curva_calib = Qt_Figure_CurvaCalibracion()
 
         layout_abuelo.addWidget(self.Qt_Mpl_curva_calib.Qt_fig)
         layout_abuelo.addLayout(layout_padre_botones)
 
-        file_name_image_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
+        file_name_image_logo = str(resources.files("Dosepy") / "Icon" / "Logo_Dosepy.png")
         #file_name_image_logo = 'Logo_Dosepy.png'
         pixmap_logo = QPixmap(file_name_image_logo)
         self.label_logo = QLabel(self)
         self.label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         self.label_logo.setPixmap(pixmap_logo)
         self.Qt_Mpl_distribucion = Qt_Figure_Imagen()
 
@@ -286,15 +286,15 @@
 
             file_name_csv, _ = QFileDialog.getSaveFileName(self, "Guardar distribución de dosis", "", "*.csv")
             np.savetxt(file_name_csv, self.Dosis_FILM, fmt = '%.3f', delimiter = ',')
             print('Guardar csv')
 
     def reducir_tamano(self):
 
-        self.Dosis_FILM = match_resolution(self.Dosis_FILM, self.image_distr_resolucion_mm_punto, float(self.QLineEdit_resol.text()))
+        self.Dosis_FILM = equate_resolution(self.Dosis_FILM, self.image_distr_resolucion_mm_punto, float(self.QLineEdit_resol.text()))
         self.Qt_Mpl_distribucion.Img(self.Dosis_FILM)
         self.Qt_Mpl_distribucion.Colores(self.Dosis_FILM)
         self.Qt_Mpl_distribucion.fig.canvas.draw()
 
     def revisar_si_es_flotante(self):
 
         data = self.QLineEdit_resol.text()
@@ -315,15 +315,16 @@
 class Qt_Figure_CurvaCalibracion:
     """
     Clase para generar el widget que contendrá la curva de calibración
     """
 
     def __init__(self):
 
-        self.fig = Figure(figsize=(4.5,3), facecolor = 'whitesmoke', tight_layout = True)
+        #self.fig = Figure(figsize=(4.5,3), facecolor = 'whitesmoke', tight_layout = True)
+        self.fig = Figure(figsize=(4.5,3), facecolor = 'whitesmoke', layout="constrained")
         self.Qt_fig = FigureCanvas(self.fig)
 
         #   Axes para la imagen
         self.ax = self.fig.add_subplot(1, 1, 1)
         self.ax.set_title('Curva de calibración', fontsize = 12)
         #self.ax.set_title('Curva de calibración', fontsize = 14)
         self.ax.set_ylabel('Dosis [Gy]')
@@ -335,15 +336,16 @@
 class Qt_Figure_Imagen:
     """
     Clase para contener la distribución de dosis
     """
 
     def __init__(self):
         #self.fig = Figure(figsize=(4,3), tight_layout = True, facecolor = 'whitesmoke')
-        self.fig = Figure(figsize=(5.5,5), facecolor = 'whitesmoke', tight_layout = True)
+        #self.fig = Figure(figsize=(5.5,5), facecolor = 'whitesmoke', tight_layout = True)
+        self.fig = Figure(figsize=(5.5,5), facecolor = 'whitesmoke', layout="constrained")
         self.Qt_fig = FigureCanvas(self.fig)
 
         self.ax1 = self.fig.add_axes([0.08, 0.08, 0.75, 0.85])
         self.ax2 = self.fig.add_axes([0.85, 0.15, 0.04, 0.72])
         self.ax2.set_ylabel('Dosis [Gy]')
         self.ax2.yaxis.set_label_position("right")
         self.ax2.yaxis.tick_right()
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/licencia_window.py` & `Dosepy-0.6.0/src/Dosepy/old/gui_components/licencia_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Físico Médico en Radioterapia, La Paz, Baja California Sur, México.
 
     Derechos Reservados (c) Luis Alfonso Olivares Jimenez 2021
 
 """
 
 import sys
-import pkg_resources
+from importlib import resources
 
 from PyQt6.QtWidgets import QWidget, QLabel, QVBoxLayout, QHBoxLayout, QApplication, QPlainTextEdit
 from PyQt6.QtGui import QPixmap
 from PyQt6.QtCore import Qt
 
 
 class Licencia_Window(QWidget):
@@ -35,15 +35,15 @@
         self.iniciar_ventana()
 
 
     def iniciar_ventana(self):
 
         layout_padre_V = QVBoxLayout()
 
-        file_name_logo = pkg_resources.resource_filename('Dosepy', 'Icon/Logo_Dosepy.png')
+        file_name_logo = str(resources.files("Dosepy") / "Icon" / "Logo_Dosepy.png")
         logo = QPixmap(file_name_logo)
         #logo.scaled(0.5, 0.5) #Qt.KeepAspectRatio)
         label_logo = QLabel(self)
         label_logo.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         label_logo.setPixmap(logo)
         label_logo.setStyleSheet(
             "border-radius: 15px;" +
```

### Comparing `Dosepy-0.5.1/src/Dosepy/GUILayouts/to_do_rendering.py` & `Dosepy-0.6.0/src/Dosepy/app_components/blitting_examples/to_do_rendering.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
-from matplotlib.backends.qt_compat import QtWidgets
-from PyQt5.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
+#from matplotlib.backends.qt_compat import QtWidgets
+from PySide6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
+from matplotlib.backends.backend_qtagg import \
+	NavigationToolbar2QT as NavigationToolbar
 import sys
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import numpy as np
 import pkg_resources
 
@@ -15,28 +17,28 @@
 	"""
 	def __init__(self, ax):
 		self.ax = ax
 		self.background = None
 		self.horizontal_line = ax.axhline(color = 'cornflowerblue', lw = 1.5, ls = '--', alpha = 0.8)
 		self.vertical_line = ax.axvline(color = 'orange', lw = 1.5, ls = '--', alpha = 0.8)
 		# text location in axes coordinates
-		self.text = ax.text(0.65, 0.9, '', transform=ax.transAxes)
+		#self.text = ax.text(0.65, 0.9, '', transform=ax.transAxes)
 		self._creating_background = False
 		ax.figure.canvas.mpl_connect('draw_event', self.on_draw)
 
 	def on_draw(self, event):
 		#De utilidad si hay un cambio en el tamaño de la ventana
 		self.create_new_background()
 		print(event)
 
 	def set_cross_hair_visible(self, visible):
 		need_redraw = self.horizontal_line.get_visible() != visible
 		self.horizontal_line.set_visible(visible)
 		self.vertical_line.set_visible(visible)
-		self.text.set_visible(visible)
+		#self.text.set_visible(visible)
 		return need_redraw
 
 	def create_new_background(self):
 		if self._creating_background:
 			# discard calls triggered from within this function
 			return
 		self._creating_background = True
@@ -58,81 +60,96 @@
 				self.ax.figure.canvas.blit(self.ax.bbox)
 		else:
 			if event.inaxes != self.ax:	#Descartar evento fuera de Axes que contiene la imagen
 				return
 			self.set_cross_hair_visible(True)
 			# update the line positions
 			x, y = event.xdata, event.ydata
+			#dose = 
 
 			self.horizontal_line.set_ydata(y)
 			self.vertical_line.set_xdata(x)
-			self.text.set_text('x=%1.0f, y=%1.0f' % (x, y))
+			#self.text.set_text('x=%1.0f, y=%1.0f' % (x, y))
 			
 			self.ax.figure.canvas.restore_region(self.background)
 			self.ax.draw_artist(self.horizontal_line)
 			self.ax.draw_artist(self.vertical_line)
-			self.ax.draw_artist(self.text)
+			#self.ax.draw_artist(self.text)
 			self.ax.figure.canvas.blit(self.ax.bbox)
 
 
-class Bloque_Imagenes(QWidget):
+class QtImageWidget(QWidget):
 	def __init__(self):
-		super().__init__()  #   Llamar al constructor de QWidget
-		self.setStyleSheet("background-color: #1d1040;")
-		self.setWindowTitle('Acerca de')
+		super().__init__()  # Call QWidget constructor
+		self.setWindowTitle('Dose distribution')
 
 		file_name_FILM = pkg_resources.resource_filename('Dosepy', 'data/D_FILM.csv')
 		self.array_refer = np.genfromtxt(file_name_FILM, delimiter = ',')
         
-		self.main_label = QVBoxLayout()
+		self.main_layout = QVBoxLayout()
 		self.iniciarUI()
         
 	def iniciarUI(self):
 		
-		self.Mpl_Izq = Qt_Figure_Imagen()
-		self.Mpl_Izq.Img(self.array_refer)
-		self.Mpl_Izq.Colores(self.array_refer) 
-		self.blitted_cross_hair = BlittedCursorCrossHair(self.Mpl_Izq.ax1)
-		self.id_on_press_perfil = self.Mpl_Izq.Qt_fig.figure.canvas.mpl_connect('motion_notify_event', self.blitted_cross_hair.on_mouse_move)
-		self.main_label.addWidget(self.Mpl_Izq.Qt_fig)
-		self.setLayout(self.main_label)	
+		self.Mpl_Izq = Canvas()
+		self.Mpl_Izq.show_dist(self.array_refer)
+		self.Mpl_Izq.set_colorbar(self.array_refer) 
+		self.blitted_cross_hair = BlittedCursorCrossHair(self.Mpl_Izq.ax)
+		#self.id_on_press_perfil = self.Mpl_Izq.canvas.figure.canvas.mpl_connect('motion_notify_event', self.blitted_cross_hair.on_mouse_move)
+		self.id_on_press_perfil = self.Mpl_Izq.canvas.figure.canvas.mpl_connect('button_press_event', self.blitted_cross_hair.on_mouse_move)
+		self.main_layout.addWidget(NavigationToolbar(self.Mpl_Izq.canvas, self))
+		self.main_layout.addWidget(self.Mpl_Izq.canvas)
+		self.setLayout(self.main_layout)
             
-class Qt_Figure_Imagen:
-	"""
-	Clase para contener la distribución de dosis
+class Canvas:
+	"""Widget to show a dose distribution.
 	"""
 
 	def __init__(self):
-		self.fig = Figure(figsize=(3.8,3), facecolor = 'whitesmoke')
-		self.Qt_fig = FigureCanvas(self.fig)
-		
-		#The dimensions (left, bottom, width, height) of the new Axes. All quantities are in fractions of figure width and height.
-		self.ax1 = self.fig.add_axes([0.08, 0.08, 0.75, 0.85])
-		self.ax2 = self.fig.add_axes([0.85, 0.15, 0.04, 0.72])
+		fig = Figure(
+			layout='constrained')
+		self.ax = fig.add_subplot()
+		self.canvas = FigureCanvas(fig)
 		
-	def Img(self, np_I):
-		'''
-		Definir la imagen a partir de un array que se proporciona como argumento.
-		'''
-		self.npI = np_I
-		self.mplI = self.ax1.imshow(self.npI)
-		print(self.mplI)
+	def show_dist(self, array):
+		''' Show the dose distribution.
 
-	def Colores(self, npI_color_ref):
+		Parameters
+		----------
+		array : numpy.ndarray
+            The image represented as a numpy array.
 		'''
-		Definir el mapa de colores a utiliar. Como argumento se requiere de una imagen de referencia para elegui mapa.
-		Por lo general se utiliza la distribución calculada por el TPS.
+		self.npI = array
+		self.mplI = self.ax.imshow(self.npI)
+
+	def set_colorbar(self, npI_color_ref):
+		''' 
+		Set a colorbar. 
+		
+		Parameters
+		----------
+		array : numpy.ndarray
+			An array used as a reference to define dose boundaries.
 		'''
-		color_map = 'viridis'
+		color_map = 'nipy_spectral'
 		bounds = np.linspace(0, round(1.15 * np.percentile(npI_color_ref, 98)), 256)
 		norm = colors.BoundaryNorm(boundaries = bounds, ncolors = 256)
 		self.mplI.set_norm(norm)
 		self.mplI.set_cmap(color_map)
-		self.cbar = self.fig.colorbar(self.mplI, cax = self.ax2, orientation = 'vertical', shrink = 0.6, format = '%.1f')
+
+		self.cbar = self.canvas.figure.colorbar(
+			self.mplI,
+			ax = self.ax,
+			orientation = 'vertical',
+			format = '%.1f',
+			shrink = 0.8,
+			)
 
 
 if __name__ == '__main__':
     app = QApplication(sys.argv)
-    ventana_raiz = Bloque_Imagenes()
+
+    ventana_raiz = QtImageWidget()
     ventana_raiz.setGeometry(100, 150, 500, 350)
     ventana_raiz.show()
-    sys.exit(app.exec_())
+
+    sys.exit(app.exec())
```

### Comparing `Dosepy-0.5.1/src/Dosepy/Icon/Logo_Dosepy.png` & `Dosepy-0.6.0/src/Dosepy/Icon/Logo_Dosepy.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/src/Dosepy/dose.py` & `Dosepy-0.6.0/src/Dosepy/old/dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/src/Dosepy/scripts/test_tutorial.py` & `Dosepy-0.6.0/src/Dosepy/scripts/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/src/Dosepy/tools/calibration.py` & `Dosepy-0.6.0/src/Dosepy/calibration.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """Class used to represent a calibration curve.
 
         Attributes
         ----------
         y : list
             The doses values that were used to expose films for calibration.
         x : list
-            Optical density if "P3" fit function wll be used, or normalized pixel value
+            Optical density if "P3" fit function is used, or normalized pixel value
             for "RF" fit function.
         func : str
             The model function used for dose-film response relationship.
             "P3": Polynomial function of degree 3.
             "RF": Rational function.
         channel : str
             Color channel. "R": Red, "G": Green and "B": Blue.
@@ -53,24 +53,24 @@
             deviation errors on the parameters, use perr = np.sqrt(np.diag(pcov)).
         """
 
     def __init__(self, y: list, x: list, func: str = "P3", channel: str = "R"):
 
         self.doses = sorted(y)
 
-        if func == "P3":
+        if func in ["P3", "Polynomial"]:
             self.x = sorted(x)  # Film response.
-        elif func == "RF":
+        elif func in ["RF", "Rational"]:
             self.x = sorted(x, reverse=True)
 
         self.func = func
 
-        if self.func == "P3":
+        if self.func in ["P3", "Polynomial"]:
             self.popt, self.pcov = curve_fit(polynomial_g3, self.x, self.doses)
-        elif self.func == "RF":
+        elif self.func in ["RF", "Rational"]:
             self.popt, self.pcov = curve_fit(
                                             rational_func,
                                             self.x,
                                             self.doses,
                                             p0=[0.1, 200, 500]
                                             )
         else:
@@ -90,19 +90,36 @@
         kwargs
             kwargs passed to plt.plot()
         """
         if ax is None:
             fig, ax = plt.subplots()
 
         x = np.linspace(self.x[0], self.x[-1], 100)
-        if self.func == "P3":
+        if self.func in ["P3", "Polynomial"]:
             y = polynomial_g3(x, *self.popt)
             ax.set_xlabel("Optical density")
-        elif self.func == "RF":
+        elif self.func in ["RF", "Rational"]:
             y = rational_func(x, *self.popt)
-            ax.set_title("Normalized pixel value")
-        ax.plot(x, y, **kwargs)
-        ax.plot(self.x, self.doses, '*', **kwargs)
-        ax.set_ylabel("Dose")
+            ax.set_xlabel("Normalized pixel value")
+
+        if self.channel in ["R", "Red", "r", "red"]:
+            color = "red"
+        elif self.channel in ["G", "Green", "g", "green"]:
+            color = "green"
+        elif self.channel in ["B", "Blue", "b", "blue"]:
+            color = "blue"
+        elif self.channel in ["M", "Mean", "m", "mean"]:
+            color = "black"
+        
+        ax.plot(x, y, color = color, **kwargs)
+        ax.plot(
+            self.x,
+            self.doses,
+            color = color,
+            marker = '*',
+            linestyle = 'None',
+            **kwargs
+            )
+        ax.set_ylabel("Dose [Gy]")
         if show:
             plt.show()
         return ax
```

### Comparing `Dosepy-0.5.1/src/Dosepy/tools/film_to_dose.py` & `Dosepy-0.6.0/src/Dosepy/tools/film_to_dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.5.1/src/Dosepy/tools/resol.py` & `Dosepy-0.6.0/src/Dosepy/tools/resol.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # -*- coding: utf-8 -*-
 """
+NAME
+    Resolution function
+
+DESCRIPTION
+    Script to match the number of rows and columns between two arrays, based on physical resolution.
+
+"""
+
+"""
 @author:
     Luis Alfonso Olivares Jimenez
 
-	Script to match the number of rows and columns between two arrays, based on physical resolution.
+	
 """
 
 import numpy as np
 
 def _points_to_average(res_A, res_B, points):
 	"""
 	Function that allows to generate a list, where each element represents 
@@ -55,93 +64,88 @@
 			accumulated_residue += residue
 
 	if remaining_points > 0:
 		points_to_average_lista.append(remaining_points)
 
 	return points_to_average_lista
 
-def match_resolution(array, array_resolution, target_resolution):
+def equate_resolution(array, array_resolution, target_resolution):
 	"""
-	Reduces the arrya size so that its new spatial resolution equals a given one. 
+	Reduces the arrya size so that its new spatial resolution equals to a target resolution. 
 	The algorithm averages a number of points given by target_resolution // array_resolution.
 
 	Parameters
 	----------
 
 	array : ndarray
 		The array that is required to reduce its size.
 
 	array_resolution : float
 		Spatial resolution of the array, in millimeters per point.
 
 	target_resolution : float
-		Reference spatial resolution, in millimeters per point.
+		Target spatial resolution, in millimeters per point.
 		
 	Returns
 	-------
 
 	ndarray
-		Reduced size array
+		Array with a reduced size
 
 	Examples
 	--------
 	**Example 1**
 
 	Let A be an array of (100, 100) with a 0.1 mm/point spatial resolution, and B another 
 	array of (10, 10) with a 1 mm/point resolution. To perform an ponit-by-point comparison, we need a
-	new (10, 10) representative array of A:
+	new (10, 10) representative array of A::
 
-		import numpy as np
-
-		A = np.random.rand(100, 100)	# With an asossiated spatial resolution of 0.1 mm/point.
-
-		new_A = resol.match_resolution(A, 0.1, 1)
+	>>> import numpy as np
+	>>> A = np.random.rand(100, 100)  # With an asossiated spatial resolution of 0.1 mm/point.
+	>>> new_A = equate_resolution(A, 0.1, 1)
 	
 
 	**Example 2**
 
 	Let A and B be two arrays of size (2362 x 2362) and (256 x 256), with spatial resolution of 0.08467 mm/point and 0.78125 mm/point, respectively.
 
 	The physical dimension of array A is 200.06 mm
 	(2362 points * 0.08467 mm/point = 200.06 mm)
 	The spatial dimension of matrix B is 199.99 mm.
 	(256 points * 0.78125 mm/point = 199.99 mm)
 
 	To reduce the size of matrix A to be equal to the size of
-	matrix B, the match_resolution function is used:
-
-		import Dosepy.tools.resol as resol
-		import numpy as np
-
-		A = np.zeros( (2362, 2362) )
-
-		C = resol.match_resolution(A, 0.08467, 0.78125)
-		C.shape
-		(256, 256)
+	matrix B, the equate_resolution function is used as::
 
+	>>> import Dosepy.tools.resol as resol
+	>>> import numpy as np
+	>>> A = np.zeros( (2362, 2362) )
+	>>> C = equate_resolution(A, 0.08467, 0.78125)
+	>>> C.shape
+	>>> (256, 256)
 	"""
 
 	list_points_column = _points_to_average(array_resolution, target_resolution, array.shape[1])
 	list_points_row = _points_to_average(array_resolution, target_resolution, array.shape[0])
 	new_reduced_array = np.zeros( (len(list_points_row), len(list_points_column) ) )
-	f = 0		#Contador para número de fila
+	f = 0  # Row counter
 	for i in np.arange( len(list_points_row) ):
-		c = 0	#Contador para número de columna
+		c = 0  # Column counter
 		for j in np.arange( len(list_points_column) ):
-			DUMMY = array[ f : f + list_points_row[i], c : c + list_points_column[j] ]
-			new_reduced_array[i,j] = np.mean(DUMMY)
+			temporal = array[ f : f + list_points_row[i], c : c + list_points_column[j] ]
+			new_reduced_array[i,j] = np.mean(temporal)
 			c = c + list_points_column[j]
 		f = f + list_points_row[i]
 	return new_reduced_array
 
 
 
-def main():         # For testing
+def main():  # For testing
 	a = _points_to_average(6, 20, 13)
 	print(a)
 
 	A = np.zeros( (2362, 2362) )
-	C = match_resolution(A, 0.08467, 0.78125)
-	print(C.shape)	# Expected (256, 256)
+	C = equate_resolution(A, 0.08467, 0.78125)
+	print(C.shape)  # Expected (256, 256)
 
 if __name__ == "__main__":
 	main()
```

