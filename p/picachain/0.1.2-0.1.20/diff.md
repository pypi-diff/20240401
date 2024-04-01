# Comparing `tmp/picachain-0.1.2.tar.gz` & `tmp/picachain-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picachain-0.1.2.tar", max compression
+gzip compressed data, was "picachain-0.1.20.tar", max compression
```

## Comparing `picachain-0.1.2.tar` & `picachain-0.1.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-03-27 18:13:06.705397 picachain-0.1.2/LICENSE
--rw-r--r--   0        0        0     1938 2024-04-01 08:06:58.761284 picachain-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-27 17:21:07.953194 picachain-0.1.2/picachain/__init__.py
--rw-r--r--   0        0        0      230 2024-03-29 17:34:59.884284 picachain-0.1.2/picachain/datastore/__init__.py
--rw-r--r--   0        0        0     3078 2024-03-31 15:09:02.564382 picachain-0.1.2/picachain/datastore/chroma.py
--rw-r--r--   0        0        0      732 2024-03-31 09:17:25.271088 picachain-0.1.2/picachain/datastore/datastore.py
--rw-r--r--   0        0        0     2874 2024-03-28 07:11:51.897969 picachain-0.1.2/picachain/datastore/pinecone.py
--rw-r--r--   0        0        0      166 2024-03-29 17:30:15.708875 picachain-0.1.2/picachain/embedding/__init__.py
--rw-r--r--   0        0        0     1836 2024-03-30 17:40:26.622816 picachain-0.1.2/picachain/embedding/clip_embedding.py
--rw-r--r--   0        0        0      570 2024-03-29 13:24:42.213948 picachain-0.1.2/picachain/embedding/embedding.py
--rw-r--r--   0        0        0      169 2024-03-31 14:45:13.557494 picachain-0.1.2/picachain/retriever/__init__.py
--rw-r--r--   0        0        0     2708 2024-03-31 14:56:25.457614 picachain-0.1.2/picachain/retriever/image_retriever.py
--rw-r--r--   0        0        0      272 2024-03-31 14:40:10.519412 picachain-0.1.2/picachain/retriever/retriever.py
--rw-r--r--   0        0        0        0 2024-03-27 17:23:26.446103 picachain-0.1.2/picachain/search/__init__.py
--rw-r--r--   0        0        0      791 2024-03-31 14:54:19.198742 picachain-0.1.2/picachain/search/image_search.py
--rw-r--r--   0        0        0      457 2024-03-31 08:34:46.916761 picachain-0.1.2/picachain/utils/image_util.py
--rw-r--r--   0        0        0      528 2024-04-01 08:07:17.157308 picachain-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 picachain-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-27 18:13:06.705397 picachain-0.1.20/LICENSE
+-rw-r--r--   0        0        0     1925 2024-04-01 09:41:20.443801 picachain-0.1.20/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 17:21:07.953194 picachain-0.1.20/picachain/__init__.py
+-rw-r--r--   0        0        0      230 2024-03-29 17:34:59.884284 picachain-0.1.20/picachain/datastore/__init__.py
+-rw-r--r--   0        0        0     3078 2024-03-31 15:09:02.564382 picachain-0.1.20/picachain/datastore/chroma.py
+-rw-r--r--   0        0        0      732 2024-03-31 09:17:25.271088 picachain-0.1.20/picachain/datastore/datastore.py
+-rw-r--r--   0        0        0     2874 2024-03-28 07:11:51.897969 picachain-0.1.20/picachain/datastore/pinecone.py
+-rw-r--r--   0        0        0      166 2024-03-29 17:30:15.708875 picachain-0.1.20/picachain/embedding/__init__.py
+-rw-r--r--   0        0        0     1836 2024-03-30 17:40:26.622816 picachain-0.1.20/picachain/embedding/clip_embedding.py
+-rw-r--r--   0        0        0      570 2024-03-29 13:24:42.213948 picachain-0.1.20/picachain/embedding/embedding.py
+-rw-r--r--   0        0        0      169 2024-03-31 14:45:13.557494 picachain-0.1.20/picachain/retriever/__init__.py
+-rw-r--r--   0        0        0     2708 2024-03-31 14:56:25.457614 picachain-0.1.20/picachain/retriever/image_retriever.py
+-rw-r--r--   0        0        0      272 2024-03-31 14:40:10.519412 picachain-0.1.20/picachain/retriever/retriever.py
+-rw-r--r--   0        0        0       81 2024-04-01 09:22:48.252396 picachain-0.1.20/picachain/search/__init__.py
+-rw-r--r--   0        0        0      791 2024-03-31 14:54:19.198742 picachain-0.1.20/picachain/search/image_search.py
+-rw-r--r--   0        0        0      457 2024-03-31 08:34:46.916761 picachain-0.1.20/picachain/utils/image_util.py
+-rw-r--r--   0        0        0      773 2024-04-01 09:42:28.124181 picachain-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0     2942 1970-01-01 00:00:00.000000 picachain-0.1.20/PKG-INFO
```

### Comparing `picachain-0.1.2/LICENSE` & `picachain-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/README.md` & `picachain-0.1.20/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div align="center">
-<img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/52945ba9-8b89-40a2-bd8e-faef1d9862c0" height=150></img>
+<img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/3a299c21-6590-4ee1-a3c1-73a92653f21e" height=150></img>
 <h3>⚡️ A Simple ready-to-use Image search engine library</h3>
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 [![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
 
 </div>
@@ -23,15 +23,15 @@
 from PIL import Image
 import matplotlib.pyplot as plt
 
 # import from picachain
 from picachain.datastore import ChromaStore
 from picachain.embedding import ClipEmbedding
 from picachain.retriever import ImageRetriever
-from picachain.search.image_search import ImageSearch
+from picachain.search import ImageSearch
 ```
 
 ```python
 img = Image.open("image-path") # query image
 images = [Image.open(os.path.join("images-path", image)) for image in os.listdir("images-path")] # image collection
 ```
```

### Comparing `picachain-0.1.2/picachain/datastore/chroma.py` & `picachain-0.1.20/picachain/datastore/chroma.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/datastore/datastore.py` & `picachain-0.1.20/picachain/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/datastore/pinecone.py` & `picachain-0.1.20/picachain/datastore/pinecone.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/embedding/clip_embedding.py` & `picachain-0.1.20/picachain/embedding/clip_embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/embedding/embedding.py` & `picachain-0.1.20/picachain/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/retriever/image_retriever.py` & `picachain-0.1.20/picachain/retriever/image_retriever.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/picachain/search/image_search.py` & `picachain-0.1.20/picachain/search/image_search.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.2/PKG-INFO` & `picachain-0.1.20/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: picachain
-Version: 0.1.2
+Version: 0.1.20
 Summary: Simple image search engine package.
+Home-page: https://github.com/d1pankarmedhi/picachain
 License: MIT
+Keywords: python,search-engine,chromadb,image,search,packages,poetry,python-packages
 Author: d1pankarmedhi
 Author-email: dipankarmedhi11@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,18 +16,19 @@
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pinecone-client (>=3.2.1,<4.0.0)
 Requires-Dist: pysqlite3-binary (>=0.5.2.post3,<0.6.0)
 Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.39.1,<5.0.0)
+Project-URL: Repository, https://github.com/d1pankarmedhi/picachain
 Description-Content-Type: text/markdown
 
 <div align="center">
-<img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/52945ba9-8b89-40a2-bd8e-faef1d9862c0" height=150></img>
+<img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/3a299c21-6590-4ee1-a3c1-73a92653f21e" height=150></img>
 <h3>⚡️ A Simple ready-to-use Image search engine library</h3>
 
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 
 [![PyPi license](https://badgen.net/pypi/license/pip/)](https://pypi.org/project/pip/) [![PyPI version fury.io](https://badge.fury.io/py/picachain.svg)](https://pypi.python.org/pypi/picachain/)
 
 </div>
@@ -45,15 +48,15 @@
 from PIL import Image
 import matplotlib.pyplot as plt
 
 # import from picachain
 from picachain.datastore import ChromaStore
 from picachain.embedding import ClipEmbedding
 from picachain.retriever import ImageRetriever
-from picachain.search.image_search import ImageSearch
+from picachain.search import ImageSearch
 ```
 
 ```python
 img = Image.open("image-path") # query image
 images = [Image.open(os.path.join("images-path", image)) for image in os.listdir("images-path")] # image collection
 ```
```

