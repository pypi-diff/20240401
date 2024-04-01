# Comparing `tmp/lastmile-eval-0.0.4.tar.gz` & `tmp/lastmile-eval-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile-eval-0.0.4.tar", last modified: Mon Apr  1 17:37:48 2024, max compression
+gzip compressed data, was "lastmile-eval-0.0.5.tar", last modified: Mon Apr  1 20:49:49 2024, max compression
```

## Comparing `lastmile-eval-0.0.4.tar` & `lastmile-eval-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.715819 lastmile-eval-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.715819 lastmile-eval-0.0.4/src/lastmile_eval/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/rag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval/text/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/metrics_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/openai_batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_custom_llm_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_default_text_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_rag_scores_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/examples/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/examples/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/rag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/src/lastmile_eval/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/metrics_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/openai_batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_custom_llm_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_default_text_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_rag_scores_e2e.py
```

### Comparing `lastmile-eval-0.0.4/LICENSE` & `lastmile-eval-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/PKG-INFO` & `lastmile-eval-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.4
+Version: 0.0.5
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -12,36 +12,35 @@
 License-File: LICENSE
 Requires-Dist: dataclasses
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 Requires-Dist: rouge_score
 Requires-Dist: nltk
 Requires-Dist: openai>=1.0.0
+Requires-Dist: anthropic
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: arize-phoenix-evals==0.5.0
 Requires-Dist: pandas==2.1.2
 Requires-Dist: instructor
 
 # LastMile AI Eval
 
 Library of tools to evaluate your RAG system.
 
 ## Setup
 
 1. Get a LastMile API token (see section below)
 2. Install this library: `pip install lastmile-eval`
