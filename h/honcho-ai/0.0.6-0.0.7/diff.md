# Comparing `tmp/honcho_ai-0.0.6.tar.gz` & `tmp/honcho_ai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honcho_ai-0.0.6.tar", max compression
+gzip compressed data, was "honcho_ai-0.0.7.tar", max compression
```

## Comparing `honcho_ai-0.0.6.tar` & `honcho_ai-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    34523 2024-02-29 09:17:36.878653 honcho_ai-0.0.6/LICENSE
--rw-r--r--   0        0        0     1357 2024-03-17 02:40:12.855561 honcho_ai-0.0.6/README.md
--rw-r--r--   0        0        0      549 2024-03-21 19:23:06.566512 honcho_ai-0.0.6/honcho/__init__.py
--rw-r--r--   0        0        0     1281 2024-03-21 19:23:06.566846 honcho_ai-0.0.6/honcho/cache.py
--rw-r--r--   0        0        0    50190 2024-03-21 19:23:06.568190 honcho_ai-0.0.6/honcho/client.py
--rw-r--r--   0        0        0       52 2024-03-21 19:23:06.568417 honcho_ai-0.0.6/honcho/ext/__init__.py
--rw-r--r--   0        0        0     2303 2024-03-21 19:23:06.568817 honcho_ai-0.0.6/honcho/ext/langchain.py
--rw-r--r--   0        0        0     2190 2024-03-21 19:23:06.569101 honcho_ai-0.0.6/honcho/schemas.py
--rw-r--r--   0        0        0    49170 2024-03-21 19:23:06.569468 honcho_ai-0.0.6/honcho/sync_client.py
--rw-r--r--   0        0        0      960 2024-03-21 19:23:06.570490 honcho_ai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1908 1970-01-01 00:00:00.000000 honcho_ai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-29 09:17:36.878653 honcho_ai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1357 2024-03-17 02:40:12.855561 honcho_ai-0.0.7/README.md
+-rw-r--r--   0        0        0      549 2024-03-21 19:23:06.566512 honcho_ai-0.0.7/honcho/__init__.py
+-rw-r--r--   0        0        0     1281 2024-03-21 19:23:06.566846 honcho_ai-0.0.7/honcho/cache.py
+-rw-r--r--   0        0        0    50750 2024-04-01 17:58:55.192634 honcho_ai-0.0.7/honcho/client.py
+-rw-r--r--   0        0        0       52 2024-03-21 19:23:06.568417 honcho_ai-0.0.7/honcho/ext/__init__.py
+-rw-r--r--   0        0        0     2304 2024-04-01 17:58:55.192828 honcho_ai-0.0.7/honcho/ext/langchain.py
+-rw-r--r--   0        0        0     2190 2024-04-01 05:16:27.970972 honcho_ai-0.0.7/honcho/schemas.py
+-rw-r--r--   0        0        0    49718 2024-04-01 17:58:55.193225 honcho_ai-0.0.7/honcho/sync_client.py
+-rw-r--r--   0        0        0      985 2024-04-01 17:58:55.194216 honcho_ai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 honcho_ai-0.0.7/PKG-INFO
```

### Comparing `honcho_ai-0.0.6/LICENSE` & `honcho_ai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.6/README.md` & `honcho_ai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.6/honcho/__init__.py` & `honcho_ai-0.0.7/honcho/__init__.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.6/honcho/cache.py` & `honcho_ai-0.0.7/honcho/cache.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.6/honcho/client.py` & `honcho_ai-0.0.7/honcho/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 This module provides asynchronous client functionality for interacting with the Honcho API.
 """
 
 from __future__ import annotations
 
 import datetime
 import json
+import os
 import uuid
 from typing import Optional
 
 import httpx
+from dotenv import load_dotenv
 
 from .schemas import Document, Message, Metamessage
 
 
 class AsyncGetPage:
     """Base class for receiving Paginated API results"""
 
@@ -341,37 +343,55 @@
             reverse=self.reverse,
         )
 
 
 class AsyncHoncho:
     """Honcho API Client Object"""
 
-    def __init__(self, app_name: str, base_url: str = "https://demo.honcho.dev"):
+    def __init__(
+        self,
+        app_name: str,
+        base_url: str = "https://demo.honcho.dev",
+        api_key: str = "default",
+    ):
         """Constructor for Client
 
         Args:
             app_name (str): Name of the application
             base_url (str): Base URL for the instance of the Honcho API defaults to
             https://demo.honcho.dev
         """
+        load_dotenv()
+        token = os.getenv("HONCHO_API_KEY", api_key)
         self.server_url: str = base_url  # Base URL for the instance of the Honcho API
-        self.client: httpx.AsyncClient = httpx.AsyncClient()
+        self.client: httpx.AsyncClient = httpx.AsyncClient(
+            headers={"Authorization": f"Bearer {token}"}
+        )
         self.app_name: str = app_name  # Representing name of the client application
         self.app_id: uuid.UUID
         self.metadata: dict
 
     async def initialize(self):
         """Run initialization tasks for the Honcho client"""
-        res = await self.client.get(
-            f"{self.server_url}/apps/get_or_create/{self.app_name}"
-        )
-        res.raise_for_status()
-        data = res.json()
-        self.app_id: uuid.UUID = data["id"]
-        self.metadata: dict = data["metadata"]
+        try:
+            res = await self.client.get(
+                f"{self.server_url}/apps/get_or_create/{self.app_name}"
+            )
+            res.raise_for_status()
+            data = res.json()
+            self.app_id: uuid.UUID = data["id"]
+            self.metadata: dict = data["metadata"]
+        except httpx.HTTPStatusError as e:
+            error_content = e.response.content
+            print(error_content)
+            raise Exception(error_content) from None
+
+    async def init(self):
+        """Synonym for initialize"""
+        await self.initialize()
 
     async def init(self):
         """Synonym for initialize"""
         await self.initialize()
 
     @property
     def base_url(self):
```

### Comparing `honcho_ai-0.0.6/honcho/ext/langchain.py` & `honcho_ai-0.0.7/honcho/ext/langchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 import importlib
 from typing import List, Union
 
 from honcho import AsyncSession, Session
 from honcho.schemas import Message
 
 
-def requires_langchain(func):
+def _requires_langchain(func):
     """A utility to check if langchain is installed before running a function"""
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         """Check if langchain is installed before running a function"""
 
         if importlib.util.find_spec("langchain") is None:  # type: ignore
             raise ImportError("Langchain must be installed to use this feature")
             # raise RuntimeError("langchain is not installed")
         return func(*args, **kwargs)
 
     return wrapper
 
 
-@requires_langchain
-def _messages_to_langchain(messages: List[Message]):
+@_requires_langchain
+def messages_to_langchain(messages: List[Message]):
     """Converts Honcho messages to Langchain messages
 
     Args:
         messages (List[Message]): The list of messages to convert
 
     Returns:
         List: The list of converted LangChain messages
