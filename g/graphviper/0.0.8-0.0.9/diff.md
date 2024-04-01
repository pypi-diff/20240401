# Comparing `tmp/graphviper-0.0.8.tar.gz` & `tmp/graphviper-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphviper-0.0.8.tar", last modified: Tue Mar 12 19:38:22 2024, max compression
+gzip compressed data, was "graphviper-0.0.9.tar", last modified: Wed Mar 20 13:40:24 2024, max compression
```

## Comparing `graphviper-0.0.8.tar` & `graphviper-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.047371 graphviper-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-12 19:38:18.000000 graphviper-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 19:38:18.000000 graphviper-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-12 19:38:22.047371 graphviper-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-12 19:38:18.000000 graphviper-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-12 19:38:18.000000 graphviper-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:38:22.047371 graphviper-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.039371 graphviper-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.039371 graphviper-0.0.8/src/graphviper/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/config/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/config/client.param.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/dask/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/menrva.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/dask/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/plugins/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/dask/plugins/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/graph_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/append.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/coordinate_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/generate_airflow_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/generate_dask_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/graph_tools/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/utils/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.043371 graphviper-0.0.8/src/graphviper/utils/data/.dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/data/.dropbox/file.download.json
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/data/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/data/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/data/remote.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8535 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.047371 graphviper-0.0.8/src/graphviper/utils/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/plugins/worker_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-12 19:38:18.000000 graphviper-0.0.8/src/graphviper/utils/protego.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.047371 graphviper-0.0.8/src/graphviper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-12 19:38:22.000000 graphviper-0.0.8/src/graphviper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-12 19:38:22.000000 graphviper-0.0.8/src/graphviper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:38:22.000000 graphviper-0.0.8/src/graphviper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-12 19:38:22.000000 graphviper-0.0.8/src/graphviper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 19:38:22.000000 graphviper-0.0.8/src/graphviper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:38:22.047371 graphviper-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-12 19:38:18.000000 graphviper-0.0.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-12 19:38:18.000000 graphviper-0.0.8/tests/test_graph_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-20 13:40:17.000000 graphviper-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-20 13:40:17.000000 graphviper-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-20 13:40:24.858764 graphviper-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-20 13:40:17.000000 graphviper-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-20 13:40:17.000000 graphviper-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 13:40:24.858764 graphviper-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.850764 graphviper-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.854764 graphviper-0.0.9/src/graphviper/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.854764 graphviper-0.0.9/src/graphviper/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/config/client.param.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.854764 graphviper-0.0.9/src/graphviper/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/menrva.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.854764 graphviper-0.0.9/src/graphviper/dask/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/plugins/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/dask/plugins/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.854764 graphviper-0.0.9/src/graphviper/graph_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/append.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22296 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/coordinate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/generate_airflow_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/generate_dask_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/graph_tools/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/src/graphviper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/src/graphviper/utils/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/src/graphviper/utils/data/.dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/data/.dropbox/file.download.json
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/data/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/data/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/data/remote.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8535 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/src/graphviper/utils/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/plugins/worker_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-20 13:40:17.000000 graphviper-0.0.9/src/graphviper/utils/protego.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/src/graphviper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-20 13:40:24.000000 graphviper-0.0.9/src/graphviper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-20 13:40:24.000000 graphviper-0.0.9/src/graphviper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 13:40:24.000000 graphviper-0.0.9/src/graphviper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-20 13:40:24.000000 graphviper-0.0.9/src/graphviper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 13:40:24.000000 graphviper-0.0.9/src/graphviper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 13:40:24.858764 graphviper-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-20 13:40:17.000000 graphviper-0.0.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-03-20 13:40:17.000000 graphviper-0.0.9/tests/test_graph_tools.py
```

### Comparing `graphviper-0.0.8/LICENSE.txt` & `graphviper-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/PKG-INFO` & `graphviper-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphviper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Astro Visibility and Image Parallel Execution Reduction 
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `graphviper-0.0.8/README.md` & `graphviper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/pyproject.toml` & `graphviper-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphviper"
-version = "0.0.8"
+version = "0.0.9"
 description = "Astro Visibility and Image Parallel Execution Reduction "
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
```

### Comparing `graphviper-0.0.8/src/graphviper/__init__.py` & `graphviper-0.0.9/src/graphviper/__init__.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/config/client.param.json` & `graphviper-0.0.9/src/graphviper/config/client.param.json`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/dask/client.py` & `graphviper-0.0.9/src/graphviper/dask/client.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/dask/menrva.py` & `graphviper-0.0.9/src/graphviper/dask/menrva.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/dask/plugins/scheduler.py` & `graphviper-0.0.9/src/graphviper/dask/plugins/scheduler.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/dask/plugins/worker.py` & `graphviper-0.0.9/src/graphviper/dask/plugins/worker.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/graph_tools/coordinate_utils.py` & `graphviper-0.0.9/src/graphviper/graph_tools/coordinate_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,20 +321,25 @@
             chunk_indx_start_stop = {}
             # Interpolate all the chunk edges. This is done for performance reasons.
 
             if "data_chunks_edges" not in pc:
                 pc["data_chunks_edges"] = _array_split_edges(pc["data_chunks"])
 
             interp_index = interpolator(pc["data_chunks_edges"]).astype(int)
-            i = 0
 
