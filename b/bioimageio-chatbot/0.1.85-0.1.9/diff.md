# Comparing `tmp/bioimageio-chatbot-0.1.85.tar.gz` & `tmp/bioimageio-chatbot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio-chatbot-0.1.85.tar", last modified: Mon Apr  1 21:37:11 2024, max compression
+gzip compressed data, was "bioimageio-chatbot-0.1.9.tar", last modified: Sun Oct 22 12:28:07 2023, max compression
```

## Comparing `bioimageio-chatbot-0.1.85.tar` & `bioimageio-chatbot-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.392688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.388688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/apps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.392688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/apps/assistants/
--rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/apps/assistants/code-interpreter.html
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/apps/assistants/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.396688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/bia_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/biii_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/docs_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/image_sc_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.396688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/web_search_extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/web_search_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/web_search_extension/langchain_websearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/chatbot_extensions/web_search_extension/llm_web_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/gpts_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/jsonschema_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/knowledge_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/bioimage-model-zoo-extension.imjoy.html
--rw-r--r--   0 runner    (1001) docker     (127)  1130918 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/bridget-bmz.png
--rw-r--r--   0 runner    (1001) docker     (127)    66236 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)   271923 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/melman-bmz.png
--rw-r--r--   0 runner    (1001) docker     (127)  1378976 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/nina-bmz.png
--rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/pyodide-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/static/worker-manager.js
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-01 21:36:59.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15242 2024-04-01 21:37:11.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-01 21:37:11.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:37:11.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-01 21:37:11.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-01 21:37:11.000000 bioimageio-chatbot-0.1.85/bioimageio_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 21:37:00.000000 bioimageio-chatbot-0.1.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:37:11.400688 bioimageio-chatbot-0.1.85/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-01 21:37:00.000000 bioimageio-chatbot-0.1.85/tests/test_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-01 21:37:00.000000 bioimageio-chatbot-0.1.85/tests/test_chatbot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-04-01 21:37:00.000000 bioimageio-chatbot-0.1.85/tests/test_eval_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-01 21:37:00.000000 bioimageio-chatbot-0.1.85/tests/test_knowledge_base.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-22 12:28:07.864681 bioimageio-chatbot-0.1.9/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1068 2023-10-20 12:10:32.000000 bioimageio-chatbot-0.1.9/LICENSE
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       35 2023-10-22 01:07:09.000000 bioimageio-chatbot-0.1.9/MANIFEST.in
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     9087 2023-10-22 12:28:07.864399 bioimageio-chatbot-0.1.9/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     8767 2023-10-22 11:25:47.000000 bioimageio-chatbot-0.1.9/README.md
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-22 12:28:07.862238 bioimageio-chatbot-0.1.9/bioimageio_chatbot/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        0 2023-10-21 20:17:21.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/__init__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     2900 2023-10-22 01:30:49.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/__main__.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    12642 2023-10-22 12:15:34.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/chatbot.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     9889 2023-10-22 00:21:40.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/knowledge_base.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-22 12:28:07.863405 bioimageio-chatbot-0.1.9/bioimageio_chatbot/static/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)    13933 2023-10-22 12:27:38.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/static/index.html
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1127 2023-10-22 00:26:12.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot/utils.py
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-22 12:28:07.863259 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     9087 2023-10-22 12:28:07.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      498 2023-10-22 12:28:07.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)        1 2023-10-22 12:28:07.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       50 2023-10-22 12:28:07.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/requires.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       19 2023-10-22 12:28:07.000000 bioimageio-chatbot-0.1.9/bioimageio_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      542 2023-10-22 12:02:01.000000 bioimageio-chatbot-0.1.9/pyproject.toml
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)       38 2023-10-22 12:28:07.864754 bioimageio-chatbot-0.1.9/setup.cfg
+drwxr-xr-x   0 wei.ouyang   (501) staff       (20)        0 2023-10-22 12:28:07.863938 bioimageio-chatbot-0.1.9/tests/
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)     1920 2023-10-21 20:17:21.000000 bioimageio-chatbot-0.1.9/tests/test_chatbot.py
+-rw-r--r--   0 wei.ouyang   (501) staff       (20)      456 2023-10-21 20:17:21.000000 bioimageio-chatbot-0.1.9/tests/test_knowledge_base.py
```

### Comparing `bioimageio-chatbot-0.1.85/LICENSE` & `bioimageio-chatbot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio-chatbot-0.1.85/bioimageio_chatbot/knowledge_base.py` & `bioimageio-chatbot-0.1.9/bioimageio_chatbot/knowledge_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import requests
 import zipfile
 import shutil
 from langchain.text_splitter import CharacterTextSplitter, RecursiveCharacterTextSplitter
