# Comparing `tmp/llmt-0.0.2.tar.gz` & `tmp/llmt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmt-0.0.2.tar", last modified: Tue Mar 26 20:37:52 2024, max compression
+gzip compressed data, was "llmt-0.0.3.tar", last modified: Mon Apr  1 19:22:50 2024, max compression
```

## Comparing `llmt-0.0.2.tar` & `llmt-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:37:52.533361 llmt-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    15829 2024-03-17 15:26:19.000000 llmt-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4625 2024-03-26 20:37:52.531736 llmt-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3753 2024-03-25 21:30:36.000000 llmt-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:37:52.503798 llmt-0.0.2/llmt/
--rw-r--r--   0 root         (0) root         (0)      546 2024-03-26 20:25:54.000000 llmt-0.0.2/llmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2024-03-25 14:36:35.000000 llmt-0.0.2/llmt/assistants.py
--rw-r--r--   0 root         (0) root         (0)      143 2024-03-24 12:26:42.000000 llmt-0.0.2/llmt/consts.py
--rw-r--r--   0 root         (0) root         (0)     3273 2024-03-25 14:36:43.000000 llmt-0.0.2/llmt/core.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-03-25 19:23:24.000000 llmt-0.0.2/llmt/managers.py
--rw-r--r--   0 root         (0) root         (0)     6709 2024-03-25 14:36:55.000000 llmt-0.0.2/llmt/prompts.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-03-25 16:20:27.000000 llmt-0.0.2/llmt/response.txt.j2
--rw-r--r--   0 root         (0) root         (0)      825 2024-03-25 13:38:08.000000 llmt-0.0.2/llmt/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:37:52.529154 llmt-0.0.2/llmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4625 2024-03-26 20:37:52.000000 llmt-0.0.2/llmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      320 2024-03-26 20:37:52.000000 llmt-0.0.2/llmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 20:37:52.000000 llmt-0.0.2/llmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      174 2024-03-26 20:37:52.000000 llmt-0.0.2/llmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-03-26 20:37:52.000000 llmt-0.0.2/llmt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-26 20:26:16.000000 llmt-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      226 2024-03-25 14:27:33.000000 llmt-0.0.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 20:37:52.534078 llmt-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-01 19:22:46.000000 llmt-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-01 19:22:50.779800 llmt-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-01 19:22:46.000000 llmt-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/llmt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/openai_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/response.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/llmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-01 19:22:46.000000 llmt-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 19:22:46.000000 llmt-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:22:50.779800 llmt-0.0.3/setup.cfg
```

### Comparing `llmt-0.0.2/LICENSE` & `llmt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmt-0.0.2/PKG-INFO` & `llmt-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,89 +13,60 @@
 License-File: LICENSE
 Requires-Dist: openai==1.14.1
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: halo==0.0.31
 Requires-Dist: inquirer==3.2.4
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: docstring-parser==0.16
+Requires-Dist: typing-extensions==4.10.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
+Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
+
+### Module import
+
 ```python
-from myfunctions import function
+from llmt import LLMT
 
-# 1. fetch table metadata
-# 2. run query
-# 3. analize results
-
-tools = [
-    {
-        "function": {
-            "required": ["value1", "value2"],
-            "name": "add_decimal_values",
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    "value2": {
-                        "type": "integer",
-                        "description": "The second decimal value to add. For example, 10",
-                    },
-                    "value1": {
-                        "type": "integer",
-                        "description": "The first decimal value to add. For example, 5",
-                    },
-                },
-            },
-            "description": "Add two decimal values and return the result.\n",
-        },
-        "type": "function",
-    }
-]
 
 llmt = LLMT()
 llmt.init_assistant(
     "dataengineer",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description=(
-        " ".join(
-            [
-                "You are a data engineer, and an expert with python,",
-                "sqlalchemy, pandas, and snowflake. Answer questions",
-                "briefly in a sentence or less.",
-            ]
-        )
-    ),
-    tools=tools,
-)
+    assistant_description="You are a data engineer, and a python expert.",)
+llmt.init_functions(["./my_functions.py"])
 llmt.init_chat("single_chat")
+
 response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?",
-    functions=functions,
+    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
 )
 ```
 
