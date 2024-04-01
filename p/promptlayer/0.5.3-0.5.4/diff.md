# Comparing `tmp/promptlayer-0.5.3.tar.gz` & `tmp/promptlayer-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlayer-0.5.3.tar", max compression
+gzip compressed data, was "promptlayer-0.5.4.tar", max compression
```

## Comparing `promptlayer-0.5.3.tar` & `promptlayer-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-03-27 16:35:39.466863 promptlayer-0.5.3/LICENSE
--rw-r--r--   0        0        0     3839 2024-03-27 16:35:39.466863 promptlayer-0.5.3/README.md
--rw-r--r--   0        0        0     1110 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/__init__.py
--rw-r--r--   0        0        0       67 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/groups/__init__.py
--rw-r--r--   0        0        0      139 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/groups/groups.py
--rw-r--r--   0        0        0     3736 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/promptlayer.py
--rw-r--r--   0        0        0      205 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/prompts/__init__.py
--rw-r--r--   0        0        0     2348 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/prompts/chat.py
--rw-r--r--   0        0        0     3215 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/prompts/prompts.py
--rw-r--r--   0        0        0       63 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/resources/__init__.py
--rw-r--r--   0        0        0      468 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/resources/base.py
--rw-r--r--   0        0        0      220 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/resources/prompt.py
--rw-r--r--   0        0        0      542 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/templates.py
--rw-r--r--   0        0        0      119 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/track/__init__.py
--rw-r--r--   0        0        0     1525 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/track/track.py
--rw-r--r--   0        0        0       61 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/types/__init__.py
--rw-r--r--   0        0        0     3752 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/types/prompt_template.py
--rw-r--r--   0        0        0    19090 2024-03-27 16:35:39.470862 promptlayer-0.5.3/promptlayer/utils.py
--rw-r--r--   0        0        0      487 2024-03-27 16:35:39.470862 promptlayer-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 promptlayer-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 18:29:27.461644 promptlayer-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3839 2024-04-01 18:29:27.461644 promptlayer-0.5.4/README.md
+-rw-r--r--   0        0        0     1110 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/groups/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/groups/groups.py
+-rw-r--r--   0        0        0     3736 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/promptlayer.py
+-rw-r--r--   0        0        0      205 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/__init__.py
+-rw-r--r--   0        0        0     2348 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/chat.py
+-rw-r--r--   0        0        0     3215 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/prompts/prompts.py
+-rw-r--r--   0        0        0       63 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/__init__.py
+-rw-r--r--   0        0        0      468 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/base.py
+-rw-r--r--   0        0        0      220 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/resources/prompt.py
+-rw-r--r--   0        0        0      542 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/templates.py
+-rw-r--r--   0        0        0      119 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/track/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/track/track.py
+-rw-r--r--   0        0        0       61 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/types/__init__.py
+-rw-r--r--   0        0        0     3752 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/types/prompt_template.py
+-rw-r--r--   0        0        0    21160 2024-04-01 18:29:27.465644 promptlayer-0.5.4/promptlayer/utils.py
+-rw-r--r--   0        0        0      487 2024-04-01 18:29:27.465644 promptlayer-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 promptlayer-0.5.4/PKG-INFO
```

### Comparing `promptlayer-0.5.3/LICENSE` & `promptlayer-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/README.md` & `promptlayer-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/__init__.py` & `promptlayer-0.5.4/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/promptlayer.py` & `promptlayer-0.5.4/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/prompts/chat.py` & `promptlayer-0.5.4/promptlayer/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/prompts/prompts.py` & `promptlayer-0.5.4/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/templates.py` & `promptlayer-0.5.4/promptlayer/templates.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/track/track.py` & `promptlayer-0.5.4/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/types/prompt_template.py` & `promptlayer-0.5.4/promptlayer/types/prompt_template.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.5.3/promptlayer/utils.py` & `promptlayer-0.5.4/promptlayer/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     request_end_time,
     api_key,
     return_pl_id=False,
 ):
     if (
         isinstance(response, types.GeneratorType)
         or isinstance(response, types.AsyncGeneratorType)
-        or type(response).__name__ in ["Stream", "AsyncStream"]
+        or type(response).__name__
+        in ["Stream", "AsyncStream", "AsyncMessageStreamManager"]
     ):
         return GeneratorProxy(
             response,
             {
                 "function_name": function_name,
                 "provider_type": provider_type,
                 "args": args,
@@ -351,30 +352,56 @@
 
     def __iter__(self):
         return self
 
     def __aiter__(self):
         return self
 
+    async def __aenter__(self):
+        api_request_arguments = self.api_request_arugments
+        if hasattr(self.generator, "_AsyncMessageStreamManager__api_request"):
+            return GeneratorProxy(
+                await self.generator._AsyncMessageStreamManager__api_request,
+                api_request_arguments,
+            )
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        pass
+
     async def __anext__(self):
         result = await self.generator.__anext__()
         return self._abstracted_next(result)
 
     def __next__(self):
         result = next(self.generator)
         return self._abstracted_next(result)
 
+    def __getattr__(self, name):
+        if name == "text_stream":  # anthropic async stream
+            return GeneratorProxy(
+                self.generator.text_stream, self.api_request_arugments
+            )
+        return getattr(self.generator, name)
+
     def _abstracted_next(self, result):
         self.results.append(result)
         provider_type = self.api_request_arugments["provider_type"]
-        end_anthropic = provider_type == "anthropic" and result.stop_reason
+        end_anthropic = False
+        if provider_type == "anthropic":
+            if hasattr(result, "stop_reason"):
+                end_anthropic = result.stop_reason
+            elif hasattr(result, "message"):
+                end_anthropic = result.message.stop_reason
+            elif hasattr(result, "type") and result.type == "message_stop":
+                end_anthropic = True
         end_openai = provider_type == "openai" and (
             result.choices[0].finish_reason == "stop"
             or result.choices[0].finish_reason == "length"
         )
+
         if end_anthropic or end_openai:
             request_id = promptlayer_api_request(
                 self.api_request_arugments["function_name"],
                 self.api_request_arugments["provider_type"],
                 self.api_request_arugments["args"],
                 self.api_request_arugments["kwargs"],
                 self.api_request_arugments["tags"],
@@ -391,17 +418,36 @@
         return result
 
     def cleaned_result(self):
         provider_type = self.api_request_arugments["provider_type"]
         if provider_type == "anthropic":
             response = ""
             for result in self.results:
-                response = f"{response}{result.completion}"
-            final_result = deepcopy(self.results[-1])
-            final_result.completion = response
+                if hasattr(result, "completion"):
+                    response = f"{response}{result.completion}"
+                elif hasattr(result, "message") and isinstance(result.message, str):
+                    response = f"{response}{result.message}"
+                elif hasattr(result, "content_block") and hasattr(
+                    result.content_block, "text"
+                ):
+                    response = f"{response}{result.content_block.text}"
+                elif hasattr(result, "delta") and hasattr(result.delta, "text"):
+                    response = f"{response}{result.delta.text}"
+            if (
+                hasattr(self.results[-1], "type")
+                and self.results[-1].type == "message_stop"
+            ):  # this is a message stream and not the correct event
+                final_result = deepcopy(self.results[0].message)
+                final_result.usage = None
+                content_block = deepcopy(self.results[1].content_block)
+                content_block.text = response
+                final_result.content = [content_block]
+            else:
+                final_result = deepcopy(self.results[-1])
+                final_result.completion = response
             return final_result
         if hasattr(self.results[0].choices[0], "text"):  # this is regular completion
             response = ""
             for result in self.results:
                 response = f"{response}{result.choices[0].text}"
             final_result = deepcopy(self.results[-1])
             final_result.choices[0].text = response
```

### Comparing `promptlayer-0.5.3/PKG-INFO` & `promptlayer-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.5.3
+Version: 0.5.4
 Summary: PromptLayer is a platform for prompt engineering and tracks your LLM requests.
 License: Apache-2.0
 Author: Magniv
 Author-email: hello@magniv.io
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.5.3 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.5.4 Summary: PromptLayer is
 a platform for prompt engineering and tracks your LLM requests. License:
 Apache-2.0 Author: Magniv Author-email: hello@magniv.io Requires-Python:
 >=3.8.1,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: requests (>=2.31.0,<3.0.0)
```

