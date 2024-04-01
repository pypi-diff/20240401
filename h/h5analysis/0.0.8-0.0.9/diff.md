# Comparing `tmp/h5analysis-0.0.8.tar.gz` & `tmp/h5analysis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5analysis-0.0.8.tar", last modified: Thu Jan 11 21:41:07 2024, max compression
+gzip compressed data, was "h5analysis-0.0.9.tar", last modified: Fri Jan 12 17:19:20 2024, max compression
```

## Comparing `h5analysis-0.0.8.tar` & `h5analysis-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:41:07.578053 h5analysis-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-11 21:40:57.000000 h5analysis-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-11 21:41:07.578053 h5analysis-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-01-11 21:40:57.000000 h5analysis-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-11 21:40:57.000000 h5analysis-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-11 21:41:07.578053 h5analysis-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:41:07.574053 h5analysis-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:41:07.574053 h5analysis-0.0.8/src/h5analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    39351 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/LoadData.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/MathData.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/ReadData.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/add_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/beamline_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/data_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/data_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/data_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/datautil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/readutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/simplemath.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-01-11 21:40:57.000000 h5analysis-0.0.8/src/h5analysis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 21:41:07.578053 h5analysis-0.0.8/src/h5analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-11 21:41:07.000000 h5analysis-0.0.8/src/h5analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-11 21:41:07.000000 h5analysis-0.0.8/src/h5analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 21:41:07.000000 h5analysis-0.0.8/src/h5analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-11 21:41:07.000000 h5analysis-0.0.8/src/h5analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-11 21:41:07.000000 h5analysis-0.0.8/src/h5analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 17:19:20.761165 h5analysis-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-12 17:19:09.000000 h5analysis-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-12 17:19:20.761165 h5analysis-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-01-12 17:19:09.000000 h5analysis-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-12 17:19:09.000000 h5analysis-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-12 17:19:20.761165 h5analysis-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 17:19:20.749164 h5analysis-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 17:19:20.757165 h5analysis-0.0.9/src/h5analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    39060 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/LoadData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/MathData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/ReadData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/add_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/beamline_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16415 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/data_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/data_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/data_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/datautil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/readutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/simplemath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-01-12 17:19:09.000000 h5analysis-0.0.9/src/h5analysis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 17:19:20.761165 h5analysis-0.0.9/src/h5analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-01-12 17:19:20.000000 h5analysis-0.0.9/src/h5analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-12 17:19:20.000000 h5analysis-0.0.9/src/h5analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 17:19:20.000000 h5analysis-0.0.9/src/h5analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-12 17:19:20.000000 h5analysis-0.0.9/src/h5analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-12 17:19:20.000000 h5analysis-0.0.9/src/h5analysis.egg-info/top_level.txt
```

### Comparing `h5analysis-0.0.8/LICENSE` & `h5analysis-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/PKG-INFO` & `h5analysis-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5analysis
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to analyse, plot, and export data stored in HDF5 files.
 Home-page: https://github.com/pmb399/H5Analysis
 Author: Patrick Braun
 Author-email: patrick.braun@lightsource.ca
 License: MIT License
 Project-URL: Tutorial, https://reixs.lightsource.ca/workshops/reixs-sxs-workshop-2023/
 Project-URL: Bug Tracker, https://github.com/pmb399/H5Analysis
```

### Comparing `h5analysis-0.0.8/README.md` & `h5analysis-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/setup.cfg` & `h5analysis-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/LoadData.py` & `h5analysis-0.0.9/src/h5analysis/LoadData.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,16 +568,14 @@
         Parameters
         ----------
         See loader function.
         Adds all scans specified in *args.
         """
 
         # Ensure that only one scan is loaded.
-        if len(args) != 1:
-            raise TypeError("You may only select one scan at a time")
         if self.data != []:
             raise TypeError("You can only append one scan per object")
 
         self.data.append(ImageAddition(config,file, x_stream,
                          detector, *args, **kwargs))
         
 
@@ -589,16 +587,14 @@
         ----------
         See loader function.
         Subtracts all imnages from the first element.
 
         """
 
         # Ensure that only one scan is loaded.
-        if len(args) != 1:
-            raise TypeError("You may only select one scan at a time")
         if self.data != []:
             raise TypeError("You can only append one scan per object")
 
         # Append all REIXS scan objects to scan list in current object.
         self.data.append(ImageSubtraction(config, file, x_stream,
                          detector, *args, **kwargs))
         
@@ -931,16 +927,14 @@
         Parameters
         ----------
         See loader function.
         Adds all scans specified in *args.
         """
 
         # Ensure that only one scan is loaded.
-        if len(args) != 1:
-            raise TypeError("You may only select one scan at a time")
         if self.data != []:
             raise TypeError("You can only append one scan per object")
         
         self.data.append(HistogramAddition(config, file, x_stream,
                          y_stream, z_stream, *args, norm=norm))
     
     def subtract(self):
```

### Comparing `h5analysis-0.0.8/src/h5analysis/MathData.py` & `h5analysis-0.0.9/src/h5analysis/MathData.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/ReadData.py` & `h5analysis-0.0.9/src/h5analysis/ReadData.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/add_subtract.py` & `h5analysis-0.0.9/src/h5analysis/add_subtract.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/beamline_info.py` & `h5analysis-0.0.9/src/h5analysis/beamline_info.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/config.py` & `h5analysis-0.0.9/src/h5analysis/config.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/data_1d.py` & `h5analysis-0.0.9/src/h5analysis/data_1d.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/data_2d.py` & `h5analysis-0.0.9/src/h5analysis/data_2d.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/data_3d.py` & `h5analysis-0.0.9/src/h5analysis/data_3d.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/datautil.py` & `h5analysis-0.0.9/src/h5analysis/datautil.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/histogram.py` & `h5analysis-0.0.9/src/h5analysis/histogram.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/parser.py` & `h5analysis-0.0.9/src/h5analysis/parser.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/readutil.py` & `h5analysis-0.0.9/src/h5analysis/readutil.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/simplemath.py` & `h5analysis-0.0.9/src/h5analysis/simplemath.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis/util.py` & `h5analysis-0.0.9/src/h5analysis/util.py`

 * *Files identical despite different names*

### Comparing `h5analysis-0.0.8/src/h5analysis.egg-info/PKG-INFO` & `h5analysis-0.0.9/src/h5analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5analysis
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library to analyse, plot, and export data stored in HDF5 files.
 Home-page: https://github.com/pmb399/H5Analysis
 Author: Patrick Braun
 Author-email: patrick.braun@lightsource.ca
 License: MIT License
 Project-URL: Tutorial, https://reixs.lightsource.ca/workshops/reixs-sxs-workshop-2023/
 Project-URL: Bug Tracker, https://github.com/pmb399/H5Analysis
```

### Comparing `h5analysis-0.0.8/src/h5analysis.egg-info/SOURCES.txt` & `h5analysis-0.0.9/src/h5analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

