# Comparing `tmp/eevee-chat-0.0.2.post1.tar.gz` & `tmp/eevee-chat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eevee-chat-0.0.2.post1.tar", last modified: Mon Apr  1 11:48:54 2024, max compression
+gzip compressed data, was "eevee-chat-0.0.3.tar", last modified: Mon Apr  1 21:11:34 2024, max compression
```

## Comparing `eevee-chat-0.0.2.post1.tar` & `eevee-chat-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:54.848816 eevee-chat-0.0.2.post1/
--rw-r--r--   0 shakedzy   (502) staff       (20)    19346 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/LICENSE
--rw-r--r--   0 shakedzy   (502) staff       (20)     2066 2024-04-01 11:48:54.847891 eevee-chat-0.0.2.post1/PKG-INFO
--rw-r--r--   0 shakedzy   (502) staff       (20)     1591 2024-03-31 20:57:08.000000 eevee-chat-0.0.2.post1/README.md
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:54.825400 eevee-chat-0.0.2.post1/eevee/
--rw-r--r--   0 shakedzy   (502) staff       (20)      293 2024-04-01 11:31:01.000000 eevee-chat-0.0.2.post1/eevee/__init__.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     2151 2024-04-01 11:36:12.000000 eevee-chat-0.0.2.post1/eevee/_run.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      404 2024-03-31 17:56:15.000000 eevee-chat-0.0.2.post1/eevee/_types.py
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:54.832995 eevee-chat-0.0.2.post1/eevee/chat_connectors/
--rw-r--r--   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:14.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/__init__.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     1328 2024-03-31 20:11:12.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/anthropic_connector.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      628 2024-03-31 20:11:38.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/connector_interface.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      679 2024-03-31 20:14:03.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/deepseek_connector.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     3074 2024-03-31 20:13:19.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/mistral_connector.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     4001 2024-03-31 20:09:28.000000 eevee-chat-0.0.2.post1/eevee/chat_connectors/openai_connector.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     8281 2024-04-01 11:32:01.000000 eevee-chat-0.0.2.post1/eevee/chatbot.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     4268 2024-03-31 20:49:22.000000 eevee-chat-0.0.2.post1/eevee/color_logger.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      804 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/eevee/framework_models.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     7099 2024-03-31 20:04:25.000000 eevee-chat-0.0.2.post1/eevee/messages.py
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:54.839040 eevee-chat-0.0.2.post1/eevee/resources/
--rw-r--r--   0 shakedzy   (502) staff       (20)      459 2024-03-31 17:56:59.000000 eevee-chat-0.0.2.post1/eevee/resources/config.toml
--rw-r--r--   0 shakedzy   (502) staff       (20)     7418 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/eevee/resources/eevee_50.png
--rw-r--r--   0 shakedzy   (502) staff       (20)     3743 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/eevee/saved_chat.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     1734 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/eevee/settings.py
--rw-r--r--   0 shakedzy   (502) staff       (20)     4836 2024-03-31 20:26:50.000000 eevee-chat-0.0.2.post1/eevee/tools.py
--rw-r--r--   0 shakedzy   (502) staff       (20)    11257 2024-04-01 11:32:53.000000 eevee-chat-0.0.2.post1/eevee/ui.py
--rw-r--r--   0 shakedzy   (502) staff       (20)      144 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/eevee/utils.py
-drwxr-xr-x   0 shakedzy   (502) staff       (20)        0 2024-04-01 11:48:54.846320 eevee-chat-0.0.2.post1/eevee_chat.egg-info/
--rw-r--r--   0 shakedzy   (502) staff       (20)     2066 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/PKG-INFO
--rw-r--r--   0 shakedzy   (502) staff       (20)      753 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/SOURCES.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)        1 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/dependency_links.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)       42 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/entry_points.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)      193 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/requires.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)        6 2024-04-01 11:48:54.000000 eevee-chat-0.0.2.post1/eevee_chat.egg-info/top_level.txt
--rw-r--r--   0 shakedzy   (502) staff       (20)       38 2024-04-01 11:48:54.849087 eevee-chat-0.0.2.post1/setup.cfg
--rw-r--r--   0 shakedzy   (502) staff       (20)     1522 2024-03-31 12:17:47.000000 eevee-chat-0.0.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:34.172457 eevee-chat-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    19346 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-01 21:11:34.172457 eevee-chat-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:34.168457 eevee-chat-0.0.3/eevee/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:34.168457 eevee-chat-0.0.3/eevee/chat_connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/anthropic_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/connector_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/deepseek_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/google_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/mistral_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chat_connectors/openai_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/color_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/framework_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:34.172457 eevee-chat-0.0.3/eevee/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/resources/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/resources/eevee_50.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/saved_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11437 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/eevee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:11:34.172457 eevee-chat-0.0.3/eevee_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:11:34.000000 eevee-chat-0.0.3/eevee_chat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:11:34.172457 eevee-chat-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-01 21:11:26.000000 eevee-chat-0.0.3/setup.py
```

### Comparing `eevee-chat-0.0.2.post1/LICENSE` & `eevee-chat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/PKG-INFO` & `eevee-chat-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevee-chat
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: A single chat interface for multiple LLMs
 Home-page: http://shakedzy.xyz/eevee-chat
 Download-URL: https://pypi.org/project/eevee-chat/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3.11
