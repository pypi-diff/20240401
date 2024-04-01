# Comparing `tmp/fastembed-0.2.5.tar.gz` & `tmp/fastembed-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastembed-0.2.5.tar", max compression
+gzip compressed data, was "fastembed-0.2.6.tar", max compression
```

## Comparing `fastembed-0.2.5.tar` & `fastembed-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-03-20 13:42:31.912760 fastembed-0.2.5/LICENSE
--rw-r--r--   0        0        0     3614 2024-03-20 13:42:31.912760 fastembed-0.2.5/README.md
--rw-r--r--   0        0        0      166 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/common/__init__.py
--rw-r--r--   0        0        0     8190 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/common/model_management.py
--rw-r--r--   0        0        0     2016 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/common/models.py
--rw-r--r--   0        0        0     4619 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/common/onnx_model.py
--rw-r--r--   0        0        0      890 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/common/utils.py
--rw-r--r--   0        0        0      620 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/embedding.py
--rw-r--r--   0        0        0        0 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/image/__init__.py
--rw-r--r--   0        0        0     7525 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/parallel_processor.py
--rw-r--r--   0        0        0        0 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/sparse/__init__.py
--rw-r--r--   0        0        0     1015 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/sparse/sparse_embedding_base.py
--rw-r--r--   0        0        0     3063 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/sparse/sparse_text_embedding.py
--rw-r--r--   0        0        0     4188 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/sparse/splade_pp.py
--rw-r--r--   0        0        0        0 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/__init__.py
--rw-r--r--   0        0        0     1923 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/e5_onnx_embedding.py
--rw-r--r--   0        0        0     2177 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/jina_onnx_embedding.py
--rw-r--r--   0        0        0     8365 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/onnx_embedding.py
--rw-r--r--   0        0        0     3399 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/text_embedding.py
--rw-r--r--   0        0        0     1772 2024-03-20 13:42:31.916761 fastembed-0.2.5/fastembed/text/text_embedding_base.py
--rw-r--r--   0        0        0     1181 2024-03-20 13:42:31.916761 fastembed-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4822 1970-01-01 00:00:00.000000 fastembed-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 15:24:42.768703 fastembed-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3591 2024-04-01 15:24:42.768703 fastembed-0.2.6/README.md
+-rw-r--r--   0        0        0      259 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/__init__.py
+-rw-r--r--   0        0        0     8338 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/model_management.py
+-rw-r--r--   0        0        0     2030 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/models.py
+-rw-r--r--   0        0        0     4701 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/onnx_model.py
+-rw-r--r--   0        0        0      890 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/common/utils.py
+-rw-r--r--   0        0        0      604 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/embedding.py
+-rw-r--r--   0        0        0        0 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/image/__init__.py
+-rw-r--r--   0        0        0     7539 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/parallel_processor.py
+-rw-r--r--   0        0        0      192 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/__init__.py
+-rw-r--r--   0        0        0     1062 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/sparse_embedding_base.py
+-rw-r--r--   0        0        0     3063 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/sparse_text_embedding.py
+-rw-r--r--   0        0        0     4669 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/sparse/splade_pp.py
+-rw-r--r--   0        0        0       85 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/__init__.py
+-rw-r--r--   0        0        0     1923 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/e5_onnx_embedding.py
+-rw-r--r--   0        0        0     2191 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/jina_onnx_embedding.py
+-rw-r--r--   0        0        0     8286 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/onnx_embedding.py
+-rw-r--r--   0        0        0     3399 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/text_embedding.py
+-rw-r--r--   0        0        0     1819 2024-04-01 15:24:42.772703 fastembed-0.2.6/fastembed/text/text_embedding_base.py
+-rw-r--r--   0        0        0     1180 2024-04-01 15:24:42.776703 fastembed-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 fastembed-0.2.6/PKG-INFO
```

### Comparing `fastembed-0.2.5/LICENSE` & `fastembed-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.5/README.md` & `fastembed-0.2.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ⚡️ What is FastEmbed?
 
 FastEmbed is a lightweight, fast, Python library built for embedding generation. We [support popular text models](https://qdrant.github.io/fastembed/examples/Supported_Models/). Please [open a GitHub issue](https://github.com/qdrant/fastembed/issues/new) if you want us to add a new model.
 
-The default text embedding (`TextEmbedding`) model is Flag Embedding, the top model in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
+The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
 
 ## 📈 Why FastEmbed?
 
 1. Light: FastEmbed is a lightweight library with few external dependencies. We don't require a GPU and don't download GBs of PyTorch dependencies, and instead use the ONNX Runtime. This makes it a great candidate for serverless runtimes like AWS Lambda. 
 
 2. Fast: FastEmbed is designed for speed. We use the ONNX Runtime, which is faster than PyTorch. We also use data-parallelism for encoding large datasets.
 
@@ -19,15 +19,14 @@
 ```bash
 pip install fastembed
 ```
 
 ## 📖 Quickstart
 
 ```python
-import numpy as np
 from fastembed import TextEmbedding
 from typing import List
 
 # Example list of documents
 documents: List[str] = [
     "This is built to be faster and lighter than other embedding libraries e.g. Transformers, Sentence-Transformers, etc.",
     "fastembed is supported by and maintained by Qdrant.",
```

### Comparing `fastembed-0.2.5/fastembed/common/model_management.py` & `fastembed-0.2.6/fastembed/common/model_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         raises:
             ValueError: If the model_name is not supported.
 
         Returns:
             Dict[str, Any]: The model description.
         """
         for model in cls.list_supported_models():
-            if model_name == model["model"]:
+            if model_name.lower() == model["model"].lower():
                 return model
 
         raise ValueError(f"Model {model_name} is not supported in {cls.__name__}.")
 
     @classmethod
     def download_file_from_gcs(cls, url: str, output_path: str, show_progress: bool = True) -> str:
         """
@@ -88,24 +88,28 @@
 
         # Warn if the total size is zero
         if total_size_in_bytes == 0:
             print(f"Warning: Content-length header is missing or zero in the response from {url}.")
 
         show_progress = total_size_in_bytes and show_progress
 
-        with tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True, disable=not show_progress) as progress_bar:
+        with tqdm(
+            total=total_size_in_bytes, unit="iB", unit_scale=True, disable=not show_progress
+        ) as progress_bar:
             with open(output_path, "wb") as file:
                 for chunk in response.iter_content(chunk_size=1024):
                     if chunk:  # Filter out keep-alive new chunks
                         progress_bar.update(len(chunk))
                         file.write(chunk)
         return output_path
 
     @classmethod
