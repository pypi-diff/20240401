# Comparing `tmp/vision_agent-0.0.41.tar.gz` & `tmp/vision_agent-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.0.41.tar", max compression
+gzip compressed data, was "vision_agent-0.0.42.tar", max compression
```

## Comparing `vision_agent-0.0.41.tar` & `vision_agent-0.0.42.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-03-29 18:29:39.365148 vision_agent-0.0.41/LICENSE
--rw-r--r--   0        0        0     4175 2024-03-29 18:29:39.365148 vision_agent-0.0.41/README.md
--rw-r--r--   0        0        0     2166 2024-03-29 18:29:39.909148 vision_agent-0.0.41/pyproject.toml
--rw-r--r--   0        0        0      229 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      306 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4493 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10101 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    17469 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     6151 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5122 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/emb/emb.py
--rw-r--r--   0        0        0     4420 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/image_utils.py
--rw-r--r--   0        0        0       32 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     3957 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       51 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0     8052 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      235 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1416 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    23447 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7476 2024-03-29 18:29:39.377148 vision_agent-0.0.41/vision_agent/tools/video.py
--rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 vision_agent-0.0.41/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 20:46:10.548754 vision_agent-0.0.42/LICENSE
+-rw-r--r--   0        0        0     4175 2024-04-01 20:46:10.548754 vision_agent-0.0.42/README.md
+-rw-r--r--   0        0        0     2166 2024-04-01 20:46:11.104759 vision_agent-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      306 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4493 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10101 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    17449 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     6151 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5122 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0     4420 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       32 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       51 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0     8438 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      235 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    23447 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7476 2024-04-01 20:46:10.560754 vision_agent-0.0.42/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     5324 1970-01-01 00:00:00.000000 vision_agent-0.0.42/PKG-INFO
```

### Comparing `vision_agent-0.0.41/LICENSE` & `vision_agent-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/README.md` & `vision_agent-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/pyproject.toml` & `vision_agent-0.0.42/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.0.41"
+version = "0.0.42"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.0.41/vision_agent/agent/easytool.py` & `vision_agent-0.0.42/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.0.42/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/agent/reflexion.py` & `vision_agent-0.0.42/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.0.42/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/agent/vision_agent.py` & `vision_agent-0.0.42/vision_agent/agent/vision_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,24 +252,22 @@
     reflections: str,
 ) -> Tuple[Dict, str]:
     tool_id = choose_tool(
         model, question, {k: v["description"] for k, v in tools.items()}, reflections
     )
     if tool_id is None:
         return {}, ""
-    _LOGGER.info(f"\t(Tool ID, name): ({tool_id}, {tools[tool_id]['name']})")
 
     tool_instructions = tools[tool_id]
     tool_usage = tool_instructions["usage"]
     tool_name = tool_instructions["name"]
 
     parameters = choose_parameter(
         model, question, tool_usage, previous_log, reflections
     )
-    _LOGGER.info(f"\tParameters: {parameters} for {tool_name}")
     if parameters is None:
         return {}, ""
     tool_results = {"task": question, "tool_name": tool_name, "parameters": parameters}
 
     _LOGGER.info(
         f"""Going to run the following tool(s) in sequence:
 {tabulate([tool_results], headers="keys", tablefmt="mixed_grid")}"""
@@ -286,15 +284,15 @@
                 call_results.append(function_call(tools[tool_id]["class"], parameters))
         return call_results
 
     call_results = parse_tool_results(tool_results)
     tool_results["call_results"] = call_results
 
     call_results_str = str(call_results)
-    _LOGGER.info(f"\tCall Results: {call_results_str}")
+    # _LOGGER.info(f"\tCall Results: {call_results_str}")
     return tool_results, call_results_str
 
 
 def create_tasks(
     task_model: Union[LLM, LMM], question: str, tools: Dict[int, Any], reflections: str
 ) -> List[Dict]:
     tasks = task_decompose(
@@ -340,15 +338,17 @@
     ):
         return reflect_model(prompt, image=image)  # type: ignore
     return reflect_model(prompt)
 
 
 def parse_reflect(reflect: str) -> bool:
     # GPT-4V has a hard time following directions, so make the criteria less strict
-    return "finish" in reflect.lower() and len(reflect) < 100
+    return (
+        "finish" in reflect.lower() and len(reflect) < 100
+    ) or "finish" in reflect.lower()[-10:]
 
 
 def visualize_result(all_tool_results: List[Dict]) -> List[str]:
     image_to_data: Dict[str, Dict] = {}
     for tool_result in all_tool_results:
         if not tool_result["tool_name"] in ["grounding_sam_", "grounding_dino_"]:
             continue
@@ -419,18 +419,24 @@
         task_model: Optional[Union[LLM, LMM]] = None,
         answer_model: Optional[Union[LLM, LMM]] = None,
         reflect_model: Optional[Union[LLM, LMM]] = None,
         max_retries: int = 2,
         verbose: bool = False,
     ):
         self.task_model = (
-            OpenAILLM(json_mode=True) if task_model is None else task_model
+            OpenAILLM(json_mode=True, temperature=0.1)
+            if task_model is None
+            else task_model
+        )
+        self.answer_model = (
+            OpenAILLM(temperature=0.1) if answer_model is None else answer_model
+        )
+        self.reflect_model = (
+            OpenAILMM(temperature=0.1) if reflect_model is None else reflect_model
         )