@@ -44,11 +44,11 @@
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
 
 ## 🎯 Roadmap
 
 - [ ] Code interpreter
 - [x] DeepSeek integration
-- [ ] Google Gemini integration
+- [x] Google Gemini integration
 - [ ] Add files as text
 - [ ] Add images to multi-modal models
- 
+- [ ] Enable speech-to-text as input
```

### Comparing `eevee-chat-0.0.2.post1/README.md` & `eevee-chat-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,11 @@
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
 
 ## 🎯 Roadmap
 
 - [ ] Code interpreter
 - [x] DeepSeek integration
-- [ ] Google Gemini integration
+- [x] Google Gemini integration
 - [ ] Add files as text
 - [ ] Add images to multi-modal models
- 
+- [ ] Enable speech-to-text as input
```

### Comparing `eevee-chat-0.0.2.post1/eevee/_run.py` & `eevee-chat-0.0.3/eevee/_run.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chat_connectors/anthropic_connector.py` & `eevee-chat-0.0.3/eevee/chat_connectors/anthropic_connector.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chat_connectors/connector_interface.py` & `eevee-chat-0.0.3/eevee/chat_connectors/connector_interface.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chat_connectors/deepseek_connector.py` & `eevee-chat-0.0.3/eevee/chat_connectors/deepseek_connector.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chat_connectors/mistral_connector.py` & `eevee-chat-0.0.3/eevee/chat_connectors/mistral_connector.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chat_connectors/openai_connector.py` & `eevee-chat-0.0.3/eevee/chat_connectors/openai_connector.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/chatbot.py` & `eevee-chat-0.0.3/eevee/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .framework_models import get_model_framework
 from .saved_chat import SavedChat
 from .chat_connectors.connector_interface import Connector
 from .chat_connectors.openai_connector import OpenAIConnector
 from .chat_connectors.anthropic_connector import AnthropicConnector
 from .chat_connectors.mistral_connector import MistralConnector
 from .chat_connectors.deepseek_connector import DeepSeekConnector
+from .chat_connectors.google_connector import GoogleConnector
 from ._types import Framework
 from . import ROOT_DIR
 
 
 class Chatbot:
     def __init__(self, available_frameworks: Set[Framework]) -> None:
         if not available_frameworks:
@@ -34,14 +35,18 @@
                     client = OpenAIConnector()
                 case 'mistral':
                     client = MistralConnector()
                 case 'anthropic':
                     client = AnthropicConnector()
                 case 'deepseek':
                     client = DeepSeekConnector()
+                case 'google':
+                    client = GoogleConnector()
+                case _:
+                    raise ValueError(f'No connector defined for framework {framework}!')
             self.clients[framework] = client
 
     def _build_tools(self) -> List[Dict[str, Any]]:
         tools = list()
         for func, v in tools_params_definitions.items():
             params = {}
             required = []
```

### Comparing `eevee-chat-0.0.2.post1/eevee/color_logger.py` & `eevee-chat-0.0.3/eevee/color_logger.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/framework_models.py` & `eevee-chat-0.0.3/eevee/framework_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import get_args, Set, Dict, List
+from typing import get_args, Set, Dict, List, Tuple
 from .settings import Settings
 from ._types import Framework
 
 
 def get_available_frameworks() -> Set[Framework]:
     available: Set[Framework] = set()
     models_dict: Dict = Settings().models
@@ -15,10 +15,18 @@
             available.add(framework)
     return available
 
 
 def get_model_framework(model: str) -> Framework:
     models_dict: Dict[Framework, List[str]] = Settings().models
     for framework, models in models_dict.items():
-        if model in models:
+        if model in [get_model_name_and_alias(m)[0] for m in models]:
             return framework
     raise ValueError(f"Model {model} does not belong to any framework!")
+
+
+def get_model_name_and_alias(model_string: str) -> Tuple[str, str | None]:
+    pieces = model_string.split('::')
+    if len(pieces) == 1:
+        return model_string, None
+    else:
+        return '::'.join(pieces[1:]), pieces[0]
```

### Comparing `eevee-chat-0.0.2.post1/eevee/messages.py` & `eevee-chat-0.0.3/eevee/messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,19 +65,23 @@
         if content:
             self.content = content
         if tool_calls:
             self.tool_calls = tool_calls
     
     def to(self, framework: Framework):
         match framework:
