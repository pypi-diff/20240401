# Comparing `tmp/clams-python-1.1.4.tar.gz` & `tmp/clams-python-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.1.4.tar", last modified: Mon Apr  1 00:00:36 2024, max compression
+gzip compressed data, was "clams-python-1.1.5.tar", last modified: Mon Apr  1 11:46:36 2024, max compression
```

## Comparing `clams-python-1.1.4.tar` & `clams-python-1.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.280627 clams-python-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-01 00:00:13.000000 clams-python-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 00:00:13.000000 clams-python-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 00:00:36.280627 clams-python-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 00:00:13.000000 clams-python-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 00:00:13.000000 clams-python-1.1.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.272627 clams-python-1.1.4/clams/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.272627 clams-python-1.1.4/clams/app/
--rw-r--r--   0 runner    (1001) docker     (127)    18934 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.272627 clams-python-1.1.4/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (127)    21448 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.272627 clams-python-1.1.4/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.268627 clams-python-1.1.4/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/mmif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/mmif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/mmif_utils/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/mmif_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 00:00:13.000000 clams-python-1.1.4/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.276627 clams-python-1.1.4/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.280627 clams-python-1.1.4/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 00:00:36.000000 clams-python-1.1.4/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 00:00:13.000000 clams-python-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:00:36.280627 clams-python-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-01 00:00:13.000000 clams-python-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:00:36.280627 clams-python-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22491 2024-04-01 00:00:13.000000 clams-python-1.1.4/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-01 00:00:13.000000 clams-python-1.1.4/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-01 11:46:13.000000 clams-python-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 11:46:13.000000 clams-python-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 11:46:36.630227 clams-python-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 11:46:13.000000 clams-python-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 11:46:13.000000 clams-python-1.1.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.622227 clams-python-1.1.5/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/mmif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 11:46:13.000000 clams-python-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:46:36.630227 clams-python-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-01 11:46:13.000000 clams-python-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-01 11:46:13.000000 clams-python-1.1.5/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-01 11:46:13.000000 clams-python-1.1.5/tests/test_clamscli.py
```

### Comparing `clams-python-1.1.4/LICENSE` & `clams-python-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/PKG-INFO` & `clams-python-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.1.4/README.md` & `clams-python-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/__init__.py` & `clams-python-1.1.5/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/app/__init__.py` & `clams-python-1.1.5/clams/app/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import warnings
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from urllib import parse as urlparser
 
 __all__ = ['ClamsApp']
 
-from typing import Union, Any, Optional, Dict, List, Iterable
+from typing import Union, Any, Optional, Dict, List, Tuple
 
 from mmif import Mmif, Document, DocumentTypes, View
-from clams.appmetadata import AppMetadata, RuntimeParameter, real_valued_primitives
+from clams.appmetadata import AppMetadata, real_valued_primitives, python_type, map_param_kv_delimiter
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(asctime)s %(name)s %(levelname)-8s %(thread)d %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S")
 
 
@@ -24,33 +24,42 @@
     """
     An abstract class to define API's for ClamsApps. A CLAMS app should inherit
     this class and then can be used with classes in :mod:`.restify` to work as
     web applications.
     """
     # A set of "universal runtime parameters that can be used for both GET and POST anytime".
     # The behavioral changes based on these parameters must be implemented on the SDK level. 
+    # This needs to stay as a list of dicts for compatibility with the metadata.py file (templated).
     universal_parameters = [
-        RuntimeParameter(**{
+        {
             'name': 'pretty', 'type': 'boolean', 'choices': None, 'default': False, 'multivalued': False,
             'description': 'The JSON body of the HTTP response will be re-formatted with 2-space indentation',
-        }),
+        },
     ]
+    
     # this key is used to store users' raw input params in the parameter dict 
     # even after "refinement" (i.e., casting to proper data types)
     _RAW_PARAMS_KEY = "#RAW#"
 
     def __init__(self):
         self.metadata: AppMetadata = self._load_appmetadata()
         super().__init__()
-        # data type specification for common parameters
-
+        
+        # data type spec to be used in type caster
+        self.metadata_param_spec = {}
+        self.annotate_param_spec = {}
         for param in ClamsApp.universal_parameters:
-            self.metadata.parameters.append(param)
-        self.metadata_param_caster = ParameterCaster(ClamsApp.universal_parameters)  # pytype: disable=wrong-arg-types
-        self.annotate_param_caster = ParameterCaster(self.metadata.parameters)  # pytype: disable=wrong-arg-types
+            # in addition to building the param spec, add them as regular params, so they are serialized in metadata
+            self.metadata.add_parameter(**param)  
+            self.metadata_param_spec[param['name']] = (param['type'], param.get('multivalued', False))
+        for param_spec in self.metadata.parameters:
+            self.annotate_param_spec[param_spec.name] = (param_spec.type, param_spec.multivalued)
+
+        self.metadata_param_caster = ParameterCaster(self.metadata_param_spec)
+        self.annotate_param_caster = ParameterCaster(self.annotate_param_spec)
         self.logger = logging.getLogger(self.metadata.identifier)
         
     def appmetadata(self, **kwargs: List[str]) -> str:
         """
         A public method to get metadata for this app as a string.
 
         :return: Serialized JSON string of the metadata
@@ -106,15 +115,15 @@
         :param runtime_params: An arbitrary set of k-v pairs to configure the app at runtime
         :return: Serialized JSON string of the output of the app
         """
         if not isinstance(mmif, Mmif):
             mmif = Mmif(mmif)
         issued_warnings = []
         for key in runtime_params:
-            if key not in self.annotate_param_caster.param_spec:
+            if key not in self.annotate_param_spec:
                 issued_warnings.append(UserWarning(f'An undefined parameter "{key}" (value: "{runtime_params[key]}") is passed'))
         # this will do casting + refinement altogether
         refined = self._refine_params(**runtime_params)
         pretty = refined.get('pretty', False)
         with warnings.catch_warnings(record=True) as ws:
             annotated = self._annotate(mmif, **refined)
             if ws:
@@ -293,27 +302,24 @@
                     finally:
                         document_file.close()
                 else:
                     raise FileNotFoundError(p.path)
 
 
 class ParameterCaster(object):
-    KV_DELIMITER = ':'
-    python_type = {"boolean": bool, "number": float, "integer": int, "string": str, "map": dict}
 
-    """
-    A helper class to convert parameters passed by HTTP query strings to
-    proper python data types.
+    def __init__(self, param_spec: Dict[str, Tuple[str, bool]]):
+        """
+        A helper class to convert parameters passed by HTTP query strings to
+        proper python data types.
 
