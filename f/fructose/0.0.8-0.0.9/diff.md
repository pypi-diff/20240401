# Comparing `tmp/fructose-0.0.8.tar.gz` & `tmp/fructose-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fructose-0.0.8.tar", last modified: Mon Feb 26 16:48:25 2024, max compression
+gzip compressed data, was "fructose-0.0.9.tar", last modified: Tue Feb 27 10:30:11 2024, max compression
```

## Comparing `fructose-0.0.8.tar` & `fructose-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-26 16:48:25.846765 fructose-0.0.8/
--rw-r--r--   0 nik        (501) staff       (20)      249 2024-02-26 16:48:25.846651 fructose-0.0.8/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)     4874 2024-02-26 14:25:11.000000 fructose-0.0.8/README.md
--rw-r--r--   0 nik        (501) staff       (20)       38 2024-02-26 16:48:25.846819 fructose-0.0.8/setup.cfg
--rw-r--r--   0 nik        (501) staff       (20)      421 2024-02-26 16:47:33.000000 fructose-0.0.8/setup.py
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-26 16:48:25.845025 fructose-0.0.8/src/
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-26 16:48:25.845875 fructose-0.0.8/src/fructose/
--rw-r--r--   0 nik        (501) staff       (20)       18 2024-02-26 14:29:37.000000 fructose-0.0.8/src/fructose/__init__.py
--rw-r--r--   0 nik        (501) staff       (20)     6931 2024-02-26 16:47:58.000000 fructose-0.0.8/src/fructose/ai.py
--rw-r--r--   0 nik        (501) staff       (20)     2258 2024-02-23 04:22:28.000000 fructose-0.0.8/src/fructose/function_helpers.py
--rw-r--r--   0 nik        (501) staff       (20)     6127 2024-02-20 20:45:17.000000 fructose-0.0.8/src/fructose/type_parser.py
-drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-26 16:48:25.846504 fructose-0.0.8/src/fructose.egg-info/
--rw-r--r--   0 nik        (501) staff       (20)      249 2024-02-26 16:48:25.000000 fructose-0.0.8/src/fructose.egg-info/PKG-INFO
--rw-r--r--   0 nik        (501) staff       (20)      302 2024-02-26 16:48:25.000000 fructose-0.0.8/src/fructose.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (501) staff       (20)        1 2024-02-26 16:48:25.000000 fructose-0.0.8/src/fructose.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (501) staff       (20)       14 2024-02-26 16:48:25.000000 fructose-0.0.8/src/fructose.egg-info/requires.txt
--rw-r--r--   0 nik        (501) staff       (20)        9 2024-02-26 16:48:25.000000 fructose-0.0.8/src/fructose.egg-info/top_level.txt
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.264917 fructose-0.0.9/
+-rw-r--r--   0 nik        (501) staff       (20)       50 2024-02-27 10:30:09.000000 fructose-0.0.9/MANIFEST.in
+-rw-r--r--   0 nik        (501) staff       (20)      249 2024-02-27 10:30:11.264819 fructose-0.0.9/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)     4874 2024-02-26 14:25:11.000000 fructose-0.0.9/README.md
+-rw-r--r--   0 nik        (501) staff       (20)       38 2024-02-27 10:30:11.264958 fructose-0.0.9/setup.cfg
+-rw-r--r--   0 nik        (501) staff       (20)      452 2024-02-27 10:29:56.000000 fructose-0.0.9/setup.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.262719 fructose-0.0.9/src/
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.263777 fructose-0.0.9/src/fructose/
+-rw-r--r--   0 nik        (501) staff       (20)       18 2024-02-26 14:29:37.000000 fructose-0.0.9/src/fructose/__init__.py
+-rw-r--r--   0 nik        (501) staff       (20)     7317 2024-02-27 10:27:28.000000 fructose-0.0.9/src/fructose/ai.py
+-rw-r--r--   0 nik        (501) staff       (20)     2258 2024-02-23 04:22:28.000000 fructose-0.0.9/src/fructose/function_helpers.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.264557 fructose-0.0.9/src/fructose/templates/
+-rw-r--r--   0 nik        (501) staff       (20)        0 2024-02-26 14:20:17.000000 fructose-0.0.9/src/fructose/templates/__init__.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.264677 fructose-0.0.9/src/fructose/templates/__pycache__/
+-rw-r--r--   0 nik        (501) staff       (20)      156 2024-02-26 14:21:16.000000 fructose-0.0.9/src/fructose/templates/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nik        (501) staff       (20)      556 2024-02-20 22:41:29.000000 fructose-0.0.9/src/fructose/templates/chain_of_thought_json.jinja
+-rw-r--r--   0 nik        (501) staff       (20)     6127 2024-02-20 20:45:17.000000 fructose-0.0.9/src/fructose/type_parser.py
+drwxr-xr-x   0 nik        (501) staff       (20)        0 2024-02-27 10:30:11.264352 fructose-0.0.9/src/fructose.egg-info/
+-rw-r--r--   0 nik        (501) staff       (20)      249 2024-02-27 10:30:11.000000 fructose-0.0.9/src/fructose.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (501) staff       (20)      459 2024-02-27 10:30:11.000000 fructose-0.0.9/src/fructose.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (501) staff       (20)        1 2024-02-27 10:30:11.000000 fructose-0.0.9/src/fructose.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (501) staff       (20)       14 2024-02-27 10:30:11.000000 fructose-0.0.9/src/fructose.egg-info/requires.txt
+-rw-r--r--   0 nik        (501) staff       (20)        9 2024-02-27 10:30:11.000000 fructose-0.0.9/src/fructose.egg-info/top_level.txt
```

### Comparing `fructose-0.0.8/README.md` & `fructose-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fructose-0.0.8/src/fructose/ai.py` & `fructose-0.0.9/src/fructose/ai.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import wraps
 import inspect
 import json
 import os