-from langchain_community.vectorstores import FAISS
-from langchain_community.document_loaders import TextLoader, PyPDFLoader
-from langchain_openai import OpenAIEmbeddings
+from langchain.vectorstores import FAISS
+from langchain.document_loaders import TextLoader, PyPDFLoader
+from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.docstore.document import Document
 import json
 import pickle
 from bioimageio_chatbot.utils import get_manifest, download_file
 
 KNOWLEDGE_BASE_URL = os.environ.get("BIOIMAGEIO_KNOWLEDGE_BASE_URL", "https://uk1s3.embassy.ebi.ac.uk/public-datasets/bioimageio-knowledge-base")
 
@@ -23,15 +23,15 @@
     
     if not os.path.exists(os.path.join(db_path, f"{collection_name}.pkl")):
         print(f"Downloading {collection_name}.pkl from {KNOWLEDGE_BASE_URL}/{collection_name}.pkl")
         download_file(f"{KNOWLEDGE_BASE_URL}/{collection_name}.pkl", os.path.join(db_path, f"{collection_name}.pkl"))
 
     # Load from vector store
     embeddings = OpenAIEmbeddings()
-    docs_store = FAISS.load_local(index_name=collection_name, folder_path=db_path, embeddings=embeddings, allow_dangerous_deserialization=True)
+    docs_store = FAISS.load_local(index_name=collection_name, folder_path=db_path, embeddings=embeddings)
     return docs_store
 
 
 def load_knowledge_base(db_path):
     collections = get_manifest()['collections']
     docs_store_dict = {}
     
@@ -134,55 +134,50 @@
             zip_ref.extractall(result_folder)
         
         # Clean up - remove the downloaded ZIP file
         os.remove(zip_file_path)
         print(f"Downloaded and unzipped {url} to {result_folder}")
     elif filename.endswith(".pdf"):
         result_folder = os.path.join(target_directory, ".".join(filename.split(".")[:-1]))
-        os.makedirs(result_folder, exist_ok=True)
         print(f"Downloading {url} to {result_folder}")
         pdf_file_path = os.path.join(result_folder, filename)
         download_file(url, pdf_file_path)
         print(f"Downloaded {url} to {result_folder}")
+        
     else:
         raise Exception("Unsupported file format")
     
     if len(os.listdir(result_folder)) == 0:
         raise Exception("Downloaded folder is empty")
     elif len(os.listdir(result_folder)) == 1:
         # strip the folder name of the unzipped repo
-        r_dir = os.path.join(result_folder, os.listdir(result_folder)[0])
-        if os.path.isdir(r_dir):
-            return r_dir
+        return os.path.join(result_folder, os.listdir(result_folder)[0])
     # get the folder name of the unzipped repo
     return result_folder
 
 
 def create_vector_knowledge_base(output_dir=None, collections=None):
     """Create a vector knowledge base from the downloaded documents"""
     if output_dir is None:
-        output_dir = os.environ.get("BIOIMAGEIO_KNOWLEDGE_BASE_PATH", "./bioimageio-knowledge-base")
+        output_dir = os.environ.get("BIOIMAGEIO_KNOWLEDGE_BASE", "./bioimageio-knowledge-base")
     os.makedirs(output_dir, exist_ok=True)
     
     if not collections:
         collections = get_manifest()['collections']
     
     embeddings = OpenAIEmbeddings()
     for collection in collections:
-        if collection.get("format") and collection.get("format").startswith("custom:"):
-            print(f"Skipping {collection['id']} because it is a custom collection.")
-            continue
-        url = collection['source']
+        url = collection['url']
         cached_docs_file = os.path.join(output_dir, collection['id'] + "-docs.pickle")
         if os.path.exists(cached_docs_file):
             with open(cached_docs_file, "rb") as f:
                 documents = pickle.load(f)
         else:    
             docs_dir = download_docs("./data", url)
-            documents = parse_docs(os.path.join(docs_dir, collection.get('directory', '')),md_separator=collection.get('md_separator', None), pdf_separator=collection.get('pdf_separator', None), chunk_size=collection.get('chunk_size', 1000), chunk_overlap=collection.get('chunk_overlap', 10))
+            documents = parse_docs(os.path.join(docs_dir, collection.get('directory', '')))
         if len(documents) > 10000:
             print(f"Waring: {len(documents)} documents found in {url}.")
         # save the vector db to output_dir
         print(f"Creating embeddings (#documents={len(documents)}))")
 
         # Choose an appropriate batch size
         batch_size = 1000
```

