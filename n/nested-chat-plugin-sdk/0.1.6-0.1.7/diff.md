# Comparing `tmp/nested_chat_plugin_sdk-0.1.6.tar.gz` & `tmp/nested_chat_plugin_sdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_chat_plugin_sdk-0.1.6.tar", max compression
+gzip compressed data, was "nested_chat_plugin_sdk-0.1.7.tar", max compression
```

## Comparing `nested_chat_plugin_sdk-0.1.6.tar` & `nested_chat_plugin_sdk-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-02-02 06:09:26.194068 nested_chat_plugin_sdk-0.1.6/LICENSE
--rw-r--r--   0        0        0     1547 2024-02-02 16:33:45.142251 nested_chat_plugin_sdk-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-03-29 07:23:26.025683 nested_chat_plugin_sdk-0.1.6/nested_chat_plugin_sdk/__init__.py
--rw-r--r--   0        0        0      253 2024-03-29 07:23:26.025683 nested_chat_plugin_sdk-0.1.6/nested_chat_plugin_sdk/schemes.py
--rw-r--r--   0        0        0     2452 2024-03-29 09:52:17.665256 nested_chat_plugin_sdk-0.1.6/nested_chat_plugin_sdk/sdk.py
--rw-r--r--   0        0        0      355 2024-03-29 09:49:00.265266 nested_chat_plugin_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 nested_chat_plugin_sdk-0.1.6/setup.py
--rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 nested_chat_plugin_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-02 06:09:26.194068 nested_chat_plugin_sdk-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1547 2024-02-02 16:33:45.142251 nested_chat_plugin_sdk-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 07:23:26.025683 nested_chat_plugin_sdk-0.1.7/nested_chat_plugin_sdk/__init__.py
+-rw-r--r--   0        0        0      253 2024-03-29 07:23:26.025683 nested_chat_plugin_sdk-0.1.7/nested_chat_plugin_sdk/schemes.py
+-rw-r--r--   0        0        0     2664 2024-04-01 11:40:44.483138 nested_chat_plugin_sdk-0.1.7/nested_chat_plugin_sdk/sdk.py
+-rw-r--r--   0        0        0      355 2024-04-01 11:40:44.483138 nested_chat_plugin_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2313 1970-01-01 00:00:00.000000 nested_chat_plugin_sdk-0.1.7/setup.py
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 nested_chat_plugin_sdk-0.1.7/PKG-INFO
```

### Comparing `nested_chat_plugin_sdk-0.1.6/LICENSE` & `nested_chat_plugin_sdk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_chat_plugin_sdk-0.1.6/README.md` & `nested_chat_plugin_sdk-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nested_chat_plugin_sdk-0.1.6/nested_chat_plugin_sdk/sdk.py` & `nested_chat_plugin_sdk-0.1.7/nested_chat_plugin_sdk/sdk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from .schemes import SyncRequest
 from typing import Callable
-from fastapi import APIRouter, Request, HTTPException
+from fastapi import APIRouter, Request, HTTPException, status
 import aiohttp
 class PluginRouter(APIRouter):
     def __init__(self, api_url: str=None, plugin_name: str = None):
         super().__init__()
         self.plugin_name = plugin_name
         self.api_url = api_url
         self.create_handler = None
         self.update_handler = None
         self.delete_handler = None
         self.execute_handler = None
+        self.add_api_route("/health", self._health_check, methods=["GET"])
 
     def on_create(self, handler: Callable):
         self.create_handler = handler
         self.add_api_route("/sync", self._handle_create, methods=["POST"])
 
     def on_update(self, handler: Callable):
         self.update_handler = handler
@@ -33,14 +34,17 @@
             payload = {"name": self.plugin_name}
             try:
                 async with session.post(self.api_url, json=payload) as response:
                     return response.status
             except aiohttp.ClientError as e:
                 return 404
 
+    async def _health_check(self):
+        return HTTPException(status_code=status.HTTP_200_OK, detail={"status": "available"})
+
     async def _handle_create(self, request_data: SyncRequest):
         if not self.create_handler:
             raise HTTPException(status_code=404, detail="Create handler not found")
         return await self.create_handler(request_data)
 
     async def _handle_execute(self, request: Request):
         request_data = await request.json()
```

### Comparing `nested_chat_plugin_sdk-0.1.6/setup.py` & `nested_chat_plugin_sdk-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['aiohttp>=3.9.3,<4.0.0',
  'fastapi>=0.103.0,<0.104.0',
  'pydantic-settings>=2.0.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'nested-chat-plugin-sdk',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Test',
     'long_description': '\n\n# Plugin SDK for FastAPI\n\nThe Plugin SDK nested-chat-plugin-sdk is a FastAPI extension that provides a convenient way to handle requests for creating, updating, deleting, and executing operations.\n\n## Installation\n\nInstall dependencies using Poetry and activate the virtual environment. [Learn how to install Poetry](https://python-poetry.org/docs/)\n\n```bash\npoetry install\npoetry shell\n````\n\nInstall the SDK using [Poetry](https://python-poetry.org/):\n\n```bash\npoetry add nested-chat-plugin-sdk\n```\n\n## Example\n```python\nfrom fastapi import FastAPI, Request\nfrom nested_chat_plugin_sdk.sdk import PluginRouter, SyncRequest\n\napp = FastAPI()\nplugin_router = PluginRouter(api_url="")\n\n@plugin_router.on_create\nasync def handle_create(data: SyncRequest):\n    print("create", data)\n\n@plugin_router.on_update\nasync def handle_update(data: SyncRequest):\n    print("update", data)\n\n@plugin_router.on_delete\nasync def handle_delete(data: SyncRequest):\n    print("delete", data)\n\n@plugin_router.on_execute\nasync def handle_execute(request: Request):\n    print("execute", request)\n\napp.include_router(plugin_router)\n\n```\n\n## API Routes\n\n### `/sync`\n\n- `POST`: Create data\n- `PUT`: Update data\n- `DELETE`: Delete data\n\n### `/execute`\n\n- `POST`: Execute operation\n\n## SyncRequest Schema\n\n```python\nfrom nested_chat_plugin_sdk.schemes import SyncRequest\n\nclass SyncRequest(BaseModel):\n    project: dict[str, Any]\n    core: dict[str, Any]\n    variable: dict[str, Any]\n    variable_enum_item: dict[str, Any] = {}\n    variable_group: str | None = None\n\n\n```\n\n\n\n',
     'author': 'vladvavilov',
     'author_email': 'vladvav94@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nested_chat_plugin_sdk-0.1.6/PKG-INFO` & `nested_chat_plugin_sdk-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nested-chat-plugin-sdk
-Version: 0.1.6
+Version: 0.1.7
 Summary: Test
 Author: vladvavilov
 Author-email: vladvav94@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

