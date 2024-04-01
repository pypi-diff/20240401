# Comparing `tmp/langchain_ai21-0.1.2.tar.gz` & `tmp/langchain_ai21-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ai21-0.1.2.tar", max compression
+gzip compressed data, was "langchain_ai21-0.1.3.tar", max compression
```

## Comparing `langchain_ai21-0.1.2.tar` & `langchain_ai21-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/LICENSE
--rw-r--r--   0        0        0     2524 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/README.md
--rw-r--r--   0        0        0      306 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/__init__.py
--rw-r--r--   0        0        0     1475 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/ai21_base.py
--rw-r--r--   0        0        0     6208 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/chat_models.py
--rw-r--r--   0        0        0     3067 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/contextual_answers.py
--rw-r--r--   0        0        0     2255 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/embeddings.py
--rw-r--r--   0        0        0     5238 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/llms.py
--rw-r--r--   0        0        0        0 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/langchain_ai21/py.typed
--rw-r--r--   0        0        0     2331 2024-03-19 02:47:37.974400 langchain_ai21-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 langchain_ai21-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3146 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/README.md
+-rw-r--r--   0        0        0      413 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/langchain_ai21/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-01 17:48:43.198428 langchain_ai21-0.1.3/langchain_ai21/ai21_base.py
+-rw-r--r--   0        0        0     6208 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/chat_models.py
+-rw-r--r--   0        0        0     3067 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/contextual_answers.py
+-rw-r--r--   0        0        0     2255 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/embeddings.py
+-rw-r--r--   0        0        0     5238 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/llms.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/py.typed
+-rw-r--r--   0        0        0     5121 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/langchain_ai21/semantic_text_splitter.py
+-rw-r--r--   0        0        0     2367 2024-04-01 17:48:43.202427 langchain_ai21-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 langchain_ai21-0.1.3/PKG-INFO
```

### Comparing `langchain_ai21-0.1.2/LICENSE` & `langchain_ai21-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/README.md` & `langchain_ai21-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -98,8 +98,24 @@
 
 tsm = AI21ContextualAnswers()
 chain = tsm | StrOutputParser()
 
 response = chain.invoke(
     {"context": "Your context", "question": "Your question"},
 )
+```
+
+## Text Splitters
+
+### Semantic Text Splitter
+
+You can use AI21's semantic text splitter to split a text into segments.
+Instead of merely using punctuation and newlines to divide the text, it identifies distinct topics that will work well together and will form a coherent piece of text.
+
+For a list for examples, see [this page](https://github.com/langchain-ai/langchain/blob/master/docs/docs/modules/data_connection/document_transformers/semantic_text_splitter.ipynb).
+
+```python
+from langchain_ai21 import AI21SemanticTextSplitter
+
+splitter = AI21SemanticTextSplitter()
+response = splitter.split_text("Your text")
 ```
```

### Comparing `langchain_ai21-0.1.2/langchain_ai21/ai21_base.py` & `langchain_ai21-0.1.3/langchain_ai21/ai21_base.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/langchain_ai21/chat_models.py` & `langchain_ai21-0.1.3/langchain_ai21/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/langchain_ai21/contextual_answers.py` & `langchain_ai21-0.1.3/langchain_ai21/contextual_answers.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/langchain_ai21/embeddings.py` & `langchain_ai21-0.1.3/langchain_ai21/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/langchain_ai21/llms.py` & `langchain_ai21-0.1.3/langchain_ai21/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_ai21-0.1.2/pyproject.toml` & `langchain_ai21-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "langchain-ai21"
-version = "0.1.2"
+version = "0.1.3"
 description = "An integration package connecting AI21 and LangChain"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.22"
+langchain-core = "^0.1.28"
+langchain-text-splitters = "^0.0.1"
 ai21 = "^2.1.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_ai21-0.1.2/PKG-INFO` & `langchain_ai21-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: langchain-ai21
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration package connecting AI21 and LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ai21 (>=2.1.2,<3.0.0)
-Requires-Dist: langchain-core (>=0.1.22,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.28,<0.2.0)
+Requires-Dist: langchain-text-splitters (>=0.0.1,<0.0.2)
 Description-Content-Type: text/markdown
 
 # langchain-ai21
 
 This package contains the LangChain integrations for [AI21](https://docs.ai21.com/) through their [AI21](https://pypi.org/project/ai21/) SDK.
 
 ## Installation and Setup
@@ -113,7 +114,23 @@
 tsm = AI21ContextualAnswers()
 chain = tsm | StrOutputParser()
 
 response = chain.invoke(
     {"context": "Your context", "question": "Your question"},
 )
 ```
+
+## Text Splitters
+
+### Semantic Text Splitter
+
+You can use AI21's semantic text splitter to split a text into segments.
+Instead of merely using punctuation and newlines to divide the text, it identifies distinct topics that will work well together and will form a coherent piece of text.
+
+For a list for examples, see [this page](https://github.com/langchain-ai/langchain/blob/master/docs/docs/modules/data_connection/document_transformers/semantic_text_splitter.ipynb).
+
+```python
+from langchain_ai21 import AI21SemanticTextSplitter
+
+splitter = AI21SemanticTextSplitter()
+response = splitter.split_text("Your text")
+```
```

