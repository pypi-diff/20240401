# Comparing `tmp/MacroQueue-0.2.2.tar.gz` & `tmp/MacroQueue-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MacroQueue-0.2.2.tar", last modified: Mon Apr  1 17:01:26 2024, max compression
+gzip compressed data, was "MacroQueue-0.2.3.tar", last modified: Mon Apr  1 17:07:35 2024, max compression
```

## Comparing `MacroQueue-0.2.2.tar` & `MacroQueue-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.201068 MacroQueue-0.2.2/
--rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.2.2/LICENSE.md
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.057242 MacroQueue-0.2.2/MacroQueue/
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.145527 MacroQueue-0.2.2/MacroQueue/Bitmaps/
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.2.2/MacroQueue/Bitmaps/DownArrow.bmp
--rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.2.2/MacroQueue/Bitmaps/Remove.bmp
--rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.2.2/MacroQueue/Bitmaps/UpArrow.bmp
--rw-rw-rw-   0        0        0    68756 2024-03-27 14:08:48.000000 MacroQueue-0.2.2/MacroQueue/Dialogs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.176880 MacroQueue-0.2.2/MacroQueue/Functions/
--rw-rw-rw-   0        0        0     1043 2024-01-11 19:05:47.000000 MacroQueue-0.2.2/MacroQueue/Functions/BField.py
--rw-rw-rw-   0        0        0    21517 2024-04-01 13:25:42.000000 MacroQueue-0.2.2/MacroQueue/Functions/CreaTec.py
--rw-rw-rw-   0        0        0     1517 2024-03-27 16:22:52.000000 MacroQueue-0.2.2/MacroQueue/Functions/General.py
--rw-rw-rw-   0        0        0     1656 2024-03-25 14:52:53.000000 MacroQueue-0.2.2/MacroQueue/Functions/RF.py
--rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.2.2/MacroQueue/Functions/RHK.py
--rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.2.2/MacroQueue/Functions/SXM.py
--rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.2.2/MacroQueue/Functions/SXMRemote.py
--rw-rw-rw-   0        0        0    24521 2024-03-21 18:30:14.000000 MacroQueue-0.2.2/MacroQueue/GUIDesign.py
--rw-rw-rw-   0        0        0    54897 2024-04-01 15:32:11.000000 MacroQueue-0.2.2/MacroQueue/MacroQueue.py
--rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.2.2/MacroQueue/MacroQueueIcon.ico
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.185793 MacroQueue-0.2.2/MacroQueue/Macros/
--rw-rw-rw-   0        0        0    13972 2024-03-27 16:23:14.000000 MacroQueue-0.2.2/MacroQueue/Macros/CreaTecMacro.json
--rw-rw-rw-   0        0        0     7924 2022-06-13 16:55:53.000000 MacroQueue-0.2.2/MacroQueue/Macros/RHKMacro.json
--rw-rw-rw-   0        0        0      539 2024-04-01 15:21:24.000000 MacroQueue-0.2.2/MacroQueue/MakeExe.sh
--rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.000000 MacroQueue-0.2.2/MacroQueue/__init__.py
--rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.2.2/MacroQueue/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.197067 MacroQueue-0.2.2/MacroQueue.egg-info/
--rw-rw-rw-   0        0        0     3799 2024-04-01 17:01:25.000000 MacroQueue-0.2.2/MacroQueue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      819 2024-04-01 17:01:25.000000 MacroQueue-0.2.2/MacroQueue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 17:01:25.000000 MacroQueue-0.2.2/MacroQueue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-01 17:01:25.000000 MacroQueue-0.2.2/MacroQueue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-01 17:01:25.000000 MacroQueue-0.2.2/MacroQueue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3799 2024-04-01 17:01:26.200070 MacroQueue-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2908 2024-04-01 15:15:43.000000 MacroQueue-0.2.2/README.md
--rw-rw-rw-   0        0        0       86 2024-04-01 17:01:26.217296 MacroQueue-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2284 2024-04-01 16:59:34.000000 MacroQueue-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 17:01:26.194053 MacroQueue-0.2.2/test/
--rw-rw-rw-   0        0        0      562 2024-03-19 18:06:33.000000 MacroQueue-0.2.2/test/test_MainFrame.py
--rw-rw-rw-   0        0        0      774 2024-03-19 18:07:50.000000 MacroQueue-0.2.2/test/test_STMthread.py
--rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.2.2/test/test_readdata.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.297634 MacroQueue-0.2.3/
+-rw-rw-rw-   0        0        0     1088 2024-03-19 20:51:50.000000 MacroQueue-0.2.3/LICENSE.md
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.208660 MacroQueue-0.2.3/MacroQueue/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.247160 MacroQueue-0.2.3/MacroQueue/Bitmaps/
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:04.000000 MacroQueue-0.2.3/MacroQueue/Bitmaps/DownArrow.bmp
+-rw-rw-rw-   0        0        0   786570 2022-02-15 20:38:07.000000 MacroQueue-0.2.3/MacroQueue/Bitmaps/Remove.bmp
+-rw-rw-rw-   0        0        0    65674 2022-02-15 20:38:12.000000 MacroQueue-0.2.3/MacroQueue/Bitmaps/UpArrow.bmp
+-rw-rw-rw-   0        0        0    68756 2024-03-27 14:08:48.000000 MacroQueue-0.2.3/MacroQueue/Dialogs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.277167 MacroQueue-0.2.3/MacroQueue/Functions/
+-rw-rw-rw-   0        0        0     1043 2024-01-11 19:05:47.000000 MacroQueue-0.2.3/MacroQueue/Functions/BField.py
+-rw-rw-rw-   0        0        0    21517 2024-04-01 13:25:42.000000 MacroQueue-0.2.3/MacroQueue/Functions/CreaTec.py
+-rw-rw-rw-   0        0        0     1517 2024-03-27 16:22:52.000000 MacroQueue-0.2.3/MacroQueue/Functions/General.py
+-rw-rw-rw-   0        0        0     1656 2024-03-25 14:52:53.000000 MacroQueue-0.2.3/MacroQueue/Functions/RF.py
+-rw-rw-rw-   0        0        0    23101 2023-04-19 20:00:33.000000 MacroQueue-0.2.3/MacroQueue/Functions/RHK.py
+-rw-rw-rw-   0        0        0     6042 2024-03-20 15:39:38.000000 MacroQueue-0.2.3/MacroQueue/Functions/SXM.py
+-rw-rw-rw-   0        0        0    16085 2024-03-19 20:14:36.000000 MacroQueue-0.2.3/MacroQueue/Functions/SXMRemote.py
+-rw-rw-rw-   0        0        0    24521 2024-03-21 18:30:14.000000 MacroQueue-0.2.3/MacroQueue/GUIDesign.py
+-rw-rw-rw-   0        0        0    54897 2024-04-01 15:32:11.000000 MacroQueue-0.2.3/MacroQueue/MacroQueue.py
+-rw-rw-rw-   0        0        0   181242 2022-03-08 20:23:43.000000 MacroQueue-0.2.3/MacroQueue/MacroQueueIcon.ico
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.277167 MacroQueue-0.2.3/MacroQueue/Macros/
+-rw-rw-rw-   0        0        0    13972 2024-03-27 16:23:14.000000 MacroQueue-0.2.3/MacroQueue/Macros/CreaTecMacro.json
+-rw-rw-rw-   0        0        0     7924 2022-06-13 16:55:53.000000 MacroQueue-0.2.3/MacroQueue/Macros/RHKMacro.json
+-rw-rw-rw-   0        0        0      539 2024-04-01 15:21:24.000000 MacroQueue-0.2.3/MacroQueue/MakeExe.sh
+-rw-rw-rw-   0        0        0      578 2024-03-19 20:16:23.000000 MacroQueue-0.2.3/MacroQueue/__init__.py
+-rw-rw-rw-   0        0        0      178 2024-03-19 19:42:01.000000 MacroQueue-0.2.3/MacroQueue/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.288122 MacroQueue-0.2.3/MacroQueue.egg-info/
+-rw-rw-rw-   0        0        0     3976 2024-04-01 17:07:35.000000 MacroQueue-0.2.3/MacroQueue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2024-04-01 17:07:35.000000 MacroQueue-0.2.3/MacroQueue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 17:07:35.000000 MacroQueue-0.2.3/MacroQueue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-01 17:07:35.000000 MacroQueue-0.2.3/MacroQueue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-01 17:07:35.000000 MacroQueue-0.2.3/MacroQueue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3976 2024-04-01 17:07:35.297634 MacroQueue-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2024-04-01 17:06:33.000000 MacroQueue-0.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-01 17:07:35.297634 MacroQueue-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2284 2024-04-01 17:06:55.000000 MacroQueue-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:07:35.288122 MacroQueue-0.2.3/test/
+-rw-rw-rw-   0        0        0      562 2024-03-19 18:06:33.000000 MacroQueue-0.2.3/test/test_MainFrame.py
+-rw-rw-rw-   0        0        0      774 2024-03-19 18:07:50.000000 MacroQueue-0.2.3/test/test_STMthread.py
+-rw-rw-rw-   0        0        0      730 2024-03-19 18:07:48.000000 MacroQueue-0.2.3/test/test_readdata.py
```

### Comparing `MacroQueue-0.2.2/LICENSE.md` & `MacroQueue-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Bitmaps/DownArrow.bmp` & `MacroQueue-0.2.3/MacroQueue/Bitmaps/DownArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Bitmaps/Remove.bmp` & `MacroQueue-0.2.3/MacroQueue/Bitmaps/Remove.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Bitmaps/UpArrow.bmp` & `MacroQueue-0.2.3/MacroQueue/Bitmaps/UpArrow.bmp`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Dialogs.py` & `MacroQueue-0.2.3/MacroQueue/Dialogs.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/BField.py` & `MacroQueue-0.2.3/MacroQueue/Functions/BField.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/CreaTec.py` & `MacroQueue-0.2.3/MacroQueue/Functions/CreaTec.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/General.py` & `MacroQueue-0.2.3/MacroQueue/Functions/General.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/RF.py` & `MacroQueue-0.2.3/MacroQueue/Functions/RF.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/RHK.py` & `MacroQueue-0.2.3/MacroQueue/Functions/RHK.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/SXM.py` & `MacroQueue-0.2.3/MacroQueue/Functions/SXM.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Functions/SXMRemote.py` & `MacroQueue-0.2.3/MacroQueue/Functions/SXMRemote.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/GUIDesign.py` & `MacroQueue-0.2.3/MacroQueue/GUIDesign.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/MacroQueue.py` & `MacroQueue-0.2.3/MacroQueue/MacroQueue.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/MacroQueueIcon.ico` & `MacroQueue-0.2.3/MacroQueue/MacroQueueIcon.ico`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Macros/CreaTecMacro.json` & `MacroQueue-0.2.3/MacroQueue/Macros/CreaTecMacro.json`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/Macros/RHKMacro.json` & `MacroQueue-0.2.3/MacroQueue/Macros/RHKMacro.json`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/MakeExe.sh` & `MacroQueue-0.2.3/MacroQueue/MakeExe.sh`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue/__init__.py` & `MacroQueue-0.2.3/MacroQueue/__init__.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/MacroQueue.egg-info/PKG-INFO` & `MacroQueue-0.2.3/MacroQueue.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.2.2
+Version: 0.2.3
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
 Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
@@ -29,15 +29,17 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
-![Brief image of MacroQueue](docs_src/source/ReadMe.png)
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ReadMe.png)
+
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ExpandingFigure.png)
 
 Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
```