-    def download_files_from_huggingface(cls, hf_source_repo: str, cache_dir: Optional[str] = None) -> str:
+    def download_files_from_huggingface(
+        cls, hf_source_repo: str, cache_dir: Optional[str] = None
+    ) -> str:
         """
         Downloads a model from HuggingFace Hub.
         Args:
             hf_source_repo (str): Name of the model on HuggingFace Hub, e.g. "qdrant/all-MiniLM-L6-v2-onnx".
             cache_dir (Optional[str]): The path to the cache directory.
         Returns:
             Path: The path to the model directory.
@@ -212,15 +216,20 @@
         """
 
         hf_source = model.get("sources", {}).get("hf")
         url_source = model.get("sources", {}).get("url")
 
         if hf_source:
             try:
-                return Path(cls.download_files_from_huggingface(hf_source, cache_dir=str(cache_dir)))
+                return Path(
+                    cls.download_files_from_huggingface(hf_source, cache_dir=str(cache_dir))
+                )
             except (EnvironmentError, RepositoryNotFoundError, ValueError) as e:
-                logger.error(f"Could not download model from HuggingFace: {e}" "Falling back to other sources.")
+                logger.error(
+                    f"Could not download model from HuggingFace: {e}"
+                    "Falling back to other sources."
+                )
 
         if url_source:
             return cls.retrieve_model_gcs(model["model"], url_source, str(cache_dir))
 
         raise ValueError(f"Could not download model {model['model']} from any source.")
```

### Comparing `fastembed-0.2.5/fastembed/common/models.py` & `fastembed-0.2.6/fastembed/common/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         tokenizer_config = json.load(tokenizer_config_file)
 
     with open(str(tokens_map_path)) as tokens_map_file:
         tokens_map = json.load(tokens_map_file)
 
     tokenizer = Tokenizer.from_file(str(tokenizer_path))
     tokenizer.enable_truncation(max_length=min(tokenizer_config["model_max_length"], max_length))
