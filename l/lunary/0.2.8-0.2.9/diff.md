# Comparing `tmp/lunary-0.2.8.tar.gz` & `tmp/lunary-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-0.2.8.tar", max compression
+gzip compressed data, was "lunary-0.2.9.tar", max compression
```

## Comparing `lunary-0.2.8.tar` & `lunary-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0      604 2024-02-24 01:43:56.000000 lunary-0.2.8/README.md
--rw-r--r--   0        0        0    56745 2024-04-01 04:53:20.289919 lunary-0.2.8/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-03-27 12:45:10.024740 lunary-0.2.8/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-09 04:19:24.000000 lunary-0.2.8/lunary/event_queue.py
--rw-r--r--   0        0        0     2384 2024-02-23 21:19:34.000000 lunary-0.2.8/lunary/openai_utils.py
--rw-r--r--   0        0        0      398 2024-02-23 21:19:34.000000 lunary-0.2.8/lunary/parent.py
--rw-r--r--   0        0        0      488 2024-03-27 12:45:08.428090 lunary-0.2.8/lunary/parsers.py
--rw-r--r--   0        0        0      378 2024-03-27 12:45:06.573143 lunary-0.2.8/lunary/tags.py
--rw-r--r--   0        0        0      841 2024-02-23 21:19:34.000000 lunary-0.2.8/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-02-23 21:19:34.000000 lunary-0.2.8/lunary/users.py
--rw-r--r--   0        0        0      747 2024-04-01 04:53:36.708366 lunary-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 lunary-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-0.2.9/README.md
+-rw-r--r--   0        0        0    57082 2024-04-01 15:34:27.919485 lunary-0.2.9/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-0.2.9/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-0.2.9/lunary/event_queue.py
+-rw-r--r--   0        0        0      834 2024-03-03 18:24:22.696583 lunary-0.2.9/lunary/langchain/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      620 2024-03-03 18:23:24.270210 lunary-0.2.9/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-0.2.9/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-0.2.9/lunary/parent.py
+-rw-r--r--   0        0        0      488 2024-03-04 00:09:26.744865 lunary-0.2.9/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-0.2.9/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-0.2.9/lunary/tags.py
+-rw-r--r--   0        0        0      841 2024-03-04 00:09:26.744980 lunary-0.2.9/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-0.2.9/lunary/users.py
+-rw-r--r--   0        0        0      747 2024-04-01 15:34:51.305094 lunary-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 lunary-0.2.9/PKG-INFO
```

### Comparing `lunary-0.2.8/README.md` & `lunary-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/lunary/__init__.py` & `lunary-0.2.9/lunary/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 )
 from .openai_utils import OpenAIUtils
 from .event_queue import EventQueue
 from .consumer import Consumer
 # DO NOT REMOVE `identify` import
 from .users import user_ctx, user_props_ctx, identify # DO NOT REMOVE `identify`` import
 from .tags import tags_ctx, tags  # DO NOT REMOVE `tags` import
-from .parent import parent_ctx, parent # DO NOT REMOVE `parent` import
+from .parent import parent_ctx, parent, get_parent # DO NOT REMOVE `parent` import
+from .project import project_ctx # DO NOT REMOVE `project` import
 from .thread import Thread
 
 DEFAULT_API_URL = "https://api.lunary.ai"
 
 logger = logging.getLogger(__name__)
 
 run_ctx = ContextVar("run_ids", default=None)
@@ -60,27 +61,31 @@
             key: clean_nones(val)
             for key, val in value.items()
             if val is not None
         }
     else:
         return value
 
-def get_parent_run_id(parent_run_id: str, run_type: str, app_id: str):
+def get_parent_run_id(parent_run_id: str, run_type: str, app_id: str, run_id: str, is_openai: bool):
     if parent_run_id == "None":
         parent_run_id = None
 
-    if parent_run_id is not None:
-        return str(create_uuid_from_string(str(parent_run_id) + str(app_id)))
+    if is_openai:
         return str(parent_run_id)
 
-    if parent_ctx.get() and run_type != "thread":
-        return str(parent_ctx.get())
-    
+    parent_from_ctx = get_parent()
+    if parent_from_ctx and run_type != "thread":
+        return str(create_uuid_from_string(str(parent_from_ctx) + str(app_id)))
+
     if run_ctx.get() is not None and str(run_id) != str(run_ctx.get()):
-       return str(run_ctx.get())
+       return str(create_uuid_from_string(str(run_ctx.get()) + str(app_id)))
+
+    if parent_run_id is not None:
+        return str(create_uuid_from_string(str(parent_run_id) + str(app_id)))
+
 
 def create_uuid_from_string(seed_string):
     seed_bytes = seed_string.encode('utf-8')
     sha256_hash = hashlib.sha256()
     sha256_hash.update(seed_bytes)
     hash_hex = sha256_hash.hexdigest()
     uuid_hex = hash_hex[:32]
@@ -106,28 +111,29 @@
     thread_tags=None,
     feedback=None,
     extra=None,
     template_id=None,
     metadata=None,
     runtime=None,
     app_id=None,
-    callback_queue=None
+    callback_queue=None,
+    is_openai=False
 ):
     # Load here in case load_dotenv done after
     APP_ID = (
         app_id or os.environ.get("LUNARY_PUBLIC_KEY") or os.environ.get(
             "LUNARY_APP_ID") or os.environ.get("LLMONITOR_APP_ID")
     )
     VERBOSE = os.environ.get(
         "LUNARY_VERBOSE") or os.environ.get("LLMONITOR_VERBOSE")
 
     if not APP_ID:
         return warnings.warn("LUNARY_PUBLIC_KEY is not set, not sending events")
 
-    parent_run_id = get_parent_run_id(parent_run_id, run_type, app_id=app_id)
+    parent_run_id = get_parent_run_id(parent_run_id, run_type, app_id=app_id, run_id=run_id, is_openai=is_openai)
     
     event = {
         "event": event_name,
         "type": run_type,
         "name": name,
         "userId": user_id or user_ctx.get(),
         "userProps": user_props or user_props_ctx.get(),
@@ -358,14 +364,15 @@
                         "user_id", None) or user_ctx.get() or user_id,
                     user_props=kwargs.pop("user_props", None)
                     or user_props
                     or user_props_ctx.get(),
                     tags=kwargs.pop("tags", None) or tags or tags_ctx.get(),
                     extra=kwargs.get("extra", None),
                     template_id=kwargs.get("extra_headers", {}).get("Template-Id", None),
+                    is_openai=True
                 )
             except Exception as e:
                 handle_internal_error(e)
 
             if kwargs.get("stream") == True:
                 return stream_handler(
                     fn, run_id, name or parsed_input["name"], type, *args, **kwargs
```

### Comparing `lunary-0.2.8/lunary/consumer.py` & `lunary-0.2.9/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/lunary/event_queue.py` & `lunary-0.2.9/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/lunary/openai_utils.py` & `lunary-0.2.9/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/lunary/thread.py` & `lunary-0.2.9/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/lunary/users.py` & `lunary-0.2.9/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-0.2.8/pyproject.toml` & `lunary-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "0.2.8"
+version = "0.2.9"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary/lunary.ai/"
 documentation = "https://lunary.ai/docs/py/usage"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
```

### Comparing `lunary-0.2.8/PKG-INFO` & `lunary-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 0.2.8
+Version: 0.2.9
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary/lunary.ai/
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```

