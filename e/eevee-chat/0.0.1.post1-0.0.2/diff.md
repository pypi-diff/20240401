# Comparing `tmp/eevee-chat-0.0.1.post1.tar.gz` & `tmp/eevee-chat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eevee-chat-0.0.1.post1.tar", last modified: Sun Mar 31 16:49:53 2024, max compression
+gzip compressed data, was "eevee-chat-0.0.2.tar", last modified: Mon Apr  1 11:39:43 2024, max compression
```

## Comparing `eevee-chat-0.0.1.post1.tar` & `eevee-chat-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-03-31 16:49:53.666147 eevee-chat-0.0.1.post1/
--rw-r--r--   0 shakedzy   (502) staff       (20)    19346 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/LICENSE
--rw-r--r--   0 shakedzy   (502) staff       (20)     1756 2024-03-31 16:49:53.655557 eevee-chat-0.0.1.post1/PKG-INFO
--rw-r--r--   0 shakedzy   (502) staff       (20)     1282 2024-03-31 16:47:22.000000 eevee-chat-0.0.1.post1/README.md
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-03-31 16:49:53.623199 eevee-chat-0.0.1.post1/eevee/
--rw-r--r--   0 shakedzy   (502) staff       (20)      214 2024-03-31 13:43:48.000000 eevee-chat-0.0.1.post1/eevee/__init__.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     1460 2024-03-31 16:04:17.000000 eevee-chat-0.0.1.post1/eevee/_run.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      392 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/_types.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     8304 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/chatbot.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     4139 2024-03-31 13:48:24.000000 eevee-chat-0.0.1.post1/eevee/color_logger.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      804 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/framework_models.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     7121 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/messages.py
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-03-31 16:49:53.635213 eevee-chat-0.0.1.post1/eevee/resources/
--rw-r--r--   0 shakedzy   (502) staff       (20)     7418 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/resources/eevee_50.png
--rw-r--r--   0 shakedzy   (502) staff       (20)     3743 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/saved_chat.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     1734 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/settings.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     4295 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/tools.py
--rw-r--r--   0 shakedzy   (502) staff       (20)    11270 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/ui.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      144 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/eevee/utils.py
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-03-31 16:49:53.654173 eevee-chat-0.0.1.post1/eevee_chat.egg-info/
--rw-r--r--   0 shakedzy   (502) staff       (20)     1756 2024-03-31 16:49:52.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/PKG-INFO
--rw-r--r--   0 shakedzy   (502) staff       (20)      472 2024-03-31 16:49:53.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/SOURCES.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)        1 2024-03-31 16:49:52.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/dependency_links.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)       42 2024-03-31 16:49:52.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/entry_points.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)      193 2024-03-31 16:49:52.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/requires.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)        6 2024-03-31 16:49:52.000000 eevee-chat-0.0.1.post1/eevee_chat.egg-info/top_level.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)       38 2024-03-31 16:49:53.666518 eevee-chat-0.0.1.post1/setup.cfg
--rw-r--r--   0 shakedzy   (502) staff       (20)     1522 2024-03-31 12:17:47.000000 eevee-chat-0.0.1.post1/setup.py
+drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:39:43.252952 eevee-chat-0.0.2/
+-rw-r--r--   0 shakedzy   (502) staff       (20)    19346 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/LICENSE
+-rw-r--r--   0 shakedzy   (502) staff       (20)     2060 2024-04-01 11:39:43.250054 eevee-chat-0.0.2/PKG-INFO
+-rw-r--r--   0 shakedzy   (502) staff       (20)     1591 2024-03-31 20:57:08.000000 eevee-chat-0.0.2/README.md
+drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:39:43.099720 eevee-chat-0.0.2/eevee/
+-rw-r--r--   0 shakedzy   (502) staff       (20)      293 2024-04-01 11:31:01.000000 eevee-chat-0.0.2/eevee/__init__.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     2151 2024-04-01 11:36:12.000000 eevee-chat-0.0.2/eevee/_run.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)      404 2024-03-31 17:56:15.000000 eevee-chat-0.0.2/eevee/_types.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     8281 2024-04-01 11:32:01.000000 eevee-chat-0.0.2/eevee/chatbot.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     4268 2024-03-31 20:49:22.000000 eevee-chat-0.0.2/eevee/color_logger.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)      804 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/eevee/framework_models.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     7099 2024-03-31 20:04:25.000000 eevee-chat-0.0.2/eevee/messages.py
+drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:39:43.109385 eevee-chat-0.0.2/eevee/resources/
+-rw-r--r--   0 shakedzy   (502) staff       (20)      459 2024-03-31 17:56:59.000000 eevee-chat-0.0.2/eevee/resources/config.toml
+-rw-r--r--   0 shakedzy   (502) staff       (20)     7418 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/eevee/resources/eevee_50.png
+-rw-r--r--   0 shakedzy   (502) staff       (20)     3743 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/eevee/saved_chat.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     1734 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/eevee/settings.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)     4836 2024-03-31 20:26:50.000000 eevee-chat-0.0.2/eevee/tools.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)    11257 2024-04-01 11:32:53.000000 eevee-chat-0.0.2/eevee/ui.py
+-rw-r--r--   0 shakedzy   (502) staff       (20)      144 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/eevee/utils.py
+drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:39:43.246659 eevee-chat-0.0.2/eevee_chat.egg-info/
+-rw-r--r--   0 shakedzy   (502) staff       (20)     2060 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/PKG-INFO
+-rw-r--r--   0 shakedzy   (502) staff       (20)      500 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 shakedzy   (502) staff       (20)        1 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 shakedzy   (502) staff       (20)       42 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/entry_points.txt
+-rw-r--r--   0 shakedzy   (502) staff       (20)      193 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/requires.txt
+-rw-r--r--   0 shakedzy   (502) staff       (20)        6 2024-04-01 11:39:42.000000 eevee-chat-0.0.2/eevee_chat.egg-info/top_level.txt
+-rw-r--r--   0 shakedzy   (502) staff       (20)       38 2024-04-01 11:39:43.253304 eevee-chat-0.0.2/setup.cfg
+-rw-r--r--   0 shakedzy   (502) staff       (20)     1522 2024-03-31 12:17:47.000000 eevee-chat-0.0.2/setup.py
```

### Comparing `eevee-chat-0.0.1.post1/LICENSE` & `eevee-chat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.1.post1/PKG-INFO` & `eevee-chat-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevee-chat
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: A single chat interface for multiple LLMs
 Home-page: http://shakedzy.xyz/eevee-chat
 Download-URL: https://pypi.org/project/eevee-chat/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3.11
