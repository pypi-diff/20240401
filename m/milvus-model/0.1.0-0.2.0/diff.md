# Comparing `tmp/milvus-model-0.1.0.tar.gz` & `tmp/milvus-model-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus-model-0.1.0.tar", last modified: Wed Mar 20 06:37:30 2024, max compression
+gzip compressed data, was "milvus-model-0.2.0.tar", last modified: Mon Apr  1 15:20:31 2024, max compression
```

## Comparing `milvus-model-0.1.0.tar` & `milvus-model-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,43 @@
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      303 2024-03-20 03:16:09.000000 milvus-model-0.1.0/.gitignore
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)    11357 2024-03-20 03:16:09.000000 milvus-model-0.1.0/LICENSE
--rw-r--r--   0 yangxuan  (1000) yangxuan  (1000)     1769 2024-03-20 06:37:30.646199 milvus-model-0.1.0/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     1013 2024-03-20 03:16:09.000000 milvus-model-0.1.0/README.md
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.642199 milvus-model-0.1.0/milvus_model/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      247 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      272 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/base.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/milvus_model/dense/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      194 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/dense/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2280 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/dense/openai.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     2699 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/dense/sentence_transformer.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/milvus_model/hybrid/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       81 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/hybrid/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3509 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/hybrid/bge_m3.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/milvus_model/sparse/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      148 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/__init__.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/milvus_model/sparse/bm25/
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      243 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/bm25/__init__.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     8630 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/bm25/bm25.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     3142 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/bm25/lang.yaml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     6402 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/bm25/tokenizers.py
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     7880 2024-03-20 03:16:09.000000 milvus-model-0.1.0/milvus_model/sparse/splade.py
-drwxrwxr-x   0 yangxuan  (1000) yangxuan  (1000)        0 2024-03-20 06:37:30.646199 milvus-model-0.1.0/milvus_model.egg-info/
--rw-r--r--   0 yangxuan  (1000) yangxuan  (1000)     1769 2024-03-20 06:37:30.000000 milvus-model-0.1.0/milvus_model.egg-info/PKG-INFO
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      639 2024-03-20 06:37:30.000000 milvus-model-0.1.0/milvus_model.egg-info/SOURCES.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)        1 2024-03-20 06:37:30.000000 milvus-model-0.1.0/milvus_model.egg-info/dependency_links.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)      154 2024-03-20 06:37:30.000000 milvus-model-0.1.0/milvus_model.egg-info/requires.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       13 2024-03-20 06:37:30.000000 milvus-model-0.1.0/milvus_model.egg-info/top_level.txt
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)     4149 2024-03-20 06:36:45.000000 milvus-model-0.1.0/pyproject.toml
--rw-rw-r--   0 yangxuan  (1000) yangxuan  (1000)       38 2024-03-20 06:37:30.646199 milvus-model-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.006065 milvus-model-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 15:20:24.000000 milvus-model-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:20:31.014065 milvus-model-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 15:20:24.000000 milvus-model-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-01 15:20:24.000000 milvus-model-0.2.0/_version_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/dense/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/hybrid/bge_m3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/bgereranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/cross_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model/sparse/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/lang.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/splade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-01 15:20:31.000000 milvus-model-0.2.0/milvus_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-01 15:20:24.000000 milvus-model-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:20:31.014065 milvus-model-0.2.0/setup.cfg
```

### Comparing `milvus-model-0.1.0/LICENSE` & `milvus-model-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/PKG-INFO` & `milvus-model-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.1.0
+Version: 0.2.0
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.12.0
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding>=1.2.2
 Requires-Dist: nltk
-Requires-Dist: transformers>=4.33.0
+Requires-Dist: transformers>=4.36.0
 Requires-Dist: jieba
 Requires-Dist: konlpy
 Requires-Dist: mecab-python3
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: protobuf==3.20.0
 Requires-Dist: unidic-lite
