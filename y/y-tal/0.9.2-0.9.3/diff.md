# Comparing `tmp/y-tal-0.9.2.tar.gz` & `tmp/y-tal-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y-tal-0.9.2.tar", last modified: Wed Mar 22 15:01:23 2023, max compression
+gzip compressed data, was "y-tal-0.9.3.tar", last modified: Tue May 16 09:30:08 2023, max compression
```

## Comparing `y-tal-0.9.2.tar` & `y-tal-0.9.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.427230 y-tal-0.9.2/
--rw-r--r--   0 droyo     (1000) droyo     (1000)    35149 2022-06-02 13:28:28.000000 y-tal-0.9.2/LICENSE
--rw-r--r--   0 droyo     (1000) droyo     (1000)     5270 2023-03-22 15:01:23.427230 y-tal-0.9.2/PKG-INFO
--rw-r--r--   0 droyo     (1000) droyo     (1000)     4752 2023-02-21 14:43:39.000000 y-tal-0.9.2/README.md
--rw-r--r--   0 droyo     (1000) droyo     (1000)       38 2023-03-22 15:01:23.427230 y-tal-0.9.2/setup.cfg
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1166 2023-02-21 15:26:41.000000 y-tal-0.9.2/setup.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/
--rw-r--r--   0 droyo     (1000) droyo     (1000)       31 2022-06-09 10:36:48.000000 y-tal-0.9.2/tal/.tal.conf.example
--rw-r--r--   0 droyo     (1000) droyo     (1000)      182 2023-03-22 11:51:35.000000 y-tal-0.9.2/tal/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     6723 2023-01-19 11:48:13.000000 y-tal-0.9.2/tal/__main__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     8459 2023-02-21 18:09:58.000000 y-tal-0.9.2/tal/config.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     4848 2023-02-21 18:20:32.000000 y-tal-0.9.2/tal/enums.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/io/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1248 2023-03-03 17:36:16.000000 y-tal-0.9.2/tal/io/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     9722 2023-02-28 11:43:13.000000 y-tal-0.9.2/tal/io/capture_data.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     9264 2022-11-11 13:36:35.000000 y-tal-0.9.2/tal/io/format.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/plot/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3325 2023-03-01 09:00:39.000000 y-tal-0.9.2/tal/plot/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     4380 2023-02-21 17:32:50.000000 y-tal-0.9.2/tal/plot/compare.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3107 2023-02-21 17:25:44.000000 y-tal-0.9.2/tal/plot/plotter3d.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     8163 2023-03-01 08:59:04.000000 y-tal-0.9.2/tal/plot/xy.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/reconstruct/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3680 2023-03-01 09:09:45.000000 y-tal-0.9.2/tal/reconstruct/__init__.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/reconstruct/bp/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     2069 2023-02-27 17:32:21.000000 y-tal-0.9.2/tal/reconstruct/bp/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3107 2023-02-21 17:38:30.000000 y-tal-0.9.2/tal/reconstruct/bp/backprojection.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/reconstruct/fbp/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1742 2023-02-28 11:42:59.000000 y-tal-0.9.2/tal/reconstruct/fbp/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     4401 2022-12-22 15:33:34.000000 y-tal-0.9.2/tal/reconstruct/filters.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/reconstruct/pf/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     7112 2023-02-21 17:42:28.000000 y-tal-0.9.2/tal/reconstruct/pf/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    15744 2022-11-04 12:04:17.000000 y-tal-0.9.2/tal/reconstruct/pf/pf_solver.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    10332 2022-07-29 11:13:21.000000 y-tal-0.9.2/tal/reconstruct/pf/propagator.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     6461 2022-07-29 11:13:21.000000 y-tal-0.9.2/tal/reconstruct/pf/rsd_kernel.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/reconstruct/pf_dev/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     2660 2023-03-01 09:09:14.000000 y-tal-0.9.2/tal/reconstruct/pf_dev/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    11650 2023-03-01 09:29:22.000000 y-tal-0.9.2/tal/reconstruct/pf_dev/phasor_fields.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     4284 2023-03-01 09:30:40.000000 y-tal-0.9.2/tal/reconstruct/utils.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/tal/render/
--rw-r--r--   0 droyo     (1000) droyo     (1000)      938 2023-02-21 18:03:28.000000 y-tal-0.9.2/tal/render/__init__.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     3287 2022-06-21 10:25:49.000000 y-tal-0.9.2/tal/render/create.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     7925 2023-02-21 18:22:49.000000 y-tal-0.9.2/tal/render/mitsuba2_transient_nlos.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)    24095 2023-03-22 11:50:50.000000 y-tal-0.9.2/tal/render/render.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1866 2023-03-22 11:51:01.000000 y-tal-0.9.2/tal/render/scene_defaults.yaml
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1623 2023-01-31 17:45:45.000000 y-tal-0.9.2/tal/util.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/test/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1354 2023-02-21 18:05:37.000000 y-tal-0.9.2/test/test_io.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)     2006 2022-11-04 12:04:17.000000 y-tal-0.9.2/test/test_pf.py
--rw-r--r--   0 droyo     (1000) droyo     (1000)      301 2023-01-31 18:07:10.000000 y-tal-0.9.2/test/test_plot.py
-drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-03-22 15:01:23.423230 y-tal-0.9.2/y_tal.egg-info/
--rw-r--r--   0 droyo     (1000) droyo     (1000)     5270 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/PKG-INFO
--rw-r--r--   0 droyo     (1000) droyo     (1000)     1000 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/SOURCES.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)        1 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/dependency_links.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)       42 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/entry_points.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)      148 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/requires.txt
--rw-r--r--   0 droyo     (1000) droyo     (1000)        4 2023-03-22 15:01:23.000000 y-tal-0.9.2/y_tal.egg-info/top_level.txt
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.422387 y-tal-0.9.3/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)    35149 2022-06-02 13:28:28.000000 y-tal-0.9.3/LICENSE
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     5270 2023-05-16 09:30:08.418387 y-tal-0.9.3/PKG-INFO
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     4752 2023-02-21 14:43:39.000000 y-tal-0.9.3/README.md
+-rw-r--r--   0 droyo     (1000) droyo     (1000)       38 2023-05-16 09:30:08.422387 y-tal-0.9.3/setup.cfg
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1166 2023-02-21 15:26:41.000000 y-tal-0.9.3/setup.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.402387 y-tal-0.9.3/tal/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)       31 2022-06-09 10:36:48.000000 y-tal-0.9.3/tal/.tal.conf.example
+-rw-r--r--   0 droyo     (1000) droyo     (1000)      182 2023-05-16 09:29:58.000000 y-tal-0.9.3/tal/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     6723 2023-01-19 11:48:13.000000 y-tal-0.9.3/tal/__main__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     8459 2023-02-21 18:09:58.000000 y-tal-0.9.3/tal/config.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     4848 2023-02-21 18:20:32.000000 y-tal-0.9.3/tal/enums.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.402387 y-tal-0.9.3/tal/io/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1248 2023-03-03 17:36:16.000000 y-tal-0.9.3/tal/io/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     9722 2023-02-28 11:43:13.000000 y-tal-0.9.3/tal/io/capture_data.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     9264 2022-11-11 13:36:35.000000 y-tal-0.9.3/tal/io/format.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.406386 y-tal-0.9.3/tal/plot/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     3325 2023-03-01 09:00:39.000000 y-tal-0.9.3/tal/plot/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     4380 2023-02-21 17:32:50.000000 y-tal-0.9.3/tal/plot/compare.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     3107 2023-02-21 17:25:44.000000 y-tal-0.9.3/tal/plot/plotter3d.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     8163 2023-03-01 08:59:04.000000 y-tal-0.9.3/tal/plot/xy.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.406386 y-tal-0.9.3/tal/reconstruct/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     3680 2023-03-01 09:09:45.000000 y-tal-0.9.3/tal/reconstruct/__init__.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.406386 y-tal-0.9.3/tal/reconstruct/bp/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     2069 2023-02-27 17:32:21.000000 y-tal-0.9.3/tal/reconstruct/bp/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     3107 2023-02-21 17:38:30.000000 y-tal-0.9.3/tal/reconstruct/bp/backprojection.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.410387 y-tal-0.9.3/tal/reconstruct/fbp/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1742 2023-02-28 11:42:59.000000 y-tal-0.9.3/tal/reconstruct/fbp/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     4401 2022-12-22 15:33:34.000000 y-tal-0.9.3/tal/reconstruct/filters.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.410387 y-tal-0.9.3/tal/reconstruct/pf/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     7112 2023-02-21 17:42:28.000000 y-tal-0.9.3/tal/reconstruct/pf/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)    15744 2022-11-04 12:04:17.000000 y-tal-0.9.3/tal/reconstruct/pf/pf_solver.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)    10332 2022-07-29 11:13:21.000000 y-tal-0.9.3/tal/reconstruct/pf/propagator.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     6461 2022-07-29 11:13:21.000000 y-tal-0.9.3/tal/reconstruct/pf/rsd_kernel.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.410387 y-tal-0.9.3/tal/reconstruct/pf_dev/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     2660 2023-03-01 09:09:14.000000 y-tal-0.9.3/tal/reconstruct/pf_dev/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)    11650 2023-05-16 09:28:40.000000 y-tal-0.9.3/tal/reconstruct/pf_dev/phasor_fields.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     4284 2023-03-01 09:30:40.000000 y-tal-0.9.3/tal/reconstruct/utils.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.414387 y-tal-0.9.3/tal/render/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)      938 2023-02-21 18:03:28.000000 y-tal-0.9.3/tal/render/__init__.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     3287 2022-06-21 10:25:49.000000 y-tal-0.9.3/tal/render/create.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     7925 2023-02-21 18:22:49.000000 y-tal-0.9.3/tal/render/mitsuba2_transient_nlos.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)    24112 2023-05-16 09:28:53.000000 y-tal-0.9.3/tal/render/render.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1866 2023-03-22 11:51:01.000000 y-tal-0.9.3/tal/render/scene_defaults.yaml
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1623 2023-01-31 17:45:45.000000 y-tal-0.9.3/tal/util.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.414387 y-tal-0.9.3/test/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1354 2023-02-21 18:05:37.000000 y-tal-0.9.3/test/test_io.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     2006 2022-11-04 12:04:17.000000 y-tal-0.9.3/test/test_pf.py
+-rw-r--r--   0 droyo     (1000) droyo     (1000)      301 2023-01-31 18:07:10.000000 y-tal-0.9.3/test/test_plot.py
+drwxr-xr-x   0 droyo     (1000) droyo     (1000)        0 2023-05-16 09:30:08.418387 y-tal-0.9.3/y_tal.egg-info/
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     5270 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/PKG-INFO
+-rw-r--r--   0 droyo     (1000) droyo     (1000)     1000 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/SOURCES.txt
+-rw-r--r--   0 droyo     (1000) droyo     (1000)        1 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/dependency_links.txt
+-rw-r--r--   0 droyo     (1000) droyo     (1000)       42 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/entry_points.txt
+-rw-r--r--   0 droyo     (1000) droyo     (1000)      148 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/requires.txt
+-rw-r--r--   0 droyo     (1000) droyo     (1000)        4 2023-05-16 09:30:08.000000 y-tal-0.9.3/y_tal.egg-info/top_level.txt
```

### Comparing `y-tal-0.9.2/LICENSE` & `y-tal-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/PKG-INFO` & `y-tal-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y-tal
-Version: 0.9.2
+Version: 0.9.3
 Summary: (Your) Transient Auxiliary Library - Analysis and processing of time-resolved light transport
 Home-page: https://github.com/diegoroyo/tal
 Author: Diego Royo & Pablo Luesia
 Author-email: droyo@unizar.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `y-tal-0.9.2/README.md` & `y-tal-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/setup.py` & `y-tal-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/__main__.py` & `y-tal-0.9.3/tal/__main__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/config.py` & `y-tal-0.9.3/tal/config.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/enums.py` & `y-tal-0.9.3/tal/enums.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/io/__init__.py` & `y-tal-0.9.3/tal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/io/capture_data.py` & `y-tal-0.9.3/tal/io/capture_data.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/io/format.py` & `y-tal-0.9.3/tal/io/format.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/plot/__init__.py` & `y-tal-0.9.3/tal/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/plot/compare.py` & `y-tal-0.9.3/tal/plot/compare.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/plot/plotter3d.py` & `y-tal-0.9.3/tal/plot/plotter3d.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/plot/xy.py` & `y-tal-0.9.3/tal/plot/xy.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/__init__.py` & `y-tal-0.9.3/tal/reconstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/bp/__init__.py` & `y-tal-0.9.3/tal/reconstruct/bp/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/bp/backprojection.py` & `y-tal-0.9.3/tal/reconstruct/bp/backprojection.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/fbp/__init__.py` & `y-tal-0.9.3/tal/reconstruct/fbp/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/filters.py` & `y-tal-0.9.3/tal/reconstruct/filters.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf/__init__.py` & `y-tal-0.9.3/tal/reconstruct/pf/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf/pf_solver.py` & `y-tal-0.9.3/tal/reconstruct/pf/pf_solver.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf/propagator.py` & `y-tal-0.9.3/tal/reconstruct/pf/propagator.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf/rsd_kernel.py` & `y-tal-0.9.3/tal/reconstruct/pf/rsd_kernel.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf_dev/__init__.py` & `y-tal-0.9.3/tal/reconstruct/pf_dev/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/pf_dev/phasor_fields.py` & `y-tal-0.9.3/tal/reconstruct/pf_dev/phasor_fields.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/reconstruct/utils.py` & `y-tal-0.9.3/tal/reconstruct/utils.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/render/__init__.py` & `y-tal-0.9.3/tal/render/__init__.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/render/create.py` & `y-tal-0.9.3/tal/render/create.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/render/mitsuba2_transient_nlos.py` & `y-tal-0.9.3/tal/render/mitsuba2_transient_nlos.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/render/render.py` & `y-tal-0.9.3/tal/render/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         assert material_id in materials.keys(), \
             f'Geometry {name} has material {material_id}, but it must be one of {", ".join(materials.keys())}'
         shape_material = materials[material_id]
         material_keys = get_material_keys(shape_material)
         for key in material_keys:
             assert key in g('material'), \
                 f'Material {material_id} for geometry {name} must have a value for {key}'
-            shape_material.replace(f'${key}', g('material')[key])
+            shape_material = shape_material.replace(f'${key}', g('material')[key])
 
         shape_transform = fdent(f'''\
             <transform name="to_world">
                 <scale x="{g('scale') or 1.0}" y="{g('scale') or 1.0}" z="{g('scale') or 1.0}"/>
                 <rotate x="1" angle="{g('rot_degrees_x') or 0.0}"/>
                 <rotate y="1" angle="{g('rot_degrees_y') or 0.0}"/>
                 <rotate z="1" angle="{g('rot_degrees_z') or 0.0}"/>
```

### Comparing `y-tal-0.9.2/tal/render/scene_defaults.yaml` & `y-tal-0.9.3/tal/render/scene_defaults.yaml`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/tal/util.py` & `y-tal-0.9.3/tal/util.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/test/test_io.py` & `y-tal-0.9.3/test/test_io.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/test/test_pf.py` & `y-tal-0.9.3/test/test_pf.py`

 * *Files identical despite different names*

### Comparing `y-tal-0.9.2/y_tal.egg-info/PKG-INFO` & `y-tal-0.9.3/y_tal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y-tal
-Version: 0.9.2
+Version: 0.9.3
 Summary: (Your) Transient Auxiliary Library - Analysis and processing of time-resolved light transport
 Home-page: https://github.com/diegoroyo/tal
 Author: Diego Royo & Pablo Luesia
 Author-email: droyo@unizar.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `y-tal-0.9.2/y_tal.egg-info/SOURCES.txt` & `y-tal-0.9.3/y_tal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

