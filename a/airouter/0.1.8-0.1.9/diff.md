# Comparing `tmp/airouter-0.1.8.tar.gz` & `tmp/airouter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airouter-0.1.8.tar", max compression
+gzip compressed data, was "airouter-0.1.9.tar", max compression
```

## Comparing `airouter-0.1.8.tar` & `airouter-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-11-07 08:20:34.824687 airouter-0.1.8/LICENSE
--rw-r--r--   0        0        0     1136 2023-11-10 06:43:46.252338 airouter-0.1.8/README.md
--rw-r--r--   0        0        0      165 2023-11-09 18:28:00.384238 airouter-0.1.8/airouter/__init__.py
--rw-r--r--   0        0        0     4516 2024-02-08 14:38:50.888188 airouter-0.1.8/airouter/models.py
--rw-r--r--   0        0        0        0 2023-11-07 08:20:34.828813 airouter-0.1.8/airouter/providers/__init__.py
--rw-r--r--   0        0        0     2660 2023-11-09 18:23:48.280094 airouter-0.1.8/airouter/providers/aws_bedrock_provider.py
--rw-r--r--   0        0        0      649 2024-02-08 14:41:50.946523 airouter-0.1.8/airouter/providers/azure_openai_provider.py
--rw-r--r--   0        0        0     4804 2023-11-13 06:40:22.177144 airouter-0.1.8/airouter/providers/base_provider.py
--rw-r--r--   0        0        0     1006 2024-02-08 14:41:01.485314 airouter-0.1.8/airouter/providers/factory.py
--rw-r--r--   0        0        0     1607 2024-02-08 14:47:40.549464 airouter-0.1.8/airouter/providers/openai_provider.py
--rw-r--r--   0        0        0     1690 2023-11-09 18:23:48.285490 airouter-0.1.8/airouter/providers/vertex_ai_text_provider.py
--rw-r--r--   0        0        0    14311 2024-02-08 14:53:05.902412 airouter-0.1.8/airouter/streamed_completion.py
--rw-r--r--   0        0        0        0 2023-11-07 08:20:34.829753 airouter-0.1.8/airouter/utils/__init__.py
--rw-r--r--   0        0        0     3551 2023-11-09 18:34:27.775433 airouter-0.1.8/airouter/utils/interactive.py
--rw-r--r--   0        0        0      468 2023-11-07 08:20:34.829938 airouter-0.1.8/airouter/utils/logs.py
--rw-r--r--   0        0        0     2283 2023-11-09 18:21:59.659409 airouter-0.1.8/airouter/utils/tokens.py
--rw-r--r--   0        0        0      347 2024-02-08 14:37:36.555616 airouter-0.1.8/airouter/xperiments/exp_multi.py
--rw-r--r--   0        0        0      492 2024-02-08 14:59:37.570527 airouter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 airouter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-18 12:15:05.072935 airouter-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1136 2024-03-18 12:15:05.072989 airouter-0.1.9/README.md
+-rw-r--r--   0        0        0      165 2024-03-18 12:15:05.073081 airouter-0.1.9/airouter/__init__.py
+-rw-r--r--   0        0        0     5102 2024-03-22 10:27:34.041125 airouter-0.1.9/airouter/models.py
+-rw-r--r--   0        0        0        0 2024-03-18 12:15:05.073263 airouter-0.1.9/airouter/providers/__init__.py
+-rw-r--r--   0        0        0     2779 2024-03-22 09:52:30.048308 airouter-0.1.9/airouter/providers/aws_bedrock_provider.py
+-rw-r--r--   0        0        0      679 2024-03-22 09:52:30.048476 airouter-0.1.9/airouter/providers/azure_openai_provider.py
+-rw-r--r--   0        0        0     5156 2024-03-22 10:27:34.041512 airouter-0.1.9/airouter/providers/base_provider.py
+-rw-r--r--   0        0        0     1165 2024-03-22 10:27:34.041904 airouter-0.1.9/airouter/providers/factory.py
+-rw-r--r--   0        0        0      740 2024-03-22 10:27:34.042196 airouter-0.1.9/airouter/providers/ollama_provider.py
+-rw-r--r--   0        0        0     1610 2024-03-22 09:52:30.049639 airouter-0.1.9/airouter/providers/openai_provider.py
+-rw-r--r--   0        0        0     1690 2024-03-18 12:15:05.073625 airouter-0.1.9/airouter/providers/vertex_ai_text_provider.py
+-rw-r--r--   0        0        0    14518 2024-03-22 09:52:30.049917 airouter-0.1.9/airouter/streamed_completion.py
+-rw-r--r--   0        0        0        0 2024-03-18 12:15:05.073809 airouter-0.1.9/airouter/utils/__init__.py
+-rw-r--r--   0        0        0     3551 2024-03-18 12:15:05.073881 airouter-0.1.9/airouter/utils/interactive.py
+-rw-r--r--   0        0        0      468 2024-03-18 12:15:05.073934 airouter-0.1.9/airouter/utils/logs.py
+-rw-r--r--   0        0        0     2283 2024-03-18 12:15:05.073997 airouter-0.1.9/airouter/utils/tokens.py
+-rw-r--r--   0        0        0      528 2024-03-22 09:52:30.050059 airouter-0.1.9/airouter/xperiments/exp.py
+-rw-r--r--   0        0        0      587 2024-03-22 10:27:34.042552 airouter-0.1.9/airouter/xperiments/exp_multi.py
+-rw-r--r--   0        0        0      557 2024-03-22 10:27:34.043920 airouter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 airouter-0.1.9/PKG-INFO
```

### Comparing `airouter-0.1.8/LICENSE` & `airouter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `airouter-0.1.8/README.md` & `airouter-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `airouter-0.1.8/airouter/models.py` & `airouter-0.1.9/airouter/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   USER = "user"
   ASSISTANT = "assistant"
 
 class ProviderName(str, Enum):
   OPENAI = "openai",
   VERTEX_AI_TEXT = "vertex_ai_text"
   AWS_BEDROCK = "aws_bedrock"