+Requires-Dist: cohere
+Requires-Dist: voyageai>=0.2.0
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
 
 `milvus-model` supports Python 3.8 and above. Install it via pip:
 ```bash
 pip install milvus-model
 ```
 This command installs milvus-model directly. If you're working within the PyMilvus ecosystem and want to include milvus-model as an optional component, you can install it using:
 ```bash
-pip install pymilvus[model]
+pip install pymilvus[model] 
+# or pip install "pymilvus[model]" for zsh.
 ```
 To upgrade milvus-model to the latest version, use:
 ```
 pip install milvus-model --upgrade
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
```

### Comparing `milvus-model-0.1.0/README.md` & `milvus-model-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 `milvus-model` supports Python 3.8 and above. Install it via pip:
 ```bash
 pip install milvus-model
 ```
 This command installs milvus-model directly. If you're working within the PyMilvus ecosystem and want to include milvus-model as an optional component, you can install it using:
 ```bash
-pip install pymilvus[model]
+pip install pymilvus[model] 
+# or pip install "pymilvus[model]" for zsh.
 ```
 To upgrade milvus-model to the latest version, use:
 ```
 pip install milvus-model --upgrade
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
```

### Comparing `milvus-model-0.1.0/milvus_model/dense/openai.py` & `milvus-model-0.2.0/milvus_model/dense/openai.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/milvus_model/dense/sentence_transformer.py` & `milvus-model-0.2.0/milvus_model/dense/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/milvus_model/hybrid/bge_m3.py` & `milvus-model-0.2.0/milvus_model/hybrid/bge_m3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from collections import defaultdict
 from typing import Dict, List
 
 from scipy.sparse import csr_array, vstack
 
 from milvus_model.base import BaseEmbeddingFunction
 
 logger = logging.getLogger(__name__)
@@ -54,28 +53,25 @@
             "return_sparse": return_sparse,
             "return_colbert_vecs": return_colbert_vecs,
         }
         self._model_config = _model_config
         self._encode_config = _encode_config
 
         self.model = BGEM3FlagModel(**self._model_config)
-        meta_info = defaultdict(dict)
-        meta_info["BAAI/bge-m3"]["dim"] = {
-            "dense": 1024,
-            "sparse": len(self.model.tokenizer),
-            "colbert_vecs": 1024,
-        }
-        self._meta_info = meta_info
 
     def __call__(self, texts: List[str]) -> Dict:
         return self._encode(texts)
 
     @property
     def dim(self) -> Dict:
-        return self._meta_info[self.model_name]["dim"]
+        return {
+            "dense": self.model.model.model.config.hidden_size,
+            "colbert_vecs": self.model.model.colbert_linear.out_features,
+            "sparse": len(self.model.tokenizer),
+        }
 
     def _encode(self, texts: List[str]) -> Dict:
         output = self.model.encode(sentences=texts, **self._encode_config)
         results = {}
         if self._encode_config["return_dense"] is True:
             results["dense"] = list(output["dense_vecs"])
         if self._encode_config["return_sparse"] is True:
