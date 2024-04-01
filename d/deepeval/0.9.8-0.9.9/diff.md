# Comparing `tmp/deepeval-0.9.8.tar.gz` & `tmp/deepeval-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepeval-0.9.8.tar", last modified: Thu Aug 24 07:11:31 2023, max compression
+gzip compressed data, was "deepeval-0.9.9.tar", last modified: Fri Aug 25 07:54:40 2023, max compression
```

## Comparing `deepeval-0.9.8.tar` & `deepeval-0.9.9.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-24 07:11:31.887678 deepeval-0.9.8/
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-08-15 13:14:51.000000 deepeval-0.9.8/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      285 2023-08-24 07:11:31.887238 deepeval-0.9.8/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     4403 2023-08-23 11:24:17.000000 deepeval-0.9.8/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-24 07:11:31.865252 deepeval-0.9.8/deepeval/
--rw-r--r--   0 jackywong   (501) staff       (20)      439 2023-08-23 11:24:17.000000 deepeval-0.9.8/deepeval/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)       27 2023-08-24 07:11:12.000000 deepeval-0.9.8/deepeval/_version.py
--rw-r--r--   0 jackywong   (501) staff       (20)     9122 2023-08-23 08:09:42.000000 deepeval-0.9.8/deepeval/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1544 2023-08-24 06:49:36.000000 deepeval-0.9.8/deepeval/bulk_runner.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2822 2023-08-24 02:23:49.000000 deepeval-0.9.8/deepeval/client.py
--rw-r--r--   0 jackywong   (501) staff       (20)      202 2023-08-23 08:09:42.000000 deepeval-0.9.8/deepeval/constants.py
--rw-r--r--   0 jackywong   (501) staff       (20)     7735 2023-08-24 06:43:09.000000 deepeval-0.9.8/deepeval/dataset.py
--rw-r--r--   0 jackywong   (501) staff       (20)     5019 2023-08-23 08:09:42.000000 deepeval-0.9.8/deepeval/evaluator.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-24 07:11:31.874173 deepeval-0.9.8/deepeval/metrics/
--rw-r--r--   0 jackywong   (501) staff       (20)      152 2023-08-16 07:51:21.000000 deepeval-0.9.8/deepeval/metrics/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1922 2023-08-23 03:49:08.000000 deepeval-0.9.8/deepeval/metrics/alert_score.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1759 2023-08-24 06:57:32.000000 deepeval-0.9.8/deepeval/metrics/answer_relevancy.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1045 2023-08-24 05:30:51.000000 deepeval-0.9.8/deepeval/metrics/bertscore_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2209 2023-08-24 05:25:32.000000 deepeval-0.9.8/deepeval/metrics/bias_classifier.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1809 2023-08-23 03:49:08.000000 deepeval-0.9.8/deepeval/metrics/bleu_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1356 2023-08-24 05:26:41.000000 deepeval-0.9.8/deepeval/metrics/cohere_reranker_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1309 2023-08-24 02:48:15.000000 deepeval-0.9.8/deepeval/metrics/conceptual_similarity.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1520 2023-08-24 05:21:43.000000 deepeval-0.9.8/deepeval/metrics/entailment_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)      592 2023-08-24 04:38:49.000000 deepeval-0.9.8/deepeval/metrics/factual_consistency.py
--rw-r--r--   0 jackywong   (501) staff       (20)     4026 2023-08-24 06:49:50.000000 deepeval-0.9.8/deepeval/metrics/metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1954 2023-08-24 05:28:26.000000 deepeval-0.9.8/deepeval/metrics/overall_score.py
--rw-r--r--   0 jackywong   (501) staff       (20)      358 2023-08-24 02:25:25.000000 deepeval-0.9.8/deepeval/metrics/randomscore.py
--rw-r--r--   0 jackywong   (501) staff       (20)     6450 2023-08-23 03:49:08.000000 deepeval-0.9.8/deepeval/metrics/ranking_similarity.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1801 2023-08-24 02:48:30.000000 deepeval-0.9.8/deepeval/metrics/toxic_classifier.py
--rw-r--r--   0 jackywong   (501) staff       (20)      252 2023-08-14 22:05:05.000000 deepeval-0.9.8/deepeval/pipeline.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1637 2023-08-14 22:05:05.000000 deepeval-0.9.8/deepeval/query_generator.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1443 2023-08-23 15:05:58.000000 deepeval-0.9.8/deepeval/retry.py
--rw-r--r--   0 jackywong   (501) staff       (20)      479 2023-08-24 05:21:46.000000 deepeval-0.9.8/deepeval/singleton.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1918 2023-08-24 06:42:57.000000 deepeval-0.9.8/deepeval/test_case.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2313 2023-08-24 06:57:17.000000 deepeval-0.9.8/deepeval/test_utils.py
--rw-r--r--   0 jackywong   (501) staff       (20)      387 2023-08-21 11:56:07.000000 deepeval-0.9.8/deepeval/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-24 07:11:31.867257 deepeval-0.9.8/deepeval.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      285 2023-08-24 07:11:31.000000 deepeval-0.9.8/deepeval.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     1448 2023-08-24 07:11:31.000000 deepeval-0.9.8/deepeval.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-08-24 07:11:31.000000 deepeval-0.9.8/deepeval.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)      121 2023-08-24 07:11:31.000000 deepeval-0.9.8/deepeval.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-08-24 07:11:31.000000 deepeval-0.9.8/deepeval.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-08-24 07:11:31.887891 deepeval-0.9.8/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      951 2023-08-23 11:24:17.000000 deepeval-0.9.8/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-24 07:11:31.882007 deepeval-0.9.8/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-08-22 02:44:10.000000 deepeval-0.9.8/tests/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1343 2023-08-22 02:44:10.000000 deepeval-0.9.8/tests/test_alert_score.py
--rw-r--r--   0 jackywong   (501) staff       (20)      550 2023-08-24 06:49:05.000000 deepeval-0.9.8/tests/test_answer_relevancy.py
--rw-r--r--   0 jackywong   (501) staff       (20)      288 2023-08-22 04:40:40.000000 deepeval-0.9.8/tests/test_bert_score.py
--rw-r--r--   0 jackywong   (501) staff       (20)      708 2023-08-23 08:09:42.000000 deepeval-0.9.8/tests/test_bias.py
--rw-r--r--   0 jackywong   (501) staff       (20)      619 2023-08-23 15:05:58.000000 deepeval-0.9.8/tests/test_bulk_runner.py
--rw-r--r--   0 jackywong   (501) staff       (20)      966 2023-08-23 11:24:17.000000 deepeval-0.9.8/tests/test_clients.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1124 2023-08-22 15:02:11.000000 deepeval-0.9.8/tests/test_custom_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)      639 2023-08-24 06:43:45.000000 deepeval-0.9.8/tests/test_dataset.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1004 2023-08-24 01:56:48.000000 deepeval-0.9.8/tests/test_factual_consistency.py
--rw-r--r--   0 jackywong   (501) staff       (20)      562 2023-08-18 05:43:44.000000 deepeval-0.9.8/tests/test_metric.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1057 2023-08-22 02:44:10.000000 deepeval-0.9.8/tests/test_overall_score.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1417 2023-08-24 06:43:58.000000 deepeval-0.9.8/tests/test_quickstart.py
--rw-r--r--   0 jackywong   (501) staff       (20)      690 2023-08-24 06:44:10.000000 deepeval-0.9.8/tests/test_sample.py
--rw-r--r--   0 jackywong   (501) staff       (20)     1055 2023-08-23 03:49:08.000000 deepeval-0.9.8/tests/test_similar_ranking.py
--rw-r--r--   0 jackywong   (501) staff       (20)      748 2023-08-22 05:15:16.000000 deepeval-0.9.8/tests/test_toxic.py
--rw-r--r--   0 jackywong   (501) staff       (20)      152 2023-08-22 02:44:10.000000 deepeval-0.9.8/tests/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-25 07:54:40.922698 deepeval-0.9.9/
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-08-15 13:14:51.000000 deepeval-0.9.9/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      285 2023-08-25 07:54:40.922408 deepeval-0.9.9/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     4655 2023-08-24 16:32:04.000000 deepeval-0.9.9/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-25 07:54:40.910463 deepeval-0.9.9/deepeval/
+-rw-r--r--   0 jackywong   (501) staff       (20)      439 2023-08-23 11:24:17.000000 deepeval-0.9.9/deepeval/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       27 2023-08-25 07:24:59.000000 deepeval-0.9.9/deepeval/_version.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     9244 2023-08-25 07:34:56.000000 deepeval-0.9.9/deepeval/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1544 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/bulk_runner.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2822 2023-08-24 02:23:49.000000 deepeval-0.9.9/deepeval/client.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      202 2023-08-23 08:09:42.000000 deepeval-0.9.9/deepeval/constants.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     7735 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/dataset.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     5019 2023-08-23 08:09:42.000000 deepeval-0.9.9/deepeval/evaluator.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-25 07:54:40.917271 deepeval-0.9.9/deepeval/metrics/
+-rw-r--r--   0 jackywong   (501) staff       (20)      152 2023-08-16 07:51:21.000000 deepeval-0.9.9/deepeval/metrics/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1922 2023-08-23 03:49:08.000000 deepeval-0.9.9/deepeval/metrics/alert_score.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1759 2023-08-24 07:44:26.000000 deepeval-0.9.9/deepeval/metrics/answer_relevancy.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1045 2023-08-24 05:30:51.000000 deepeval-0.9.9/deepeval/metrics/bertscore_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2209 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/metrics/bias_classifier.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1809 2023-08-23 03:49:08.000000 deepeval-0.9.9/deepeval/metrics/bleu_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1356 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/metrics/cohere_reranker_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1309 2023-08-24 02:48:15.000000 deepeval-0.9.9/deepeval/metrics/conceptual_similarity.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      926 2023-08-25 05:16:22.000000 deepeval-0.9.9/deepeval/metrics/entailment_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1502 2023-08-25 07:40:55.000000 deepeval-0.9.9/deepeval/metrics/factual_consistency.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     4731 2023-08-25 07:42:09.000000 deepeval-0.9.9/deepeval/metrics/metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2435 2023-08-25 07:48:20.000000 deepeval-0.9.9/deepeval/metrics/overall_score.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      358 2023-08-24 02:25:25.000000 deepeval-0.9.9/deepeval/metrics/randomscore.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     6450 2023-08-23 03:49:08.000000 deepeval-0.9.9/deepeval/metrics/ranking_similarity.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1801 2023-08-24 02:48:30.000000 deepeval-0.9.9/deepeval/metrics/toxic_classifier.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      252 2023-08-14 22:05:05.000000 deepeval-0.9.9/deepeval/pipeline.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1637 2023-08-14 22:05:05.000000 deepeval-0.9.9/deepeval/query_generator.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1443 2023-08-23 15:05:58.000000 deepeval-0.9.9/deepeval/retry.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      479 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/singleton.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1918 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/test_case.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2313 2023-08-24 07:19:58.000000 deepeval-0.9.9/deepeval/test_utils.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      387 2023-08-21 11:56:07.000000 deepeval-0.9.9/deepeval/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-25 07:54:40.911980 deepeval-0.9.9/deepeval.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      285 2023-08-25 07:54:40.000000 deepeval-0.9.9/deepeval.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     1427 2023-08-25 07:54:40.000000 deepeval-0.9.9/deepeval.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-08-25 07:54:40.000000 deepeval-0.9.9/deepeval.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)      121 2023-08-25 07:54:40.000000 deepeval-0.9.9/deepeval.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-08-25 07:54:40.000000 deepeval-0.9.9/deepeval.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-08-25 07:54:40.922791 deepeval-0.9.9/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      951 2023-08-23 11:24:17.000000 deepeval-0.9.9/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-08-25 07:54:40.922001 deepeval-0.9.9/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-08-22 02:44:10.000000 deepeval-0.9.9/tests/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1343 2023-08-22 02:44:10.000000 deepeval-0.9.9/tests/test_alert_score.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      550 2023-08-24 07:19:58.000000 deepeval-0.9.9/tests/test_answer_relevancy.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      288 2023-08-22 04:40:40.000000 deepeval-0.9.9/tests/test_bert_score.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      708 2023-08-23 08:09:42.000000 deepeval-0.9.9/tests/test_bias.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      619 2023-08-23 15:05:58.000000 deepeval-0.9.9/tests/test_bulk_runner.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      966 2023-08-23 11:24:17.000000 deepeval-0.9.9/tests/test_clients.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1124 2023-08-22 15:02:11.000000 deepeval-0.9.9/tests/test_custom_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      639 2023-08-24 07:19:58.000000 deepeval-0.9.9/tests/test_dataset.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1004 2023-08-24 01:56:48.000000 deepeval-0.9.9/tests/test_factual_consistency.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      562 2023-08-18 05:43:44.000000 deepeval-0.9.9/tests/test_metric.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1116 2023-08-25 07:48:11.000000 deepeval-0.9.9/tests/test_overall_score.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1419 2023-08-25 07:52:07.000000 deepeval-0.9.9/tests/test_quickstart.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     1055 2023-08-23 03:49:08.000000 deepeval-0.9.9/tests/test_similar_ranking.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      748 2023-08-22 05:15:16.000000 deepeval-0.9.9/tests/test_toxic.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      152 2023-08-22 02:44:10.000000 deepeval-0.9.9/tests/utils.py
```

### Comparing `deepeval-0.9.8/LICENSE` & `deepeval-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/README.md` & `deepeval-0.9.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # 👩‍⚖️ DeepEval
 
 [![](https://dcbadge.vercel.app/api/server/a3K9c8GRGt)](https://discord.gg/a3K9c8GRGt)
 
+<a target="_blank" href="https://colab.research.google.com/github/https://colab.research.google.com/drive/1Lfq5geYsvfVoquDqv84UkWS57SdAHm30?usp=sharing">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
+
 DeepEval provides a Pythonic way to run offline evaluations on your LLM pipelines so you can launch comfortably into production. The guiding philosophy is a "Pytest for LLM" that aims to make productionizing and evaluating LLMs as easy as ensuring all tests pass.
 
 Looking for DeepEval API? Please join the waitlist here: https://forms.gle/y3uqNBkmfxVYLXGq6
 
 # Documentation
 
 We highly recommend getting started through our documentation here: https://docs.confident-ai.com/docs/
```

### Comparing `deepeval-0.9.8/deepeval/api.py` & `deepeval-0.9.9/deepeval/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
         self.api_key = api_key
 
         self._auth = (self.api_key, "")
         self._headers = {
             "Content-Type": "application/json",
             "User-Agent": self._generate_useragent(user_agent_extension),
-            "Authorization": "Bearer " + api_key,
+            # "Authorization": "Bearer " + api_key,
+            # This is what gets sent now - auth gets sent to firebase instead
+            "CONFIDENT_API_KEY": api_key,
         }
         self._headers_multipart_form_data = {
             "User-Agent": self._generate_useragent(user_agent_extension),
         }
         self.base_api_url = api_instance_url or API_BASE_URL
 
         self.verify = verify
```

### Comparing `deepeval-0.9.8/deepeval/bulk_runner.py` & `deepeval-0.9.9/deepeval/bulk_runner.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/client.py` & `deepeval-0.9.9/deepeval/client.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/dataset.py` & `deepeval-0.9.9/deepeval/dataset.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/evaluator.py` & `deepeval-0.9.9/deepeval/evaluator.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/alert_score.py` & `deepeval-0.9.9/deepeval/metrics/alert_score.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/answer_relevancy.py` & `deepeval-0.9.9/deepeval/metrics/answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/bertscore_metric.py` & `deepeval-0.9.9/deepeval/metrics/bertscore_metric.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/bias_classifier.py` & `deepeval-0.9.9/deepeval/metrics/bias_classifier.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/bleu_metric.py` & `deepeval-0.9.9/deepeval/metrics/bleu_metric.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/cohere_reranker_metric.py` & `deepeval-0.9.9/deepeval/metrics/cohere_reranker_metric.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/conceptual_similarity.py` & `deepeval-0.9.9/deepeval/metrics/conceptual_similarity.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/entailment_metric.py` & `deepeval-0.9.9/deepeval/metrics/entailment_metric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import asyncio
 from sentence_transformers import CrossEncoder
-from typing import Optional
 from ..utils import softmax
 from ..singleton import Singleton
 from .metric import Metric
 
 
 class EntailmentScoreMetric(Metric, metaclass=Singleton):
     def __init__(
@@ -26,24 +24,7 @@
 
     def is_successful(self) -> bool:
         return self.success
 
     @property
     def __name__(self):
         return "Entailment"
-
-    def __call__(self, output, expected_output, query: Optional[str] = "-"):
-        score = self.measure(output, expected_output)
-        success = False
-        if score > self.minimum_score:
-            success = True
-        asyncio.create_task(
-            self._send_to_server(
-                metric_score=score,
-                metric_name=self.__name__,
-                query=query,
-                output=output,
-                expected_output=expected_output,
-                success=success,
-            )
-        )
-        return score
```

### Comparing `deepeval-0.9.8/deepeval/metrics/metric.py` & `deepeval-0.9.9/deepeval/metrics/metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-"""Available metrics. The best metric that
-you want is Cohere's reranker metric.
-"""
 import asyncio
 import os
 import warnings
 from typing import Optional
 from ..constants import (
     API_KEY_ENV,
     IMPLEMENTATION_ID_ENV,
     LOG_TO_SERVER_ENV,
     IMPLEMENTATION_ID_NAME,
 )
 from abc import abstractmethod
 from ..client import Client
-from ..api import Api
 from ..utils import softmax
+from ..singleton import Singleton
 
 
-class Metric:
+class Metric(metaclass=Singleton):
     # set an arbitrary minimum score that will get over-ridden later
     minimum_score: float = 0
 
     # Measure function signature is subject to be different - not sure
     # how applicable this is - might need a better abstraction
     @abstractmethod
     def measure(self, output, expected_output, query: Optional[str] = None):
@@ -40,37 +37,63 @@
     def is_successful(self) -> bool:
         raise NotImplementedError
 
     def _is_api_key_set(self):
         result = os.getenv(API_KEY_ENV) is not None
         if result is False:
             warnings.warn(
-                """API key is not set. Please set it by visiting https://app.confident-ai.com
-"""
+                """API key is not set. Please set it by visiting https://app.confident-ai.com"""
             )
         return result
 
     def _is_send_okay(self):
         # DOing this until the API endpoint is fixed
         return self._is_api_key_set() and os.getenv(LOG_TO_SERVER_ENV) != "Y"
 
-    def __call__(self, output, expected_output, query: Optional[str] = "-"):
-        score = self.measure(output, expected_output)
+    def __call__(self, *args, **kwargs):
+        score = self.measure(*args, **kwargs)
         success = score >= self.minimum_score
         asyncio.create_task(
             self._send_to_server(
                 metric_score=score,
                 metric_name=self.__name__,
+                query=kwargs.get("query", "-"),
+                output=kwargs.get("output", "-"),
+                expected_output=kwargs.get("expected_output", "-"),
+                success=success,
+            )
+        )
+        return score
+
+    def log(
+        self,
+        success: bool = True,
+        score: float = 1e-10,
+        metric_name: str = "-",
+        query: str = "-",
+        output: str = "-",
+        expected_output: str = "-",
+    ):
+        """Log to the server.
+
+        Parameters
+        - query: What was asked to the model. This can also be context.
+        - output: The LLM output.
+        - expected_output: The output that's expected.
+        """
+        asyncio.create_task(
+            self._send_to_server(
+                metric_score=score,
+                metric_name=metric_name,
                 query=query,
                 output=output,
                 expected_output=expected_output,
                 success=success,
             )
         )
-        return score
 
     async def _send_to_server(
         self,
         metric_score: float,
         metric_name: str,
         query: str = "-",
         output: str = "-",
```

### Comparing `deepeval-0.9.8/deepeval/metrics/overall_score.py` & `deepeval-0.9.9/deepeval/metrics/overall_score.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,83 @@
 """Overall Score
 """
 import asyncio
 from .metric import Metric
 from .entailment_metric import EntailmentScoreMetric
+from .answer_relevancy import AnswerRelevancy
 from ..singleton import Singleton
 
 
 class OverallScoreMetric(Metric, metaclass=Singleton):
     def __init__(self, minimum_score: float = 0.5):
         self.minimum_score = minimum_score
         self.entailment_metric = EntailmentScoreMetric()
+        self.answer_relevancy = AnswerRelevancy()
 
-    def __call__(self, generated_text: str, expected_output: str, context: str):
-        score = self.measure(generated_text, expected_output, context)
+    def __call__(self, query, generated_text: str, expected_output: str, context: str):
+        score = self.measure(
+            query=query,
+            generated_text=generated_text,
+            expected_output=expected_output,
+            context=context,
+        )
         success = score > self.minimum_score
         asyncio.create_task(
             self._send_to_server(
                 metric_score=score,
                 metric_name=self.__name__,
                 query=context,
                 output=generated_text,
                 expected_output=expected_output,
                 success=success,
             )
         )
         return score
 
-    def measure(self, generated_text: str, expected_output: str, context: str) -> float:
+    def measure(
+        self, query: str, generated_text: str, expected_output: str, context: str
+    ) -> float:
         entailment_score = self.entailment_metric.measure(
             context,
             generated_text,
         )
 
         answer_expected_score = self.entailment_metric.measure(
             generated_text,
             expected_output,
         )
 
-        overall_score = 0.5 * entailment_score + 0.5 * answer_expected_score
+        answer_relevancy_score = self.answer_relevancy.measure(
+            query=query, output=generated_text
+        )
+
+        overall_score = (
+            0.33 * entailment_score
+            + 0.33 * answer_expected_score
+            + 0.33 * answer_relevancy_score
+        )
         self.success = overall_score > self.minimum_score
         return overall_score
 
     def is_successful(self) -> bool:
         return self.success
 
     @property
     def __name__(self):
         return "Alert Score"
 
 
 def assert_overall_score(
+    query: str,
     generated_text: str,
     expected_output: str,
     context: str,
     minimum_score: float = 0.5,
 ):
     metric = OverallScoreMetric(minimum_score=minimum_score)
     score = metric.measure(
+        query=query,
         generated_text=generated_text,
         expected_output=expected_output,
         context=context,
     )
     assert metric.is_successful(), f"Metric is not conceptually similar - got {score}"
```

### Comparing `deepeval-0.9.8/deepeval/metrics/ranking_similarity.py` & `deepeval-0.9.9/deepeval/metrics/ranking_similarity.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/metrics/toxic_classifier.py` & `deepeval-0.9.9/deepeval/metrics/toxic_classifier.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/query_generator.py` & `deepeval-0.9.9/deepeval/query_generator.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/retry.py` & `deepeval-0.9.9/deepeval/retry.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/test_case.py` & `deepeval-0.9.9/deepeval/test_case.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval/test_utils.py` & `deepeval-0.9.9/deepeval/test_utils.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/deepeval.egg-info/SOURCES.txt` & `deepeval-0.9.9/deepeval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,11 +45,10 @@
 tests/test_clients.py
 tests/test_custom_metric.py
 tests/test_dataset.py
 tests/test_factual_consistency.py
 tests/test_metric.py
 tests/test_overall_score.py
 tests/test_quickstart.py
-tests/test_sample.py
 tests/test_similar_ranking.py
 tests/test_toxic.py
 tests/utils.py
```

### Comparing `deepeval-0.9.8/setup.py` & `deepeval-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_alert_score.py` & `deepeval-0.9.9/tests/test_alert_score.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_answer_relevancy.py` & `deepeval-0.9.9/tests/test_answer_relevancy.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_bias.py` & `deepeval-0.9.9/tests/test_bias.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_bulk_runner.py` & `deepeval-0.9.9/tests/test_bulk_runner.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_clients.py` & `deepeval-0.9.9/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_custom_metric.py` & `deepeval-0.9.9/tests/test_custom_metric.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_dataset.py` & `deepeval-0.9.9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_factual_consistency.py` & `deepeval-0.9.9/tests/test_factual_consistency.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_metric.py` & `deepeval-0.9.9/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_overall_score.py` & `deepeval-0.9.9/tests/test_overall_score.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 expected_output = "French national football team"
 context = "The FIFA World Cup in 2018 was won by the French national football team. They defeated Croatia 4-2 in the final match to claim the championship."
 
 
 @pytest.mark.asyncio
 async def test_overall_score():
     assert_overall_score(
+        query=query,
         generated_text=generated_text,
         expected_output=expected_output,
         context=context,
     )
 
 
 @pytest.mark.asyncio
 async def test_overall_score_metric():
     metric = OverallScoreMetric()
     score = metric.measure(
-        generated_text=generated_text, expected_output=expected_output, context=context
+        query=query,
+        generated_text=generated_text,
+        expected_output=expected_output,
+        context=context,
     )
     assert metric.is_successful(), "Overall score metric not working"
     assert_viable_score(score)
```

### Comparing `deepeval-0.9.8/tests/test_quickstart.py` & `deepeval-0.9.9/tests/test_quickstart.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import os
 from deepeval.api import Api
 from deepeval.metrics.factual_consistency import assert_factual_consistency
 from deepeval.metrics.bertscore_metric import BertScoreMetric
 from deepeval.constants import API_KEY_ENV
 
-IMPLEMENTATION_NAME = "Quickstart Example"
+IMPLEMENTATION_NAME = "Quickstart Example 2"
 os.environ["CONFIDENT_AI_IMP_NAME"] = IMPLEMENTATION_NAME
 
 
 def generate_llm_output(query: str):
     expected_output = "Our customer success phone line is 1200-231-231."
     return expected_output
```

### Comparing `deepeval-0.9.8/tests/test_similar_ranking.py` & `deepeval-0.9.9/tests/test_similar_ranking.py`

 * *Files identical despite different names*

### Comparing `deepeval-0.9.8/tests/test_toxic.py` & `deepeval-0.9.9/tests/test_toxic.py`

 * *Files identical despite different names*