-    :param param_spec: A specification of a data types of parameters
-    """
-    def __init__(self, params: Iterable[RuntimeParameter]):
-        self.param_spec = {}
-        for param in params:
-            self.param_spec[param.name] = (self.python_type[param.type], param.multivalued)
+        :param param_spec: A specification of a data types of parameters
+        """
+        self.param_spec = {pname: (python_type[ptype_str], pmultivalued) 
+                           for pname, (ptype_str, pmultivalued) in param_spec.items()}
 
     def cast(self, args: Dict[str, List[str]]) \
             -> Dict[str, Union[real_valued_primitives, List[real_valued_primitives], Dict[str, str]]]:
         """
         Given parameter specification, tries to cast values of args to specified Python data types.
         Note that this caster deals with query strings, thus all keys and values in the input args are plain strings. 
         Also note that the caster does not handle "unexpected" parameters came as an input. 
@@ -391,8 +397,8 @@
         return value
     
     @staticmethod
     def kv_param(value) -> Dict[str, str]:
         """
         Helper function to convert string values to key-value pair type.
         """
-        return dict([value.split(ParameterCaster.KV_DELIMITER, 1)])
+        return dict([value.split(map_param_kv_delimiter, 1)])
```

### Comparing `clams-python-1.1.4/clams/appmetadata/__init__.py` & `clams-python-1.1.5/clams/appmetadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 unresolved_app_version_num = 'unresolvable'
 app_version_envvar_key = 'CLAMS_APP_VERSION'
 # type aliases to use in app metadata and runtime parameter processing 
 real_valued_primitives = Union[int, float, bool, str]
 # these names are taken from the JSON schema data types
 param_value_types = Literal['integer', 'number', 'string', 'boolean', 'map']
+# and the specific delimiter for the map type
+map_param_kv_delimiter = ':'
+
+# dict to map app parameter data types to Python data types
+python_type = {"boolean": bool, "number": float, "integer": int, "string": str, "map": dict}
 
 param_value_types_values = param_value_types.__args__  # pytype: disable=attribute-error
 app_directory_baseurl = "http://apps.clams.ai"
 
 
 def get_clams_pyver():
     # real hack to avoid import clams as a package in gh-action workflow
```

### Comparing `clams-python-1.1.4/clams/develop/__init__.py` & `clams-python-1.1.5/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/app/.gitignore.template` & `clams-python-1.1.5/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/app/Containerfile.template` & `clams-python-1.1.5/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/app/README.md.template` & `clams-python-1.1.5/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/app/app.py.template` & `clams-python-1.1.5/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/app/metadata.py.template` & `clams-python-1.1.5/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.1.5/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.1.5/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/mmif_utils/rewind.py` & `clams-python-1.1.5/clams/mmif_utils/rewind.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/mmif_utils/source.py` & `clams-python-1.1.5/clams/mmif_utils/source.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams/restify/__init__.py` & `clams-python-1.1.5/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/clams_python.egg-info/PKG-INFO` & `clams-python-1.1.5/clams_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.4
+Version: 1.1.5
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

### Comparing `clams-python-1.1.4/clams_python.egg-info/SOURCES.txt` & `clams-python-1.1.5/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/setup.py` & `clams-python-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.4/tests/test_clamsapp.py` & `clams-python-1.1.5/tests/test_clamsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import jsonschema
 import pytest
 from mmif import Mmif, Document, DocumentTypes, AnnotationTypes, View, __specver__
 
 import clams.app
 import clams.restify
 from clams.app import ParameterCaster
-from clams.appmetadata import AppMetadata, Input, RuntimeParameter
+from clams.appmetadata import AppMetadata, Input
 
 
 class ExampleInputMMIF(object):
     EXAMPLE_TEXT = 'this is a temp file.'
 
     @staticmethod
     def get_rawmmif() -> Mmif:
@@ -416,37 +416,35 @@
         self.assertEqual(res.status_code, 500)
         self.assertEqual(res.mimetype, 'text/plain')
 
 
 class TestParameterCaster(unittest.TestCase):
     
     def setUp(self) -> None:
-        self.params = []
-        specs = {'str_param': ('string', False),
-                 'number_param': ('number', False),
-                 'int_param': ('integer', False),
-                 'bool_param': ('boolean', False), 
-                 'str_multi_param': ('string', True),
-                 'map_param': ('map', True),
-                 }
-        for name, (t, mv) in specs.items():
-            self.params.append(RuntimeParameter(**{'name': name, 'type': t, 'multivalued': mv, 'description': ""}))
+        self.param_spec = {'str_param': ('string', False),
+                           'number_param': ('number', False),
+                           'int_param': ('integer', False),
+                           'bool_param': ('boolean', False),
+                           'str_multi_param': ('string', True),
+                           'map_param': ('map', True),
+                           }
 
     def test_cast(self):
-        caster = ParameterCaster(self.params)
+        caster = ParameterCaster(self.param_spec)
         params = {
             'str_param': ["a_string"], 
             'number_param': ["1.11"], 
             'int_param': [str(sys.maxsize)], 
             'bool_param': ['true'],
             'str_multi_param': ['value1', 'value2'],
             'undefined_param_single': ['undefined_value1'],
             'undefined_param_multi': ['undefined_value1', 'undefined_value2'],
             'map_param': ['key1:val1', 'key2:val2', 'key3:val3', 'key1:val4']
         }
+        # all "RAW" parameter values are assumed to be strings
         self.assertTrue(all(map(lambda x: isinstance(x, str), itertools.chain.from_iterable(params.values()))))
         casted = caster.cast(params)
         # must push out to the list
         self.assertEqual(casted['str_param'], params['str_param'][0])
         self.assertEqual(casted['number_param'], 1.11)
         self.assertTrue(isinstance(casted['int_param'], int))
         self.assertTrue(casted['bool_param'])
```

### Comparing `clams-python-1.1.4/tests/test_clamscli.py` & `clams-python-1.1.5/tests/test_clamscli.py`

 * *Files identical despite different names*