### Comparing `MacroQueue-0.2.2/MacroQueue.egg-info/SOURCES.txt` & `MacroQueue-0.2.3/MacroQueue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/PKG-INFO` & `MacroQueue-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MacroQueue
-Version: 0.2.2
+Version: 0.2.3
 Summary: Automating Scanning Probe Microscopy
 Home-page: https://github.com/guptagroupstm/STMMacroQueue
 Download-URL: https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz
 Author: Brad Goff
 Author-email: guptagroupstm@gmail.com
 License: MIT
 Keywords: Automation,Scanning Probe Microscopy,Macro,Queue
@@ -29,15 +29,17 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
-![Brief image of MacroQueue](docs_src/source/ReadMe.png)
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ReadMe.png)
+
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ExpandingFigure.png)
 
 Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
```

### Comparing `MacroQueue-0.2.2/README.md` & `MacroQueue-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 Users can easily add python functions to control new and existing equipment.  Although any arbitary python function can be added, the base functions were created with the functional programming paradigm in mind, so the functions are small and each perform a single task.  For example, the function "Set RF Frequency", changes the frequency on the RF generator and records the new value.  This allows the functions to be reused for many types of measurements.
 
 The functions can be grouped into macros for each type of measurement.  Macros are added to a queue with different values for each parameter (e.g. bias, magnetic field, etc.) to perform measurements throughout a parameter space.  Each measurement is performed consecutively on a seperate thread to enable measurements in the queue to be modified.
 These features allow users to easily control several instruments in sync, perform a long series of measurements with minimal input, and add new instruments to a system. 
 The goal of MacroQueue is to provide a GUI that allow users to perform measurements in high-dimensional parameter spaces without requiring coding ability while still providing users with coding ability the flexibility to write arbitrarily complex functions.  
 
