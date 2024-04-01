# Comparing `tmp/analysta_index-0.2.8.tar.gz` & `tmp/analysta_index-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysta_index-0.2.8.tar", last modified: Tue Mar  5 08:05:17 2024, max compression
+gzip compressed data, was "analysta_index-0.2.9.tar", last modified: Tue Mar  5 11:19:46 2024, max compression
```

## Comparing `analysta_index-0.2.8.tar` & `analysta_index-0.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.875584 analysta_index-0.2.8/
--rw-r--r--   0 arozumenko   (501) staff       (20)    11349 2024-01-22 11:37:26.000000 analysta_index-0.2.8/LICENSE
--rw-r--r--   0 arozumenko   (501) staff       (20)     1634 2024-03-05 08:05:17.875170 analysta_index-0.2.8/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)       75 2024-01-22 11:36:59.000000 analysta_index-0.2.8/README.md
--rw-r--r--   0 arozumenko   (501) staff       (20)      707 2024-03-04 17:14:22.000000 analysta_index-0.2.8/pyproject.toml
--rw-r--r--   0 arozumenko   (501) staff       (20)      571 2024-02-18 12:26:44.000000 analysta_index-0.2.8/requirements.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-03-05 08:05:17.875698 analysta_index-0.2.8/setup.cfg
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.865320 analysta_index-0.2.8/src/
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.866579 analysta_index-0.2.8/src/analysta_index/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.870247 analysta_index-0.2.8/src/analysta_index/document_loaders/
--rw-r--r--   0 arozumenko   (501) staff       (20)     1910 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaCSVLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      689 2024-02-27 19:15:13.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaConfluenceLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     6198 2024-03-04 17:14:22.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaDirectoryLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1469 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaExcelLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2557 2024-03-01 09:31:53.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaGitRepoLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3501 2024-03-04 11:25:52.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaTableLoader.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2330 2024-02-27 19:15:13.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/constants.py
--rw-r--r--   0 arozumenko   (501) staff       (20)      875 2024-02-27 19:15:13.000000 analysta_index-0.2.8/src/analysta_index/document_loaders/utils.py
--rw-r--r--   0 arozumenko   (501) staff       (20)    20463 2024-03-05 08:04:47.000000 analysta_index-0.2.8/src/analysta_index/indexer.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.872287 analysta_index-0.2.8/src/analysta_index/interfaces/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/interfaces/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2137 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/interfaces/kwextractor.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     5451 2024-03-05 07:17:28.000000 analysta_index-0.2.8/src/analysta_index/interfaces/llm_processor.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2862 2024-02-29 14:24:10.000000 analysta_index-0.2.8/src/analysta_index/interfaces/loaders.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3472 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/interfaces/splitters.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.872607 analysta_index-0.2.8/src/analysta_index/llms/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/llms/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     4088 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/llms/analysta.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.873679 analysta_index-0.2.8/src/analysta_index/retrievers/
--rw-r--r--   0 arozumenko   (501) staff       (20)     5011 2024-03-05 07:17:28.000000 analysta_index-0.2.8/src/analysta_index/retrievers/AnalystaRetriever.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3016 2024-03-04 11:25:52.000000 analysta_index-0.2.8/src/analysta_index/retrievers/SimpleRetriever.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     1809 2024-02-29 14:24:10.000000 analysta_index-0.2.8/src/analysta_index/retrievers/VectorstoreRetriever.py
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/retrievers/__init__.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.874601 analysta_index-0.2.8/src/analysta_index/tools/
--rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/tools/__init__.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     9116 2024-01-22 11:37:26.000000 analysta_index-0.2.8/src/analysta_index/tools/git.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     2785 2024-02-27 19:15:13.000000 analysta_index-0.2.8/src/analysta_index/tools/log.py
--rw-r--r--   0 arozumenko   (501) staff       (20)       88 2024-02-08 08:49:52.000000 analysta_index-0.2.8/src/analysta_index/tools/state.py
--rw-r--r--   0 arozumenko   (501) staff       (20)     3557 2024-03-05 08:05:11.000000 analysta_index-0.2.8/src/analysta_index/tools/utils.py
-drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 08:05:17.874781 analysta_index-0.2.8/src/analysta_index.egg-info/
--rw-r--r--   0 arozumenko   (501) staff       (20)     1634 2024-03-05 08:05:17.000000 analysta_index-0.2.8/src/analysta_index.egg-info/PKG-INFO
--rw-r--r--   0 arozumenko   (501) staff       (20)     1479 2024-03-05 08:05:17.000000 analysta_index-0.2.8/src/analysta_index.egg-info/SOURCES.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-03-05 08:05:17.000000 analysta_index-0.2.8/src/analysta_index.egg-info/dependency_links.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)      571 2024-03-05 08:05:17.000000 analysta_index-0.2.8/src/analysta_index.egg-info/requires.txt
--rw-r--r--   0 arozumenko   (501) staff       (20)       15 2024-03-05 08:05:17.000000 analysta_index-0.2.8/src/analysta_index.egg-info/top_level.txt
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.766555 analysta_index-0.2.9/
+-rw-r--r--   0 arozumenko   (501) staff       (20)    11349 2024-01-22 11:37:26.000000 analysta_index-0.2.9/LICENSE
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1634 2024-03-05 11:19:46.766330 analysta_index-0.2.9/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)       75 2024-01-22 11:36:59.000000 analysta_index-0.2.9/README.md
+-rw-r--r--   0 arozumenko   (501) staff       (20)      707 2024-03-05 11:19:31.000000 analysta_index-0.2.9/pyproject.toml
+-rw-r--r--   0 arozumenko   (501) staff       (20)      571 2024-02-18 12:26:44.000000 analysta_index-0.2.9/requirements.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       38 2024-03-05 11:19:46.766610 analysta_index-0.2.9/setup.cfg
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.755194 analysta_index-0.2.9/src/
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.756585 analysta_index-0.2.9/src/analysta_index/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.759695 analysta_index-0.2.9/src/analysta_index/document_loaders/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1910 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaCSVLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      689 2024-02-27 19:15:13.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaConfluenceLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     6198 2024-03-04 17:14:22.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaDirectoryLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1469 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaExcelLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2557 2024-03-01 09:31:53.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaGitRepoLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3501 2024-03-04 11:25:52.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaTableLoader.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2330 2024-02-27 19:15:13.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/constants.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)      875 2024-02-27 19:15:13.000000 analysta_index-0.2.9/src/analysta_index/document_loaders/utils.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)    20580 2024-03-05 11:19:14.000000 analysta_index-0.2.9/src/analysta_index/indexer.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.761674 analysta_index-0.2.9/src/analysta_index/interfaces/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/interfaces/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2137 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/interfaces/kwextractor.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     5451 2024-03-05 07:17:28.000000 analysta_index-0.2.9/src/analysta_index/interfaces/llm_processor.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2862 2024-02-29 14:24:10.000000 analysta_index-0.2.9/src/analysta_index/interfaces/loaders.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3472 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/interfaces/splitters.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.762023 analysta_index-0.2.9/src/analysta_index/llms/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/llms/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     4088 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/llms/analysta.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.764410 analysta_index-0.2.9/src/analysta_index/retrievers/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     5011 2024-03-05 07:17:28.000000 analysta_index-0.2.9/src/analysta_index/retrievers/AnalystaRetriever.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3016 2024-03-04 11:25:52.000000 analysta_index-0.2.9/src/analysta_index/retrievers/SimpleRetriever.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1809 2024-02-29 14:24:10.000000 analysta_index-0.2.9/src/analysta_index/retrievers/VectorstoreRetriever.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/retrievers/__init__.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.765573 analysta_index-0.2.9/src/analysta_index/tools/
+-rw-r--r--   0 arozumenko   (501) staff       (20)        0 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/tools/__init__.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     9116 2024-01-22 11:37:26.000000 analysta_index-0.2.9/src/analysta_index/tools/git.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     2785 2024-02-27 19:15:13.000000 analysta_index-0.2.9/src/analysta_index/tools/log.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)       88 2024-02-08 08:49:52.000000 analysta_index-0.2.9/src/analysta_index/tools/state.py
+-rw-r--r--   0 arozumenko   (501) staff       (20)     3557 2024-03-05 08:08:47.000000 analysta_index-0.2.9/src/analysta_index/tools/utils.py
+drwxr-xr-x   0 arozumenko   (501) staff       (20)        0 2024-03-05 11:19:46.765998 analysta_index-0.2.9/src/analysta_index.egg-info/
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1634 2024-03-05 11:19:46.000000 analysta_index-0.2.9/src/analysta_index.egg-info/PKG-INFO
+-rw-r--r--   0 arozumenko   (501) staff       (20)     1479 2024-03-05 11:19:46.000000 analysta_index-0.2.9/src/analysta_index.egg-info/SOURCES.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)        1 2024-03-05 11:19:46.000000 analysta_index-0.2.9/src/analysta_index.egg-info/dependency_links.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)      571 2024-03-05 11:19:46.000000 analysta_index-0.2.9/src/analysta_index.egg-info/requires.txt
+-rw-r--r--   0 arozumenko   (501) staff       (20)       15 2024-03-05 11:19:46.000000 analysta_index-0.2.9/src/analysta_index.egg-info/top_level.txt
```

### Comparing `analysta_index-0.2.8/LICENSE` & `analysta_index-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/PKG-INFO` & `analysta_index-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysta_index
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension of Langchain loaders, llms and retrievers for Analysta
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://analysta.ai
 Project-URL: Issues, https://github.com/analysta-ai/indexer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `analysta_index-0.2.8/pyproject.toml` & `analysta_index-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "analysta_index"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Artem Rozumenko", email="support@analysta.ai" },
 ]
 description = "Extension of Langchain loaders, llms and retrievers for Analysta"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `analysta_index-0.2.8/requirements.txt` & `analysta_index-0.2.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaCSVLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaCSVLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaConfluenceLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaConfluenceLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaDirectoryLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaDirectoryLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaExcelLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaExcelLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaGitRepoLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaGitRepoLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/AnalystaTableLoader.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/AnalystaTableLoader.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/constants.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/constants.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/document_loaders/utils.py` & `analysta_index-0.2.9/src/analysta_index/document_loaders/utils.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/indexer.py` & `analysta_index-0.2.9/src/analysta_index/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import importlib
 
 from typing import Optional
 
 from langchain_core.documents import Document
 from langchain.schema import HumanMessage
+from operator import le, ge
 from json import dumps, loads
 
 from .interfaces.loaders import loader
 from .interfaces.kwextractor import KWextractor
 from .interfaces.splitters import Splitter
 from .interfaces.llm_processor import get_embeddings, summarize, get_model, get_vectorstore, add_documents, generateResponse
 from .tools.utils import unpack_json, download_nltk, replace_source
@@ -430,22 +431,27 @@
     response_text = ai.invoke(messages).content
     return {
         "response": response_text,
         "references": references
     }
 
 
+func_mapping = {
+    "le": le,
+    "ge": ge,
+}
+
 def deduplicate(
         embedding_model,
         embedding_model_params,
         vectorstore,
         vectorstore_params,
         collection,
         cut_off_score,
-        columns=None,
+        cutoff_func = "le" # or "ge"
 ):
     """ Deduplication """
     embedding = get_embeddings(embedding_model, embedding_model_params)
     vectorstore = get_vectorstore(vectorstore, vectorstore_params, embedding_func=embedding)
     #
     data = vectorstore.get(
         where={"$and": [{"library": collection}, {"type": "data"}]},
@@ -471,15 +477,15 @@
     #
     # Legacy code below
     #
     cosine_scores = util.cos_sim(embeddins_lib['embeddings'], embeddins_lib['embeddings'])
     pairs = []
     for index, scores in enumerate(cosine_scores):
         for jindex, score in enumerate(scores):
-            if score > cutoff and index < jindex:
+            if func_mapping[cutoff_func](score, cutoff) and index < jindex:
                 record = {
                     'score': round(score.item(), 3)
                 }
                 # print(index)
                 # Calculate similarity score based on composite value of selected columns
                 
                 if (isinstance(embeddins_lib["sentences"][index], str)):
```