-3. Gather your data that needs evaluation.
-4. See examples/ folder for API usage.
+3. Gather your data that needs evaluation
+4. See the `examples/` folder for API usage
 
 ## LastMile API token
 
 To get a LastMile AI token, please go to the [LastMile token's webpage](https://lastmileai.dev/settings?page=tokens).
 You can create an account with Google or Github and then click the "Create new token" in the "API Tokens" section. Once a token is created, be sure to save it somewhere since you won't be able to see the value of it from the website again (though you can create a new one if that happens).
 
-**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead.
-See examples/ for how to do this.
-
+**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead. See the `examples/` folder for how to do this.
 
 ## LLM Provider Tokens (`.env` file)
 
 In order to use LLM-based evaluators, add your other API tokens to your .env file.
 Example: `OPENAI_API_KEY=<TOKEN_HERE>`
```

### Comparing `lastmile-eval-0.0.4/README.md` & `lastmile-eval-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 Library of tools to evaluate your RAG system.
 
 ## Setup
 
 1. Get a LastMile API token (see section below)
 2. Install this library: `pip install lastmile-eval`
-3. Gather your data that needs evaluation.
-4. See examples/ folder for API usage.
+3. Gather your data that needs evaluation
+4. See the `examples/` folder for API usage
 
 ## LastMile API token
 
 To get a LastMile AI token, please go to the [LastMile token's webpage](https://lastmileai.dev/settings?page=tokens).
 You can create an account with Google or Github and then click the "Create new token" in the "API Tokens" section. Once a token is created, be sure to save it somewhere since you won't be able to see the value of it from the website again (though you can create a new one if that happens).
 
-**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead.
-See examples/ for how to do this.
-
+**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead. See the `examples/` folder for how to do this.
 
 ## LLM Provider Tokens (`.env` file)
 
 In order to use LLM-based evaluators, add your other API tokens to your .env file.
-Example: `OPENAI_API_KEY=<TOKEN_HERE>`
+Example: `OPENAI_API_KEY=<TOKEN_HERE>`
```

### Comparing `lastmile-eval-0.0.4/pyproject.toml` & `lastmile-eval-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile-eval"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="LastMile AI" },
 ]
 description = "An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/text/__init__.py` & `lastmile-eval-0.0.5/src/lastmile_eval/text/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/text/batch_lib.py` & `lastmile-eval-0.0.5/src/lastmile_eval/text/batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/text/metrics.py` & `lastmile-eval-0.0.5/src/lastmile_eval/text/metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/text/metrics_lib.py` & `lastmile-eval-0.0.5/src/lastmile_eval/text/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/text/openai_batch_lib.py` & `lastmile-eval-0.0.5/src/lastmile_eval/text/openai_batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval/utils.py` & `lastmile-eval-0.0.5/src/lastmile_eval/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval.egg-info/PKG-INFO` & `lastmile-eval-0.0.5/src/lastmile_eval.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastmile-eval
-Version: 0.0.4
+Version: 0.0.5
 Summary: An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/eval
 Project-URL: Bug Tracker, https://github.com/lastmile-ai/eval/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -12,36 +12,35 @@
 License-File: LICENSE
 Requires-Dist: dataclasses
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 Requires-Dist: rouge_score
 Requires-Dist: nltk
 Requires-Dist: openai>=1.0.0
+Requires-Dist: anthropic
 Requires-Dist: evaluate==0.4.1
 Requires-Dist: arize-phoenix-evals==0.5.0
 Requires-Dist: pandas==2.1.2
 Requires-Dist: instructor
 
 # LastMile AI Eval
 
 Library of tools to evaluate your RAG system.
 
 ## Setup
 
 1. Get a LastMile API token (see section below)
 2. Install this library: `pip install lastmile-eval`
-3. Gather your data that needs evaluation.
-4. See examples/ folder for API usage.
+3. Gather your data that needs evaluation
+4. See the `examples/` folder for API usage
 
 ## LastMile API token
 
 To get a LastMile AI token, please go to the [LastMile token's webpage](https://lastmileai.dev/settings?page=tokens).
 You can create an account with Google or Github and then click the "Create new token" in the "API Tokens" section. Once a token is created, be sure to save it somewhere since you won't be able to see the value of it from the website again (though you can create a new one if that happens).
 
-**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead.
-See examples/ for how to do this.
-
+**Please be careful not to share your token on GitHub**. Instead we recommend saving it under your project’s (or home directory) `.env` file as: `LASTMILE_API_TOKEN=<TOKEN_HERE>`, and use loadenv instead. See the `examples/` folder for how to do this.
 
 ## LLM Provider Tokens (`.env` file)
 
 In order to use LLM-based evaluators, add your other API tokens to your .env file.
 Example: `OPENAI_API_KEY=<TOKEN_HERE>`
```

### Comparing `lastmile-eval-0.0.4/src/lastmile_eval.egg-info/SOURCES.txt` & `lastmile-eval-0.0.5/src/lastmile_eval.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 requirements.txt
 src/lastmile_eval/utils.py
 src/lastmile_eval.egg-info/PKG-INFO
 src/lastmile_eval.egg-info/SOURCES.txt
 src/lastmile_eval.egg-info/dependency_links.txt
 src/lastmile_eval.egg-info/requires.txt
 src/lastmile_eval.egg-info/top_level.txt
+src/lastmile_eval/examples/rag.py
+src/lastmile_eval/examples/text.py
 src/lastmile_eval/rag/__init__.py
 src/lastmile_eval/text/__init__.py
 src/lastmile_eval/text/batch_lib.py
 src/lastmile_eval/text/metrics.py
 src/lastmile_eval/text/metrics_lib.py
 src/lastmile_eval/text/openai_batch_lib.py
 src/lastmile_eval/text/utils.py
```

### Comparing `lastmile-eval-0.0.4/tests/test_custom_llm_metrics.py` & `lastmile-eval-0.0.5/tests/test_custom_llm_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/tests/test_default_text_metrics.py` & `lastmile-eval-0.0.5/tests/test_default_text_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.4/tests/test_rag_scores_e2e.py` & `lastmile-eval-0.0.5/tests/test_rag_scores_e2e.py`

 * *Files identical despite different names*