-from typing import Any, Type, TypeVar
+from typing import Any, ForwardRef, Type, TypeVar, get_type_hints
 from openai.types.chat import ChatCompletionMessageParam, ChatCompletionSystemMessageParam, ChatCompletionUserMessageParam, ChatCompletionToolMessageParam
 from pathlib import Path
 from fructose import type_parser
 from . import function_helpers
 import openai
 from jinja2 import Environment, PackageLoader, FileSystemLoader, select_autoescape, StrictUndefined
 
@@ -127,39 +127,19 @@
             ]
 
             if debug:
                 print(f"\033[91mTools: {tools}\033[0m")
 
 
         def decorator(func):
-            @wraps(func)
-            def wrapper(*args, **kwargs):
-                labeled_arguments = function_helpers.collect_arguments(func, args, kwargs)
-                rendered_prompt = self._render_prompt(labeled_arguments)
-
-                messages = [
-                    ChatCompletionSystemMessageParam(
-                        role="system",
-                        content=rendered_system
-                    ),
-                    ChatCompletionUserMessageParam(
-                        role="user",
-                        content=rendered_prompt
-                    )
-                ]
-                raw_result = self._call_llm(messages, tools, uses, debug)
-                result = self._parse_llm_result(raw_result, inspect.signature(func).return_annotation)
-
-                return result
-
             def _render_system(func_doc_string: str, return_type_str: str ) -> str:
                 if _template is None:
                     # loader=PackageLoader("fructose", "templates")
                     p = Path(__file__).parent / 'templates'
-                    loader = FileSystemLoader(p)
+                    loader=FileSystemLoader(p)
                 else:
                     loader=FileSystemLoader(searchpath="./")
 
                 jinja_env = Environment(
                     loader=loader,
                     undefined=StrictUndefined
                     # autoescape=select_autoescape()
@@ -171,18 +151,45 @@
                     .render(func_doc_string=func_doc_string, return_type_string=return_type_str)\
                     .strip()
                 
                 if "random" in _flavors:
                     system += "\n\nRandom seed: " + str(os.urandom(16)) + "\n\n"
 
                 return system
-            
-            return_annotation = inspect.signature(func).return_annotation
-            _validate_return_type_for_function(func.__name__, return_annotation)
 
-            return_type_str = type_parser.type_to_string(return_annotation)
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                type_hints = get_type_hints(func)
+                return_annotation = type_hints.get('return', inspect.Signature.empty)
+                _validate_return_type_for_function(func.__name__, return_annotation)
+
+                return_type_str = type_parser.type_to_string(return_annotation)
+
+                rendered_system = _render_system(func.__doc__, return_type_str)
+
+                labeled_arguments = function_helpers.collect_arguments(func, args, kwargs)
+                rendered_prompt = self._render_prompt(labeled_arguments)
+
+                messages = [
+                    ChatCompletionSystemMessageParam(
+                        role="system",
+                        content=rendered_system
+                    ),
+                    ChatCompletionUserMessageParam(
+                        role="user",
+                        content=rendered_prompt
+                    )
+                ]
+                raw_result = self._call_llm(messages, tools, uses, debug)
+                result = self._parse_llm_result(raw_result, return_annotation)
+
+                return result
+
+            return_annotation = inspect.signature(func).return_annotation
 
-            rendered_system = _render_system(func.__doc__, return_type_str)
+            # if the return type is a string, we assume it's a forward reference and delay the validation
+            if not isinstance(return_annotation, str):
+                _validate_return_type_for_function(func.__name__, return_annotation)
             
             return wrapper
         
         return decorator
```

### Comparing `fructose-0.0.8/src/fructose/function_helpers.py` & `fructose-0.0.9/src/fructose/function_helpers.py`

 * *Files identical despite different names*

### Comparing `fructose-0.0.8/src/fructose/type_parser.py` & `fructose-0.0.9/src/fructose/type_parser.py`

 * *Files identical despite different names*