@@ -43,16 +43,16 @@
         if message.is_user:
             new_messages.append(HumanMessage(content=message.content))
         else:
             new_messages.append(AIMessage(content=message.content))
     return new_messages
 
 
-@requires_langchain
-def _langchain_to_messages(
+@_requires_langchain
+def langchain_to_messages(
     messages, session: Union[Session, AsyncSession]
 ) -> List[Message]:
     """Converts Langchain messages to Honcho messages and adds to appropriate session
 
     Args:
         messages: The LangChain messages to convert
         session: The session to add the messages to
```

### Comparing `honcho_ai-0.0.6/honcho/schemas.py` & `honcho_ai-0.0.7/honcho/schemas.py`

 * *Files identical despite different names*

### Comparing `honcho_ai-0.0.6/honcho/sync_client.py` & `honcho_ai-0.0.7/honcho/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 This module provides synchronous client functionality for interacting with the Honcho API.
 """
 
 from __future__ import annotations
 
 import datetime
 import json
+import os
 import uuid
 from typing import Optional
 
 import httpx
+from dotenv import load_dotenv
 
 from .schemas import Document, Message, Metamessage
 
 
 class GetPage:
     """Base class for receiving Paginated API results"""
 
@@ -341,37 +343,55 @@
             reverse=self.reverse,
         )
 
 
 class Honcho:
     """Honcho API Client Object"""
 
-    def __init__(self, app_name: str, base_url: str = "https://demo.honcho.dev"):
+    def __init__(
+        self,
+        app_name: str,
+        base_url: str = "https://demo.honcho.dev",
+        api_key: str = "default",
+    ):
         """Constructor for Client
 
         Args:
             app_name (str): Name of the application
             base_url (str): Base URL for the instance of the Honcho API defaults to
             https://demo.honcho.dev
         """
+        load_dotenv()
+        token = os.getenv("HONCHO_API_KEY", api_key)
         self.server_url: str = base_url  # Base URL for the instance of the Honcho API
-        self.client: httpx.Client = httpx.Client()
+        self.client: httpx.Client = httpx.Client(
+            headers={"Authorization": f"Bearer {token}"}
+        )
         self.app_name: str = app_name  # Representing name of the client application
         self.app_id: uuid.UUID
         self.metadata: dict
 
     def initialize(self):
         """Run initialization tasks for the Honcho client"""
-        res = self.client.get(
-            f"{self.server_url}/apps/get_or_create/{self.app_name}"
-        )
-        res.raise_for_status()
-        data = res.json()
-        self.app_id: uuid.UUID = data["id"]
-        self.metadata: dict = data["metadata"]
+        try:
+            res = self.client.get(
+                f"{self.server_url}/apps/get_or_create/{self.app_name}"
+            )
+            res.raise_for_status()
+            data = res.json()
+            self.app_id: uuid.UUID = data["id"]
+            self.metadata: dict = data["metadata"]
+        except httpx.HTTPStatusError as e:
+            error_content = e.response.content
+            print(error_content)
+            raise Exception(error_content) from None
+
+    def init(self):
+        """Synonym for initialize"""
+        self.initialize()
 
     def init(self):
         """Synonym for initialize"""
         self.initialize()
 
     @property
     def base_url(self):
```

### Comparing `honcho_ai-0.0.6/pyproject.toml` & `honcho_ai-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "honcho-ai"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python Client SDK for Honcho"
 authors = ["Plastic Labs <hello@plasticlabs.ai>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [{include = "honcho"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.26.0"
+python-dotenv = "^1.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 pytest-asyncio = "^0.23.4"
 coverage = "^7.4.3"
 interrogate = "^1.5.0"
```

### Comparing `honcho_ai-0.0.6/PKG-INFO` & `honcho_ai-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: honcho-ai
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Client SDK for Honcho
 License: AGPL-3.0
 Author: Plastic Labs
 Author-email: hello@plasticlabs.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Honcho
 
 A User context management solution for building AI Agents and LLM powered
 applications.
```