@@ -15,14 +15,16 @@
 
 ![banner](https://shakedzy.xyz/eevee-chat/images/wide_banner.png)
 
 # Eevee Chat
 
 [![PyPI Version](https://img.shields.io/pypi/v/eevee-chat?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
 [![Python Version](https://img.shields.io/pypi/pyversions/eevee-chat.svg?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
+[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-green?style=for-the-badge)](https://creativecommons.org/licenses/by-nc/4.0/)
+
 
 Eevee Chat is a unified chat UI for all LLM frameworks. It allows you to use GPT, Claude and many others from the same window, and switch between them even in the middle of a conversation.
 
 Using Eevee is simple and intuitive. LLMs are connected to the web (supporting LLMs only) with either Google Search or DuckDuckGo, and so it suppose to mimic working with the official web apps.
 
 Eevee can also be configured to support custom frameworks and tools easily. See the docs for more information.
 
@@ -37,7 +39,16 @@
 
 ## Running
 Once installed, simply run:
 ```bash
 eevee
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
+
+## 🎯 Roadmap
+
+- [ ] Code interpreter
+- [x] DeepSeek integration
+- [ ] Google Gemini integration
+- [ ] Add files as text
+- [ ] Add images to multi-modal models
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eevee-chat-0.0.1.post1/README.md` & `eevee-chat-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 ![banner](https://shakedzy.xyz/eevee-chat/images/wide_banner.png)
 
 # Eevee Chat
 
 [![PyPI Version](https://img.shields.io/pypi/v/eevee-chat?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
 [![Python Version](https://img.shields.io/pypi/pyversions/eevee-chat.svg?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
+[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-green?style=for-the-badge)](https://creativecommons.org/licenses/by-nc/4.0/)
+
 
 Eevee Chat is a unified chat UI for all LLM frameworks. It allows you to use GPT, Claude and many others from the same window, and switch between them even in the middle of a conversation.
 
 Using Eevee is simple and intuitive. LLMs are connected to the web (supporting LLMs only) with either Google Search or DuckDuckGo, and so it suppose to mimic working with the official web apps.
 
 Eevee can also be configured to support custom frameworks and tools easily. See the docs for more information.
 
@@ -22,7 +24,16 @@
 
 ## Running
 Once installed, simply run:
 ```bash
 eevee
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
+
+## 🎯 Roadmap
+
+- [ ] Code interpreter
+- [x] DeepSeek integration
+- [ ] Google Gemini integration
+- [ ] Add files as text
+- [ ] Add images to multi-modal models
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eevee-chat-0.0.1.post1/eevee/chatbot.py` & `eevee-chat-0.0.2/eevee/chatbot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
-import pathlib
 import traceback
 from datetime import datetime
 from typing import Set, Dict, List, Generator, Any, Tuple
-from .messages import Messages, Message, ToolCall
-from .tools import tools_params_definitions
+from .messages import Messages, Message, ChatMessagePiece
+from .tools import tools_params_definitions, tool_display_message
 from .color_logger import get_logger
 from .framework_models import get_model_framework
 from .saved_chat import SavedChat
 from .chat_connectors.connector_interface import Connector
 from .chat_connectors.openai_connector import OpenAIConnector
 from .chat_connectors.anthropic_connector import AnthropicConnector
 from .chat_connectors.mistral_connector import MistralConnector
+from .chat_connectors.deepseek_connector import DeepSeekConnector
 from ._types import Framework
+from . import ROOT_DIR
 
 
 class Chatbot:
-    METADATA_TOKEN = "$%^"
-
     def __init__(self, available_frameworks: Set[Framework]) -> None:
         if not available_frameworks:
             raise RuntimeError('No available frameworks found! Make sure you supplied API keys')
 
         self.clients: Dict[Framework, Connector] = dict()
         self.callables = {f.__name__: f for f in tools_params_definitions.keys()}
         self.tools = self._build_tools()
@@ -33,19 +32,18 @@
             match framework:
                 case 'openai':
                     client = OpenAIConnector()
                 case 'mistral':
                     client = MistralConnector()
                 case 'anthropic':
                     client = AnthropicConnector()
+                case 'deepseek':
+                    client = DeepSeekConnector()
             self.clients[framework] = client
 
-        self.INFO_TOKEN = self.clients[list(self.clients.keys())[0]].INFO_TOKEN
-        self.WARNING_TOKEN = self.clients[list(self.clients.keys())[0]].WARNING_TOKEN
-
     def _build_tools(self) -> List[Dict[str, Any]]:
         tools = list()
         for func, v in tools_params_definitions.items():
             params = {}
             required = []
             for p in v:
                 params[p[0]] = p[1]
@@ -61,20 +59,19 @@
                         "type": "object",
                         "properties": params
                     },
                     "required": required
                 }
             })
         return tools 
-
+    
     @property
     def saved_chats_dir(self) -> str:
         SAVED_CHATS_DIR = "saved_chats"
-        current_dir = pathlib.Path(__file__).parent.resolve()
-        directory = os.path.join(current_dir, SAVED_CHATS_DIR)
+        directory = os.path.join(ROOT_DIR, SAVED_CHATS_DIR)
         if not os.path.exists(directory):
             os.makedirs(directory)
         return directory
     
     def reset_chat(self) -> None:
         self.messages = Messages()
         self.start_time = datetime.now()
@@ -92,72 +89,70 @@
     def _prepare_for_response(self, prompt: str, system_prompt: str) -> None:
         if self.messages.empty:
             self.messages.append("system", system_prompt)
         else:
             self.messages.edit(0, content=system_prompt)
         self.messages.append('user', prompt)      
 
-    def get_stream_response(self, prompt: str, *, system_prompt: str, model: str, temperature: float) -> Generator[str, None, None]:        
+    def get_stream_response(self, prompt: str, *, system_prompt: str, model: str, temperature: float) -> Generator[ChatMessagePiece, None, None]:        
         framework = get_model_framework(model)
         self._prepare_for_response(prompt=prompt, system_prompt=system_prompt)
 
         try:
             final_message = False
             while not final_message:
                 final_message = True
                 generator = self.clients[framework].get_streaming_response(model=model, temperature=temperature, messages=self.messages, tools=self.tools)
-                for token in generator:
-                    if isinstance(token, list):
-                        # Only option is list of ToolCall
-                        tool_calls: List[ToolCall] = token
+                for chat_piece in generator:
+                    if chat_piece.tool_calls:
                         final_message = False
                         if self.messages[self.messages.last_message_index].role == 'assistant':
-                            self.messages.update(self.messages.last_message_index, tool_calls=tool_calls)
+                            self.messages.update(self.messages.last_message_index, tool_calls=chat_piece.tool_calls)
                         else:
-                            self.messages.append('assistant', content=None, tool_calls=tool_calls, model=model)
-                        for tool_call in tool_calls:
-                            yield self.INFO_TOKEN + "Running tool: " + tool_call.function
+                            self.messages.append('assistant', content=None, tool_calls=chat_piece.tool_calls, model=model)
+                        for tool_call in chat_piece.tool_calls:
+                            yield ChatMessagePiece(info_message=tool_display_message(tool_call.function, **tool_call.arguments))
                             self.logger.info(f"Running tool {tool_call.function}: {str(tool_call.arguments)}", color='yellow')
                             tool_output = self.callables[tool_call.function](**tool_call.arguments)
                             self.logger.debug("Tool output:\n" + tool_output)
                             self.messages.append(role='tool', content=tool_output, tool_calls=[tool_call])
                     else:
                         if self.messages[self.messages.last_message_index].role == 'assistant':
-                            self.messages.update(self.messages.last_message_index, content=token)
+                            self.messages.update(self.messages.last_message_index, content=chat_piece.content)
                         else:
-                            self.messages.append('assistant', content=token, model=model)
-                        yield token + self.METADATA_TOKEN + model
+                            self.messages.append('assistant', content=chat_piece.content, model=model)
+                        chat_piece.model = model
+                        yield chat_piece
         
         except Exception as e:
             self.logger.error(traceback.format_exc())
-            yield f'❌ _**{e.__class__.__name__}:** {e}_'
+            yield ChatMessagePiece(content=f'❌ _**{e.__class__.__name__}:** {e}_')
 
-    def get_json_response(self, prompt: str, *, system_prompt: str, model: str, temperature: float) -> Generator[str, None, None]:
+    def get_json_response(self, prompt: str, *, system_prompt: str, model: str, temperature: float) -> Generator[ChatMessagePiece, None, None]:
         framework = get_model_framework(model)
         self._prepare_for_response(prompt=prompt, system_prompt=system_prompt)
 
         final_message = False
         while not final_message:
             final_message = True
             response = self.clients[framework].get_json_response(model=model, temperature=temperature, messages=self.messages, tools=self.tools)
-            for chunk in response:
-                if isinstance(chunk, list):
-                    # Only option is list of ToolCall
+            for chat_piece in response:
+                if chat_piece.tool_calls:
                     final_message = False
-                    tool_calls: List[ToolCall] = chunk
-                    self.messages.append(role='assistant', content=None, tool_calls=tool_calls, model=model)
-                    for tool_call in tool_calls:
-                        yield self.INFO_TOKEN + "Running tool: "  + tool_call.function
+                    self.messages.append(role='assistant', content=None, tool_calls=chat_piece.tool_calls, model=model)
+                    for tool_call in chat_piece.tool_calls:
+                        yield ChatMessagePiece(info_message=tool_display_message(tool_call.function, **tool_call.arguments))
                         self.logger.info(f"Running tool {tool_call.function}: {str(tool_call.arguments)}", color='yellow')
                         tool_output = self.callables[tool_call.function](**tool_call.arguments)
                         self.logger.debug("Tool output:\n" + tool_output)
                         self.messages.append(role='tool', content=tool_output, tool_calls=[tool_call])
                 else:
-                    self.messages.append(role='assistant', content=chunk, model=model)
-                    yield chunk + self.METADATA_TOKEN + model
+                    self.messages.append(role='assistant', content=chat_piece.content, model=model)
+                    chat_piece.model = model
+                    yield chat_piece
 
     def export_chat(self) -> None:
         SavedChat(messages=self.messages, start_time=self.start_time, directory=self.saved_chats_dir).save_to_file()
 
     def load_chat(self, title: str, start_time: datetime) -> None:
         self.reset_chat()
         saved_chat = SavedChat.from_chat_title_and_time(title, start_time, directory=self.saved_chats_dir)
```

### Comparing `eevee-chat-0.0.1.post1/eevee/color_logger.py` & `eevee-chat-0.0.2/eevee/color_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from types import TracebackType
 from typing import Mapping, Dict
 from ._types import Color
 
-_DEFAULT_LOG_LEVEL = logging.INFO
+_DEFAULT_LOG_LEVEL = "INFO"
 _DEFAULT_LOGGER_NAME = "root"
 
 
 class ColorLogger(logging.Logger):
     def __init__(self, name: str, level: int | str) -> None:
         super().__init__(name, level)
         self.propagate = False
@@ -56,9 +56,14 @@
     
     def critical(self, msg: object, *args: object, color: Color | None = None, exc_info: bool | tuple[type[BaseException], BaseException, TracebackType | None] | tuple[None, None, None] | BaseException | None = None, stack_info: bool = False, stacklevel: int = 1, extra: Mapping[str, object] | None = None) -> None:
         if color:
             msg = self._add_color(str(msg), color)
         return super().critical(msg, *args, exc_info=exc_info, stack_info=stack_info, stacklevel=stacklevel, extra=extra)
     
 
-def get_logger(name: str| None = None, level: str | int | None = None):
-    return ColorLogger(name or _DEFAULT_LOGGER_NAME, level=level or _DEFAULT_LOG_LEVEL)
+def get_logger(name: str| None = None, level: str | int | None = None) -> ColorLogger:
+    return ColorLogger(name or _DEFAULT_LOGGER_NAME, level=level or _DEFAULT_LOG_LEVEL)
+
+
+def change_default_log_level(level: str | int) -> None:
+    global _DEFAULT_LOG_LEVEL
+    _DEFAULT_LOG_LEVEL = level
```

### Comparing `eevee-chat-0.0.1.post1/eevee/framework_models.py` & `eevee-chat-0.0.2/eevee/framework_models.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.1.post1/eevee/messages.py` & `eevee-chat-0.0.2/eevee/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import json
-from typing import List, Dict, Any, Generator
-from dataclasses import dataclass
+from typing import List, Dict, Any
+from dataclasses import dataclass, asdict
 from mistralai.models.chat_completion import ChatMessage as MistralChatMessage, ToolCall as MistralToolCall, FunctionCall as MistralFunctionCall
 from ._types import Role, Framework
 
 
 @dataclass
 class ToolCall:
     call_id: str
     function: str
     arguments: Dict[str, Any]
-
-    def __str__(self) -> str:
-        return f"{self.function}: {json.dumps(self.arguments)}"
     
-    def as_dict(self) -> Dict[str, Any]:
-        return {
-            'call_id': self.call_id,
-            'function': self.function,
-            'arguments': self.arguments
-        }
+    as_dict = asdict
+
+
+@dataclass
+class ChatMessagePiece:
+    content: str | None = None
+    info_message: str | None = None
+    warning_message: str | None = None
+    model: str | None = None
+    tool_calls: List[ToolCall] | None = None
+
+    as_dict = asdict
 
 
 class Message:
     def __init__(self, role: Role, content: str | None = None, tool_calls: List[ToolCall] = [], *, model: str | None = None) -> None:
         if role == 'assistant' and not model:
             raise ValueError('AI generated messages must be provided with model name')
         self.role: Role = role
```

### Comparing `eevee-chat-0.0.1.post1/eevee/resources/eevee_50.png` & `eevee-chat-0.0.2/eevee/resources/eevee_50.png`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.1.post1/eevee/saved_chat.py` & `eevee-chat-0.0.2/eevee/saved_chat.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.1.post1/eevee/settings.py` & `eevee-chat-0.0.2/eevee/settings.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.1.post1/eevee/tools.py` & `eevee-chat-0.0.2/eevee/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import os
 import inspect
 import requests
+from urllib.parse import urlparse
 from tqdm import tqdm
 from bs4 import BeautifulSoup
 from duckduckgo_search import DDGS
 from googleapiclient.discovery import build
 from typing import List, Tuple
 from .color_logger import get_logger
 from .settings import Settings
@@ -16,14 +17,16 @@
 _GOOGLE_SEARCH_CSE_ID = os.environ.get('GOOGLE_SEARCH_CSE_ID', None)
 
 
 def handle_tool_error(e: Exception) -> None:
     get_logger().error(f'ERROR [{e.__class__.__name__} in {inspect.stack()[1].function}]: {str(e)}', color='red')
 
 
+### TOOLS ###
+
 def web_search(query: str, max_results: int = 10) -> str:
     """
     Search the web for the provided query, and returns the title, URL and description of the results.
     Search results are separated by: =====
 
     Example of two search results:
 
@@ -97,13 +100,27 @@
         else:
             raise RuntimeError(f"ERROR: Failed to retrieve the webpage. Status code: {response.status_code}")
     except Exception as e:
         handle_tool_error(e)
         return f"ERROR: {e}"
 
 
+#######
+    
+
+def tool_display_message(tool_name: str, **arguments) -> str:
+    match tool_name:
+        case 'web_search':
+            return f'Searching the web: {arguments["query"]}'
+        case 'visit_website':
+            domain = urlparse(arguments['url']).netloc
+            return f'Visiting website: {domain}'
+        case _:
+            capitalized_name = ' '.join([s.capitalize() for s in tool_name.split(' ')])
+            return f'Running tool: {capitalized_name}'
+            
 
 tools_params_definitions: ToolsDefType = {
     web_search: [("query", {"type": "string", "description": "The query to search on the web"}, True),
                  ("max_results", {"type": "number", "description": "Maximal number of results to retrieve. Must be between 1 and 10, default is 10."}, False)],
     visit_website: [("url", {"type": "string", "description": "The URL of the page to scrape"}, True)],
 }
```

### Comparing `eevee-chat-0.0.1.post1/eevee/ui.py` & `eevee-chat-0.0.2/eevee/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import json
-import pathlib
 import gradio as gr
 from datetime import datetime
 from typing import List, Tuple, Generator, Set, Tuple, Dict, Any
 from .saved_chat import SavedChat
 from .chatbot import Chatbot
 from .settings import Settings
 from .utils import path_to_resource
 from ._types import Framework
+from . import ROOT_DIR
 
 
 class UI:
     CHAT_FILE_TIME_FORMAT = "%d/%m/%Y, %H:%M:%S"
     MODEL_NAME_SEPARATOR = "\n\n🤖 "
 
     def __init__(self, chatbot: Chatbot, available_frameworks: Set[Framework], port: int) -> None:
@@ -34,16 +34,15 @@
             self.ui.close()
             with open(self.preferences_file_path, 'w') as f:
                 json.dump(self.preferences, f)
 
     @property
     def preferences_file_path(self) -> str:
         filename = "pref.json"
-        current_dir = pathlib.Path(__file__).parent.resolve()
-        return os.path.join(current_dir, filename)
+        return os.path.join(ROOT_DIR, filename)
 
     def _load_preferences_from_file(self) -> Dict[str, Any]:
         try:
             with open(self.preferences_file_path, 'r') as f:
                 return json.load(f)
         except:
             return {}
@@ -57,34 +56,34 @@
     
     def _stop_text_generation(self) -> None:
         self._generate_text = False
 
     def _add_user_message_to_chat(self, prompt: str, history: List[List[str | None]]) -> Tuple[str, List[List[str | None]]]:
         return '', history + [[prompt, None]]
 
-    def _add_bot_message_to_chat(self, history: List[List[str | None]], model: str, temperature: float, as_json: bool, system_prompt: str) -> Generator:
+    def _add_bot_message_to_chat(self, history: List[List[str | None]], model: str, temperature: float, as_json: bool, system_prompt: str) -> Generator[List[List[str | None]], None, None]:
         self._generate_text = True
         if as_json:
             generator = self.chatbot.get_json_response(history[-1][0] or '', system_prompt=system_prompt, model=model, temperature=temperature)
         else:
             generator = self.chatbot.get_stream_response(history[-1][0] or '', system_prompt=system_prompt, model=model, temperature=temperature)
         
-        for chunk in generator:
+        for chat_piece in generator:
             if not self._generate_text:
                 break
-            if chunk.startswith(self.chatbot.INFO_TOKEN):
-                gr.Info(chunk.strip(self.chatbot.INFO_TOKEN))
-            elif chunk.startswith(self.chatbot.WARNING_TOKEN):
-                gr.Warning(chunk.strip(self.chatbot.WARNING_TOKEN))
-            else:
-                chunk, model = chunk.split(self.chatbot.METADATA_TOKEN, 1)
+            if chat_piece.info_message:
+                gr.Info(chat_piece.info_message)
+            if chat_piece.warning_message:
+                gr.Warning(chat_piece.warning_message)
+            if chat_piece.content:
                 current_message: str = history[-1][1] or ''
                 current_message = self.MODEL_NAME_SEPARATOR.join(current_message.split(self.MODEL_NAME_SEPARATOR)[:-1])
-                current_message += chunk
-                current_message += f'{self.MODEL_NAME_SEPARATOR}_{model}_'
+                current_message += chat_piece.content
+                if chat_piece.model:
+                    current_message += f'{self.MODEL_NAME_SEPARATOR}_{chat_piece.model}_'
                 history[-1][1] = current_message
                 yield history 
 
     def _undo_last_message(self, history: List[List[str]]) -> List[List[str]]:
         self._generate_text = False
         history.pop()
         self.chatbot.delete_last_interaction()
@@ -172,15 +171,15 @@
                 with gr.Column(scale=1, variant='panel'):
                     with gr.Group():
                         model = gr.Dropdown(label="Model", interactive=True, choices=available_models, value=self.preferences['model'])  # type: ignore
                         with gr.Accordion(label="System Prompt", open=False):
                             system_prompt = gr.TextArea(value="You are a helpful AI assistance, and your task is to assist the user with all its requests in the best possible way", container=False, interactive=True, lines=10)
                         temperature = gr.Slider(label="Temperature", minimum=0., maximum=1., step=.01, value=self.preferences.get('temperature', 0.))
                         force_json = gr.Checkbox(label="Force JSON", value=False, interactive=True)
-                    gr.Markdown("Not all models support all options, see documentation for more information")
+                    gr.Markdown("Not all models support all options, see [documentation](https://shakedzy.xyz/eevee-chat/tools/#known-limitations) for more information")
                     gr.Markdown("\n---\n")
                     with gr.Group():
                         saved_chats = gr.Radio(label="Saved Chats", choices=self._list_saved_chats(), elem_classes="files_list", value=None)  # type: ignore
                         load_chat = gr.Button("Load")
                         delete_chat = gr.Button("Delete", variant='stop')
 
                 with gr.Column(scale=10):
```

### Comparing `eevee-chat-0.0.1.post1/eevee_chat.egg-info/PKG-INFO` & `eevee-chat-0.0.2/eevee_chat.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevee-chat
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: A single chat interface for multiple LLMs
 Home-page: http://shakedzy.xyz/eevee-chat
 Download-URL: https://pypi.org/project/eevee-chat/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3.11
@@ -15,14 +15,16 @@
 
 ![banner](https://shakedzy.xyz/eevee-chat/images/wide_banner.png)
 
 # Eevee Chat
 
 [![PyPI Version](https://img.shields.io/pypi/v/eevee-chat?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
 [![Python Version](https://img.shields.io/pypi/pyversions/eevee-chat.svg?style=for-the-badge)](https://pypi.org/project/eevee-chat/)
+[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-green?style=for-the-badge)](https://creativecommons.org/licenses/by-nc/4.0/)
+
 
 Eevee Chat is a unified chat UI for all LLM frameworks. It allows you to use GPT, Claude and many others from the same window, and switch between them even in the middle of a conversation.
 
 Using Eevee is simple and intuitive. LLMs are connected to the web (supporting LLMs only) with either Google Search or DuckDuckGo, and so it suppose to mimic working with the official web apps.
 
 Eevee can also be configured to support custom frameworks and tools easily. See the docs for more information.
 
@@ -37,7 +39,16 @@
 
 ## Running
 Once installed, simply run:
 ```bash
 eevee
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
+
+## 🎯 Roadmap
+
+- [ ] Code interpreter
+- [x] DeepSeek integration
+- [ ] Google Gemini integration
+- [ ] Add files as text
+- [ ] Add images to multi-modal models
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eevee-chat-0.0.1.post1/setup.py` & `eevee-chat-0.0.2/setup.py`

 * *Files identical despite different names*

