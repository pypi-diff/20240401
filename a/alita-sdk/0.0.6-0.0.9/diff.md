# Comparing `tmp/alita_sdk-0.0.6.tar.gz` & `tmp/alita_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alita_sdk-0.0.6.tar", last modified: Wed Mar 13 15:14:44 2024, max compression
+gzip compressed data, was "alita_sdk-0.0.9.tar", last modified: Mon Mar 18 10:32:47 2024, max compression
```

## Comparing `alita_sdk-0.0.6.tar` & `alita_sdk-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.493570 alita_sdk-0.0.6/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.0.6/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-13 15:14:44.493324 alita_sdk-0.0.6/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.0.6/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-03-13 15:14:33.000000 alita_sdk-0.0.6/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)       92 2024-03-10 17:05:00.000000 alita_sdk-0.0.6/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-03-13 15:14:44.493615 alita_sdk-0.0.6/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.489262 alita_sdk-0.0.6/src/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.0.6/src/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.489350 alita_sdk-0.0.6/src/alita_sdk/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.0.6/src/alita_sdk/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.491157 alita_sdk-0.0.6/src/alita_sdk/agents/
--rw-r--r--   0 arozumenko   (501) staff       (20)     2345 2024-03-13 12:42:57.000000 alita_sdk-0.0.6/src/alita_sdk/agents/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.0.6/src/alita_sdk/agents/base_actions.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2250 2024-03-13 14:23:56.000000 alita_sdk-0.0.6/src/alita_sdk/agents/mixedAgentParser.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1111 2024-03-13 12:18:47.000000 alita_sdk-0.0.6/src/alita_sdk/agents/mixedAgentRenderes.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1231 2024-03-13 15:14:36.000000 alita_sdk-0.0.6/src/alita_sdk/agents/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.491571 alita_sdk-0.0.6/src/alita_sdk/clients/
--rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.0.6/src/alita_sdk/clients/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    12028 2024-03-13 14:25:32.000000 alita_sdk-0.0.6/src/alita_sdk/clients/client.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.492107 alita_sdk-0.0.6/src/alita_sdk/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.0.6/src/alita_sdk/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     8311 2024-03-10 11:45:00.000000 alita_sdk-0.0.6/src/alita_sdk/llms/alita.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.492824 alita_sdk-0.0.6/src/alita_sdk/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.0.6/src/alita_sdk/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      863 2024-03-13 12:05:45.000000 alita_sdk-0.0.6/src/alita_sdk/tools/datasource.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:46:26.000000 alita_sdk-0.0.6/src/alita_sdk/tools/prompt.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.492917 alita_sdk-0.0.6/src/alita_sdk/utils/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.0.6/src/alita_sdk/utils/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:44.493059 alita_sdk-0.0.6/src/alita_sdk.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-13 15:14:44.000000 alita_sdk-0.0.6/src/alita_sdk.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)      712 2024-03-13 15:14:44.000000 alita_sdk-0.0.6/src/alita_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-03-13 15:14:44.000000 alita_sdk-0.0.6/src/alita_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       93 2024-03-13 15:14:44.000000 alita_sdk-0.0.6/src/alita_sdk.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-03-13 15:14:44.000000 alita_sdk-0.0.6/src/alita_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.414049 alita_sdk-0.0.9/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11357 2024-03-08 11:24:37.000000 alita_sdk-0.0.9/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-18 10:32:47.413834 alita_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3200 2024-03-10 12:01:09.000000 alita_sdk-0.0.9/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      705 2024-03-18 10:32:28.000000 alita_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)       92 2024-03-10 17:05:00.000000 alita_sdk-0.0.9/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-03-18 10:32:47.414093 alita_sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.409391 alita_sdk-0.0.9/src/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:38.000000 alita_sdk-0.0.9/src/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.409477 alita_sdk-0.0.9/src/alita_sdk/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-08 11:25:50.000000 alita_sdk-0.0.9/src/alita_sdk/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.411252 alita_sdk-0.0.9/src/alita_sdk/agents/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2412 2024-03-18 10:31:52.000000 alita_sdk-0.0.9/src/alita_sdk/agents/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2993 2024-03-18 10:31:45.000000 alita_sdk-0.0.9/src/alita_sdk/agents/alita_openai.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-10 11:28:03.000000 alita_sdk-0.0.9/src/alita_sdk/agents/base_actions.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2325 2024-03-13 17:32:26.000000 alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentParser.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2283 2024-03-18 10:31:02.000000 alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentRenderes.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1231 2024-03-13 15:14:36.000000 alita_sdk-0.0.9/src/alita_sdk/agents/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.411929 alita_sdk-0.0.9/src/alita_sdk/clients/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       31 2024-03-09 15:53:40.000000 alita_sdk-0.0.9/src/alita_sdk/clients/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    14057 2024-03-18 09:54:26.000000 alita_sdk-0.0.9/src/alita_sdk/clients/client.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.412627 alita_sdk-0.0.9/src/alita_sdk/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)       33 2024-03-09 14:45:23.000000 alita_sdk-0.0.9/src/alita_sdk/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     8311 2024-03-10 11:45:00.000000 alita_sdk-0.0.9/src/alita_sdk/llms/alita.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413373 alita_sdk-0.0.9/src/alita_sdk/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:45:42.000000 alita_sdk-0.0.9/src/alita_sdk/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      863 2024-03-13 12:05:45.000000 alita_sdk-0.0.9/src/alita_sdk/tools/datasource.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-11 07:46:26.000000 alita_sdk-0.0.9/src/alita_sdk/tools/prompt.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413469 alita_sdk-0.0.9/src/alita_sdk/utils/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-03-13 15:14:37.000000 alita_sdk-0.0.9/src/alita_sdk/utils/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-18 10:32:47.413606 alita_sdk-0.0.9/src/alita_sdk.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3905 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)      749 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       93 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       19 2024-03-18 10:32:47.000000 alita_sdk-0.0.9/src/alita_sdk.egg-info/top_level.txt
```

### Comparing `alita_sdk-0.0.6/LICENSE` & `alita_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.6/PKG-INFO` & `alita_sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.0.6
+Version: 0.0.9
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.0.6/README.md` & `alita_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.6/pyproject.toml` & `alita_sdk-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alita_sdk"
-version = "0.0.6"
+version = "0.0.9"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "SDK for building langchain agents using resouces from Alita"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk/agents/__init__.py` & `alita_sdk-0.0.9/src/alita_sdk/agents/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from langchain.agents import AgentOutputParser
 from langchain.agents.format_scratchpad import format_log_to_str
 
 from langchain.tools.render import ToolsRenderer
 
 from .mixedAgentRenderes import render_text_description_and_args, format_log_to_str
