# Comparing `tmp/composio_langchain-0.1.8.tar.gz` & `tmp/composio_langchain-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.8.tar", last modified: Tue Mar 19 19:45:53 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.9.tar", last modified: Tue Mar 19 19:57:50 2024, max compression
```

## Comparing `composio_langchain-0.1.8.tar` & `composio_langchain-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:53.242269 composio_langchain-0.1.8/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.8/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      872 2024-03-19 19:45:53.242050 composio_langchain-0.1.8/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      128 2024-03-16 10:30:52.000000 composio_langchain-0.1.8/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:53.240880 composio_langchain-0.1.8/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)       47 2024-03-16 10:01:33.000000 composio_langchain-0.1.8/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1150 2024-03-19 19:39:10.000000 composio_langchain-0.1.8/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.8/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:45:53.241821 composio_langchain-0.1.8/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      872 2024-03-19 19:45:53.000000 composio_langchain-0.1.8/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-03-19 19:45:53.000000 composio_langchain-0.1.8/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-03-19 19:45:53.000000 composio_langchain-0.1.8/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      151 2024-03-19 19:45:53.000000 composio_langchain-0.1.8/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-03-19 19:45:53.000000 composio_langchain-0.1.8/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      457 2024-03-19 19:45:37.000000 composio_langchain-0.1.8/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-03-19 19:45:53.242316 composio_langchain-0.1.8/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      856 2024-03-19 19:45:29.000000 composio_langchain-0.1.8/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:57:50.442612 composio_langchain-0.1.9/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.9/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      872 2024-03-19 19:57:50.442382 composio_langchain-0.1.9/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      128 2024-03-16 10:30:52.000000 composio_langchain-0.1.9/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:57:50.441487 composio_langchain-0.1.9/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       47 2024-03-16 10:01:33.000000 composio_langchain-0.1.9/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1150 2024-03-19 19:39:10.000000 composio_langchain-0.1.9/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.9/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-03-19 19:57:50.442185 composio_langchain-0.1.9/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      872 2024-03-19 19:57:50.000000 composio_langchain-0.1.9/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-03-19 19:57:50.000000 composio_langchain-0.1.9/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-03-19 19:57:50.000000 composio_langchain-0.1.9/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      151 2024-03-19 19:57:50.000000 composio_langchain-0.1.9/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-03-19 19:57:50.000000 composio_langchain-0.1.9/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      457 2024-03-19 19:57:41.000000 composio_langchain-0.1.9/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-03-19 19:57:50.442660 composio_langchain-0.1.9/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      856 2024-03-19 19:57:37.000000 composio_langchain-0.1.9/setup.py
```

### Comparing `composio_langchain-0.1.8/PKG-INFO` & `composio_langchain-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.8
+Version: 0.1.9
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,14 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain===0.1.0
 Requires-Dist: langchain-openai===0.0.2.post1
 Requires-Dist: langchainhub==0.1.15
 Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.8
+Requires-Dist: composio_core===0.1.9
 
 Composio <> LangChain
 Use Composio to get an array of tools with your LangChain agent.
 
 # Usage
 Inside your LangChain codebase:
```

### Comparing `composio_langchain-0.1.8/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.9/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.8/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.9/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.8/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.9/composio_langchain.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.8
+Version: 0.1.9
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,14 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain===0.1.0
 Requires-Dist: langchain-openai===0.0.2.post1
 Requires-Dist: langchainhub==0.1.15
 Requires-Dist: pydantic===2.6.4
-Requires-Dist: composio_core===0.1.8
+Requires-Dist: composio_core===0.1.9
 
 Composio <> LangChain
 Use Composio to get an array of tools with your LangChain agent.
 
 # Usage
 Inside your LangChain codebase:
```

### Comparing `composio_langchain-0.1.8/setup.py` & `composio_langchain-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def resolve_paths(*paths):
     return os.path.join(*paths)
 
 readme_path = resolve_paths(get_current_dir(), 'README.md')
 
 setup(
     name = 'composio_langchain',
-    version = '0.1.8',
+    version = '0.1.9',
     author = 'Karan',
     author_email = 'karan@composio.dev',
     description = 'Use Composio to get an array of tools with your LangChain agent.',
     long_description = open(readme_path).read(),
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/SamparkAI/composio_sdk',
     classifiers = [
```