-    tokenizer.enable_padding(pad_id=config.get("pad_token_id", 0), pad_token=tokenizer_config["pad_token"])
+    tokenizer.enable_padding(
+        pad_id=config.get("pad_token_id", 0), pad_token=tokenizer_config["pad_token"]
+    )
 
     for token in tokens_map.values():
         if isinstance(token, str):
             tokenizer.add_special_tokens([token])
         elif isinstance(token, dict):
             tokenizer.add_special_tokens([AddedToken(**token)])
```

### Comparing `fastembed-0.2.5/fastembed/common/onnx_model.py` & `fastembed-0.2.6/fastembed/common/onnx_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,29 @@
         so.graph_optimization_level = ort.GraphOptimizationLevel.ORT_ENABLE_ALL
 
         if threads is not None:
             so.intra_op_num_threads = threads
             so.inter_op_num_threads = threads
 
         self.tokenizer = load_tokenizer(model_dir=model_dir, max_length=max_length)
-        self.model = ort.InferenceSession(str(model_path), providers=onnx_providers, sess_options=so)
+        self.model = ort.InferenceSession(
+            str(model_path), providers=onnx_providers, sess_options=so
+        )
 
     def onnx_embed(self, documents: List[str]) -> Tuple[np.ndarray, np.ndarray]:
         encoded = self.tokenizer.encode_batch(documents)
         input_ids = np.array([e.ids for e in encoded])
         attention_mask = np.array([e.attention_mask for e in encoded])
 
         onnx_input = {
             "input_ids": np.array(input_ids, dtype=np.int64),
             "attention_mask": np.array(attention_mask, dtype=np.int64),
-            "token_type_ids": np.array([np.zeros(len(e), dtype=np.int64) for e in input_ids], dtype=np.int64),
+            "token_type_ids": np.array(
+                [np.zeros(len(e), dtype=np.int64) for e in input_ids], dtype=np.int64
+            ),
         }
 
         onnx_input = self._preprocess_onnx_input(onnx_input)
 
         model_output = self.model.run(None, onnx_input)
         embeddings = model_output[0]
         return embeddings, attention_mask
@@ -93,15 +97,17 @@
                 yield from self._post_process_onnx_output(self.onnx_embed(batch))
         else:
             start_method = "forkserver" if "forkserver" in get_all_start_methods() else "spawn"
             params = {
                 "model_name": model_name,
                 "cache_dir": cache_dir,
             }
-            pool = ParallelWorkerPool(parallel, self._get_worker_class(), start_method=start_method)
+            pool = ParallelWorkerPool(
+                parallel, self._get_worker_class(), start_method=start_method
+            )
             for batch in pool.ordered_map(iter_batch(documents, batch_size), **params):
                 yield from self._post_process_onnx_output(batch)
 
 
 class EmbeddingWorker(Worker):
     def init_embedding(
         self,
```

### Comparing `fastembed-0.2.5/fastembed/common/utils.py` & `fastembed-0.2.6/fastembed/common/utils.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.5/fastembed/embedding.py` & `fastembed-0.2.6/fastembed/embedding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
 from loguru import logger
 
-from fastembed.text.text_embedding import TextEmbedding
+from fastembed import TextEmbedding
 
 logger.warning(
-    "DefaultEmbedding, FlagEmbedding, JinaEmbedding are deprecated." "Use from fastembed import TextEmbedding instead."
+    "DefaultEmbedding, FlagEmbedding, JinaEmbedding are deprecated."
+    "Use from fastembed import TextEmbedding instead."
 )
 
 DefaultEmbedding = TextEmbedding
 FlagEmbedding = TextEmbedding
 
 
 class JinaEmbedding(TextEmbedding):
```

### Comparing `fastembed-0.2.5/fastembed/parallel_processor.py` & `fastembed-0.2.6/fastembed/parallel_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,17 @@
 
         for idx, item in self.semi_ordered_map(stream, *args, **kwargs):
             buffer[idx] = item
             while next_expected in buffer:
                 yield buffer.pop(next_expected)
                 next_expected += 1
 
-    def semi_ordered_map(self, stream: Iterable[Any], *args: Any, **kwargs: Any) -> Iterable[Tuple[int, Any]]:
+    def semi_ordered_map(
+        self, stream: Iterable[Any], *args: Any, **kwargs: Any
+    ) -> Iterable[Tuple[int, Any]]:
         try:
             self.start(**kwargs)
 
             assert self.input_queue is not None, "Input queue was not initialized"
             assert self.output_queue is not None, "Output queue was not initialized"
 
             pushed = 0
```

### Comparing `fastembed-0.2.5/fastembed/sparse/sparse_embedding_base.py` & `fastembed-0.2.6/fastembed/sparse/sparse_embedding_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,21 @@
         }
 
     def as_dict(self) -> Dict[int, float]:
         return {i: v for i, v in zip(self.indices, self.values)}
 
 
 class SparseTextEmbeddingBase(ModelManagement):