-In a workspace
+### Local workspace
+
+Install Docker and make command. Make is not required since you can use docker compose.
 
-- Install Docker and make command.
-- Optionally create custom functions in the udf/ directory and import them in cli.py.
-- Update or create a new configuration file in configs/.
-- Make sure the configuration file describes your custom functions in `assistants.tools`.
-- Run `make run`.
+- Clone this repo.
+- If using custom functions, create your functions in the udf/ directory and import them in cli.py.
+- Update the default configuration file, or create a new one in configs/.
+- Run `make run`. Default config will let you use input and output files.
 - Use files/input.md to send messages.
 - Use files/output.md to receive messages.
 - CTRL + C to quit out of the container and clean up orphans.
 
 ### Configuration file
 
 If both (input_file, output_file) are ommited, then the default terminal will be used.
```

### Comparing `llmt-0.0.2/README.md` & `llmt-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,75 +2,44 @@
 
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
+Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
+
+### Module import
+
 ```python
-from myfunctions import function
+from llmt import LLMT
 
-# 1. fetch table metadata
-# 2. run query
-# 3. analize results
-
-tools = [
-    {
-        "function": {
-            "required": ["value1", "value2"],
-            "name": "add_decimal_values",
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    "value2": {
-                        "type": "integer",
-                        "description": "The second decimal value to add. For example, 10",
-                    },
-                    "value1": {
-                        "type": "integer",
-                        "description": "The first decimal value to add. For example, 5",
-                    },
-                },
-            },
-            "description": "Add two decimal values and return the result.\n",
-        },
-        "type": "function",
-    }
-]
 
 llmt = LLMT()
 llmt.init_assistant(
     "dataengineer",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description=(
-        " ".join(
-            [
-                "You are a data engineer, and an expert with python,",
-                "sqlalchemy, pandas, and snowflake. Answer questions",
-                "briefly in a sentence or less.",
-            ]
-        )
-    ),
-    tools=tools,
-)
+    assistant_description="You are a data engineer, and a python expert.",)
+llmt.init_functions(["./my_functions.py"])
 llmt.init_chat("single_chat")
+
 response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?",
-    functions=functions,
+    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
 )
 ```
 
-In a workspace
+### Local workspace
+
+Install Docker and make command. Make is not required since you can use docker compose.
 
-- Install Docker and make command.
-- Optionally create custom functions in the udf/ directory and import them in cli.py.
-- Update or create a new configuration file in configs/.
-- Make sure the configuration file describes your custom functions in `assistants.tools`.
-- Run `make run`.
+- Clone this repo.
+- If using custom functions, create your functions in the udf/ directory and import them in cli.py.
+- Update the default configuration file, or create a new one in configs/.
+- Run `make run`. Default config will let you use input and output files.
 - Use files/input.md to send messages.
 - Use files/output.md to receive messages.
 - CTRL + C to quit out of the container and clean up orphans.
 
 ### Configuration file
 
 If both (input_file, output_file) are ommited, then the default terminal will be used.
```

### Comparing `llmt-0.0.2/llmt/core.py` & `llmt-0.0.3/llmt/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,108 @@
 import os
 
-from .managers import ChatManager, FileHandler
+from .managers import ChatManager, FileManager, FunctionManager
 from .utils import load_config
 from .assistants import OpenAIAssistant
-from .prompts import prompt_create_chat, prompt_init, chat, chat_once
+from .prompts import prompt_create_chat, prompt_init, ask, ask_once
 
 
 class LLMT:
     def __init__(self, **kwargs):
         self.configs = None
         self.chat = None
         self.assistant = None
-        self.file_handler = None
+        self.file_manager = None
+        self.function_manager = None
         self.config_file = kwargs.get("config_file", None)
         self.root_path = kwargs.get("root_path", os.getcwd())
         self.chat_manager = ChatManager(self.root_path)
 
         if self.config_file:
             self.configs = load_config(self.config_file)
 
