# Comparing `tmp/outpostkit-0.0.7.tar.gz` & `tmp/outpostkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outpostkit-0.0.7.tar", last modified: Wed Jan 31 11:02:43 2024, max compression
+gzip compressed data, was "outpostkit-0.0.9.tar", last modified: Wed Jan 31 11:17:12 2024, max compression
```

## Comparing `outpostkit-0.0.7.tar` & `outpostkit-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:02:43.380497 outpostkit-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-31 11:02:35.000000 outpostkit-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-01-31 11:02:43.380497 outpostkit-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-31 11:02:35.000000 outpostkit-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:02:43.376497 outpostkit-0.0.7/outpostkit/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:02:43.380497 outpostkit-0.0.7/outpostkit/template_gen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/template_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-01-31 11:02:35.000000 outpostkit-0.0.7/outpostkit/template_gen/gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:02:43.380497 outpostkit-0.0.7/outpostkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-01-31 11:02:43.000000 outpostkit-0.0.7/outpostkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-31 11:02:43.000000 outpostkit-0.0.7/outpostkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 11:02:43.000000 outpostkit-0.0.7/outpostkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-31 11:02:43.000000 outpostkit-0.0.7/outpostkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-31 11:02:43.000000 outpostkit-0.0.7/outpostkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-01-31 11:02:35.000000 outpostkit-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 11:02:43.380497 outpostkit-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:17:12.643536 outpostkit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-31 11:17:00.000000 outpostkit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-01-31 11:17:12.643536 outpostkit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-31 11:17:00.000000 outpostkit-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:17:12.639536 outpostkit-0.0.9/outpostkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:17:12.639536 outpostkit-0.0.9/outpostkit/template_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/template_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-01-31 11:17:00.000000 outpostkit-0.0.9/outpostkit/template_gen/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 11:17:12.639536 outpostkit-0.0.9/outpostkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-01-31 11:17:12.000000 outpostkit-0.0.9/outpostkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-31 11:17:12.000000 outpostkit-0.0.9/outpostkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 11:17:12.000000 outpostkit-0.0.9/outpostkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-31 11:17:12.000000 outpostkit-0.0.9/outpostkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-31 11:17:12.000000 outpostkit-0.0.9/outpostkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-01-31 11:17:00.000000 outpostkit-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 11:17:12.643536 outpostkit-0.0.9/setup.cfg
```

### Comparing `outpostkit-0.0.7/LICENSE` & `outpostkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/PKG-INFO` & `outpostkit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outpostkit
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for Outpost
 Author: Outpost Innovations, Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `outpostkit-0.0.7/README.md` & `outpostkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/client.py` & `outpostkit-0.0.9/outpostkit/client.py`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/files.py` & `outpostkit-0.0.9/outpostkit/files.py`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/inference.py` & `outpostkit-0.0.9/outpostkit/inference.py`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/json.py` & `outpostkit-0.0.9/outpostkit/json.py`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/resource.py` & `outpostkit-0.0.9/outpostkit/resource.py`

 * *Files identical despite different names*

### Comparing `outpostkit-0.0.7/outpostkit/template_gen/gen.py` & `outpostkit-0.0.9/outpostkit/template_gen/gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import json
 import os
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from asyncio import Semaphore
 from tempfile import TemporaryDirectory
 
 from fastapi import Request
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from transformers import pipeline as transformers_pipeline
 
 from outpostkit.exceptions import OutpostError
 from outpostkit.template_gen.templates.audio_classification import (
     request_parser as audio_classification_request_parser,
 )
+from outpostkit.template_gen.templates.text_classification import (
+    request_parser as text_classification_request_parser,
+)
 from outpostkit.template_gen.utils.precision import parse_dtype
 from outpostkit.template_gen.utils.repo import clone_outpost_repo
 
-task_type_handlers = {"audio-classification": audio_classification_request_parser}
+task_type_handlers = {"audio-classification": audio_classification_request_parser,"text-classification":text_classification_request_parser}
 
 
 def add_generic_template_args(parser: ArgumentParser) -> ArgumentParser:
     parser.add_argument(
         "--max-concurrent-inferences",
         type=int,
         default=1,
@@ -61,18 +64,15 @@
     parser.add_argument("--model-kwargs", type=json.loads, default=None, help="kwargs")
     parser.add_argument("--task-type", type=str, default=None, help="task type")
     parser.add_argument("--model-store", type=str, default="/model", help="task type")
     parser.add_argument("--device-map", type=str, default="auto", help="device-map")
     return parser
 
 
-def create_template_class_from_args(parser: ArgumentParser):
-    args, unknown = parser.parse_known_args()
-    if unknown:
-        print("ignoring unknown arguements: ", unknown)
+def create_template_class_from_args(args:Namespace):
     model_dir: str
     init_f = None
     if args.load_source == "huggingface":
         model_dir = args.model_name
 
         def init_funct(self):
             token = None
@@ -154,8 +154,11 @@
     )
     return TemplateClass
 
 
 def gen_inference_template():
     parser = ArgumentParser("Templated Task Type class generator")
     parser = add_generic_template_args(parser)
-    return create_template_class_from_args(parser=parser)
+    args, unknown = parser.parse_known_args()
+    if unknown:
+        print("ignoring unknown arguements: ", unknown)
+    return create_template_class_from_args(args=args)
```

### Comparing `outpostkit-0.0.7/outpostkit.egg-info/PKG-INFO` & `outpostkit-0.0.9/outpostkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outpostkit
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python client for Outpost
 Author: Outpost Innovations, Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `outpostkit-0.0.7/pyproject.toml` & `outpostkit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "outpostkit"
-version = "0.0.7"
+version = "0.0.9"
 description = "Python client for Outpost"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Outpost Innovations, Inc." }]
 requires-python = ">=3.8"
 dependencies = [
     "httpx>=0.21.0,<1",
```