-            case 'openai':
+            case 'openai' | 'deepseek':
                 if self.role == 'tool':
+                    if framework == 'deepseek':
+                        return None
                     tool_call_id = self.tool_calls[0].call_id
                     tool_calls = None
                 elif self.tool_calls:
+                    if framework == 'deepseek':
+                        return None
                     tool_call_id = None
                     tool_calls = list()
                     for tool_call in self.tool_calls:
                         tool_call_dict = dict()
                         tool_call_dict['id'] = tool_call.call_id
                         tool_call_dict['type'] = 'function'
                         tool_call_dict['function'] = {'name': tool_call.function, 'arguments': str(tool_call.arguments)}
@@ -92,21 +96,17 @@
                 if tool_calls:
                     message['tool_calls'] = tool_calls
                 if tool_call_id:
                     message['tool_call_id'] = tool_call_id
                 return message
             
             case 'anthropic':
-                if self.role == 'system':
+                if self.role in ['system', 'tool'] or self.tool_calls:
                     return None
                 message = {'role': self.role, 'content': self.content}
-                if not message['content'] and self.tool_calls:
-                    message['content'] = f"Executing functions: [{', '.join([str(t) for t in self.tool_calls])}]"
-                elif message['role'] == 'tool':
-                    message['role'] = 'user'
                 return message
 
             case 'mistral':
                 if self.role in ['system', 'user']:
                     message = MistralChatMessage(role=self.role, content=self.content or '')
                 elif self.role == 'tool':
                     message = MistralChatMessage(role=self.role, content=self.content or '', name=self.tool_calls[0].function)
@@ -117,14 +117,25 @@
                             function_call = MistralFunctionCall(name=tool_call.function, arguments=json.dumps(tool_call.arguments))
                             mistral_tool_calls.append(MistralToolCall(function=function_call))
                     else:
                         mistral_tool_calls = None
                     message = MistralChatMessage(role=self.role, content=self.content or '', tool_calls=mistral_tool_calls)
                 return message
 
+            case 'google':
+                if self.role in ['system', 'tool'] or self.tool_calls:
+                    return None
+                google_role: str = self.role
+                if google_role == 'assistant':
+                    google_role = 'model'
+                message = {'role': google_role, 'parts': [self.content]}
+                return message
+
+            case _:
+                raise ValueError(f"Can't convert messages to framework {framework}")
 
 class Messages(list[Message]):
     def __init__(self, *args) -> None:
         super().__init__(*args)
 
     @classmethod
     def from_dict(cls, messages_as_dict: List[Dict[str, Any]]):
```

### Comparing `eevee-chat-0.0.2.post1/eevee/resources/eevee_50.png` & `eevee-chat-0.0.3/eevee/resources/eevee_50.png`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/saved_chat.py` & `eevee-chat-0.0.3/eevee/saved_chat.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/settings.py` & `eevee-chat-0.0.3/eevee/settings.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/tools.py` & `eevee-chat-0.0.3/eevee/tools.py`

 * *Files identical despite different names*

### Comparing `eevee-chat-0.0.2.post1/eevee/ui.py` & `eevee-chat-0.0.3/eevee/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 import json
+import pathlib
 import gradio as gr
 from datetime import datetime
 from typing import List, Tuple, Generator, Set, Tuple, Dict, Any
 from .saved_chat import SavedChat
 from .chatbot import Chatbot
 from .settings import Settings
 from .utils import path_to_resource
+from .framework_models import get_model_name_and_alias
 from ._types import Framework
-from . import ROOT_DIR
 
 
 class UI:
     CHAT_FILE_TIME_FORMAT = "%d/%m/%Y, %H:%M:%S"
     MODEL_NAME_SEPARATOR = "\n\n🤖 "
 
     def __init__(self, chatbot: Chatbot, available_frameworks: Set[Framework], port: int) -> None:
@@ -33,29 +34,29 @@
         if self.ui:
             self.ui.close()
             with open(self.preferences_file_path, 'w') as f:
                 json.dump(self.preferences, f)
 
     @property
     def preferences_file_path(self) -> str:
-        filename = "pref.json"
-        return os.path.join(ROOT_DIR, filename)
+        return path_to_resource("pref.json")
 
     def _load_preferences_from_file(self) -> Dict[str, Any]:
         try:
             with open(self.preferences_file_path, 'r') as f:
                 return json.load(f)
         except:
             return {}
 