-    def __init__(self, model_name: str, cache_dir: Optional[str] = None, threads: Optional[int] = None, **kwargs):
+    def __init__(
+        self,
+        model_name: str,
+        cache_dir: Optional[str] = None,
+        threads: Optional[int] = None,
+        **kwargs,
+    ):
         self.model_name = model_name
         self.cache_dir = cache_dir
         self.threads = threads
 
     def embed(
         self,
         documents: Union[str, Iterable[str]],
```

### Comparing `fastembed-0.2.5/fastembed/sparse/sparse_text_embedding.py` & `fastembed-0.2.6/fastembed/sparse/sparse_text_embedding.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.5/fastembed/sparse/splade_pp.py` & `fastembed-0.2.6/fastembed/sparse/splade_pp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, Type
 
 import numpy as np
 
 from fastembed.common.onnx_model import EmbeddingWorker, OnnxModel
 from fastembed.common.utils import define_cache_dir
 from fastembed.sparse.sparse_embedding_base import SparseEmbedding, SparseTextEmbeddingBase
 
 supported_splade_models = [
     {
         "model": "prithvida/Splade_PP_en_v1",
         "vocab_size": 30522,
+        "description": "Misspelled version of the model. Retained for backward compatibility. Independent Implementation of SPLADE++ Model for English",
+        "size_in_GB": 0.532,
+        "sources": {
+            "hf": "Qdrant/SPLADE_PP_en_v1",
+        },
+    },
+    {
+        "model": "prithivida/Splade_PP_en_v1",
+        "vocab_size": 30522,
         "description": "Independent Implementation of SPLADE++ Model for English",
         "size_in_GB": 0.532,
         "sources": {
             "hf": "Qdrant/SPLADE_PP_en_v1",
         },
     },
 ]
 
 
 class SpladePP(SparseTextEmbeddingBase, OnnxModel[SparseEmbedding]):
     @classmethod
-    def _post_process_onnx_output(cls, output: Tuple[np.ndarray, np.ndarray]) -> Iterable[SparseEmbedding]:
+    def _post_process_onnx_output(
+        cls, output: Tuple[np.ndarray, np.ndarray]
+    ) -> Iterable[SparseEmbedding]:
         logits, attention_mask = output
         relu_log = np.log(1 + np.maximum(logits, 0))
 
         weighted_log = relu_log * np.expand_dims(attention_mask, axis=-1)
 
         scores = np.max(weighted_log, axis=1)
 
@@ -101,14 +112,18 @@
             model_name=self.model_name,
             cache_dir=str(self._cache_dir),
             documents=documents,
             batch_size=batch_size,
             parallel=parallel,
         )
 
+    @classmethod
+    def _get_worker_class(cls) -> Type[EmbeddingWorker]:
+        return SpladePPEmbeddingWorker
+
 
 class SpladePPEmbeddingWorker(EmbeddingWorker):
     def init_embedding(
         self,
         model_name: str,
         cache_dir: str,
     ) -> SpladePP:
```

### Comparing `fastembed-0.2.5/fastembed/text/e5_onnx_embedding.py` & `fastembed-0.2.6/fastembed/text/e5_onnx_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             "hf": "qdrant/multilingual-e5-large-onnx",
         },
     },
     {
         "model": "sentence-transformers/paraphrase-multilingual-mpnet-base-v2",
         "dim": 768,
         "description": "Sentence-transformers model for tasks like clustering or semantic search",
-        "size_in_GB": 1.11,
+        "size_in_GB": 1.00,
         "sources": {
             "hf": "xenova/paraphrase-multilingual-mpnet-base-v2",
         },
     },
 ]