-        self.answer_model = OpenAILLM() if answer_model is None else answer_model
-        self.reflect_model = OpenAILMM() if reflect_model is None else reflect_model
         self.max_retries = max_retries
 
         self.tools = TOOLS
         if verbose:
             _LOGGER.setLevel(logging.INFO)
 
     def __call__(
@@ -462,40 +468,39 @@
         reflections = ""
         final_answer = ""
         all_tool_results: List[Dict] = []
 
         for _ in range(self.max_retries):
             task_list = create_tasks(self.task_model, question, self.tools, reflections)
 
-            _LOGGER.info(f"Task Dependency: {task_list}")
             task_depend = {"Original Quesiton": question}
             previous_log = ""
             answers = []
             for task in task_list:
                 task_depend[task["id"]] = {"task": task["task"], "answer": "", "call_result": ""}  # type: ignore
             all_tool_results = []
 
             for task in task_list:
                 task_str = task["task"]
                 previous_log = str(task_depend)
-                _LOGGER.info(f"\tSubtask: {task_str}")
                 tool_results, call_results = retrieval(
                     self.task_model,
                     task_str,
                     self.tools,
                     previous_log,
                     reflections,
                 )
                 answer = answer_generate(
                     self.answer_model, task_str, call_results, previous_log, reflections
                 )
 
                 tool_results["answer"] = answer
                 all_tool_results.append(tool_results)
 
+                _LOGGER.info(f"\tCall Result: {call_results}")
                 _LOGGER.info(f"\tAnswer: {answer}")
                 answers.append({"task": task_str, "answer": answer})
                 task_depend[task["id"]]["answer"] = answer  # type: ignore
                 task_depend[task["id"]]["call_result"] = call_results  # type: ignore
             final_answer = answer_summarize(
                 self.answer_model, question, answers, reflections
             )
@@ -506,15 +511,15 @@
                 self.reflect_model,
                 question,
                 self.tools,
                 all_tool_results,
                 final_answer,
                 visualized_images[0] if len(visualized_images) > 0 else image,
             )
-            _LOGGER.info(f"\tReflection: {reflection}")
+            _LOGGER.info(f"Reflection: {reflection}")
             if parse_reflect(reflection):
                 break
             else:
                 reflections += reflection
 
         return final_answer, all_tool_results
