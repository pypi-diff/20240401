# Comparing `tmp/so-ml-tools-0.1.98.tar.gz` & `tmp/so-ml-tools-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so-ml-tools-0.1.98.tar", last modified: Thu Nov 16 12:53:15 2023, max compression
+gzip compressed data, was "so-ml-tools-0.1.99.tar", last modified: Thu Nov 16 13:19:18 2023, max compression
```

## Comparing `so-ml-tools-0.1.98.tar` & `so-ml-tools-0.1.99.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.184541 so-ml-tools-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-16 12:53:15.184541 so-ml-tools-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 12:53:15.184541 so-ml-tools-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.176541 so-ml-tools-0.1.98/so_ml_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/data/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/evaluate/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    16513 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/evaluate/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/nlp/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/nlp/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/nlp/embedding/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/nlp/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/pd/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/pd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32613 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/pd/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/pd/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/pd/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/shap/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/shap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/shap/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/sklearn/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/sklearn/imputer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/tf/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.180541 so-ml-tools-0.1.98/so_ml_tools/tf/fit/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/fit/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/mixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.184541 so-ml-tools-0.1.98/so_ml_tools/tf/model/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/model/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/tf/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.184541 so-ml-tools-0.1.98/so_ml_tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2023-11-16 12:50:54.000000 so-ml-tools-0.1.98/so_ml_tools/util/label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 12:53:15.176541 so-ml-tools-0.1.98/so_ml_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-16 12:53:15.000000 so-ml-tools-0.1.98/so_ml_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-16 12:53:15.000000 so-ml-tools-0.1.98/so_ml_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 12:53:15.000000 so-ml-tools-0.1.98/so_ml_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-16 12:53:15.000000 so-ml-tools-0.1.98/so_ml_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-16 12:53:15.000000 so-ml-tools-0.1.98/so_ml_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.047895 so-ml-tools-0.1.99/so_ml_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/data/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/evaluate/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16515 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/evaluate/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/nlp/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/nlp/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/nlp/embedding/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/nlp/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/pd/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/pd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32613 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/pd/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/pd/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/pd/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/shap/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/shap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/shap/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/sklearn/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/sklearn/imputer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.051895 so-ml-tools-0.1.99/so_ml_tools/tf/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/so_ml_tools/tf/fit/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/fit/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/mixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/so_ml_tools/tf/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/model/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/tf/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.055895 so-ml-tools-0.1.99/so_ml_tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2023-11-16 13:16:55.000000 so-ml-tools-0.1.99/so_ml_tools/util/label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:19:18.047895 so-ml-tools-0.1.99/so_ml_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-11-16 13:19:17.000000 so-ml-tools-0.1.99/so_ml_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-16 13:19:18.000000 so-ml-tools-0.1.99/so_ml_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 13:19:17.000000 so-ml-tools-0.1.99/so_ml_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-16 13:19:17.000000 so-ml-tools-0.1.99/so_ml_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-16 13:19:17.000000 so-ml-tools-0.1.99/so_ml_tools.egg-info/top_level.txt
```

### Comparing `so-ml-tools-0.1.98/setup.py` & `so-ml-tools-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/data/image.py` & `so-ml-tools-0.1.99/so_ml_tools/data/image.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/data/loader.py` & `so-ml-tools-0.1.99/so_ml_tools/data/loader.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/data/plot.py` & `so-ml-tools-0.1.99/so_ml_tools/data/plot.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/data/split.py` & `so-ml-tools-0.1.99/so_ml_tools/data/split.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/evaluate/analyze.py` & `so-ml-tools-0.1.99/so_ml_tools/evaluate/analyze.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/evaluate/plot.py` & `so-ml-tools-0.1.99/so_ml_tools/evaluate/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Returns:
         None
     """
 
     if isinstance(y_true, _tf.data.Dataset):
         raise TypeError('y_true is a dataset, please get the labels from the dataset using '
-                        '\'y_labels = ml.tf.dataset.get_labels(dataset=dataset)\'')
+                        '\'y_labels = soml.tf.dataset.get_labels(dataset=dataset)\'')
 
     y_true = _soml.util.label.to_prediction(y_prob=y_true)
     if y_pred is None and y_prob is not None:
         y_pred = _soml.util.label.to_prediction(y_prob=y_prob)
     elif y_pred is None and y_prob is None:
         raise "Must specify 'y_pred' or 'y_prob'"
```

### Comparing `so-ml-tools-0.1.98/so_ml_tools/nlp/embedding/export.py` & `so-ml-tools-0.1.99/so_ml_tools/nlp/embedding/export.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/nlp/text.py` & `so-ml-tools-0.1.99/so_ml_tools/nlp/text.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/pd/dataframe.py` & `so-ml-tools-0.1.99/so_ml_tools/pd/dataframe.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/pd/plot.py` & `so-ml-tools-0.1.99/so_ml_tools/pd/plot.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/shap/report.py` & `so-ml-tools-0.1.99/so_ml_tools/shap/report.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/sklearn/encoder.py` & `so-ml-tools-0.1.99/so_ml_tools/sklearn/encoder.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/sklearn/imputer.py` & `so-ml-tools-0.1.99/so_ml_tools/sklearn/imputer.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/dataset.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/dataset.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/fit/callback.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/fit/callback.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/mixed_precision.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/augment.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/augment.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/inspect.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/inspect.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/io.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/io.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/layer.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/layer.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/plot.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/plot.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/model/predict.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/model/predict.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/tf/tensor.py` & `so-ml-tools-0.1.99/so_ml_tools/tf/tensor.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/util/io.py` & `so-ml-tools-0.1.99/so_ml_tools/util/io.py`

 * *Files identical despite different names*

### Comparing `so-ml-tools-0.1.98/so_ml_tools/util/label.py` & `so-ml-tools-0.1.99/so_ml_tools/util/label.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,25 @@
         True if it is a multiclass classification, False if not.
 
     Raises:
         TypeError: If `y_prob` is neither a 'list', 'tf.Tensor' or 'np.array'.
     """
     assert y_prob is not None, "y_prob is null"
 
