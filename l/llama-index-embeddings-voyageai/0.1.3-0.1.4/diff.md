# Comparing `tmp/llama_index_embeddings_voyageai-0.1.3.tar.gz` & `tmp/llama_index_embeddings_voyageai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_voyageai-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_embeddings_voyageai-0.1.4.tar", max compression
```

## Comparing `llama_index_embeddings_voyageai-0.1.3.tar` & `llama_index_embeddings_voyageai-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       46 2024-03-08 15:46:46.692619 llama_index_embeddings_voyageai-0.1.3/README.md
--rw-r--r--   0        0        0       96 2024-03-08 15:46:46.692619 llama_index_embeddings_voyageai-0.1.3/llama_index/embeddings/voyageai/__init__.py
--rw-r--r--   0        0        0     4284 2024-03-08 15:46:46.692619 llama_index_embeddings_voyageai-0.1.3/llama_index/embeddings/voyageai/base.py
--rw-r--r--   0        0        0     1474 2024-03-08 15:46:46.692619 llama_index_embeddings_voyageai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 llama_index_embeddings_voyageai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-04-01 21:22:23.800398 llama_index_embeddings_voyageai-0.1.4/README.md
+-rw-r--r--   0        0        0       96 2024-04-01 21:22:23.800398 llama_index_embeddings_voyageai-0.1.4/llama_index/embeddings/voyageai/__init__.py
+-rw-r--r--   0        0        0     4314 2024-04-01 21:22:23.800398 llama_index_embeddings_voyageai-0.1.4/llama_index/embeddings/voyageai/base.py
+-rw-r--r--   0        0        0     1474 2024-04-01 21:22:23.800398 llama_index_embeddings_voyageai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 llama_index_embeddings_voyageai-0.1.4/PKG-INFO
```

### Comparing `llama_index_embeddings_voyageai-0.1.3/llama_index/embeddings/voyageai/base.py` & `llama_index_embeddings_voyageai-0.1.4/llama_index/embeddings/voyageai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Voyage embeddings file."""
 
 import logging
 from typing import Any, List, Optional
 
+from llama_index.core.bridge.pydantic import PrivateAttr
 from llama_index.core.base.embeddings.base import BaseEmbedding
 from llama_index.core.callbacks.base import CallbackManager
 
 import voyageai
-from pydantic import PrivateAttr
 
 logger = logging.getLogger(__name__)
 
 
 class VoyageEmbedding(BaseEmbedding):
     """Class for Voyage embeddings.
 
@@ -19,16 +19,16 @@
         model_name (str): Model for embedding.
             Defaults to "voyage-01".
 
         voyage_api_key (Optional[str]): Voyage API key. Defaults to None.
             You can either specify the key here or store it as an environment variable.
     """
 
-    client: voyageai.Client = PrivateAttr(None)
-    aclient: voyageai.client_async.AsyncClient = PrivateAttr()
+    _client: voyageai.Client = PrivateAttr(None)
+    _aclient: voyageai.client_async.AsyncClient = PrivateAttr()
     truncation: Optional[bool] = None
 
     def __init__(
         self,
         model_name: str,
         voyage_api_key: Optional[str] = None,
         embed_batch_size: Optional[int] = None,
@@ -49,34 +49,34 @@
         super().__init__(
             model_name=model_name,
             embed_batch_size=embed_batch_size,
             callback_manager=callback_manager,
             **kwargs,
         )
 
-        self.client = voyageai.Client(api_key=voyage_api_key)
-        self.aclient = voyageai.AsyncClient(api_key=voyage_api_key)
+        self._client = voyageai.Client(api_key=voyage_api_key)
+        self._aclient = voyageai.AsyncClient(api_key=voyage_api_key)
         self.truncation = truncation
 
     @classmethod
     def class_name(cls) -> str:
         return "VoyageEmbedding"
 
     def _get_embedding(self, texts: List[str], input_type: str) -> List[List[float]]:
-        return self.client.embed(
+        return self._client.embed(
             texts,
             model=self.model_name,
             input_type=input_type,
             truncation=self.truncation,
         ).embeddings
 
     async def _aget_embedding(
         self, texts: List[str], input_type: str
     ) -> List[List[float]]:
-        r = await self.aclient.embed(
+        r = await self._aclient.embed(
             texts,
             model=self.model_name,
             input_type=input_type,
             truncation=self.truncation,
         )
         return r.embeddings
```

### Comparing `llama_index_embeddings_voyageai-0.1.3/pyproject.toml` & `llama_index_embeddings_voyageai-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings voyageai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-voyageai"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 voyageai = "^0.1.6"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_embeddings_voyageai-0.1.3/PKG-INFO` & `llama_index_embeddings_voyageai-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-voyageai
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index embeddings voyageai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