-from .mixedAgentParser import MixedAgentOutputParser
+from .mixedAgentParser import MixedAgentOutputParser, FORMAT_INSTRUCTIONS
 
 logger = logging.getLogger(__name__)
 
 
 def create_mixed_agent(
     llm: BaseLanguageModel,
     tools: Sequence[BaseTool],
@@ -45,14 +45,15 @@
     )
     if missing_vars:
         raise ValueError(f"Prompt missing required variables: {missing_vars}")
 
     prompt = prompt.partial(
         tools=tools_renderer(list(tools)),
         tool_names=", ".join([t.name for t in tools]),
+        response_format = FORMAT_INSTRUCTIONS
     )
     # llm_with_stop = llm.bind(stop=["\"tool\":", "Running Tool:"])
     output_parser = output_parser or MixedAgentOutputParser()
     logger.debug("Prompt in mixed agent: %s", prompt)
     agent = (
         RunnablePassthrough.assign(
             agent_scratchpad=lambda x: format_log_to_str(x['intermediate_steps']),
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk/agents/mixedAgentParser.py` & `alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 Running Tool:
 {action} with param {tool_input}
 """
         if action:
             if action == 'complete_task':
                 return AgentFinish({"output": tool_input[list(tool_input.keys())[0]]}, log=log)
             return AgentAction(action, tool_input, log)
+        elif txt:
+            return AgentFinish({"output": txt}, log=log)
         else:
             raise OutputParserException(f"""ERROR: RESPONSE FORMAT IS INCORRECT
 The response may have a great data, format response to the required JSON strcuture. 
 Expected format: {FORMAT_INSTRUCTIONS}
 
 Recieved data: {response}""")
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk/agents/mixedAgentRenderes.py` & `alita_sdk-0.0.9/src/alita_sdk/agents/mixedAgentRenderes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Parser for MixedAgentTools."""
 import logging
 from typing import  List, Tuple, Dict, Any
+from uuid import uuid4
 from langchain_core.tools import BaseTool
 from langchain_core.agents import AgentAction
-from langchain_core.messages import ToolMessage, AIMessage
+from langchain_core.messages import ToolMessage, AIMessage, BaseMessage, SystemMessage, HumanMessage
 logger = logging.getLogger(__name__)
 
 def render_text_description_and_args(tools: List[BaseTool]) -> str:
     """Render the tool name, description, and args in plain text."""
     tool_strings = []
     for tool in tools:
         args_schema = ""
@@ -21,7 +22,33 @@
 ) -> str:
     """Construct the scratchpad that lets the agent continue its thought process."""
     thoughts = ""
     for action, result in intermediate_steps:
         thoughts += action.log
         thoughts += f"\nTool Result:\n{result}"
     return thoughts
+
+def format_to_messages(intermediate_steps: List[Tuple[AgentAction, str]]) -> List[BaseMessage]:
+    """Format the intermediate steps to messages."""
+    messages = []
+    for action, result in intermediate_steps:
+        messages.append(
+            {"role": "ai", "content": action.log}
+        )
+        messages.append(
+            {"role": "tool", "content": result, "tool_call_id": str(uuid4())}
+        )
+    return messages
+
+def conversaiont_to_messages(conversation: List[Dict[str, str]]) -> List[BaseMessage]:
+    """Format the conversation to messages."""
+    messages = []
+    for message in conversation:
+        if message["role"] == "user":
+            messages.append(HumanMessage(content=message["content"]))
+        elif message["role"] == "ai" or message["role"] == "bot" or message["role"] == "assistant":
+            messages.append(AIMessage(content=message["content"]))
+        elif message["role"] == "tool":
+            messages.append(HumanMessage(content=message["content"]))
+        else:
+            messages.append(SystemMessage(content=message["content"]))
+    return messages
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk/agents/utils.py` & `alita_sdk-0.0.9/src/alita_sdk/agents/utils.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.6/src/alita_sdk/clients/client.py` & `alita_sdk-0.0.9/src/alita_sdk/clients/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,19 @@
     AIMessage,
     HumanMessage,
     SystemMessage,
     BaseMessage,
     ToolMessage
 )
 from langchain_core.prompts import ChatPromptTemplate