```

### Comparing `vision_agent-0.0.41/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.0.42/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/data/data.py` & `vision_agent-0.0.42/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/emb/emb.py` & `vision_agent-0.0.42/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/image_utils.py` & `vision_agent-0.0.42/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/llm/llm.py` & `vision_agent-0.0.42/vision_agent/llm/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from abc import ABC, abstractmethod
-from typing import Callable, Dict, List, Mapping, Union, cast
+from typing import Any, Callable, Dict, List, Mapping, Union, cast
 
 from openai import OpenAI
 
 from vision_agent.tools import (
     CHOOSE_PARAMS,
     CLIP,
     SYSTEM_PROMPT,
@@ -27,38 +27,41 @@
         pass
 
 
 class OpenAILLM(LLM):
     r"""An LLM class for any OpenAI LLM model."""
 
     def __init__(
-        self, model_name: str = "gpt-4-turbo-preview", json_mode: bool = False
+        self,
+        model_name: str = "gpt-4-turbo-preview",
+        json_mode: bool = False,
+        **kwargs: Any
     ):
         self.model_name = model_name
         self.client = OpenAI()
-        self.json_mode = json_mode
+        self.kwargs = kwargs
+        if json_mode:
+            self.kwargs["response_format"] = {"type": "json_object"}
 
     def generate(self, prompt: str) -> str:
-        kwargs = {"response_format": {"type": "json_object"}} if self.json_mode else {}
         response = self.client.chat.completions.create(
             model=self.model_name,
             messages=[
                 {"role": "user", "content": prompt},
             ],
-            **kwargs,  # type: ignore
+            **self.kwargs,
         )
 
         return cast(str, response.choices[0].message.content)
 
     def chat(self, chat: List[Dict[str, str]]) -> str:
-        kwargs = {"response_format": {"type": "json_object"}} if self.json_mode else {}
         response = self.client.chat.completions.create(
             model=self.model_name,
             messages=chat,  # type: ignore
-            **kwargs,
+            **self.kwargs,
         )
 
         return cast(str, response.choices[0].message.content)
 
     def __call__(self, input: Union[str, List[Dict[str, str]]]) -> str:
         if isinstance(input, str):
             return self.generate(input)
```

### Comparing `vision_agent-0.0.41/vision_agent/lmm/lmm.py` & `vision_agent-0.0.42/vision_agent/lmm/lmm.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,19 +93,23 @@
         return cast(str, resp_json["data"])
 
 
 class OpenAILMM(LMM):
     r"""An LMM class for the OpenAI GPT-4 Vision model."""
 
     def __init__(
-        self, model_name: str = "gpt-4-vision-preview", max_tokens: int = 1024
+        self,
+        model_name: str = "gpt-4-vision-preview",
+        max_tokens: int = 1024,
+        **kwargs: Any,
     ):
         self.model_name = model_name
         self.max_tokens = max_tokens
         self.client = OpenAI()
+        self.kwargs = kwargs
 
     def __call__(
         self,
         input: Union[str, List[Dict[str, str]]],
         image: Optional[Union[str, Path]] = None,
     ) -> str:
         if isinstance(input, str):
@@ -119,27 +123,34 @@
         for c in chat:
             fixed_c = {"role": c["role"]}
             fixed_c["content"] = [{"type": "text", "text": c["content"]}]  # type: ignore
             fixed_chat.append(fixed_c)
 
         if image:
             extension = Path(image).suffix
+            if extension.lower() == ".jpeg" or extension.lower() == ".jpg":
+                extension = "jpg"
+            elif extension.lower() == ".png":
+                extension = "png"
+            else:
+                raise ValueError(f"Unsupported image extension: {extension}")
+
             encoded_image = encode_image(image)
             fixed_chat[0]["content"].append(  # type: ignore
                 {
                     "type": "image_url",
                     "image_url": {
                         "url": f"data:image/{extension};base64,{encoded_image}",
                         "detail": "low",
                     },
                 },
             )
 
         response = self.client.chat.completions.create(
-            model=self.model_name, messages=fixed_chat, max_tokens=self.max_tokens  # type: ignore
+            model=self.model_name, messages=fixed_chat, max_tokens=self.max_tokens, **self.kwargs  # type: ignore
         )
 
         return cast(str, response.choices[0].message.content)
 
     def generate(self, prompt: str, image: Optional[Union[str, Path]] = None) -> str:
         message: List[Dict[str, Any]] = [
             {
@@ -159,15 +170,15 @@
                         "url": f"data:image/{extension};base64,{encoded_image}",
                         "detail": "low",
                     },
                 },
             )
 
         response = self.client.chat.completions.create(
-            model=self.model_name, messages=message, max_tokens=self.max_tokens  # type: ignore
+            model=self.model_name, messages=message, max_tokens=self.max_tokens, **self.kwargs  # type: ignore
         )
         return cast(str, response.choices[0].message.content)
 
     def generate_classifier(self, question: str) -> Callable:
         api_doc = CLIP.description + "\n" + str(CLIP.usage)
         prompt = CHOOSE_PARAMS.format(api_doc=api_doc, question=question)
         response = self.client.chat.completions.create(
```

### Comparing `vision_agent-0.0.41/vision_agent/tools/prompts.py` & `vision_agent-0.0.42/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/tools/tools.py` & `vision_agent-0.0.42/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/vision_agent/tools/video.py` & `vision_agent-0.0.42/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.0.41/PKG-INFO` & `vision_agent-0.0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.0.41
+Version: 0.0.42
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