+    if isinstance(y_prob, _pd.DataFrame):
+        y_prob = y_prob.to_numpy()
+    elif isinstance(y_prob, _pd.Series):
+        y_prob = _np.expand_dims(y_prob.to_numpy(), axis=-1)
+
     if isinstance(y_prob, list):
         return len(y_prob) > 0 and isinstance(y_prob[0], (list | _np.ndarray)) and len(y_prob[0]) > 1
     elif _tf.is_tensor(y_prob):
         return y_prob.get_shape().ndims == 2 and y_prob.shape[1] > 1
-    elif isinstance(y_prob, _pd.DataFrame):
-        return y_prob.ndims == 2 and y_prob.shape[1] > 1
+    # elif isinstance(y_prob, _pd.DataFrame):
+    #     return y_prob.ndims == 2 and y_prob.shape[1] > 1
     elif isinstance(y_prob, _np.ndarray):
         return y_prob.ndim == 2 and y_prob.shape[1] > 1
 
     raise TypeError('y should be of type tf.Tensor, np.array or pd.DataFrame.')
 
 
 def is_binary_classification(y_prob: any) -> bool:
@@ -50,14 +55,19 @@
         True if it is a binary classification, False if not.
 
     Raises:
         TypeError: If `y_prob` is neither a  'list', 'tf.Tensor' or 'np.array'.
     """
     assert y_prob is not None, "y_prob is null"
 
+    if isinstance(y_prob, _pd.DataFrame):
+        y_prob = y_prob.to_numpy()
+    elif isinstance(y_prob, _pd.Series):
+        y_prob = _np.expand_dims(y_prob.to_numpy(), axis=-1)
+
     if isinstance(y_prob, list):
         if len(y_prob) > 0 and isinstance(y_prob[0], (list | _np.ndarray)):
             if len(y_prob[0]) == 1: # [[1], [0], [1]]
                 if 0 <= _np.max(y_prob) <= 2:
                     return True
         elif len(y_prob) > 0: # [0, 1, 1, 0, 1]
             if 0 <= max(y_prob) <= 2:
@@ -67,21 +77,21 @@
     if _tf.is_tensor(y_prob):
         if y_prob.get_shape().ndims == 2 and y_prob.shape[1] == 1 and 0 <= _tf.math.reduce_max(y_prob) <= 2:  # [[1], [0], [1]]
             return True
         elif y_prob.get_shape().ndims == 1 and 0 <= _tf.math.reduce_max(y_prob) <= 2:  # [0, 1, 1, 0, 1]
             return True
 
         return False
-    elif isinstance(y_prob, _pd.DataFrame):
-        if y_prob.ndims == 2 and y_prob.shape[1] == 1 and 0 <= y_prob.max() <= 2:  # [[1], [0], [1]]
-            return True
-        elif y_prob.ndims == 1 and 0 <= y_prob.max() <= 2:  # [0, 1, 1, 0, 1]
-            return True
-
-        return False
+    # elif isinstance(y_prob, _pd.DataFrame):
+    #     if y_prob.ndims == 2 and y_prob.shape[1] == 1 and 0 <= y_prob.max() <= 2:  # [[1], [0], [1]]
+    #         return True
+    #     elif y_prob.ndims == 1 and 0 <= y_prob.max() <= 2:  # [0, 1, 1, 0, 1]
+    #         return True
+    #
+    #     return False
     elif isinstance(y_prob, _np.ndarray):
         if y_prob.ndim == 2 and y_prob.shape[1] == 1 and 0 <= _np.max(y_prob) <= 2:  # [[1], [0], [1]]
             return True
         elif y_prob.ndim == 1 and 0 <= _np.max(y_prob) <= 2:  # [0, 1, 1, 0, 1]
             return True
 
         return False
```

### Comparing `so-ml-tools-0.1.98/so_ml_tools.egg-info/SOURCES.txt` & `so-ml-tools-0.1.99/so_ml_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