```

### Comparing `milvus-model-0.1.0/milvus_model/sparse/bm25/bm25.py` & `milvus-model-0.2.0/milvus_model/sparse/bm25/bm25.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/milvus_model/sparse/bm25/lang.yaml` & `milvus-model-0.2.0/milvus_model/sparse/bm25/lang.yaml`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/milvus_model/sparse/bm25/tokenizers.py` & `milvus-model-0.2.0/milvus_model/sparse/bm25/tokenizers.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.1.0/milvus_model/sparse/splade.py` & `milvus-model-0.2.0/milvus_model/sparse/splade.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import logging
 from typing import Dict, List, Optional
 
-import numpy as np
 import torch
 from scipy.sparse import csr_array, vstack
 
 from milvus_model.base import BaseEmbeddingFunction
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -127,81 +126,81 @@
             truncation=True,
             max_length=self.tokenizer.model_max_length,
             return_tensors="pt",
             add_special_tokens=True,
             padding=True,
         )
         encoded_input = {key: val.to(self.device) for key, val in encoded_input.items()}
-        output = self.model(**encoded_input)
+        with torch.no_grad():
+            output = self.model(**encoded_input)
         return output.logits
 
     def _batchify(self, texts: List[str], batch_size: int) -> List[List[str]]:
         return [texts[i : i + batch_size] for i in range(0, len(texts), batch_size)]
 
     def forward(self, texts: List[str], k_tokens: int) -> csr_array:
         batched_texts = self._batchify(texts, self.batch_size)
         sparse_embs = []
         for batch_texts in batched_texts:
             logits = self._encode(texts=batch_texts)
             activations = self._get_activation(logits=logits)
             if k_tokens is None:
-                nonzero_indices = [
-                    torch.nonzero(activations["sparse_activations"][i]).t()[0]
-                    for i in range(len(batch_texts))
-                ]
+                nonzero_indices = torch.nonzero(activations["sparse_activations"])
                 activations["activations"] = nonzero_indices
             else:
                 activations = self._update_activations(**activations, k_tokens=k_tokens)
             batch_csr = self._convert_to_csr_array(activations)
             sparse_embs.extend(batch_csr)
 
-        return vstack(sparse_embs)
+        return vstack(sparse_embs).tocsr()
 
     def _get_activation(self, logits: torch.Tensor) -> Dict[str, torch.Tensor]:
         return {"sparse_activations": torch.amax(torch.log1p(self.relu(logits)), dim=1)}
 
     def _update_activations(self, sparse_activations: torch.Tensor, k_tokens: int) -> torch.Tensor:
         activations = torch.topk(input=sparse_activations, k=k_tokens, dim=1).indices
 
         # Set value of max sparse_activations which are not in top k to 0.
         sparse_activations = sparse_activations * torch.zeros(
             (sparse_activations.shape[0], sparse_activations.shape[1]),
             dtype=int,
             device=self.device,
         ).scatter_(dim=1, index=activations.long(), value=1)
 
+        activations = torch.cat(
+            (
+                torch.arange(activations.shape[0], device=activations.device)
+                .repeat_interleave(activations.shape[1])
+                .reshape(-1, 1),
+                activations.reshape((-1, 1)),
+            ),
+            dim=1,
+        )
+
         return {
             "activations": activations,
             "sparse_activations": sparse_activations,
         }
 
     def _filter_activations(
         self, activations: torch.Tensor, k_tokens: int, **kwargs
     ) -> torch.Tensor:
         _, activations = torch.topk(input=activations, k=k_tokens, dim=1, **kwargs)
         return activations
 
     def _convert_to_csr_array(self, activations: Dict):
-        csr_array_list = []
 
-        if activations["sparse_activations"].shape[0] != len(activations["activations"]):
-            error_msg = (
-                "The shape of 'sparse_activations' does not match the length of 'activations'"
-            )
-            raise ValueError(error_msg)
-
-        for i, column_indices in enumerate(activations["activations"]):
-            values = (
-                torch.gather(activations["sparse_activations"][i], 0, column_indices)
-                .cpu()
-                .detach()
-                .numpy()
-            )
-            row_indices = np.zeros(len(activations["activations"][i]))
-            col_indices = activations["activations"][i].cpu().detach().numpy()
-            csr_array_list.append(
-                csr_array(
-                    (values.flatten(), (row_indices, col_indices)),
-                    shape=(1, activations["sparse_activations"].shape[1]),
-                )
-            )
-        return csr_array_list
+        values = (
+            activations["sparse_activations"][
+                activations["activations"][:, 0], activations["activations"][:, 1]
+            ]
+            .cpu()
+            .detach()
+            .numpy()
+        )
+
+        row_indices = activations["activations"][:, 0].cpu().detach().numpy()
+        col_indices = activations["activations"][:, 1].cpu().detach().numpy()
+        return csr_array(
+            (values.flatten(), (row_indices, col_indices)),
+            shape=activations["sparse_activations"].shape,
+        )
```