+from langchain.agents import  AgentExecutor
 
 logger = logging.getLogger(__name__)
+from ..agents import create_mixed_agent
+from ..agents.alita_openai import AlitaAssistantRunnable
 
 class Jinja2TemplatedChatMessagesTemplate(ChatPromptTemplate):
     
     def _resolve_variables(self, message:BaseMessage, kwargs:Dict) -> BaseMessage:
         environment = Environment(undefined=DebugUndefined)
         template = environment.from_string(message.content)
         content = template.render(kwargs)
@@ -64,16 +67,46 @@
         return self.alita.rag(self.datasource_id, messages, 
                               self.datasource_settings, 
                               self.datasource_predict_settings)
         
     def search(self, query: str):
         return self.alita.search(self.datasource_id, [HumanMessage(content=query)], 
                                   self.datasource_settings)
+        
 
 
+class Assistant:
+    def __init__(self, client:Any, prompt:ChatPromptTemplate, tools: list, 
+                 openai_tools: Optional[Dict]=None):
+        self.prompt = prompt
+        self.client = client
+        self.tools = tools
+        self.openai_tools = openai_tools
+    
+    def getAgentExecutor(self):
+        agent = create_mixed_agent(llm=self.client, tools=self.tools, prompt=self.prompt)
+        return AgentExecutor.from_agent_and_tools(agent=agent, tools=self.tools,
+                                                  verbose=True, handle_parsing_errors=True, 
+                                                  max_execution_time=None, return_intermediate_steps=True)
+        
+    def getOpenAIAgentExecutor(self):
+        agent = AlitaAssistantRunnable(client=self.client, assistant=self)
+        return AgentExecutor.from_agent_and_tools(agent=agent, tools=self.tools,
+                                                  verbose=True, handle_parsing_errors=True, 
+                                                  max_execution_time=None,
+                                                  return_intermediate_steps=True)
+    
+    # This one is used only in Alita OpenAI
+    def apredict(self, messages: list[BaseMessage]):
+        yield from response = self.client.ainvoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
+    
+    def predict(self, messages: list[BaseMessage]):
+        response = self.client.invoke([self.prompt.messages[0]] + messages, functions=self.openai_tools)
+        return response
+    
 
 class AlitaClient:
     def __init__(self, base_url: str, project_id: int, auth_token: str):
         self.base_url = base_url
         self.project_id = project_id
         self.auth_token = auth_token        
         self.headers = {
@@ -142,15 +175,22 @@
             "temperature": temperature,
             "top_p": top_p,
             "top_k": top_k,
             "max_length": max_length,
             "stream": stream,
         }
         return AlitaDataSource(self, datasource_id,datasource_settings, datasource_predict_settings)
