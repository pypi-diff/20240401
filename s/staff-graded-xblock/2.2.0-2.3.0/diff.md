# Comparing `tmp/staff_graded-xblock-2.2.0.tar.gz` & `tmp/staff_graded-xblock-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staff_graded-xblock-2.2.0.tar", last modified: Mon Nov  6 14:01:24 2023, max compression
+gzip compressed data, was "staff_graded-xblock-2.3.0.tar", last modified: Mon Apr  1 19:19:04 2024, max compression
```

## Comparing `staff_graded-xblock-2.2.0.tar` & `staff_graded-xblock-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.735758 staff_graded-xblock-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-11-06 14:01:24.731757 staff_graded-xblock-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.727757 staff_graded-xblock-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 14:01:24.735758 staff_graded-xblock-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.727757 staff_graded-xblock-2.2.0/staff_graded/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/staff_graded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.727757 staff_graded-xblock-2.2.0/staff_graded/static/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.727757 staff_graded-xblock-2.2.0/staff_graded/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/static/css/staff_graded.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.727757 staff_graded-xblock-2.2.0/staff_graded/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/static/html/staff_graded.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.723757 staff_graded-xblock-2.2.0/staff_graded/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.731757 staff_graded-xblock-2.2.0/staff_graded/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-11-06 14:01:15.000000 staff_graded-xblock-2.2.0/staff_graded/static/js/src/staff_graded.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 14:01:24.731757 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-06 14:01:24.000000 staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.555658 staff_graded-xblock-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 19:19:04.555658 staff_graded-xblock-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:19:04.555658 staff_graded-xblock-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/staff_graded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/static/css/staff_graded.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/static/html/staff_graded.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.551658 staff_graded-xblock-2.3.0/staff_graded/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-01 19:19:01.000000 staff_graded-xblock-2.3.0/staff_graded/static/js/src/staff_graded.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:19:04.555658 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 19:19:04.000000 staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/top_level.txt
```

### Comparing `staff_graded-xblock-2.2.0/LICENSE` & `staff_graded-xblock-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/PKG-INFO` & `staff_graded-xblock-2.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: staff_graded-xblock
-Version: 2.2.0
+Version: 2.3.0
 Summary: Staff Graded XBlock
 Home-page: https://github.com/openedx/staff_graded-xblock
 License: AGPL v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
-Requires-Dist: markdown
-Requires-Dist: XBlock
+Requires-Dist: path.py
 Requires-Dist: web-fragments
+Requires-Dist: XBlock
+Requires-Dist: markdown
 Requires-Dist: edx-bulk-grades
-Requires-Dist: path.py
 
 Staff Graded XBlock
```

### Comparing `staff_graded-xblock-2.2.0/README.rst` & `staff_graded-xblock-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/setup.py` & `staff_graded-xblock-2.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
     ],
     packages=[
         'staff_graded',
     ],
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
```

### Comparing `staff_graded-xblock-2.2.0/staff_graded/staff_graded.py` & `staff_graded-xblock-2.3.0/staff_graded/staff_graded.py`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/staff_graded/static/README.txt` & `staff_graded-xblock-2.3.0/staff_graded/static/README.txt`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/staff_graded/static/html/staff_graded.html` & `staff_graded-xblock-2.3.0/staff_graded/static/html/staff_graded.html`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/staff_graded/static/js/src/staff_graded.js` & `staff_graded-xblock-2.3.0/staff_graded/static/js/src/staff_graded.js`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/PKG-INFO` & `staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: staff-graded-xblock
-Version: 2.2.0
+Name: staff_graded-xblock
+Version: 2.3.0
 Summary: Staff Graded XBlock
 Home-page: https://github.com/openedx/staff_graded-xblock
 License: AGPL v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
-Requires-Dist: markdown
-Requires-Dist: XBlock
+Requires-Dist: path.py
 Requires-Dist: web-fragments
+Requires-Dist: XBlock
+Requires-Dist: markdown
 Requires-Dist: edx-bulk-grades
-Requires-Dist: path.py
 
 Staff Graded XBlock
```

### Comparing `staff_graded-xblock-2.2.0/staff_graded_xblock.egg-info/SOURCES.txt` & `staff_graded-xblock-2.3.0/staff_graded_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