+            i = 0
             # Split the interp_index for each chunk and fix any boundary issues.
             for chunk_index in sorted(pc["data_chunks"].keys()):
                 if interp_index[i] == -1 and interp_index[i + 1] == -1:
                     chunk_indx_start_stop[chunk_index] = slice(None)
+                    if (pc["data_chunks_edges"][i] < input_data[xds_name][dim][0])  and (pc["data_chunks_edges"][i+1] > input_data[xds_name][dim][-1]):
+                        interp_index[i] = 0
+                        interp_index[i+1] = -2 
+                        chunk_indx_start_stop[chunk_index] = slice(
+                        interp_index[i], interp_index[i + 1] + 1)
                 else:
                     if interp_index[i] == -1:
                         interp_index[i] = 0
                     if interp_index[i + 1] == -1:
                         interp_index[i + 1] = -2
                     chunk_indx_start_stop[chunk_index] = slice(
                         interp_index[i], interp_index[i + 1] + 1
@@ -387,15 +392,16 @@
                         empty_chunk = True
                 else:
                     empty_chunk = True
 
             if (
                 empty_chunk
             ):  # The xds with xds_name has no data for the parallel chunk (no slice on one of the dims).
-                node_task_data_mapping[task_id]["data_selection"][xds_name] = None
+                del node_task_data_mapping[task_id]["data_selection"][xds_name] 
+                #node_task_data_mapping[task_id]["data_selection"][xds_name] = None
 
     return node_task_data_mapping
 
 
 def _array_split(data: Union[list, np.ndarray], n_chunks: int):
     """Takes an input array and splits it into n_chunk arrays which are stored in a dictionary with numbered keys.
```

### Comparing `graphviper-0.0.8/src/graphviper/graph_tools/generate_airflow_workflow.py` & `graphviper-0.0.9/src/graphviper/graph_tools/generate_airflow_workflow.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/graph_tools/generate_dask_workflow.py` & `graphviper-0.0.9/src/graphviper/graph_tools/generate_dask_workflow.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/graph_tools/map.py` & `graphviper-0.0.9/src/graphviper/graph_tools/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import dask
 import datetime
 
 import numpy as np
 import graphviper.utils.logger as logger
 
 from typing import Dict, Union
-from typing import Callable, Any, Tuple, List
+from typing import Callable, Any, Tuple, Dict
 from xradio.vis._processing_set import processing_set
 import copy
 
 
 def map(
     input_data: Union[Dict, processing_set],
     node_task_data_mapping: dict,
     node_task: Callable[..., Any],
     input_params: dict,
     in_memory_compute: bool = False,
     client=None,
     date_time: str = None,
-) -> list:
+) -> Dict:
     """Create a perfectly parallel graph where a node is generated for each item in the :ref:`node_task_data_mapping <node task data mapping>` using the function specified in the ``node_task`` parameter.
 
     Parameters
     ----------
     input_data : Union[Dict, processing_set]
         Can either be a `processing_set <https://github.com/casangi/xradio/blob/main/src/xradio/vis/_processing_set.py>`_ or a Dictionary of `xarray.Datasets <https://docs.xarray.dev/en/stable/generated/xarray.Dataset.html>`_. Only coordinates are needed so no actual data is loaded into memory (except if ``in_memory_compute`` is True).
     node_task_data_mapping :
```

### Comparing `graphviper-0.0.8/src/graphviper/graph_tools/reduce.py` & `graphviper-0.0.9/src/graphviper/graph_tools/reduce.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def reduce(
     graph: list,
     reduce_node_task: Callable[..., Any],
     input_params: Dict,
     mode: {"tree", "single_node"} = "tree",
-) -> list:
+) -> Dict:
     """Appends a reduce step to the graph created by the :func:`graphviper.graph_tools.map`. function.
 
     Parameters
     ----------
     graph : list
         Graph produced by :func:`graphviper.graph_tools.map`.
     reduce_node_task : _type_
```

### Comparing `graphviper-0.0.8/src/graphviper/utils/console.py` & `graphviper-0.0.9/src/graphviper/utils/console.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/data/.dropbox/file.download.json` & `graphviper-0.0.9/src/graphviper/utils/data/.dropbox/file.download.json`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/data/download.py` & `graphviper-0.0.9/src/graphviper/utils/data/download.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/data/dropbox.py` & `graphviper-0.0.9/src/graphviper/utils/data/dropbox.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/data/remote.py` & `graphviper-0.0.9/src/graphviper/utils/data/remote.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/logger.py` & `graphviper-0.0.9/src/graphviper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/parameter.py` & `graphviper-0.0.9/src/graphviper/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/plugins/worker_logger.py` & `graphviper-0.0.9/src/graphviper/utils/plugins/worker_logger.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper/utils/protego.py` & `graphviper-0.0.9/src/graphviper/utils/protego.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/src/graphviper.egg-info/PKG-INFO` & `graphviper-0.0.9/src/graphviper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphviper
-Version: 0.0.8
+Version: 0.0.9
 Summary: Astro Visibility and Image Parallel Execution Reduction 
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `graphviper-0.0.8/src/graphviper.egg-info/SOURCES.txt` & `graphviper-0.0.9/src/graphviper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/tests/test_client.py` & `graphviper-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `graphviper-0.0.8/tests/test_graph_tools.py` & `graphviper-0.0.9/tests/test_graph_tools.py`

 * *Files identical despite different names*

