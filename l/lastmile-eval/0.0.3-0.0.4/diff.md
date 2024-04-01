# Comparing `tmp/lastmile-eval-0.0.3.tar.gz` & `tmp/lastmile-eval-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile-eval-0.0.3.tar", last modified: Thu Mar 28 20:13:08 2024, max compression
+gzip compressed data, was "lastmile-eval-0.0.4.tar", last modified: Mon Apr  1 17:37:48 2024, max compression
```

## Comparing `lastmile-eval-0.0.3.tar` & `lastmile-eval-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.307007 lastmile-eval-0.0.3/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     1055 2024-03-08 23:19:42.000000 lastmile-eval-0.0.3/LICENSE
--rw-r--r--   0 rossdancraig   (501) staff       (20)     2310 2024-03-28 20:13:08.306816 lastmile-eval-0.0.3/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)     1755 2024-03-28 20:12:49.000000 lastmile-eval-0.0.3/README.md
--rw-r--r--   0 rossdancraig   (501) staff       (20)      911 2024-03-28 20:13:00.000000 lastmile-eval-0.0.3/pyproject.toml
--rw-r--r--   0 rossdancraig   (501) staff       (20)       34 2024-03-11 22:29:16.000000 lastmile-eval-0.0.3/requirements.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       38 2024-03-28 20:13:08.307048 lastmile-eval-0.0.3/setup.cfg
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.304853 lastmile-eval-0.0.3/src/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.305606 lastmile-eval-0.0.3/src/lastmile_eval/
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.306373 lastmile-eval-0.0.3/src/lastmile_eval/rag/
--rw-r--r--   0 rossdancraig   (501) staff       (20)      111 2024-03-28 19:52:21.000000 lastmile-eval-0.0.3/src/lastmile_eval/rag/__init__.py
--rw-r--r--   0 rossdancraig   (501) staff       (20)     5893 2024-03-28 19:35:35.000000 lastmile-eval-0.0.3/src/lastmile_eval/utils.py
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.306630 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     2310 2024-03-28 20:13:08.000000 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/PKG-INFO
--rw-r--r--   0 rossdancraig   (501) staff       (20)      332 2024-03-28 20:13:08.000000 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/SOURCES.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)        1 2024-03-28 20:13:08.000000 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/dependency_links.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       35 2024-03-28 20:13:08.000000 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/requires.txt
--rw-r--r--   0 rossdancraig   (501) staff       (20)       14 2024-03-28 20:13:08.000000 lastmile-eval-0.0.3/src/lastmile_eval.egg-info/top_level.txt
-drwxr-xr-x   0 rossdancraig   (501) staff       (20)        0 2024-03-28 20:13:08.306476 lastmile-eval-0.0.3/tests/
--rw-r--r--   0 rossdancraig   (501) staff       (20)     3099 2024-03-19 04:48:40.000000 lastmile-eval-0.0.3/tests/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.715819 lastmile-eval-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.715819 lastmile-eval-0.0.4/src/lastmile_eval/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/rag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/metrics_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/openai_batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/src/lastmile_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 17:37:48.000000 lastmile-eval-0.0.4/src/lastmile_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:48.719819 lastmile-eval-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_custom_llm_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_default_text_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-01 17:37:44.000000 lastmile-eval-0.0.4/tests/test_rag_scores_e2e.py
```

### Comparing `lastmile-eval-0.0.3/LICENSE` & `lastmile-eval-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.3/pyproject.toml` & `lastmile-eval-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile-eval"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="LastMile AI" },
 ]
 description = "An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lastmile-eval-0.0.3/src/lastmile_eval/utils.py` & `lastmile-eval-0.0.4/src/lastmile_eval/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.3/tests/test_e2e.py` & `lastmile-eval-0.0.4/tests/test_rag_scores_e2e.py`

 * *Files identical despite different names*