-![Brief image of MacroQueue](docs_src/source/ReadMe.png)
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ReadMe.png)
+
+![Brief image of MacroQueue](https://github.com/guptagroupstm/MacroQueue/blob/main/docs_src/source/ExpandingFigure.png)
 
 Check out for the [documentation](https://guptagroupstm.github.io/MacroQueue/index.html) for more information.
 
 ## Installation
 
 See the [install documentation](https://guptagroupstm.github.io/MacroQueue/Install.html). System requirements are also found in this page.
```

### Comparing `MacroQueue-0.2.2/setup.py` & `MacroQueue-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   from pathlib import Path
   this_directory = Path(__file__).parent
   long_description = (this_directory / "README.md").read_text()
 print(long_description)
 setup(
   name = 'MacroQueue',         # How you named your package folder (MyLib)
   packages = ['MacroQueue'],   # Chose the same as "name"
-  version = '0.2.2',      # Start with a small number and increase it with every change you make
+  version = '0.2.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Automating Scanning Probe Microscopy',   # Give a short description about your library
   author = 'Brad Goff',                   # Type in your name
   author_email = 'guptagroupstm@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/guptagroupstm/STMMacroQueue',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/guptagroupstm/STMMacroQueue/archive/refs/tags/v0.2.1.tar.gz',    # I explain this later on
   keywords = ['Automation', 'Scanning Probe Microscopy', 'Macro',"Queue"],   # Keywords that define your package best
```

### Comparing `MacroQueue-0.2.2/test/test_MainFrame.py` & `MacroQueue-0.2.3/test/test_MainFrame.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/test/test_STMthread.py` & `MacroQueue-0.2.3/test/test_STMthread.py`

 * *Files identical despite different names*

### Comparing `MacroQueue-0.2.2/test/test_readdata.py` & `MacroQueue-0.2.3/test/test_readdata.py`

 * *Files identical despite different names*

