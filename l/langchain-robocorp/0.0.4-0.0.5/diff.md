# Comparing `tmp/langchain_robocorp-0.0.4.tar.gz` & `tmp/langchain_robocorp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_robocorp-0.0.4.tar", max compression
+gzip compressed data, was "langchain_robocorp-0.0.5.tar", max compression
```

## Comparing `langchain_robocorp-0.0.4.tar` & `langchain_robocorp-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-03-20 20:19:28.729232 langchain_robocorp-0.0.4/LICENSE
--rw-r--r--   0        0        0      336 2024-03-20 20:19:28.729232 langchain_robocorp-0.0.4/README.md
--rw-r--r--   0        0        0      102 2024-03-20 20:19:28.729232 langchain_robocorp-0.0.4/langchain_robocorp/__init__.py
--rw-r--r--   0        0        0     3718 2024-03-20 20:19:28.729232 langchain_robocorp-0.0.4/langchain_robocorp/_common.py
--rw-r--r--   0        0        0      686 2024-03-20 20:19:28.733232 langchain_robocorp-0.0.4/langchain_robocorp/_prompts.py
--rw-r--r--   0        0        0        0 2024-03-20 20:19:28.733232 langchain_robocorp-0.0.4/langchain_robocorp/py.typed
--rw-r--r--   0        0        0     7839 2024-03-20 20:19:28.733232 langchain_robocorp-0.0.4/langchain_robocorp/toolkits.py
--rw-r--r--   0        0        0     2535 2024-03-20 20:19:28.733232 langchain_robocorp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1211 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/LICENSE
+-rw-r--r--   0        0        0      420 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/README.md
+-rw-r--r--   0        0        0      102 2024-04-01 18:34:48.983729 langchain_robocorp-0.0.5/langchain_robocorp/__init__.py
+-rw-r--r--   0        0        0     4568 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/_common.py
+-rw-r--r--   0        0        0      525 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/py.typed
+-rw-r--r--   0        0        0     7573 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/langchain_robocorp/toolkits.py
+-rw-r--r--   0        0        0     2552 2024-04-01 18:34:48.987729 langchain_robocorp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1314 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.5/PKG-INFO
```

### Comparing `langchain_robocorp-0.0.4/LICENSE` & `langchain_robocorp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.4/langchain_robocorp/toolkits.py` & `langchain_robocorp-0.0.5/langchain_robocorp/toolkits.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,19 @@
 from langchain_core.runnables import Runnable, RunnablePassthrough
 from langchain_core.tools import BaseTool, StructuredTool, Tool
 from langchain_core.tracers.context import _tracing_v2_is_enabled
 from langsmith import Client
 
 from langchain_robocorp._common import (
     get_param_fields,
-    get_required_param_descriptions,
+    model_to_dict,
     reduce_openapi_spec,
 )
 from langchain_robocorp._prompts import (
     API_CONTROLLER_PROMPT,
-    TOOLKIT_TOOL_DESCRIPTION,
 )
 
 MAX_RESPONSE_LENGTH = 5000
 LLM_TRACE_HEADER = "X-action-trace"
 
 
 class RunDetailsCallbackHandler(BaseCallbackHandler):
@@ -152,25 +151,17 @@
         toolkit: List[BaseTool] = []
 
         # Prepare tools
         for endpoint, docs in api_spec.endpoints:
             if not endpoint.startswith("/api/actions"):
                 continue
 
-            summary = docs["summary"]
-
-            tool_description = TOOLKIT_TOOL_DESCRIPTION.format(
-                name=summary,
-                description=docs.get("description", summary),
-                required_params=get_required_param_descriptions(docs),
-            )
-
             tool_args: ToolArgs = {
-                "name": f"robocorp_action_server_{docs['operationId']}",
-                "description": tool_description,
+                "name": docs["operationId"],
+                "description": docs["description"],
                 "callback_manager": callback_manager,
             }
 
             if llm:
                 tool = self._get_unstructured_tool(endpoint, docs, tool_args, llm)
             else:
                 tool = self._get_structured_tool(endpoint, docs, tool_args)
@@ -214,24 +205,25 @@
 
         return Tool(func=chain.invoke, args_schema=ToolInputSchema, **tool_args)
 
     def _get_structured_tool(
         self, endpoint: str, docs: dict, tools_args: ToolArgs
     ) -> BaseTool:
         fields = get_param_fields(docs)
+        _DynamicToolInputSchema = create_model("DynamicToolInputSchema", **fields)
 
-        def create_function(endpoint: str) -> Callable:
-            def func(**data: dict[str, Any]) -> str:
-                return self._action_request(endpoint, **data)
+        def dynamic_func(**data: dict[str, Any]) -> str:
+            return self._action_request(endpoint, **model_to_dict(data))
 
-            return func
+        dynamic_func.__name__ = tools_args["name"]
+        dynamic_func.__doc__ = tools_args["description"]
 
         return StructuredTool(
-            func=create_function(endpoint),
-            args_schema=create_model("DynamicToolInputSchema", **fields),
+            func=dynamic_func,
+            args_schema=_DynamicToolInputSchema,
             **tools_args,
         )
 
     def _action_request(self, endpoint: str, **data: dict[str, Any]) -> str:
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
```

### Comparing `langchain_robocorp-0.0.4/pyproject.toml` & `langchain_robocorp-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-robocorp"
-version = "0.0.4"
-description = "An integration package connecting Robocorp and LangChain"
+version = "0.0.5"
+description = "An integration package connecting Robocorp Action Server and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/robocorp"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1"
+langchain-core = "^0.1.31"
 requests = "^2.31.0"
 types-requests = "^2.31.0.6"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_robocorp-0.0.4/PKG-INFO` & `langchain_robocorp-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: langchain-robocorp
-Version: 0.0.4
-Summary: An integration package connecting Robocorp and LangChain
+Version: 0.0.5
+Summary: An integration package connecting Robocorp Action Server and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1,<0.2)
+Requires-Dist: langchain-core (>=0.1.31,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-requests (>=2.31.0.6,<3.0.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/robocorp
 Description-Content-Type: text/markdown
 
 # langchain-robocorp
 
-This package contains the LangChain integrations for [Robocorp](https://github.com/robocorp/robocorp).
+This package contains the LangChain integrations for [Robocorp Action Server](https://github.com/robocorp/robocorp).
+Action Server enables an agent to execute actions in the real world. 
 
 ## Installation
 
 ```bash
 pip install -U langchain-robocorp
 ```
```

