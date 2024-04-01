# Comparing `tmp/modlee-0.0.1.post1.tar.gz` & `tmp/modlee-0.0.1.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modlee-0.0.1.post1.tar", last modified: Tue Sep  5 18:51:12 2023, max compression
+gzip compressed data, was "modlee-0.0.1.post6.tar", last modified: Mon Apr  1 18:30:58 2024, max compression
```

## Comparing `modlee-0.0.1.post1.tar` & `modlee-0.0.1.post6.tar`

### file list

```diff
@@ -1,12 +1,46 @@
-drwxr-xr-x   0 modlee     (501) staff       (20)        0 2023-09-05 18:51:12.602055 modlee-0.0.1.post1/
--rw-r--r--   0 modlee     (501) staff       (20)      145 2023-09-05 18:51:12.601948 modlee-0.0.1.post1/PKG-INFO
-drwxr-xr-x   0 modlee     (501) staff       (20)        0 2023-09-05 18:51:12.601279 modlee-0.0.1.post1/modlee/
--rw-r--r--   0 modlee     (501) staff       (20)        0 2023-09-05 18:31:28.000000 modlee-0.0.1.post1/modlee/__init__.py
-drwxr-xr-x   0 modlee     (501) staff       (20)        0 2023-09-05 18:51:12.601795 modlee-0.0.1.post1/modlee.egg-info/
--rw-r--r--   0 modlee     (501) staff       (20)      145 2023-09-05 18:51:12.000000 modlee-0.0.1.post1/modlee.egg-info/PKG-INFO
--rw-r--r--   0 modlee     (501) staff       (20)      182 2023-09-05 18:51:12.000000 modlee-0.0.1.post1/modlee.egg-info/SOURCES.txt
--rw-r--r--   0 modlee     (501) staff       (20)        1 2023-09-05 18:51:12.000000 modlee-0.0.1.post1/modlee.egg-info/dependency_links.txt
--rw-r--r--   0 modlee     (501) staff       (20)      255 2023-09-05 18:51:12.000000 modlee-0.0.1.post1/modlee.egg-info/requires.txt
--rw-r--r--   0 modlee     (501) staff       (20)        7 2023-09-05 18:51:12.000000 modlee-0.0.1.post1/modlee.egg-info/top_level.txt
--rw-r--r--   0 modlee     (501) staff       (20)     1022 2023-09-05 18:50:56.000000 modlee-0.0.1.post1/pyproject.toml
--rw-r--r--   0 modlee     (501) staff       (20)       38 2023-09-05 18:51:12.602094 modlee-0.0.1.post1/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20048 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.514089 modlee-0.0.1.post6/docs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2024-04-01 18:01:00.000000 modlee-0.0.1.post6/docs/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6260 2024-03-28 19:36:00.000000 modlee-0.0.1.post6/docs/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1994 2024-04-01 18:30:51.000000 modlee-0.0.1.post6/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 18:30:58.526089 modlee-0.0.1.post6/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.514089 modlee-0.0.1.post6/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.518089 modlee-0.0.1.post6/src/modlee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5647 2024-03-28 19:35:59.000000 modlee-0.0.1.post6/src/modlee/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10670 2024-04-01 14:21:08.000000 modlee-0.0.1.post6/src/modlee/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      369 2024-03-21 20:32:15.000000 modlee-0.0.1.post6/src/modlee/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    39155 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20782 2024-03-28 18:38:37.000000 modlee-0.0.1.post6/src/modlee/data_metafeatures.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11976 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/exp_loss_logger.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/loss_sweeper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/src/modlee/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18673 2024-04-01 16:57:28.000000 modlee-0.0.1.post6/src/modlee/model/callbacks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3443 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/model/image_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5895 2024-03-30 00:57:31.000000 modlee-0.0.1.post6/src/modlee/model/model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1867 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/model/recommended_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15787 2024-03-28 18:38:37.000000 modlee-0.0.1.post6/src/modlee/model_text_converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5050 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/modlee_image_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/src/modlee/recommender/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      893 2024-04-01 14:43:49.000000 modlee-0.0.1.post6/src/modlee/recommender/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2024-04-01 14:31:35.000000 modlee-0.0.1.post6/src/modlee/recommender/image_recommender.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14806 2024-04-01 14:16:53.000000 modlee-0.0.1.post6/src/modlee/recommender/recommender.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3638 2024-03-19 02:55:45.000000 modlee-0.0.1.post6/src/modlee/retriever.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      473 2024-03-21 20:32:15.000000 modlee-0.0.1.post6/src/modlee/trainer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8969 2024-03-28 19:36:00.000000 modlee-0.0.1.post6/src/modlee/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/src/modlee.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20048 2024-04-01 18:30:58.000000 modlee-0.0.1.post6/src/modlee.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      975 2024-04-01 18:30:58.000000 modlee-0.0.1.post6/src/modlee.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 18:30:58.000000 modlee-0.0.1.post6/src/modlee.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-04-01 18:30:58.000000 modlee-0.0.1.post6/src/modlee.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-01 18:30:58.000000 modlee-0.0.1.post6/src/modlee.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:30:58.522089 modlee-0.0.1.post6/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2005 2024-03-28 19:36:00.000000 modlee-0.0.1.post6/tests/test_callbacks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7822 2024-03-28 20:39:46.000000 modlee-0.0.1.post6/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17748 2024-03-14 15:11:57.000000 modlee-0.0.1.post6/tests/test_converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2024-03-21 20:32:15.000000 modlee-0.0.1.post6/tests/test_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1758 2024-03-14 15:11:57.000000 modlee-0.0.1.post6/tests/test_modlee.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2879 2024-03-28 19:36:00.000000 modlee-0.0.1.post6/tests/test_recommender.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3137 2024-03-14 15:11:57.000000 modlee-0.0.1.post6/tests/test_retriever.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      917 2024-03-14 15:11:57.000000 modlee-0.0.1.post6/tests/test_utils.py
```

