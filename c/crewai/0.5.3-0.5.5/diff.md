# Comparing `tmp/crewai-0.5.3.tar.gz` & `tmp/crewai-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai-0.5.3.tar", max compression
+gzip compressed data, was "crewai-0.5.5.tar", max compression
```

## Comparing `crewai-0.5.3.tar` & `crewai-0.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1073 2023-12-12 12:58:25.739514 crewai-0.5.3/LICENSE
--rw-r--r--   0        0        0     9674 2024-02-06 06:18:10.484239 crewai-0.5.3/README.md
--rw-r--r--   0        0        0     1337 2024-02-07 10:14:12.718536 crewai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      124 2024-01-13 14:30:53.605513 crewai-0.5.3/src/crewai/__init__.py
--rw-r--r--   0        0        0     8398 2024-02-03 07:15:44.228049 crewai-0.5.3/src/crewai/agent.py
--rw-r--r--   0        0        0      175 2024-01-13 14:30:53.606183 crewai-0.5.3/src/crewai/agents/__init__.py
--rw-r--r--   0        0        0       72 2024-01-13 14:30:53.606325 crewai-0.5.3/src/crewai/agents/cache/__init__.py
--rw-r--r--   0        0        0      416 2024-01-31 01:45:11.510318 crewai-0.5.3/src/crewai/agents/cache/cache_handler.py
--rw-r--r--   0        0        0      493 2024-01-13 14:30:53.606590 crewai-0.5.3/src/crewai/agents/cache/cache_hit.py
--rw-r--r--   0        0        0      841 2024-01-14 14:25:00.216180 crewai-0.5.3/src/crewai/agents/exceptions.py
--rw-r--r--   0        0        0     9296 2024-02-06 07:13:10.299937 crewai-0.5.3/src/crewai/agents/executor.py
--rw-r--r--   0        0        0     2574 2024-01-31 01:45:11.512024 crewai-0.5.3/src/crewai/agents/output_parser.py
--rw-r--r--   0        0        0     1446 2024-01-31 01:45:11.512447 crewai-0.5.3/src/crewai/agents/tools_handler.py
--rw-r--r--   0        0        0     8237 2024-02-07 10:14:03.707915 crewai-0.5.3/src/crewai/crew.py
--rw-r--r--   0        0        0      249 2024-02-03 07:15:44.229207 crewai-0.5.3/src/crewai/process.py
--rw-r--r--   0        0        0     4313 2024-02-04 19:47:43.286485 crewai-0.5.3/src/crewai/task.py
--rw-r--r--   0        0        0        0 2024-01-13 14:30:53.609554 crewai-0.5.3/src/crewai/tasks/__init__.py
--rw-r--r--   0        0        0      563 2024-01-13 14:30:53.609727 crewai-0.5.3/src/crewai/tasks/task_output.py
--rw-r--r--   0        0        0       32 2024-02-06 06:27:53.474788 crewai-0.5.3/src/crewai/telemtry/__init__.py
--rw-r--r--   0        0        0     3591 2024-02-07 10:00:56.505122 crewai-0.5.3/src/crewai/telemtry/telemetry.py
--rw-r--r--   0        0        0        0 2024-01-13 14:30:53.609768 crewai-0.5.3/src/crewai/tools/__init__.py
--rw-r--r--   0        0        0     2106 2024-02-03 07:15:44.229955 crewai-0.5.3/src/crewai/tools/agent_tools.py
--rw-r--r--   0        0        0      837 2024-01-13 14:30:53.610391 crewai-0.5.3/src/crewai/tools/cache_tools.py
--rw-r--r--   0        0        0     5908 2024-02-06 07:13:34.440101 crewai-0.5.3/src/crewai/translations/el.json
--rw-r--r--   0        0        0     3077 2024-02-06 07:13:10.300124 crewai-0.5.3/src/crewai/translations/en.json
--rw-r--r--   0        0        0      121 2024-01-14 14:25:00.218611 crewai-0.5.3/src/crewai/utilities/__init__.py
--rw-r--r--   0        0        0     1647 2024-01-31 01:45:11.513099 crewai-0.5.3/src/crewai/utilities/i18n.py
--rw-r--r--   0        0        0      432 2024-02-03 07:45:53.379637 crewai-0.5.3/src/crewai/utilities/logger.py
--rw-r--r--   0        0        0     1342 2024-01-31 01:45:11.513234 crewai-0.5.3/src/crewai/utilities/prompts.py
--rw-r--r--   0        0        0     1672 2024-02-06 07:13:48.237133 crewai-0.5.3/src/crewai/utilities/rpm_controller.py
--rw-r--r--   0        0        0    10593 1970-01-01 00:00:00.000000 crewai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-12-12 12:58:25.739514 crewai-0.5.5/LICENSE
+-rw-r--r--   0        0        0    10501 2024-02-08 06:11:52.507118 crewai-0.5.5/README.md
+-rw-r--r--   0        0        0     1447 2024-02-08 07:13:23.241225 crewai-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-01-13 14:30:53.605513 crewai-0.5.5/src/crewai/__init__.py
+-rw-r--r--   0        0        0     8398 2024-02-08 06:37:35.154223 crewai-0.5.5/src/crewai/agent.py
+-rw-r--r--   0        0        0      175 2024-01-13 14:30:53.606183 crewai-0.5.5/src/crewai/agents/__init__.py
+-rw-r--r--   0        0        0       72 2024-01-13 14:30:53.606325 crewai-0.5.5/src/crewai/agents/cache/__init__.py
+-rw-r--r--   0        0        0      416 2024-01-31 01:45:11.510318 crewai-0.5.5/src/crewai/agents/cache/cache_handler.py
+-rw-r--r--   0        0        0      493 2024-01-13 14:30:53.606590 crewai-0.5.5/src/crewai/agents/cache/cache_hit.py
+-rw-r--r--   0        0        0      841 2024-01-14 14:25:00.216180 crewai-0.5.5/src/crewai/agents/exceptions.py
+-rw-r--r--   0        0        0     9296 2024-02-06 07:13:10.299937 crewai-0.5.5/src/crewai/agents/executor.py
+-rw-r--r--   0        0        0     2574 2024-01-31 01:45:11.512024 crewai-0.5.5/src/crewai/agents/output_parser.py
+-rw-r--r--   0        0        0     1446 2024-01-31 01:45:11.512447 crewai-0.5.5/src/crewai/agents/tools_handler.py
+-rw-r--r--   0        0        0     8394 2024-02-08 07:09:16.869298 crewai-0.5.5/src/crewai/crew.py
+-rw-r--r--   0        0        0      249 2024-02-03 07:15:44.229207 crewai-0.5.5/src/crewai/process.py
+-rw-r--r--   0        0        0     4313 2024-02-04 19:47:43.286485 crewai-0.5.5/src/crewai/task.py
+-rw-r--r--   0        0        0        0 2024-01-13 14:30:53.609554 crewai-0.5.5/src/crewai/tasks/__init__.py
+-rw-r--r--   0        0        0      563 2024-01-13 14:30:53.609727 crewai-0.5.5/src/crewai/tasks/task_output.py
+-rw-r--r--   0        0        0       33 2024-02-08 06:21:06.708824 crewai-0.5.5/src/crewai/telemtry/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-08 06:21:06.982133 crewai-0.5.5/src/crewai/telemtry/telemetry.py
+-rw-r--r--   0        0        0        0 2024-01-13 14:30:53.609768 crewai-0.5.5/src/crewai/tools/__init__.py
+-rw-r--r--   0        0        0     2106 2024-02-03 07:15:44.229955 crewai-0.5.5/src/crewai/tools/agent_tools.py
+-rw-r--r--   0        0        0      837 2024-01-13 14:30:53.610391 crewai-0.5.5/src/crewai/tools/cache_tools.py
+-rw-r--r--   0        0        0     5908 2024-02-06 07:13:34.440101 crewai-0.5.5/src/crewai/translations/el.json
+-rw-r--r--   0        0        0     3077 2024-02-06 07:13:10.300124 crewai-0.5.5/src/crewai/translations/en.json
+-rw-r--r--   0        0        0      121 2024-01-14 14:25:00.218611 crewai-0.5.5/src/crewai/utilities/__init__.py
+-rw-r--r--   0        0        0     1647 2024-01-31 01:45:11.513099 crewai-0.5.5/src/crewai/utilities/i18n.py
+-rw-r--r--   0        0        0      432 2024-02-03 07:45:53.379637 crewai-0.5.5/src/crewai/utilities/logger.py
+-rw-r--r--   0        0        0     1342 2024-01-31 01:45:11.513234 crewai-0.5.5/src/crewai/utilities/prompts.py
+-rw-r--r--   0        0        0     1786 2024-02-08 07:09:30.782347 crewai-0.5.5/src/crewai/utilities/rpm_controller.py
+-rw-r--r--   0        0        0    11594 1970-01-01 00:00:00.000000 crewai-0.5.5/PKG-INFO
```

### Comparing `crewai-0.5.3/LICENSE` & `crewai-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/README.md` & `crewai-0.5.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
   - [Quick Tutorial](#quick-tutorial)
   - [Trip Planner](#trip-planner)
   - [Stock Analysis](#stock-analysis)
 - [Connecting Your Crew to a Model](#connecting-your-crew-to-a-model)
 - [How CrewAI Compares](#how-crewai-compares)
 - [Contribution](#contribution)
 - [Hire CrewAI](#hire-crewai)
+- [Telemetry](#telemetry)
 - [License](#license)
 
 ## Why CrewAI?
 
 The power of AI collaboration has too much to offer.
 CrewAI is designed to enable AI agents to assume roles, share goals, and operate in a cohesive unit - much like a well-oiled crew. Whether you're building a smart assistant platform, an automated customer service ensemble, or a multi-agent research team, CrewAI provides the backbone for sophisticated multi-agent interactions.
 
@@ -239,10 +240,28 @@
 ```
 
 ## Hire CrewAI
 
 We're a company developing crewAI and crewAI Enterprise, we for a limited time are offer consulting with selected customers, to get them early access to our enterprise solution
 If you are interested on having access to it and hiring weekly hours with our team, feel free to email us at [joao@crewai.com](mailto:joao@crewai.com).
 
+## Telemetry
+
+CrewAI uses anonymous telemetry to collect usage data with the main purpose of helping us improve the library by focusing our efforts on the most used features, integrations and tools.
+
+There is NO data being collected on the prompts, tasks descriptions agents backstories or goals nor tools usage, no API calls, nor responses nor any data that is being processed by the agents, nor any secrets and env vars.
+
+Data collected includes:
+- Version of crewAI
+- Version of Python
+- General OS (e.g. number of CPUs, macOS/Windows/Linux)
+- Number of agents and tasks in a crew
+- Crew Process being used
+- If Agents are using memory or allowing delegation
+- If Tasks are being executed in parallel or sequentially
+- Language model being used
+- Roles of agents in a crew
+- Tools names available
+
 ## License
 
 CrewAI is released under the MIT License.
```

### Comparing `crewai-0.5.3/pyproject.toml` & `crewai-0.5.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "crewai"
-version = "0.5.3"
+version = "0.5.5"
 description = "Cutting-edge framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks."
 authors = ["Joao Moura <joao@crewai.com>"]
 readme = "README.md"
 packages = [
     { include = "crewai", from = "src" },
 ]
 
@@ -17,14 +17,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 pydantic = "^2.4.2"
 langchain = "0.1.0"
 openai = "^1.7.1"
 langchain-openai = "^0.0.2"
+opentelemetry-api = "^1.22.0"
+opentelemetry-sdk = "^1.22.0"
+opentelemetry-exporter-otlp-proto-http = "^1.22.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.13.2"
 pyright = "1.1.333"
 black = {git = "https://github.com/psf/black.git", rev = "stable"}
 autoflake = "^2.2.1"
 pre-commit = "^3.6.0"
@@ -36,15 +39,14 @@
 pillow = "^10.2.0"
 cairosvg = "^2.7.1"
 
 [tool.isort]
 profile = "black"
 known_first_party = ["crewai"]
 
-
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4"
 pytest-vcr = "^1.0.2"
 python-dotenv = "1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `crewai-0.5.3/src/crewai/agent.py` & `crewai-0.5.5/src/crewai/agent.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/agents/exceptions.py` & `crewai-0.5.5/src/crewai/agents/exceptions.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/agents/executor.py` & `crewai-0.5.5/src/crewai/agents/executor.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/agents/output_parser.py` & `crewai-0.5.5/src/crewai/agents/output_parser.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/agents/tools_handler.py` & `crewai-0.5.5/src/crewai/agents/tools_handler.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/crew.py` & `crewai-0.5.5/src/crewai/crew.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 from pydantic_core import PydanticCustomError
 
 from crewai.agent import Agent
 from crewai.agents.cache import CacheHandler
 from crewai.process import Process
 from crewai.task import Task
+from crewai.telemtry import Telemetry
 from crewai.tools.agent_tools import AgentTools
 from crewai.utilities import I18N, Logger, RPMController
 
 
 class Crew(BaseModel):
     """
     Represents a group of agents, defining how they should collaborate and the tasks they should perform.
@@ -88,14 +89,16 @@
 
     @model_validator(mode="after")
     def set_private_attrs(self) -> "Crew":
         """Set private attributes."""
         self._cache_handler = CacheHandler()
         self._logger = Logger(self.verbose)
         self._rpm_controller = RPMController(max_rpm=self.max_rpm, logger=self._logger)
+        self._telemetry = Telemetry()
+        self._telemetry.crew_creation(self)
         return self
 
     @model_validator(mode="after")
     def check_manager_llm(self):
         """Validates that the language model is set when using hierarchical process."""
         if self.process == Process.hierarchical and not self.manager_llm:
             raise PydanticCustomError(
@@ -117,15 +120,16 @@
 
         if self.config:
             self._setup_from_config()
 
         if self.agents:
             for agent in self.agents:
                 agent.set_cache_handler(self._cache_handler)
-                agent.set_rpm_controller(self._rpm_controller)
+                if self.max_rpm:
+                    agent.set_rpm_controller(self._rpm_controller)
         return self
 
     def _setup_from_config(self):
         assert self.config is not None, "Config should not be None."
 
         """Initializes agents and tasks from the provided config."""
         if not self.config.get("agents") or not self.config.get("tasks"):
```

### Comparing `crewai-0.5.3/src/crewai/task.py` & `crewai-0.5.5/src/crewai/task.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/tasks/task_output.py` & `crewai-0.5.5/src/crewai/tasks/task_output.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/tools/agent_tools.py` & `crewai-0.5.5/src/crewai/tools/agent_tools.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/tools/cache_tools.py` & `crewai-0.5.5/src/crewai/tools/cache_tools.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/translations/el.json` & `crewai-0.5.5/src/crewai/translations/el.json`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/translations/en.json` & `crewai-0.5.5/src/crewai/translations/en.json`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/utilities/i18n.py` & `crewai-0.5.5/src/crewai/utilities/i18n.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/utilities/prompts.py` & `crewai-0.5.5/src/crewai/utilities/prompts.py`

 * *Files identical despite different names*

### Comparing `crewai-0.5.3/src/crewai/utilities/rpm_controller.py` & `crewai-0.5.5/src/crewai/utilities/rpm_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 class RPMController(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     max_rpm: Union[int, None] = Field(default=None)
     logger: Logger = Field(default=None)
     _current_rpm: int = PrivateAttr(default=0)
     _timer: threading.Timer | None = PrivateAttr(default=None)
     _lock: threading.Lock = PrivateAttr(default=None)
+    _shutdown_flag = False
 
     @model_validator(mode="after")
     def reset_counter(self):
         if self.max_rpm:
-            self._lock = threading.Lock()
-            self._reset_request_count()
+            if not self._shutdown_flag:
+                self._lock = threading.Lock()
+                self._reset_request_count()
         return self
 
     def check_or_wait(self):
         if not self.max_rpm:
             return True
 
         with self._lock:
@@ -47,10 +49,11 @@
         time.sleep(60)
         self._current_rpm = 0
 
     def _reset_request_count(self):
         with self._lock:
             self._current_rpm = 0
         if self._timer:
+            self._shutdown_flag = True
             self._timer.cancel()
         self._timer = threading.Timer(60.0, self._reset_request_count)
         self._timer.start()
```

### Comparing `crewai-0.5.3/PKG-INFO` & `crewai-0.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: crewai
-Version: 0.5.3
+Version: 0.5.5
 Summary: Cutting-edge framework for orchestrating role-playing, autonomous AI agents. By fostering collaborative intelligence, CrewAI empowers agents to work together seamlessly, tackling complex tasks.
 Author: Joao Moura
 Author-email: joao@crewai.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain (==0.1.0)
 Requires-Dist: langchain-openai (>=0.0.2,<0.0.3)
 Requires-Dist: openai (>=1.7.1,<2.0.0)
+Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.22.0,<2.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.22.0,<2.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Project-URL: Documentation, https://github.com/joaomdmoura/CrewAI/wiki/Index
 Project-URL: Homepage, https://crewai.io
 Project-URL: Repository, https://github.com/joaomdmoura/crewai
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -46,14 +49,15 @@
   - [Quick Tutorial](#quick-tutorial)
   - [Trip Planner](#trip-planner)
   - [Stock Analysis](#stock-analysis)
 - [Connecting Your Crew to a Model](#connecting-your-crew-to-a-model)
 - [How CrewAI Compares](#how-crewai-compares)
 - [Contribution](#contribution)
 - [Hire CrewAI](#hire-crewai)
+- [Telemetry](#telemetry)
 - [License](#license)
 
 ## Why CrewAI?
 
 The power of AI collaboration has too much to offer.
 CrewAI is designed to enable AI agents to assume roles, share goals, and operate in a cohesive unit - much like a well-oiled crew. Whether you're building a smart assistant platform, an automated customer service ensemble, or a multi-agent research team, CrewAI provides the backbone for sophisticated multi-agent interactions.
 
@@ -259,11 +263,29 @@
 ```
 
 ## Hire CrewAI
 
 We're a company developing crewAI and crewAI Enterprise, we for a limited time are offer consulting with selected customers, to get them early access to our enterprise solution
 If you are interested on having access to it and hiring weekly hours with our team, feel free to email us at [joao@crewai.com](mailto:joao@crewai.com).
 
+## Telemetry
+
+CrewAI uses anonymous telemetry to collect usage data with the main purpose of helping us improve the library by focusing our efforts on the most used features, integrations and tools.
+
+There is NO data being collected on the prompts, tasks descriptions agents backstories or goals nor tools usage, no API calls, nor responses nor any data that is being processed by the agents, nor any secrets and env vars.
+
+Data collected includes:
+- Version of crewAI
+- Version of Python
+- General OS (e.g. number of CPUs, macOS/Windows/Linux)
+- Number of agents and tasks in a crew
+- Crew Process being used
+- If Agents are using memory or allowing delegation
+- If Tasks are being executed in parallel or sequentially
+- Language model being used
+- Roles of agents in a crew
+- Tools names available
+
 ## License
 
 CrewAI is released under the MIT License.
```

