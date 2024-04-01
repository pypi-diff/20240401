# Comparing `tmp/llama_index_vector_stores_kdbai-0.1.3.tar.gz` & `tmp/llama_index_vector_stores_kdbai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_kdbai-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_kdbai-0.1.4.tar", max compression
```

## Comparing `llama_index_vector_stores_kdbai-0.1.3.tar` & `llama_index_vector_stores_kdbai-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-03-21 21:07:29.350048 llama_index_vector_stores_kdbai-0.1.3/README.md
--rw-r--r--   0        0        0       99 2024-03-21 21:07:29.350048 llama_index_vector_stores_kdbai-0.1.3/llama_index/vector_stores/kdbai/__init__.py
--rw-r--r--   0        0        0     6875 2024-03-21 21:07:29.350048 llama_index_vector_stores_kdbai-0.1.3/llama_index/vector_stores/kdbai/base.py
--rw-r--r--   0        0        0      735 2024-03-21 21:07:29.350048 llama_index_vector_stores_kdbai-0.1.3/llama_index/vector_stores/kdbai/utils.py
--rw-r--r--   0        0        0     1700 2024-03-21 21:07:29.350048 llama_index_vector_stores_kdbai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_kdbai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-03-29 16:56:50.151683 llama_index_vector_stores_kdbai-0.1.4/README.md
+-rw-r--r--   0        0        0       99 2024-03-29 16:56:50.152008 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/__init__.py
+-rw-r--r--   0        0        0     6875 2024-03-31 21:32:29.669989 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/base.py
+-rw-r--r--   0        0        0      735 2024-03-29 16:56:50.152279 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/utils.py
+-rw-r--r--   0        0        0     1700 2024-04-01 15:49:44.031952 llama_index_vector_stores_kdbai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_kdbai-0.1.4/PKG-INFO
```

### Comparing `llama_index_vector_stores_kdbai-0.1.3/llama_index/vector_stores/kdbai/base.py` & `llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from llama_index.core.bridge.pydantic import PrivateAttr
 from llama_index.core.schema import BaseNode, TextNode
 from llama_index.core.vector_stores.types import (
     BasePydanticVectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
-from llama_index.vector_stores.kbdai.utils import default_sparse_encoder
+from llama_index.vector_stores.kdbai.utils import default_sparse_encoder
 
 DEFAULT_COLUMN_NAMES = ["document_id", "text", "embedding"]
 
 DEFAULT_BATCH_SIZE = 100
 
 
 # INITIALISE LOGGER AND SET FORMAT
```

### Comparing `llama_index_vector_stores_kdbai-0.1.3/llama_index/vector_stores/kdbai/utils.py` & `llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_kdbai-0.1.3/pyproject.toml` & `llama_index_vector_stores_kdbai-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores kdbai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-kdbai"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 pykx = "^2.1.1"
 kdbai-client = "^0.1.2"
```

### Comparing `llama_index_vector_stores_kdbai-0.1.3/PKG-INFO` & `llama_index_vector_stores_kdbai-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-kdbai
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index vector_stores kdbai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