```

### Comparing `fastembed-0.2.5/fastembed/text/jina_onnx_embedding.py` & `fastembed-0.2.6/fastembed/text/jina_onnx_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from fastembed.text.onnx_embedding import OnnxTextEmbedding, OnnxTextEmbeddingWorker
 
 supported_jina_models = [
     {
         "model": "jinaai/jina-embeddings-v2-base-en",
         "dim": 768,
         "description": "English embedding model supporting 8192 sequence length",
-        "size_in_GB": 0.55,
+        "size_in_GB": 0.52,
         "sources": {"hf": "xenova/jina-embeddings-v2-base-en"},
     },
     {
         "model": "jinaai/jina-embeddings-v2-small-en",
         "dim": 512,
         "description": "English embedding model supporting 8192 sequence length",
-        "size_in_GB": 0.13,
+        "size_in_GB": 0.12,
         "sources": {"hf": "xenova/jina-embeddings-v2-small-en"},
     },
 ]
 
 
 class JinaOnnxEmbedding(OnnxTextEmbedding):
     @classmethod
@@ -45,15 +45,17 @@
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries containing the model information.
         """
         return supported_jina_models
 
     @classmethod
-    def _post_process_onnx_output(cls, output: Tuple[np.ndarray, np.ndarray]) -> Iterable[np.ndarray]:
+    def _post_process_onnx_output(
+        cls, output: Tuple[np.ndarray, np.ndarray]
+    ) -> Iterable[np.ndarray]:
         embeddings, attn_mask = output
         return normalize(cls.mean_pooling(embeddings, attn_mask)).astype(np.float32)
 
 
 class JinaEmbeddingWorker(OnnxTextEmbeddingWorker):
     def init_embedding(
         self,
```

### Comparing `fastembed-0.2.5/fastembed/text/onnx_embedding.py` & `fastembed-0.2.6/fastembed/text/onnx_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,52 +8,43 @@
 from fastembed.text.text_embedding_base import TextEmbeddingBase
 
 supported_onnx_models = [
     {
         "model": "BAAI/bge-base-en",
         "dim": 768,
         "description": "Base English model",
-        "size_in_GB": 0.5,
+        "size_in_GB": 0.42,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/fast-bge-base-en.tar.gz",
         },
     },
     {
         "model": "BAAI/bge-base-en-v1.5",
         "dim": 768,
         "description": "Base English model, v1.5",
-        "size_in_GB": 0.44,
+        "size_in_GB": 0.21,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/fast-bge-base-en-v1.5.tar.gz",
             "hf": "qdrant/bge-base-en-v1.5-onnx-q",
         },
     },
     {
-        "model": "BAAI/bge-large-en-v1.5-quantized",
-        "dim": 1024,
-        "description": "Large English model, v1.5",
-        "size_in_GB": 1.34,
-        "sources": {
-            "hf": "qdrant/bge-large-en-v1.5-onnx-q",
-        },
-    },
-    {
         "model": "BAAI/bge-large-en-v1.5",
         "dim": 1024,
         "description": "Large English model, v1.5",
-        "size_in_GB": 1.34,
+        "size_in_GB": 1.20,
         "sources": {
             "hf": "qdrant/bge-large-en-v1.5-onnx",
         },
     },
     {
         "model": "BAAI/bge-small-en",
         "dim": 384,
         "description": "Fast English model",
-        "size_in_GB": 0.2,
+        "size_in_GB": 0.13,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/BAAI-bge-small-en.tar.gz",
         },
     },
     # {
     #     "model": "BAAI/bge-small-en",
     #     "dim": 384,
@@ -65,71 +56,70 @@
     #         "https://storage.googleapis.com/qdrant-fastembed/BAAI-bge-small-en.tar.gz"
     #     ]
     # },
     {
         "model": "BAAI/bge-small-en-v1.5",
         "dim": 384,
         "description": "Fast and Default English model",
-        "size_in_GB": 0.13,
+        "size_in_GB": 0.067,
         "sources": {
-            "url": "https://storage.googleapis.com/qdrant-fastembed/fast-bge-small-en-v1.5.tar.gz",
             "hf": "qdrant/bge-small-en-v1.5-onnx-q",
         },
     },
     {
         "model": "BAAI/bge-small-zh-v1.5",
         "dim": 512,
         "description": "Fast and recommended Chinese model",
-        "size_in_GB": 0.1,
+        "size_in_GB": 0.09,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/fast-bge-small-zh-v1.5.tar.gz",
         },
     },
-    {  # todo: it is not a flag embedding
+    {
         "model": "sentence-transformers/all-MiniLM-L6-v2",
         "dim": 384,
         "description": "Sentence Transformer model, MiniLM-L6-v2",
         "size_in_GB": 0.09,
         "sources": {
             "url": "https://storage.googleapis.com/qdrant-fastembed/sentence-transformers-all-MiniLM-L6-v2.tar.gz",
             "hf": "qdrant/all-MiniLM-L6-v2-onnx",
         },
     },
     {
         "model": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
         "dim": 384,
         "description": "Sentence Transformer model, paraphrase-multilingual-MiniLM-L12-v2",
-        "size_in_GB": 0.46,
+        "size_in_GB": 0.22,
         "sources": {
             "hf": "qdrant/paraphrase-multilingual-MiniLM-L12-v2-onnx-Q",
         },
     },
     {
         "model": "nomic-ai/nomic-embed-text-v1",
         "dim": 768,
         "description": "8192 context length english model",
-        "size_in_GB": 0.54,
+        "size_in_GB": 0.52,
         "sources": {
             "hf": "nomic-ai/nomic-embed-text-v1",
         },
     },
     {
         "model": "nomic-ai/nomic-embed-text-v1.5",
         "dim": 768,
         "description": "8192 context length english model",
-        "size_in_GB": 0.54,
+        "size_in_GB": 0.52,
         "sources": {
             "hf": "nomic-ai/nomic-embed-text-v1.5",
         },
     },
     {
         "model": "thenlper/gte-large",
         "dim": 1024,
         "description": "Large general text embeddings model",
-        "size_in_GB": 1.34,
+        "size_in_GB": 1.20,
         "sources": {
             "hf": "qdrant/gte-large-onnx",
         },
     },
     # {
     #     "model": "sentence-transformers/all-MiniLM-L6-v2",
     #     "dim": 384,
@@ -139,14 +129,23 @@
     #         "qdrant/all-MiniLM-L6-v2-onnx"
     #     ],
     #     "compressed_url_sources": [
     #         "https://storage.googleapis.com/qdrant-fastembed/fast-all-MiniLM-L6-v2.tar.gz",
     #         "https://storage.googleapis.com/qdrant-fastembed/sentence-transformers-all-MiniLM-L6-v2.tar.gz"
     #     ]
     # }
+    {
+        "model": "mixedbread-ai/mxbai-embed-large-v1",
+        "dim": 1024,
+        "description": "MixedBread Base sentence embedding model, does well on MTEB",
+        "size_in_GB": 0.64,
+        "sources": {
+            "hf": "mixedbread-ai/mxbai-embed-large-v1",
+        },
+    },
 ]
 
 
 class OnnxTextEmbedding(TextEmbeddingBase, OnnxModel[np.ndarray]):
     """Implementation of the Flag Embedding model."""
 
     @classmethod
@@ -226,15 +225,17 @@
     def _preprocess_onnx_input(self, onnx_input: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
         """
         Preprocess the onnx input.
         """
         return onnx_input
 
     @classmethod
-    def _post_process_onnx_output(cls, output: Tuple[np.ndarray, np.ndarray]) -> Iterable[np.ndarray]:
+    def _post_process_onnx_output(
+        cls, output: Tuple[np.ndarray, np.ndarray]
+    ) -> Iterable[np.ndarray]:
         embeddings, _ = output
         return normalize(embeddings[:, 0]).astype(np.float32)
 
 
 class OnnxTextEmbeddingWorker(EmbeddingWorker):
     def init_embedding(
         self,
```

### Comparing `fastembed-0.2.5/fastembed/text/text_embedding.py` & `fastembed-0.2.6/fastembed/text/text_embedding.py`

 * *Files identical despite different names*

### Comparing `fastembed-0.2.5/fastembed/text/text_embedding_base.py` & `fastembed-0.2.6/fastembed/text/text_embedding_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 import numpy as np
 
 from fastembed.common.model_management import ModelManagement
 
 
 class TextEmbeddingBase(ModelManagement):
-    def __init__(self, model_name: str, cache_dir: Optional[str] = None, threads: Optional[int] = None, **kwargs):
+    def __init__(
+        self,
+        model_name: str,
+        cache_dir: Optional[str] = None,
+        threads: Optional[int] = None,
+        **kwargs,
+    ):
         self.model_name = model_name
         self.cache_dir = cache_dir
         self.threads = threads
 
     def embed(
         self,
         documents: Union[str, Iterable[str]],
```

### Comparing `fastembed-0.2.5/pyproject.toml` & `fastembed-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastembed"
-version = "0.2.5"
+version = "0.2.6"
 description = "Fast, light, accurate library built for retrieval embedding generation"
 authors = ["NirantK <nirant.bits@gmail.com>"]
 license = "Apache License"
 readme = "README.md"
 packages = [{include = "fastembed"}]
 homepage = "https://github.com/qdrant/fastembed"
 repository = "https://github.com/qdrant/fastembed"
@@ -22,15 +22,15 @@
 numpy = [
     { version = ">=1.21", python = "<3.12" },
     { version = ">=1.26", python = ">=3.12" }
 ]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
-ruff = "^0.2.2"
+ruff = "^0.3.1"
 notebook = ">=7.0.2"
 pre-commit = {version = "^3.6.2", python = ">=3.9,<3.12" }
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.5.10"
 mkdocstrings = "^0.24.0"
 pillow = "^10.2.0"
@@ -39,8 +39,8 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-line-length = 120
+line-length = 99
```

### Comparing `fastembed-0.2.5/PKG-INFO` & `fastembed-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastembed
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fast, light, accurate library built for retrieval embedding generation
 Home-page: https://github.com/qdrant/fastembed
 License: Apache License
 Keywords: vector,embedding,neural,search,qdrant,sentence-transformers
 Author: NirantK
 Author-email: nirant.bits@gmail.com
 Requires-Python: >=3.8.0,<3.13
@@ -27,15 +27,15 @@
 Project-URL: Repository, https://github.com/qdrant/fastembed
 Description-Content-Type: text/markdown
 
 # ⚡️ What is FastEmbed?
 
 FastEmbed is a lightweight, fast, Python library built for embedding generation. We [support popular text models](https://qdrant.github.io/fastembed/examples/Supported_Models/). Please [open a GitHub issue](https://github.com/qdrant/fastembed/issues/new) if you want us to add a new model.
 
-The default text embedding (`TextEmbedding`) model is Flag Embedding, the top model in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
+The default text embedding (`TextEmbedding`) model is Flag Embedding, presented in the [MTEB](https://huggingface.co/spaces/mteb/leaderboard) leaderboard. It supports "query" and "passage" prefixes for the input text. Here is an example for [Retrieval Embedding Generation](https://qdrant.github.io/fastembed/examples/Retrieval_with_FastEmbed/) and how to use [FastEmbed with Qdrant](https://qdrant.github.io/fastembed/examples/Usage_With_Qdrant/).
 
 ## 📈 Why FastEmbed?
 
 1. Light: FastEmbed is a lightweight library with few external dependencies. We don't require a GPU and don't download GBs of PyTorch dependencies, and instead use the ONNX Runtime. This makes it a great candidate for serverless runtimes like AWS Lambda. 
 
 2. Fast: FastEmbed is designed for speed. We use the ONNX Runtime, which is faster than PyTorch. We also use data-parallelism for encoding large datasets.
 
@@ -48,15 +48,14 @@
 ```bash
 pip install fastembed
 ```
 
 ## 📖 Quickstart
 
 ```python
-import numpy as np
 from fastembed import TextEmbedding
 from typing import List
 
 # Example list of documents
 documents: List[str] = [
     "This is built to be faster and lighter than other embedding libraries e.g. Transformers, Sentence-Transformers, etc.",
     "fastembed is supported by and maintained by Qdrant.",
```

