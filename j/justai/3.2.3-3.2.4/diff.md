# Comparing `tmp/justai-3.2.3.tar.gz` & `tmp/justai-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.2.3.tar", last modified: Mon Apr  1 09:16:33 2024, max compression
+gzip compressed data, was "justai-3.2.4.tar", last modified: Mon Apr  1 20:12:20 2024, max compression
```

## Comparing `justai-3.2.3.tar` & `justai-3.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.432363 justai-3.2.3/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.3/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.3/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-01 09:16:33.432005 justai-3.2.3/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-01 09:16:30.000000 justai-3.2.3/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.420510 justai-3.2.3/justai/
--rw-r--r--   0 hp         (501) staff       (20)      300 2024-02-12 20:04:37.000000 justai-3.2.3/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.423145 justai-3.2.3/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.3/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.3/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.3/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.424260 justai-3.2.3/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.3/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.3/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.3/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.426340 justai-3.2.3/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2291 2024-03-21 09:29:15.000000 justai-3.2.3/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.3/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.3/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.3/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5807 2024-03-21 09:14:50.000000 justai-3.2.3/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.428502 justai-3.2.3/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.3/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3618 2024-03-31 16:29:44.000000 justai-3.2.3/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.3/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3189 2024-03-31 21:31:39.000000 justai-3.2.3/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.3/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.430222 justai-3.2.3/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.3/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.3/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1551 2024-03-30 11:43:22.000000 justai-3.2.3/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    14079 2024-04-01 09:02:59.000000 justai-3.2.3/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.3/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 09:16:33.430947 justai-3.2.3/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-01 09:16:33.000000 justai-3.2.3/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-01 09:16:33.000000 justai-3.2.3/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-01 09:16:33.000000 justai-3.2.3/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-01 09:16:33.000000 justai-3.2.3/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-01 09:16:33.000000 justai-3.2.3/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-01 09:16:30.000000 justai-3.2.3/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-01 09:16:33.432439 justai-3.2.3/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.783529 justai-3.2.4/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.4/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.4/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-01 20:12:20.783166 justai-3.2.4/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-01 20:12:18.000000 justai-3.2.4/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.773166 justai-3.2.4/justai/
+-rw-r--r--   0 hp         (501) staff       (20)       37 2024-04-01 20:12:06.000000 justai-3.2.4/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.775137 justai-3.2.4/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.4/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.4/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.4/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.776198 justai-3.2.4/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.4/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.4/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.4/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.778366 justai-3.2.4/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2291 2024-03-21 09:29:15.000000 justai-3.2.4/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.4/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.4/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.4/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5807 2024-03-21 09:14:50.000000 justai-3.2.4/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.780046 justai-3.2.4/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.4/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3618 2024-03-31 16:29:44.000000 justai-3.2.4/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.4/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3189 2024-03-31 21:31:39.000000 justai-3.2.4/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.4/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.781726 justai-3.2.4/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.4/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.4/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1551 2024-03-30 11:43:22.000000 justai-3.2.4/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    14079 2024-04-01 09:02:59.000000 justai-3.2.4/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.4/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-01 20:12:20.782315 justai-3.2.4/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-01 20:12:20.000000 justai-3.2.4/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-01 20:12:20.000000 justai-3.2.4/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-01 20:12:20.000000 justai-3.2.4/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-01 20:12:20.000000 justai-3.2.4/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-01 20:12:20.000000 justai-3.2.4/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-01 20:12:18.000000 justai-3.2.4/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-01 20:12:20.783608 justai-3.2.4/setup.cfg
```

### Comparing `justai-3.2.3/LICENSE` & `justai-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/PKG-INFO` & `justai-3.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.3
+Version: 3.2.4
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.3
+Current version: 3.2.4
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.3/README.md` & `justai-3.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.3
+Current version: 3.2.4
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.3/justai/agent/agent.py` & `justai-3.2.4/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/agent/message.py` & `justai-3.2.4/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/interactive/commands.py` & `justai-3.2.4/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/interactive/repl.py` & `justai-3.2.4/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/models/anthropic_models.py` & `justai-3.2.4/justai/models/anthropic_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/models/gguf_models.py` & `justai-3.2.4/justai/models/gguf_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/models/model.py` & `justai-3.2.4/justai/models/model.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/models/modelfactory.py` & `justai-3.2.4/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/models/openai_models.py` & `justai-3.2.4/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/tools/cache.py` & `justai-3.2.4/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/tools/display.py` & `justai-3.2.4/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/tools/log.py` & `justai-3.2.4/justai/tools/log.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/tools/prompts.py` & `justai-3.2.4/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/translator/languages.py` & `justai-3.2.4/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/translator/prompts.toml` & `justai-3.2.4/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/translator/translator.py` & `justai-3.2.4/justai/translator/translator.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai/translator/xliff.py` & `justai-3.2.4/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/justai.egg-info/PKG-INFO` & `justai-3.2.4/justai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.3
+Version: 3.2.4
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -53,15 +53,15 @@
 Requires-Dist: nox; extra == "dev"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.3
+Current version: 3.2.4
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.3/justai.egg-info/SOURCES.txt` & `justai-3.2.4/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.2.3/pyproject.toml` & `justai-3.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.2.3"
+version = "3.2.4"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

