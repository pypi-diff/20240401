# Comparing `tmp/picachain-0.1.20.tar.gz` & `tmp/picachain-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picachain-0.1.20.tar", max compression
+gzip compressed data, was "picachain-0.1.30.tar", max compression
```

## Comparing `picachain-0.1.20.tar` & `picachain-0.1.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-03-27 18:13:06.705397 picachain-0.1.20/LICENSE
--rw-r--r--   0        0        0     1925 2024-04-01 09:41:20.443801 picachain-0.1.20/README.md
--rw-r--r--   0        0        0        0 2024-03-27 17:21:07.953194 picachain-0.1.20/picachain/__init__.py
--rw-r--r--   0        0        0      230 2024-03-29 17:34:59.884284 picachain-0.1.20/picachain/datastore/__init__.py
--rw-r--r--   0        0        0     3078 2024-03-31 15:09:02.564382 picachain-0.1.20/picachain/datastore/chroma.py
--rw-r--r--   0        0        0      732 2024-03-31 09:17:25.271088 picachain-0.1.20/picachain/datastore/datastore.py
--rw-r--r--   0        0        0     2874 2024-03-28 07:11:51.897969 picachain-0.1.20/picachain/datastore/pinecone.py
--rw-r--r--   0        0        0      166 2024-03-29 17:30:15.708875 picachain-0.1.20/picachain/embedding/__init__.py
--rw-r--r--   0        0        0     1836 2024-03-30 17:40:26.622816 picachain-0.1.20/picachain/embedding/clip_embedding.py
--rw-r--r--   0        0        0      570 2024-03-29 13:24:42.213948 picachain-0.1.20/picachain/embedding/embedding.py
--rw-r--r--   0        0        0      169 2024-03-31 14:45:13.557494 picachain-0.1.20/picachain/retriever/__init__.py
--rw-r--r--   0        0        0     2708 2024-03-31 14:56:25.457614 picachain-0.1.20/picachain/retriever/image_retriever.py
--rw-r--r--   0        0        0      272 2024-03-31 14:40:10.519412 picachain-0.1.20/picachain/retriever/retriever.py
--rw-r--r--   0        0        0       81 2024-04-01 09:22:48.252396 picachain-0.1.20/picachain/search/__init__.py
--rw-r--r--   0        0        0      791 2024-03-31 14:54:19.198742 picachain-0.1.20/picachain/search/image_search.py
--rw-r--r--   0        0        0      457 2024-03-31 08:34:46.916761 picachain-0.1.20/picachain/utils/image_util.py
--rw-r--r--   0        0        0      773 2024-04-01 09:42:28.124181 picachain-0.1.20/pyproject.toml
--rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 picachain-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-27 18:13:06.705397 picachain-0.1.30/LICENSE
+-rw-r--r--   0        0        0     1916 2024-04-01 15:35:54.123339 picachain-0.1.30/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 17:21:07.953194 picachain-0.1.30/picachain/__init__.py
+-rw-r--r--   0        0        0      230 2024-03-29 17:34:59.884284 picachain-0.1.30/picachain/datastore/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-01 15:41:21.052985 picachain-0.1.30/picachain/datastore/chroma.py
+-rw-r--r--   0        0        0      812 2024-04-01 16:56:46.230418 picachain-0.1.30/picachain/datastore/datastore.py
+-rw-r--r--   0        0        0     4523 2024-04-01 17:07:15.694551 picachain-0.1.30/picachain/datastore/pinecone.py
+-rw-r--r--   0        0        0      166 2024-03-29 17:30:15.708875 picachain-0.1.30/picachain/embedding/__init__.py
+-rw-r--r--   0        0        0     1836 2024-03-30 17:40:26.622816 picachain-0.1.30/picachain/embedding/clip_embedding.py
+-rw-r--r--   0        0        0      570 2024-03-29 13:24:42.213948 picachain-0.1.30/picachain/embedding/embedding.py
+-rw-r--r--   0        0        0      169 2024-03-31 14:45:13.557494 picachain-0.1.30/picachain/retriever/__init__.py
+-rw-r--r--   0        0        0     3383 2024-04-01 18:46:27.787337 picachain-0.1.30/picachain/retriever/image_retriever.py
+-rw-r--r--   0        0        0      272 2024-03-31 14:40:10.519412 picachain-0.1.30/picachain/retriever/retriever.py
+-rw-r--r--   0        0        0       81 2024-04-01 09:22:48.252396 picachain-0.1.30/picachain/search/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-01 18:45:01.928742 picachain-0.1.30/picachain/search/image_search.py
+-rw-r--r--   0        0        0      457 2024-03-31 08:34:46.916761 picachain-0.1.30/picachain/utils/image_util.py
+-rw-r--r--   0        0        0      785 2024-04-01 18:50:08.558119 picachain-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0     2927 1970-01-01 00:00:00.000000 picachain-0.1.30/PKG-INFO
```

### Comparing `picachain-0.1.20/LICENSE` & `picachain-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `picachain-0.1.20/README.md` & `picachain-0.1.30/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 <img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/3a299c21-6590-4ee1-a3c1-73a92653f21e" height=150></img>
 <h3>⚡️ A Simple ready-to-use Image search engine library</h3>
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
-[![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
+[![PyPi license](https://badgen.net/pypi/license/pip/)]() [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
 
 </div>
 
 ## 📌 Install Picachain
 Create a local datastore with **ChromaDB** for image search.
 
 With `pip` :
@@ -41,15 +41,16 @@
 datastore = ChromaStore("test-collection")
 retriever = ImageRetriever(datastore, embedding, images)
 
 image_search = ImageSearch(retriever=retriever, embedding=embedding, query_img=img)
 result = image_search.search_relevant_images(top_k=3) # get top 3 relevant images
 
 for img, score in result: # [(img, score), (img, score)]
-    img.show()
+    plt.imshow(img)
+    plt.show()
 
 ```
 
 It is under continuous development so currently supports only [ChromaDB](https://docs.trychroma.com/). We are working on integrating all popular vector databases such as [Pinecone](https://www.pinecone.io/), [Weaviate](https://weaviate.io/), etc.
```

### Comparing `picachain-0.1.20/picachain/datastore/chroma.py` & `picachain-0.1.30/picachain/datastore/chroma.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,39 +33,36 @@
         self.collection_name = collection_name
         self.metadata = metadata
         self.storage_path = storage_path
         self.database = database
 
         self.client = chromadb.PersistentClient()
 
-    def _embedding_ids(self):
-        str(uuid.uuid4())
-
     def _health_check(self) -> bool:
         return isinstance(self.client.heartbeat(), int)
 
     def generate_embeddings(
         self, images: List[Image], embedding: Embedding
     ) -> np.ndarray:
         return embedding.encode_images(images)
 
-    def create_collection(self):
+    def create(self):
         collection = self.client.get_or_create_collection(
             name=self.collection_name,
         )
         return collection
 
-    def add_to_collection(
+    def add(
         self,
         collection: Collection,
         embeddings: List[float],
         documents: List[str],
         ids: List[str],
     ):
-        """Add embeddings, documents to collection.
+        """Add embeddings, documents to index or collection.
 
         Args:
         - collection: created collection.
         - embeddings: list of image embeddings
         - documents: list of base64 string of images
         - ids: list of ids for images."""
         try:
@@ -73,15 +70,15 @@
                 embeddings=embeddings,
                 ids=ids,
                 documents=documents,
             )
         except Exception as e:
             raise Exception(f"Failed to add documents to Chroma store. {e}")
 
-    def query_documents(
+    def query(
         self,
         collection: Collection,
         query_embedding: List[float],
         top_k: int = 3,
     ) -> list:
         """Retrieve relevant images from chroma database.
 
@@ -93,15 +90,22 @@
         Returns:
         - list of images along with their score.
         """
         result = collection.query(query_embeddings=query_embedding, n_results=top_k)
         relevant_images = [
             base64_to_image(img_str) for img_str in result["documents"][0]
         ]
-        scores = [score for score in result["distances"][0]]
+        scores = [round(score, 3) for score in result["distances"][0]]
         return list(zip(relevant_images, scores))
 
+    def delete(self, collection_name: str):
+        try:
+            self.client.delete_collection(collection_name)
+            return True
+        except Exception as e:
+            raise Exception("Failed to delete collection", e)
+
     @staticmethod
     def collection_info(collection: Collection):
         info = defaultdict(str)
         info["count"] = collection.count()
         info["top_10_items"] = collection.peek()
```

### Comparing `picachain-0.1.20/picachain/datastore/datastore.py` & `picachain-0.1.30/picachain/datastore/datastore.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 import numpy as np
 from PIL.Image import Image
 
 from picachain.embedding import Embedding
 
 
 class DataStore(ABC):
-    pass
+    """Interface for datastores and vector databases."""
 
-    @abstractmethod
     def generate_embeddings(
         self, images: List[Image], embedding: Embedding
     ) -> np.ndarray:
-        """Generate embeddings to be stored on the datastore."""
+        return embedding.encode_images(images)
 
     @abstractmethod
-    def create_collection(self):
+    def create(self):
         """Create a collection for documents and embedding"""
 
     @abstractmethod
-    def add_to_collection(self, *args, **kwargs):
+    def add(self, *args, **kwargs):
         """Add embeddings and metadata to collection."""
 
     @abstractmethod
-    def query_documents(self, *args, **kwargs) -> list:
+    def query(self, *args, **kwargs) -> list:
         """Query similar images"""
+
+    @abstractmethod
+    def delete(self, *args, **kwargs):
+        """Delete the collection or index"""
```

### Comparing `picachain-0.1.20/picachain/embedding/clip_embedding.py` & `picachain-0.1.30/picachain/embedding/clip_embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.20/picachain/embedding/embedding.py` & `picachain-0.1.30/picachain/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.20/picachain/retriever/image_retriever.py` & `picachain-0.1.30/picachain/retriever/image_retriever.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import uuid
 from collections import defaultdict
-from typing import List
+from typing import List, Union
 
 from PIL.Image import Image
 
-from picachain.datastore import ChromaStore, DataStore, PineconeStore
+from picachain.datastore import ChromaStore, PineconeStore
 from picachain.embedding import ClipEmbedding, Embedding
-from picachain.utils.image_util import base64_to_image, image_to_base64
+from picachain.utils.image_util import image_to_base64
 
 
 class ImageRetriever:
-    datastore_collection = None
+    datastore_collection_index = None  # index or collection based on the database
 
     def __init__(
         self,
-        datastore: ChromaStore,
+        datastore: Union[ChromaStore, PineconeStore],
         embedding: Embedding,
         images: List[Image],
     ) -> None:
         """Initiate Image retriever."""
         self.datastore = datastore
         self.embedding = embedding
         self.images = images
@@ -44,38 +44,51 @@
         return [str(uuid.uuid5(uuid.NAMESPACE_URL, img)) for img in images]
 
     ## store the embeddings into datastore
     def _push_embedding_to_datastore(self):
         """Push embeddings and documents to datastore."""
         try:
             embeddings = self.datastore.generate_embeddings(self.images, self.embedding)
-            self.datastore_collection = self.datastore.create_collection()
+            self.datastore_collection_index = self.datastore.create()
             documents = self._process_images_for_storage()
             ids = self._create_ids_for_images(documents)
-            self.datastore.add_to_collection(
-                collection=self.datastore_collection,
-                embeddings=embeddings,
-                documents=documents,
-                ids=ids,
-            )
+
+            if isinstance(self.datastore, ChromaStore):
+                self.datastore.add(
+                    collection=self.datastore_collection_index,
+                    embeddings=embeddings,
+                    documents=documents,
+                    ids=ids,
+                )
+            elif isinstance(self.datastore, PineconeStore):
+                self.datastore.add(
+                    index=self.datastore_collection_index,
+                    embeddings=embeddings,
+                    documents=documents,
+                    ids=ids,
+                )
         except Exception as e:
             raise Exception("Failed to push embeddings", e)
 
-    def get_relevant_images(
-        self, collection, query_embedding: list, top_k: int
-    ) -> list:
+    def get_relevant_images(self, query_embedding: list, top_k: int) -> list:
         """Retrieve top k relevant images from datastore.
 
         Args:
-        - collection: database collection.
         - query_embedding: query image embedding.
         - top_k (int): top k relevant images to retrieve.
 
         Returns:
         - list of relevant images.
         """
-        relevant_images = self.datastore.query_documents(
-            collection=collection,
-            query_embedding=query_embedding,
-            top_k=top_k,
-        )
+        if isinstance(self.datastore, ChromaStore):
+            relevant_images = self.datastore.query(
+                collection=self.datastore_collection_index,
+                query_embedding=query_embedding,
+                top_k=top_k,
+            )
+        elif isinstance(self.datastore, PineconeStore):
+            relevant_images = self.datastore.query(
+                index=self.datastore_collection_index,
+                query_embedding=query_embedding,
+                top_k=top_k,
+            )
         return relevant_images
```

### Comparing `picachain-0.1.20/picachain/search/image_search.py` & `picachain-0.1.30/picachain/search/image_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PIL import Image
 
-from picachain.embedding import ClipEmbedding, Embedding
+from picachain.embedding import Embedding
 from picachain.retriever import ImageRetriever
 
 
 class ImageSearch:
     def __init__(
         self, retriever: ImageRetriever, query_img: Image, embedding: Embedding
     ) -> None:
@@ -17,11 +17,10 @@
         return self.embedding.encode_images([self.query_img]).tolist()
 
     def search_relevant_images(
         self,
         top_k: int = 3,
     ):
         return self.retriever.get_relevant_images(
-            collection=self.retriever.datastore_collection,
             query_embedding=self._embed_query_img(),
             top_k=top_k,
         )
```

### Comparing `picachain-0.1.20/pyproject.toml` & `picachain-0.1.30/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,29 @@
   "search-engine",
   "chromadb",
   "image",
   "search",
   "packages",
   "poetry",
   "python-packages",
+  "pinecone",
 ]
 license = "MIT"
 name = "picachain"
 packages = [{include = "picachain"}]
 readme = "README.md"
 repository = "https://github.com/d1pankarmedhi/picachain"
-version = "0.1.20"
+version = "0.1.30"
 
 [tool.poetry.dependencies]
 chromadb = "^0.4.24"
 matplotlib = "^3.8.3"
-pillow = "^10.2.0"
+pillow = "10.1.0"
 pinecone-client = "^3.2.1"
 pysqlite3-binary = "^0.5.2.post3"
 python = "^3.10"
-torch = "^2.2.2"
+torch = "2.2.1"
 transformers = "^4.39.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
```

### Comparing `picachain-0.1.20/PKG-INFO` & `picachain-0.1.30/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: picachain
-Version: 0.1.20
+Version: 0.1.30
 Summary: Simple image search engine package.
 Home-page: https://github.com/d1pankarmedhi/picachain
 License: MIT
-Keywords: python,search-engine,chromadb,image,search,packages,poetry,python-packages
+Keywords: python,search-engine,chromadb,image,search,packages,poetry,python-packages,pinecone
 Author: d1pankarmedhi
 Author-email: dipankarmedhi11@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: pillow (>=10.2.0,<11.0.0)
+Requires-Dist: pillow (==10.1.0)
 Requires-Dist: pinecone-client (>=3.2.1,<4.0.0)
 Requires-Dist: pysqlite3-binary (>=0.5.2.post3,<0.6.0)
-Requires-Dist: torch (>=2.2.2,<3.0.0)
+Requires-Dist: torch (==2.2.1)
 Requires-Dist: transformers (>=4.39.1,<5.0.0)
 Project-URL: Repository, https://github.com/d1pankarmedhi/picachain
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/3a299c21-6590-4ee1-a3c1-73a92653f21e" height=150></img>
 <h3>⚡️ A Simple ready-to-use Image search engine library</h3>
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
-[![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
+[![PyPi license](https://badgen.net/pypi/license/pip/)]() [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
 
 </div>
 
 ## 📌 Install Picachain
 Create a local datastore with **ChromaDB** for image search.
 
 With `pip` :
@@ -66,15 +66,16 @@
 datastore = ChromaStore("test-collection")
 retriever = ImageRetriever(datastore, embedding, images)
 
 image_search = ImageSearch(retriever=retriever, embedding=embedding, query_img=img)
 result = image_search.search_relevant_images(top_k=3) # get top 3 relevant images
 
 for img, score in result: # [(img, score), (img, score)]
-    img.show()
+    plt.imshow(img)
+    plt.show()
 
 ```
 
 It is under continuous development so currently supports only [ChromaDB](https://docs.trychroma.com/). We are working on integrating all popular vector databases such as [Pinecone](https://www.pinecone.io/), [Weaviate](https://weaviate.io/), etc.
```