-        
+    
+    
+    def assistant(self, prompt_id: int, prompt_version_id: int, 
+                  tools: list, openai_tools: Optional[Dict]=None, 
+                  client: Optional[Any] = None):
+        prompt = self.prompt(prompt_id=prompt_id, prompt_version_id=prompt_version_id)
+        return Assistant(client, prompt, tools, openai_tools)
+    
     def _prepare_messages(self, messages: list[BaseMessage]):
         context = ''
         chat_history = []
         if messages[0].type == "system":
             context = messages[0].content
         for message in messages[1:-1]:
             if message.type == 'human':
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk/llms/alita.py` & `alita_sdk-0.0.9/src/alita_sdk/llms/alita.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.6/src/alita_sdk/tools/datasource.py` & `alita_sdk-0.0.9/src/alita_sdk/tools/datasource.py`

 * *Files identical despite different names*

### Comparing `alita_sdk-0.0.6/src/alita_sdk.egg-info/PKG-INFO` & `alita_sdk-0.0.9/src/alita_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alita_sdk
-Version: 0.0.6
+Version: 0.0.9
 Summary: SDK for building langchain agents using resouces from Alita
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://projectalita.ai
 Project-URL: Issues, https://github.com/ProjectAlita/alita-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `alita_sdk-0.0.6/src/alita_sdk.egg-info/SOURCES.txt` & `alita_sdk-0.0.9/src/alita_sdk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/alita_sdk/__init__.py
 src/alita_sdk.egg-info/PKG-INFO
 src/alita_sdk.egg-info/SOURCES.txt
 src/alita_sdk.egg-info/dependency_links.txt
 src/alita_sdk.egg-info/requires.txt
 src/alita_sdk.egg-info/top_level.txt
 src/alita_sdk/agents/__init__.py
+src/alita_sdk/agents/alita_openai.py
 src/alita_sdk/agents/base_actions.py
 src/alita_sdk/agents/mixedAgentParser.py
 src/alita_sdk/agents/mixedAgentRenderes.py
 src/alita_sdk/agents/utils.py
 src/alita_sdk/clients/__init__.py
 src/alita_sdk/clients/client.py
 src/alita_sdk/llms/__init__.py
```

