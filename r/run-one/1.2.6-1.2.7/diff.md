# Comparing `tmp/run_one-1.2.6.tar.gz` & `tmp/run_one-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.2.6.tar", max compression
+gzip compressed data, was "run_one-1.2.7.tar", max compression
```

## Comparing `run_one-1.2.6.tar` & `run_one-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-02-08 16:37:15.112619 run_one-1.2.6/LICENSE
--rw-r--r--   0        0        0     2514 2024-02-08 16:37:15.112619 run_one-1.2.6/README.md
--rw-r--r--   0        0        0      941 2024-02-08 16:37:15.112619 run_one-1.2.6/pyproject.toml
--rw-r--r--   0        0        0      345 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/__init__.py
--rw-r--r--   0        0        0      277 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     2166 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1422 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     4945 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0     1710 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/TH2EstoreHandler.py
--rw-r--r--   0        0        0        0 2024-02-08 16:37:15.112619 run_one-1.2.6/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1434 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     7601 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/util/__init__.py
--rw-r--r--   0        0        0     1743 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/util/config.py
--rw-r--r--   0        0        0     5646 2024-02-08 16:37:15.116619 run_one-1.2.6/run_one/util/util.py
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 run_one-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 13:00:42.752598 run_one-1.2.7/LICENSE
+-rw-r--r--   0        0        0     2514 2024-04-01 13:00:42.752598 run_one-1.2.7/README.md
+-rw-r--r--   0        0        0      941 2024-04-01 13:00:42.752598 run_one-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0      345 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     2166 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1422 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     4945 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0     1710 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/TH2EstoreHandler.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1593 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     7900 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/util/config.py
+-rw-r--r--   0        0        0     5646 2024-04-01 13:00:42.752598 run_one-1.2.7/run_one/util/util.py
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 run_one-1.2.7/PKG-INFO
```

### Comparing `run_one-1.2.6/LICENSE` & `run_one-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/README.md` & `run_one-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/pyproject.toml` & `run_one-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.2.6"
+version = "1.2.7"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.2.6/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.2.7/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.2.7/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.2.7/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/run_one/action_handlers/TH2EstoreHandler.py` & `run_one-1.2.7/run_one/action_handlers/TH2EstoreHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/run_one/processors/th2_processor.py` & `run_one-1.2.7/run_one/processors/th2_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime, timezone
 from itertools import chain
 import logging
 import time
 from typing import Callable, TypeVar
 
 from th2_grpc_common.common_pb2 import EventBatch
 from th2_common.schema.event.event_batch_router import EventBatchRouter
@@ -92,18 +93,23 @@
         class_instance_mapping = {x: x(self._config, self._grpc_router, self._event_router)
                                   for x in set(action_handlers.values())}
         self.processed_actions: dict[str, HandlerType] = {action: class_instance_mapping[action_handler]
                                                           for action, action_handler in action_handlers.items()}
 
         self.logger = logging.getLogger()
 
-    def process(self, matrices_data: dict[str, dict[str, list[Action]]], time_function: Callable = generate_time):
+    def process(self, matrices_data: dict[str, dict[str, list[Action]]],
+                time_function: Callable = generate_time) -> list[tuple[datetime, datetime]]:
+
+        processing_times = []
 
         for matrix_name, test_cases in matrices_data.items():
 
+            start = datetime.now(timezone.utc)
+
             logging.info(f'Processing {matrix_name} matrix')
 
             matrix_root_event_id = create_event_id(book_name=self._config.book, scope=self._config.scope,
                                                    start_timestamp=create_timestamp(self._config.timestamp_shift))
             matrix_root_event = EventBatch(events=[create_event(name=matrix_name,
                                                                 event_id=matrix_root_event_id,
                                                                 parent_id=self.root_event_id,
@@ -151,9 +157,14 @@
                     time.sleep(self._config.sleep)
 
                 for handler in self.processed_actions.values():
                     handler.on_test_case_end()
 
                 Context.clear()
 
+            end = datetime.now(timezone.utc)
+            processing_times.append((start, end))
+
+        return processing_times
+
     def close(self):
         self._common_factory.close()
```

### Comparing `run_one-1.2.6/run_one/util/config.py` & `run_one-1.2.7/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/run_one/util/util.py` & `run_one-1.2.7/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.2.6/PKG-INFO` & `run_one-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.2.6
+Version: 1.2.7
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