-        self.init_file_handler()
+        self.init_file_manager()
 
     def get_chats(self):
         return list(self.chat_manager.list_chats())
 
     def prompt_create_chat(self):
         return prompt_create_chat()
 
     def init_prompt(self):
         if not self.configs:
             raise ValueError("No configuration file provided.")
 
         return prompt_init(self.configs["assistants"], self.get_chats())
 
+    def find_assistant(self, assistant_name):
+        return next(
+            (x for x in self.configs["assistants"] if x["name"] == assistant_name),
+            None,
+        )
+
     def init_assistant(self, assistant_name, **kwargs):
         if not self.configs:
             self.assistant = OpenAIAssistant(
                 kwargs.get("api_key"),
                 kwargs.get("model"),
                 assistant_name,
                 kwargs.get("assistant_description"),
-                kwargs.get("tools", None),
             )
 
         if self.configs:
-            selected_assistant = next(
-                (x for x in self.configs["assistants"] if x["name"] == assistant_name),
-                None,
-            )
+            selected_assistant = self.find_assistant(assistant_name)
 
             self.assistant = OpenAIAssistant(
                 selected_assistant["api_key"],
                 selected_assistant["model"],
                 selected_assistant["assistant_name"],
                 selected_assistant["assistant_description"],
-                selected_assistant.get("tools", []),
             )
 
+    def init_functions(self, paths):
+        self.function_manager = FunctionManager(paths)
+
     def init_chat(self, chat_name):
         self.chat = chat_name
         self.chat_manager.init_chat(chat_name)
 
-    def init_file_handler(self, **kwargs):
+    def init_file_manager(self, **kwargs):
         if not self.configs:
             input_file = kwargs.get("input_file", None)
             output_file = kwargs.get("output_file", None)
 
         if self.configs:
             input_file = self.configs.get("input_file", None)
             output_file = self.configs.get("output_file", None)
 
         if input_file or output_file:
-            self.file_handler = FileHandler(self.root_path, input_file, output_file)
+            self.file_manager = FileManager(self.root_path, input_file, output_file)
 
     def init_first_messages(self):
         if not self.assistant:
             raise ValueError("No assistant initialized.")
         if not self.chat:
             raise ValueError("No chat initialized.")
 
         if self.chat_manager.list_messages() == 0:
             self.chat_manager.save_to_chat(
                 {"role": "system", "content": self.assistant.description}
             )
 
-    def run_live(self, functions=None):
+    def run_forever(self):
         self.init_first_messages()
-        yield from chat(
+        yield from ask(
             self.chat_manager,
-            self.file_handler,
+            self.file_manager,
+            self.function_manager,
             self.assistant,
-            functions,
         )
 
     def run(self, message, functions=None):
         self.init_first_messages()
-        return chat_once(
+        return ask_once(
             message,
             self.chat_manager,
+            self.function_manager,
             self.assistant,
-            functions,
         )
```

### Comparing `llmt-0.0.2/llmt/prompts.py` & `llmt-0.0.3/llmt/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inquirer
 
 from typing import List
 from halo import Halo
+from llmt.openai_types import FunctionCall
 from openai.types import CompletionChoice, CompletionUsage
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionMessage,
     ChatCompletionMessageToolCall,
 )
 
@@ -67,43 +68,48 @@
             f'completion tokens: {usage["completion_tokens"]}',
             f'prompt tokens: {usage["prompt_tokens"]}',
             f'total tokens: {usage["total_tokens"]}',
         ]
     )
 
 
-def handle_chat_completion(messages, assistant, chat_manager, functions):
+def run_until_response(messages, assistant, chat_manager, function_manager):
     function_calls = []
 
     while True:
-        chat_completion: ChatCompletion = assistant.generate_response(messages)
+        chat_completion: ChatCompletion = assistant.generate_message(
+            messages, function_manager.functions_schema
+        )
         chat_completion_choice: CompletionChoice = chat_completion.choices[0]
         chat_completion_message: ChatCompletionMessage = chat_completion_choice.message
         usage: CompletionUsage = chat_completion.usage
         response: str = chat_completion_message.content
 
         if chat_completion_choice.finish_reason == "tool_calls":
             tool_calls: List[ChatCompletionMessageToolCall] = (
                 chat_completion_message.tool_calls
             )
             message = {"role": "assistant", "tool_calls": tool_calls}
             messages.append(message)
 
             for tool_call in tool_calls:
+                args = tool_call.function.arguments
                 fn_name = tool_call.function.name
-                arguments = tool_call.function.arguments
-                function = getattr(functions, fn_name)
-                result = function(arguments)
+                function_call: FunctionCall = {
+                    "name": fn_name,
+                    "arguments": args,
+                }
+                result = function_manager.run_function(function_call)
                 message = {
                     "role": "tool",
-                    "content": str(result),
+                    "content": str(result.content),
                     "tool_call_id": tool_call.id,
                     "name": fn_name,
                 }
-                template_message = {**message, "arguments": arguments}
+                template_message = {**message, "arguments": args}
                 messages.append(message)
                 chat_manager.save_to_chat(message)
                 function_calls.append(template_message)
 
             continue
 
         if chat_completion_choice.finish_reason == "stop":
@@ -117,78 +123,85 @@
             "completion_tokens": usage.completion_tokens,
             "prompt_tokens": usage.prompt_tokens,
             "total_tokens": usage.total_tokens,
         },
     }
 
 
-def chat_once(
+def ask_once(
     input_text,
     chat_manager,
+    function_manager,
     assistant: OpenAIAssistant,
-    functions,
 ):
     """Chat with the assistant once.
 
     Args:
         input_text (str): The input text.
         chat_manager (ChatManager): The chat manager.
+        function_manager (FunctionManager): The function manager.
         assistant (OpenAIAssistant): The assistant.
         functions (module): The functions module.
 
     Returns:
         dict: The assistant, response, function calls, and usage information.
     """
     message = {"role": "user", "content": input_text}
     messages = [{"role": "system", "content": assistant.description}, message]
     chat_manager.save_to_chat(message)
 
-    response = handle_chat_completion(messages, assistant, chat_manager, functions)
+    response = run_until_response(
+        messages,
+        assistant,
+        chat_manager,
+        function_manager,
+    )
     messages = response["messages"]
     message = {"role": "assistant", "content": response["response"]}
     messages.append(message)
     chat_manager.save_to_chat(message)
 
     return {
         "assistant": assistant,
         "response": response["response"],
         "function_calls": response["function_calls"],
         "info": get_usage_as_string(response["usage"]),
     }
 
 
-def chat(
+def ask(
     chat_manager,
-    file_handler,
+    file_manager,
+    function_manager,
     assistant: OpenAIAssistant,
-    functions,
 ):
     """Chat with the assistant.
 
     Args:
         chat_manager (ChatManager): The chat manager.
-        file_handler (InputFileHandler or None): The input file handler object or None.
+        file_manager (FileManager or None): The input file handler object or None.
+        function_manager (FunctionManager): The function manager.
         assistant (OpenAIAssistant): The assistant.
 
     Returns:
         None
 
     Yields:
         str: The response.
     """
     input_text = ""
     response = ""
     messages = [{"role": "system", "content": assistant.description}]
     spinner = Halo(text="Working...", spinner="dots")
 
     while True:
-        if file_handler:
-            print(f"{Style.GREEN}You{Style.RESET}: using {file_handler.input_file}")
+        if file_manager:
+            print(f"{Style.GREEN}You{Style.RESET}: using {file_manager.input_file}")
 
-            for event in file_handler.events_generator():
+            for event in file_manager.events_generator():
                 input_text = event
                 break
         else:
             input_text = input(f"{Style.GREEN}You{Style.RESET}: ").strip()
 
         if len(input_text) == 0:
             continue
@@ -197,30 +210,35 @@
             break
 
         message = {"role": "user", "content": input_text}
         messages.append(message)
         chat_manager.save_to_chat(message)
 
         spinner.start()
-        response = handle_chat_completion(messages, assistant, chat_manager, functions)
+        response = run_until_response(
+            messages,
+            assistant,
+            chat_manager,
+            function_manager,
+        )
         messages = response["messages"]
         spinner.stop()
 
         message = {"role": "assistant", "content": response["response"]}
         messages.append(message)
         chat_manager.save_to_chat(message)
-        full_respose = {
+        to_user_response = {
             "assistant": assistant,
             "response": response["response"],
             "function_calls": response["function_calls"],
             "info": get_usage_as_string(response["usage"]),
         }
 
-        if file_handler:
-            file_handler.write_to_output(full_respose)
+        if file_manager:
+            file_manager.write_to_output(to_user_response)
         else:
             yield " ".join(
                 [
                     f"{Style.GREEN}{assistant.name}{Style.RESET}:",
                     f"{response['response']}\n\n{Style.YELLOW}usage{Style.RESET}:",
                     f"{get_usage_as_string(response['usage'])}",
                 ]
```

### Comparing `llmt-0.0.2/llmt/utils.py` & `llmt-0.0.3/llmt/utils.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.2/llmt.egg-info/PKG-INFO` & `llmt-0.0.3/llmt.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.2
+Version: 0.0.3
 Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,89 +13,60 @@
 License-File: LICENSE
 Requires-Dist: openai==1.14.1
 Requires-Dist: watchdog==4.0.0
 Requires-Dist: halo==0.0.31
 Requires-Dist: inquirer==3.2.4
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: PyYAML==6.0.1
+Requires-Dist: docstring-parser==0.16
+Requires-Dist: typing-extensions==4.10.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: pandas==2.2.1
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
+Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
+
+### Module import
+
 ```python
-from myfunctions import function
+from llmt import LLMT
 
-# 1. fetch table metadata
-# 2. run query
-# 3. analize results
-
-tools = [
-    {
-        "function": {
-            "required": ["value1", "value2"],
-            "name": "add_decimal_values",
-            "parameters": {
-                "type": "object",
-                "properties": {
-                    "value2": {
-                        "type": "integer",
-                        "description": "The second decimal value to add. For example, 10",
-                    },
-                    "value1": {
-                        "type": "integer",
-                        "description": "The first decimal value to add. For example, 5",
-                    },
-                },
-            },
-            "description": "Add two decimal values and return the result.\n",
-        },
-        "type": "function",
-    }
-]
 
 llmt = LLMT()
 llmt.init_assistant(
     "dataengineer",
     api_key="...",
     model="gpt-3.5-turbo",
-    assistant_description=(
-        " ".join(
-            [
-                "You are a data engineer, and an expert with python,",
-                "sqlalchemy, pandas, and snowflake. Answer questions",
-                "briefly in a sentence or less.",
-            ]
-        )
-    ),
-    tools=tools,
-)
+    assistant_description="You are a data engineer, and a python expert.",)
+llmt.init_functions(["./my_functions.py"])
 llmt.init_chat("single_chat")
+
 response = llmt.run(
-    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?",
-    functions=functions,
+    "What's the result of 22 plus 5 in decimal added to the hexadecimal number A?"
 )
 ```
 
-In a workspace
+### Local workspace
+
+Install Docker and make command. Make is not required since you can use docker compose.
 
-- Install Docker and make command.
-- Optionally create custom functions in the udf/ directory and import them in cli.py.
-- Update or create a new configuration file in configs/.
-- Make sure the configuration file describes your custom functions in `assistants.tools`.
-- Run `make run`.
+- Clone this repo.
+- If using custom functions, create your functions in the udf/ directory and import them in cli.py.
+- Update the default configuration file, or create a new one in configs/.
+- Run `make run`. Default config will let you use input and output files.
 - Use files/input.md to send messages.
 - Use files/output.md to receive messages.
 - CTRL + C to quit out of the container and clean up orphans.
 
 ### Configuration file
 
 If both (input_file, output_file) are ommited, then the default terminal will be used.
```

### Comparing `llmt-0.0.2/pyproject.toml` & `llmt-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmt"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Artem Golub", email="artem @ outermeasure.com"}
 ]
 description = "Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

