# Comparing `tmp/streaming_assistants-0.8.0.tar.gz` & `tmp/streaming_assistants-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming_assistants-0.8.0.tar", max compression
+gzip compressed data, was "streaming_assistants-0.9.0.tar", max compression
```

## Comparing `streaming_assistants-0.8.0.tar` & `streaming_assistants-0.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2576 2024-02-01 18:15:42.032983 streaming_assistants-0.8.0/README.md
--rw-r--r--   0        0        0      541 2024-02-01 18:16:18.341755 streaming_assistants-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       26 2024-01-29 17:31:10.604926 streaming_assistants-0.8.0/streaming_assistants/__init__.py
--rw-r--r--   0        0        0    12511 2024-02-01 17:04:23.691294 streaming_assistants-0.8.0/streaming_assistants/patch.py
--rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 streaming_assistants-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2576 2024-02-01 18:15:42.032983 streaming_assistants-0.9.0/README.md
+-rw-r--r--   0        0        0      541 2024-02-01 18:18:24.520436 streaming_assistants-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-01-29 17:31:10.604926 streaming_assistants-0.9.0/streaming_assistants/__init__.py
+-rw-r--r--   0        0        0    12505 2024-02-01 18:17:51.979745 streaming_assistants-0.9.0/streaming_assistants/patch.py
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 streaming_assistants-0.9.0/PKG-INFO
```

### Comparing `streaming_assistants-0.8.0/README.md` & `streaming_assistants-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `streaming_assistants-0.8.0/pyproject.toml` & `streaming_assistants-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streaming-assistants"
-version = "0.8.0"
+version = "0.9.0"
 description = "Streaming enabled Assistants API"
 authors = ["phact <estevezsebastian@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.26.0"
```

### Comparing `streaming_assistants-0.8.0/streaming_assistants/patch.py` & `streaming_assistants-0.9.0/streaming_assistants/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                         MessageListWithStreamingParams,
                     ),
                 ),
             )
             return response
         else:
             # Call the original 'list' method for non-streaming requests
-            return await original_list(self, *args, **kwargs)
+            return await original_list(*args, **kwargs)
 
     # Check if the original function is async and choose the appropriate wrapper
     func_is_async = is_async(original_list)
     wrapper_function = async_list if func_is_async else sync_list
 
     # Set documentation for the wrapper function
     wrapper_function.__doc__ = original_list.__doc__
```

### Comparing `streaming_assistants-0.8.0/PKG-INFO` & `streaming_assistants-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-assistants
-Version: 0.8.0
+Version: 0.9.0
 Summary: Streaming enabled Assistants API
 Author: phact
 Author-email: estevezsebastian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