-    def _get_list_of_models(self) -> List[Tuple[Framework, str]]:
-        available_models: List[Tuple[Framework, str]] = list()
+    def _get_list_of_models_and_display_names(self) -> List[Tuple[str, str]]:
+        available_models: List[Tuple[str, str]] = list()
         for framework in self.available_frameworks:
             models: List[str] = Settings().models[framework]
-            available_models += [(framework, model) for model in models]
+            models_and_aliases: List[Tuple[str, str | None]] = [get_model_name_and_alias(m) for m in models]
+            available_models += [(model, f'{self._display_name_of_framework(framework)}: {alias or model}') for model, alias in models_and_aliases]
         return available_models
     
     def _stop_text_generation(self) -> None:
         self._generate_text = False
 
     def _add_user_message_to_chat(self, prompt: str, history: List[List[str | None]]) -> Tuple[str, List[List[str | None]]]:
         return '', history + [[prompt, None]]
@@ -149,30 +150,30 @@
                 min-height: 150px;
                 width: 100%;
                 overflow-x: auto !important;
                 overflow-y: auto !important;
                 scrollbar-width: thin !important;
             }  
         """
-        available_models = self._get_list_of_models()
-        available_models = [(f'{self._display_name_of_framework(framework)}: {model}', model) for (framework, model) in available_models]
+        available_models = self._get_list_of_models_and_display_names()
+        available_models = [(display_name, model) for (model, display_name) in available_models]
         available_models = sorted(available_models, key=lambda t: t[0])
         preferred_model = self.preferences.get('model', '')
         if preferred_model not in [t[1] for t in available_models]:
             self.preferences['model'] = available_models[0][1]
 
         with gr.Blocks(title="Eevee Chat", css=scrollable_checkbox_group_css, theme=gr.themes.Base()) as ui:
             with gr.Row():
                 with gr.Column(scale=10):
                     gr.Markdown(f"# 💬 Eevee Chat")
                 with gr.Column(scale=1):
                     new_chat = gr.Button("New Chat")
             
             with gr.Row():
-                with gr.Column(scale=1, variant='panel'):
+                with gr.Column(scale=2, variant='panel'):
                     with gr.Group():
                         model = gr.Dropdown(label="Model", interactive=True, choices=available_models, value=self.preferences['model'])  # type: ignore
                         with gr.Accordion(label="System Prompt", open=False):
                             system_prompt = gr.TextArea(value="You are a helpful AI assistance, and your task is to assist the user with all its requests in the best possible way", container=False, interactive=True, lines=10)
                         temperature = gr.Slider(label="Temperature", minimum=0., maximum=1., step=.01, value=self.preferences.get('temperature', 0.))
                         force_json = gr.Checkbox(label="Force JSON", value=False, interactive=True)
                     gr.Markdown("Not all models support all options, see [documentation](https://shakedzy.xyz/eevee-chat/tools/#known-limitations) for more information")
```

### Comparing `eevee-chat-0.0.2.post1/eevee_chat.egg-info/PKG-INFO` & `eevee-chat-0.0.3/eevee_chat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eevee-chat
-Version: 0.0.2.post1
+Version: 0.0.3
 Summary: A single chat interface for multiple LLMs
 Home-page: http://shakedzy.xyz/eevee-chat
 Download-URL: https://pypi.org/project/eevee-chat/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: CC BY-NC 4.0
 Classifier: Programming Language :: Python :: 3.11
@@ -44,11 +44,11 @@
 ```
 Eevee Chat will automatically launch on `127.0.0.1:4242` by default.
 
 ## 🎯 Roadmap
 
 - [ ] Code interpreter
 - [x] DeepSeek integration
-- [ ] Google Gemini integration
+- [x] Google Gemini integration
 - [ ] Add files as text
 - [ ] Add images to multi-modal models
- 
+- [ ] Enable speech-to-text as input
```

### Comparing `eevee-chat-0.0.2.post1/eevee_chat.egg-info/SOURCES.txt` & `eevee-chat-0.0.3/eevee_chat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 eevee/tools.py
 eevee/ui.py
 eevee/utils.py
 eevee/chat_connectors/__init__.py
 eevee/chat_connectors/anthropic_connector.py
 eevee/chat_connectors/connector_interface.py
 eevee/chat_connectors/deepseek_connector.py
+eevee/chat_connectors/google_connector.py
 eevee/chat_connectors/mistral_connector.py
 eevee/chat_connectors/openai_connector.py
 eevee/resources/config.toml
 eevee/resources/eevee_50.png
 eevee_chat.egg-info/PKG-INFO
 eevee_chat.egg-info/SOURCES.txt
 eevee_chat.egg-info/dependency_links.txt
```

### Comparing `eevee-chat-0.0.2.post1/setup.py` & `eevee-chat-0.0.3/setup.py`

 * *Files identical despite different names*