### Comparing `milvus-model-0.1.0/milvus_model.egg-info/PKG-INFO` & `milvus-model-0.2.0/milvus_model.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.1.0
+Version: 0.2.0
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1.12.0
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding>=1.2.2
 Requires-Dist: nltk
-Requires-Dist: transformers>=4.33.0
+Requires-Dist: transformers>=4.36.0
 Requires-Dist: jieba
 Requires-Dist: konlpy
 Requires-Dist: mecab-python3
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: protobuf==3.20.0
 Requires-Dist: unidic-lite
+Requires-Dist: cohere
+Requires-Dist: voyageai>=0.2.0
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
 
 ## Installation
 
 `milvus-model` supports Python 3.8 and above. Install it via pip:
 ```bash
 pip install milvus-model
 ```
 This command installs milvus-model directly. If you're working within the PyMilvus ecosystem and want to include milvus-model as an optional component, you can install it using:
 ```bash
-pip install pymilvus[model]
+pip install pymilvus[model] 
+# or pip install "pymilvus[model]" for zsh.
 ```
 To upgrade milvus-model to the latest version, use:
 ```
 pip install milvus-model --upgrade
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
```

### Comparing `milvus-model-0.1.0/milvus_model.egg-info/SOURCES.txt` & `milvus-model-0.2.0/milvus_model.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 .gitignore
 LICENSE
 README.md
+_version_helper.py
 pyproject.toml
+.github/workflows/publish_dev_package.yml
+.github/workflows/publish_on_release.yml
 milvus_model/__init__.py
 milvus_model/base.py
 milvus_model.egg-info/PKG-INFO
 milvus_model.egg-info/SOURCES.txt
 milvus_model.egg-info/dependency_links.txt
 milvus_model.egg-info/requires.txt
 milvus_model.egg-info/top_level.txt
 milvus_model/dense/__init__.py
 milvus_model/dense/openai.py
 milvus_model/dense/sentence_transformer.py
+milvus_model/dense/voyageai.py
 milvus_model/hybrid/__init__.py
 milvus_model/hybrid/bge_m3.py
+milvus_model/reranker/__init__.py
+milvus_model/reranker/bgereranker.py
+milvus_model/reranker/cohere.py
+milvus_model/reranker/cross_encoder.py
+milvus_model/reranker/voyageai.py
 milvus_model/sparse/__init__.py
 milvus_model/sparse/splade.py
 milvus_model/sparse/bm25/__init__.py
 milvus_model/sparse/bm25/bm25.py
 milvus_model/sparse/bm25/lang.yaml
 milvus_model/sparse/bm25/tokenizers.py
```

### Comparing `milvus-model-0.1.0/pyproject.toml` & `milvus-model-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,43 @@
   "gitpython",
   "setuptools_scm[toml] >= 6.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "milvus-model"
-version = "0.1.0"  # Update with your current version
 authors = [
   {name = "Milvus Team", email = "milvus-team@zilliz.com"},
 ]
 requires-python = ">=3.8"
 description = "Model components for PyMilvus, the Python SDK for Milvus"
 readme = "README.md"
 dependencies = [
     "openai >= 1.12.0",
     "sentence-transformers",
     "FlagEmbedding >= 1.2.2",
     "nltk",
-    "transformers >= 4.33.0",
+    "transformers >= 4.36.0",
     "jieba",
     "konlpy",
     "mecab-python3",
     "scipy >= 1.10.0",
     "protobuf==3.20.0",
     "unidic-lite",
+    "cohere",
+    "voyageai >= 0.2.0",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 
+dynamic = ["version"]
+
 [project.urls]
 repository = "https://github.com/milvus-io/milvus-model"  # Update the repository URL
 
 [tool.setuptools.dynamic]
 version = { attr = "_version_helper.version" }
 
 [tool.setuptools_scm]
```

