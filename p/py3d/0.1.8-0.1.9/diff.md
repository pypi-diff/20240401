# Comparing `tmp/py3d-0.1.8.tar.gz` & `tmp/py3d-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.8.tar", last modified: Wed Jul  5 01:05:29 2023, max compression
+gzip compressed data, was "py3d-0.1.9.tar", last modified: Wed Jul 12 15:21:54 2023, max compression
```

## Comparing `py3d-0.1.8.tar` & `py3d-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.844173 py3d-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-05 01:05:29.844173 py3d-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-05 01:05:11.000000 py3d-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.840173 py3d-0.1.8/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29637 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-07-05 01:04:26.000000 py3d-0.1.8/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 01:05:29.840173 py3d-0.1.8/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-05 01:05:29.000000 py3d-0.1.8/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-05 01:05:29.844173 py3d-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-07-05 01:04:26.000000 py3d-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:21:54.490630 py3d-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-12 15:21:54.490630 py3d-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-12 15:21:39.000000 py3d-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:21:54.490630 py3d-0.1.9/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-12 15:20:48.000000 py3d-0.1.9/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29637 2023-07-12 15:20:48.000000 py3d-0.1.9/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22761 2023-07-12 15:20:48.000000 py3d-0.1.9/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:21:54.490630 py3d-0.1.9/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-12 15:21:54.000000 py3d-0.1.9/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-12 15:21:54.000000 py3d-0.1.9/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 15:21:54.000000 py3d-0.1.9/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-12 15:21:54.000000 py3d-0.1.9/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 15:21:54.000000 py3d-0.1.9/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 15:21:54.490630 py3d-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-07-12 15:20:48.000000 py3d-0.1.9/setup.py
```

### Comparing `py3d-0.1.8/PKG-INFO` & `py3d-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.8
+Version: 0.1.9
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.8/README.md` & `py3d-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.8/py3d/core.py` & `py3d-0.1.9/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.1.8/py3d/viewer.html` & `py3d-0.1.9/py3d/viewer.html`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,20 @@
         static ceil(value, base) {
             return Math.ceil(value / base) * base
         }
         static ticks(min, max, step) {
             if (max <= min) {
                 return [[min], min, max]
             }
-            let r_step = 10 ** Math.round(Math.log10(step))
+            let digits = Math.round(Math.log10(step))
+            let r_step = 10 ** digits
             let r_min = mat.floor(min, r_step)
             let r_max = mat.ceil(max, r_step)
             let size = Math.ceil((r_max - r_min) / r_step) + 1
-            let ticks = Array.from({ length: size }, (v, i) => r_min + r_step * i)
+            let ticks = Array.from({ length: size }, (v, i) => (r_min + r_step * i).toFixed(digits > 0 ? 0 : -digits))
             return [ticks, ticks[0], ticks[ticks.length - 1]]
         }
     }
     class Camera {
         PERSPECTIVE = "P"
         ORTHOGRAPHIC = "O"
         constructor(type, fovy, aspect, near, far, min, max) {
```

### Comparing `py3d-0.1.8/py3d.egg-info/PKG-INFO` & `py3d-0.1.9/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.8
+Version: 0.1.9
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.8/setup.py` & `py3d-0.1.9/setup.py`

 * *Files identical despite different names*