+  OLLAMA = "ollama"
   AZURE_OPENAI = "azure_openai"
 
   @classmethod
   def from_str(cls, value):
     for item in cls:
       if item.value == value:
         return item
@@ -39,14 +40,23 @@
   GPT_4_1106_PREVIEW = "gpt-4-1106-preview" # 128K
 
   ANTROPHIC_CLAUDE_INSTANT_V1 = "anthropic.claude-instant-v1"
   ANTROPHIC_CLAUDE_V2 = "anthropic.claude-v2"
 
   PALM_TEXT_BISON_32K = "text-bison-32k"
 
+  MISTRAL = 'mistral'
+  MIXTRAL = 'mixtral'
+  MIXTRAL_8X7B = 'mixtral:8x7b'
+  LLAMA2 = 'llama2'
+  LLAMA2_TEXT = 'llama2_text'
+  LLAMA2_13B = 'llama2:13b'
+  LLAMA2_70B = 'llama2:70b'
+
+
   @classmethod
   def from_str(cls, value):
     for item in cls:
       if item.value == value:
         return item
     raise ValueError(f"{value} is not a valid LLM")
 
@@ -144,14 +154,24 @@
     ],
     ProviderName.AWS_BEDROCK: [
       LLM.ANTROPHIC_CLAUDE_INSTANT_V1,
       LLM.ANTROPHIC_CLAUDE_V2,
     ],
     ProviderName.VERTEX_AI_TEXT: [
       LLM.PALM_TEXT_BISON_32K,
+    ],
+    ProviderName.OLLAMA: [
+      LLM.MISTRAL,
+      LLM.MIXTRAL,
+      LLM.MIXTRAL_8X7B,
+
+      LLM.LLAMA2,
+      LLM.LLAMA2_TEXT,
+      LLM.LLAMA2_13B,
+      LLM.LLAMA2_70B,
     ]
   }
 
   map_llm_to_provider = {llm: p for p, llms in map_provider_to_llms.items() for llm in llms}
 
   map_context_size = {
     LLM.GPT_3_5_TURBO: 4_096,
@@ -171,14 +191,23 @@
 
     LLM.GPT_4_1106_PREVIEW: 128_000,
 
     LLM.ANTROPHIC_CLAUDE_INSTANT_V1: 100_000,
     LLM.ANTROPHIC_CLAUDE_V2: 100_000,
 
     LLM.PALM_TEXT_BISON_32K: 32_000,
+
+    LLM.MISTRAL: 8_192, # TODO: recheck
+    LLM.MIXTRAL: 8_192,
+    LLM.MIXTRAL_8X7B: 8_192,
+    LLM.LLAMA2: 4_096,
+    LLM.LLAMA2_TEXT: 4_096,
+    LLM.LLAMA2_13B: 4_096,
+    LLM.LLAMA2_70B: 4_096,
+
   }
 
   map_role_for_prompt = {
     ChatRole.SYSTEM: "System",
     ChatRole.USER: "Human",
     ChatRole.ASSISTANT: "Assistant"
   }