### Comparing `analysta_index-0.2.8/src/analysta_index/interfaces/kwextractor.py` & `analysta_index-0.2.9/src/analysta_index/interfaces/kwextractor.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/interfaces/llm_processor.py` & `analysta_index-0.2.9/src/analysta_index/interfaces/llm_processor.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/interfaces/loaders.py` & `analysta_index-0.2.9/src/analysta_index/interfaces/loaders.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/interfaces/splitters.py` & `analysta_index-0.2.9/src/analysta_index/interfaces/splitters.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/llms/analysta.py` & `analysta_index-0.2.9/src/analysta_index/llms/analysta.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/retrievers/AnalystaRetriever.py` & `analysta_index-0.2.9/src/analysta_index/retrievers/AnalystaRetriever.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/retrievers/SimpleRetriever.py` & `analysta_index-0.2.9/src/analysta_index/retrievers/SimpleRetriever.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/retrievers/VectorstoreRetriever.py` & `analysta_index-0.2.9/src/analysta_index/retrievers/VectorstoreRetriever.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/tools/git.py` & `analysta_index-0.2.9/src/analysta_index/tools/git.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/tools/log.py` & `analysta_index-0.2.9/src/analysta_index/tools/log.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index/tools/utils.py` & `analysta_index-0.2.9/src/analysta_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index.egg-info/PKG-INFO` & `analysta_index-0.2.9/src/analysta_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysta_index
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension of Langchain loaders, llms and retrievers for Analysta
 Author-email: Artem Rozumenko <support@analysta.ai>
 Project-URL: Homepage, https://analysta.ai
 Project-URL: Issues, https://github.com/analysta-ai/indexer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `analysta_index-0.2.8/src/analysta_index.egg-info/SOURCES.txt` & `analysta_index-0.2.9/src/analysta_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysta_index-0.2.8/src/analysta_index.egg-info/requires.txt` & `analysta_index-0.2.9/src/analysta_index.egg-info/requires.txt`

 * *Files identical despite different names*