```

### Comparing `airouter-0.1.8/airouter/providers/aws_bedrock_provider.py` & `airouter-0.1.9/airouter/providers/aws_bedrock_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import httpx
 from airouter.providers.base_provider import BaseProvider, GenerationOutput
 from airouter.models import map_context_size
 from decouple import config
 
 PROVIDER_CONFIGURED = False
 
 try:
@@ -45,17 +46,19 @@
       'accept': accept,
       'contentType': contentType,
     }
 
   def get_response(self):
     aws_config = None
     if self.timeout is not None:
+      if isinstance(self.timeout, float):
+        self.timeout = httpx.Timeout(self.timeout)
       aws_config = Config(
-        connect_timeout=self.timeout,
-        read_timeout=self.timeout,
+        connect_timeout=self.timeout.connect,
+        read_timeout=self.timeout.read,
         retries={'max_attempts': 0}
       )
 
     boto3_sess = boto3.Session(**BOTO3_KWARGS)
     boto3_bedrock = boto3_sess.client(
       service_name='bedrock-runtime',
       config=aws_config,
```

### Comparing `airouter-0.1.8/airouter/providers/azure_openai_provider.py` & `airouter-0.1.9/airouter/providers/azure_openai_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 
 PROVIDER_CONFIGURED = False
 
 try:
   import openai
   os.environ['AZURE_OPENAI_ENDPOINT'] = config("AZURE_OPENAI_ENDPOINT")
   os.environ['AZURE_OPENAI_API_KEY'] = config("AZURE_OPENAI_API_KEY")
+  os.environ['OPENAI_API_VERSION'] = config("OPENAI_API_VERSION", "2023-09-01-preview")
   PROVIDER_CONFIGURED = True
 except:
   pass
 
 class AzureOpenAIProvider(OpenAIProvider):
   def __init__(self, **kwargs):
     super(OpenAIProvider, self).__init__(**kwargs)
     return
 
   @property
   def openai_client(self):
-    return openai.AzureOpenAI(
-      api_version="2023-09-01-preview",
-      azure_deployment=self.model.value.replace('.', '')
-    )
+    return openai.AzureOpenAI(api_version=os.environ['OPENAI_API_VERSION'])
```

### Comparing `airouter-0.1.8/airouter/providers/base_provider.py` & `airouter-0.1.9/airouter/providers/base_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import abc
 import typing as t
 import json
 import time
 import statistics
 import numpy as np
+import httpx
 from pydantic import BaseModel, Extra
 from airouter.models import (
   LLM, Messages, Functions, map_context_size, map_role_for_prompt,
   ChatRole, GenerationOutput,
 )
 
+
+
 class Schema(BaseModel):
   model: LLM
   messages: Messages
   max_tokens: t.Optional[int] = None
   temperature: t.Optional[float] = None
   functions: t.Optional[Functions] = None
   n: t.Optional[int] = None
   top_p: t.Optional[float] = None
   frequence_penalty: t.Optional[float] = None
   presence_penalty: t.Optional[float] = None
   stop: t.Optional[t.Union[str, t.List[str]]] = None
   user: t.Optional[str] = None
 
-  timeout: t.Optional[float] = None
+  timeout: t.Optional[float | httpx.Timeout] = None
+
+  class Config:
+    arbitrary_types_allowed = True
+
 
 def basic_statistics(lst):
   if len(lst) == 0:
     return {
       'min': np.nan, 'max': np.nan,
       'avg': np.nan, 'median': np.nan,
     }
@@ -53,23 +60,25 @@
     median_value = np.nan
 
   return {
     'min': min_value, 'max': max_value,
     'avg': avg_value, 'median': median_value,
   }
 
+
 def _default_timings():
   return {
     'response_time': np.nan,
     'first_event_time': np.nan,
     'next_events_times': [],
     'execution_time': np.nan,
     'speed': np.nan, # chars per second
   }
 
+
 class BaseProvider(Schema, extra=Extra.allow, arbitrary_types_allowed=True):
   _attrs = {
     'parameters': {},
     'timings': _default_timings(),
     'last_exception': None,
   }
 
@@ -83,19 +92,23 @@
     return self._attrs['last_exception']
 
   @last_exception.setter
   def last_exception(self, exc):
     self._attrs['last_exception'] = exc
 
   def clean_parameters(self):
-    self._attrs['parameters'] = json.loads(self.json(exclude={'_attrs', 'retry'}))
+    self._attrs['parameters'] = self.model_dump(exclude={'_attrs', 'retry'})
     keys = list(self._attrs['parameters'].keys())
     for k in keys:
       if self._attrs['parameters'][k] is None:
         self._attrs['parameters'].pop(k)
+      elif isinstance(self._attrs['parameters'][k], httpx.Timeout):
+        timeout = self._attrs['parameters'][k]
+        if timeout.read is None and timeout.connect is None and timeout.write is None and timeout.pool is None:
+          self._attrs['parameters'].pop(k)
     return
 
   def refresh_timings(self):
     self._attrs['timings'] = _default_timings()
     return
 
   def set_response_time(self, nr_seconds):
@@ -167,15 +180,15 @@
 
     self.set_response_time(end-start)
 
     i = -1
     start = time.time()
     for event in response:
       # TODO event can be None??
-      i+=1
+      i += 1
       end = time.time()
       if i == 0:
         self.set_first_event_time(end-start)
       else:
         self.append_next_event_time(end-start)
       start = time.time()
       yield i,event
```

### Comparing `airouter-0.1.8/airouter/providers/factory.py` & `airouter-0.1.9/airouter/providers/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import typing as t
 from airouter.models import ProviderName
 from airouter.providers.base_provider import BaseProvider
 from airouter.providers.openai_provider import OpenAIProvider
 from airouter.providers.aws_bedrock_provider import AWSBedrockProvider
 from airouter.providers.vertex_ai_text_provider import VertexAITextProvider
+from airouter.providers.ollama_provider import OllamaProvider
 from airouter.providers.azure_openai_provider import AzureOpenAIProvider
 
+
 def provider_factory(provider_name, **llm_params) -> t.Optional[BaseProvider]:
   if isinstance(provider_name, str):
     provider_name = ProviderName.from_str(provider_name)
 
   if provider_name == ProviderName.OPENAI:
     return OpenAIProvider(stream=True, **llm_params)
 
   if provider_name == ProviderName.AWS_BEDROCK:
     return AWSBedrockProvider(stream=True, **llm_params)
 
   if provider_name == ProviderName.VERTEX_AI_TEXT:
     return VertexAITextProvider(stream=True, **llm_params)
 
+  if provider_name == ProviderName.OLLAMA:
+    return OllamaProvider(stream=True, **llm_params)
   if provider_name == ProviderName.AZURE_OPENAI:
     return AzureOpenAIProvider(stream=True, **llm_params)
 
   return
```

### Comparing `airouter-0.1.8/airouter/providers/openai_provider.py` & `airouter-0.1.9/airouter/providers/openai_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 try:
   import openai
   os.environ['OPENAI_API_KEY'] = config("OPENAI_API_KEY")
   PROVIDER_CONFIGURED = True
 except:
   pass
 
+
 class OpenAIProvider(BaseProvider):
   def __init__(self, **kwargs):
     super(OpenAIProvider, self).__init__(**kwargs)
     return
 
   @property
   def openai_client(self):
@@ -23,14 +24,15 @@
 
   def get_response(self):
     client = self.openai_client
     if isinstance(self.last_exception, openai.RateLimitError):
       sleep_before = 20.0
       print(f"Sleeping {sleep_before}s before making the LLM call")
       time.sleep(sleep_before)
+
     response = client.chat.completions.create(**self.cleaned_parameters)
     return response
 
   def get_generation_output(self, event) -> GenerationOutput:
     kwargs = {
       'finish_reason': None,
       'content': None,
@@ -50,9 +52,9 @@
     kwargs['function_call'] = crt_function_call
     return GenerationOutput(**kwargs)
 
   def get_timeout_params(self):
     return {
       'start': 5.0,
       'maximum': 20.0,
-      'increment': 5.0,
+      'increment': 10.0,
     }
```

### Comparing `airouter-0.1.8/airouter/providers/vertex_ai_text_provider.py` & `airouter-0.1.9/airouter/providers/vertex_ai_text_provider.py`

 * *Files identical despite different names*

### Comparing `airouter-0.1.8/airouter/streamed_completion.py` & `airouter-0.1.9/airouter/streamed_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import typing as t
 import uuid
 import time
-import json
+import httpx
 import concurrent.futures
 from tenacity import (
   after_log,
   retry,
   stop_after_attempt,
   wait_exponential,
 )
@@ -18,14 +18,15 @@
 import airouter
 from airouter.utils.interactive import enable_interactiveness
 from airouter.providers.factory import provider_factory
 
 SingleCreateOutput = t.Union[GenerationOutput, t.Tuple[t.Any, GenerationOutput]]
 MultipleCreateOutputs = t.List[SingleCreateOutput]
 
+
 class StreamedCompletion(object):
   def __init__(
       self,
       call_name: t.Optional[str] = None,
       completion_timeout: t.Optional[int] = None,
       request_timeout_start: t.Optional[float] = None,
       request_timeout_max: t.Optional[float] = None,
@@ -247,27 +248,26 @@
     request_timeout = self.compute_request_timeout(
       attempt_number=func.retry.statistics.get('attempt_number', 1),
       start=self.request_timeout_start or request_timeout_params.get('start'),
       maximum=self.request_timeout_max or request_timeout_params.get('maximum'),
       increment=self.request_timeout_increment or request_timeout_params.get('increment'),
     )
 
-    self.provider.timeout = request_timeout
+    self.provider.timeout = httpx.Timeout(request_timeout)
     self.provider.clean_parameters()
     self.provider.refresh_timings()
 
     try:
       gen_events = self.provider.get_stream()
       return gen_events
     except Exception as e:
       self.provider.last_exception = e
       airouter.logger.error(f"Exception of type '{type(e)}' for `get_stream`: {e}")
       raise e
 
-
   def _handle_stream_step(self, i, event, start):
     self.step_generation_output = self.provider.get_generation_output(event)
     elapsed = time.time() - start
     finished = self.step_generation_output.finish_reason is not None
     crt_content = self.step_generation_output.content
     crt_function_call = self.step_generation_output.function_call
 
@@ -312,26 +312,32 @@
   def _streamed_request_with_retry(self) -> t.Optional[GenerationOutput]:
     if self._should_stop_prematurely():
       return
 
     gen_events = self._provider_stream(func=self._streamed_request_with_retry)
     self.full_generation_output = GenerationOutput()
 
+    start = time.time()
+    last_event = time.time()
+
     try:
-      start = time.time()
       for i, event in gen_events:
+        last_event = time.time()
         r = self._handle_stream_step(i, event, start)
         if r == 'break':
           break
         elif r == 'return':
           return
       #endfor
     except Exception as e:
+      elapsed_from_last_event = time.time() - last_event
       self.provider.last_exception = e
-      airouter.logger.error(f"Exception of type '{type(e)}': {e}")
+      airouter.logger.error(
+        f"Exception of type '{type(e)}': {e}. Elapsed from last event: {elapsed_from_last_event:.2f}s"
+      )
       raise e
 
     if self.full_generation_output.content is not None:
       self.full_generation_output.content = self.full_generation_output.content.strip('\n')
 
     if self.on_stop_generation_callback is not None:
       self.on_stop_generation_callback(self)
```

### Comparing `airouter-0.1.8/airouter/utils/interactive.py` & `airouter-0.1.9/airouter/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `airouter-0.1.8/airouter/utils/tokens.py` & `airouter-0.1.9/airouter/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `airouter-0.1.8/PKG-INFO` & `airouter-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: airouter
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Laurentiu Piciu
 Author-email: laurentiupiciu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.28.82,<2.0.0)
 Requires-Dist: botocore (>=1.31.82,<2.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.36.1,<2.0.0)
+Requires-Dist: ollama (>=0.1.7,<0.2.0)
 Requires-Dist: openai (>=1.2.0,<2.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tenacity (>=8.0,<9.0)
 Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
 Requires-Dist: urwid (>=2.2.3,<3.0.0)
```

