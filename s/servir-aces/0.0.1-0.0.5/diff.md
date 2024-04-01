# Comparing `tmp/servir-aces-0.0.1.tar.gz` & `tmp/servir-aces-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servir-aces-0.0.1.tar", last modified: Sun Mar 24 22:54:56 2024, max compression
+gzip compressed data, was "servir-aces-0.0.5.tar", last modified: Mon Apr  1 21:01:31 2024, max compression
```

## Comparing `servir-aces-0.0.1.tar` & `servir-aces-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:56.530147 servir-aces-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-24 22:54:45.000000 servir-aces-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-24 22:54:45.000000 servir-aces-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-24 22:54:56.530147 servir-aces-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-24 22:54:45.000000 servir-aces-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:56.526147 servir-aces-0.0.1/aces/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25317 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20938 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/ee_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20493 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/remote_sensing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-03-24 22:54:45.000000 servir-aces-0.0.1/aces/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:56.526147 servir-aces-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:45.000000 servir-aces-0.0.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-24 22:54:45.000000 servir-aces-0.0.1/examples/count_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-24 22:54:45.000000 servir-aces-0.0.1/examples/run_model_example.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:45.000000 servir-aces-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:56.530147 servir-aces-0.0.1/servir_aces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-24 22:54:56.000000 servir-aces-0.0.1/servir_aces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-24 22:54:56.000000 servir-aces-0.0.1/servir_aces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 22:54:56.000000 servir-aces-0.0.1/servir_aces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-24 22:54:56.000000 servir-aces-0.0.1/servir_aces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-24 22:54:56.000000 servir-aces-0.0.1/servir_aces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 22:54:56.530147 servir-aces-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-24 22:54:45.000000 servir-aces-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 22:54:56.530147 servir-aces-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-24 22:54:45.000000 servir-aces-0.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.177303 servir-aces-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.165303 servir-aces-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.169303 servir-aces-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.169303 servir-aces-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-01 21:01:20.000000 servir-aces-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-01 21:01:20.000000 servir-aces-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-01 21:01:20.000000 servir-aces-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 21:01:20.000000 servir-aces-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-01 21:01:31.177303 servir-aces-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-01 21:01:20.000000 servir-aces-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.173303 servir-aces-0.0.5/aces/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25272 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20938 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/remote_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-01 21:01:20.000000 servir-aces-0.0.5/aces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.173303 servir-aces-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/data_processor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/ee_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/model_builder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/model_trainer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.173303 servir-aces-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/remote_sensing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 21:01:20.000000 servir-aces-0.0.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.173303 servir-aces-0.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:20.000000 servir-aces-0.0.5/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 21:01:20.000000 servir-aces-0.0.5/examples/count_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-01 21:01:20.000000 servir-aces-0.0.5/examples/run_model_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-01 21:01:20.000000 servir-aces-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 21:01:20.000000 servir-aces-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 21:01:20.000000 servir-aces-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 21:01:20.000000 servir-aces-0.0.5/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.177303 servir-aces-0.0.5/servir_aces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-01 21:01:31.000000 servir-aces-0.0.5/servir_aces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-01 21:01:31.000000 servir-aces-0.0.5/servir_aces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:01:31.000000 servir-aces-0.0.5/servir_aces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 21:01:31.000000 servir-aces-0.0.5/servir_aces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 21:01:31.000000 servir-aces-0.0.5/servir_aces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:01:31.177303 servir-aces-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.177303 servir-aces-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 21:01:20.000000 servir-aces-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.165303 servir-aces-0.0.5/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.177303 servir-aces-0.0.5/workflow/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v1/1.s1_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:31.177303 servir-aces-0.0.5/workflow/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/1.planet_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/2.generate_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/4.export_image_for_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/5.prediction_dnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/5.prediction_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/generate_training_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-01 21:01:20.000000 servir-aces-0.0.5/workflow/v2/host_vertex_ai.py
```

### Comparing `servir-aces-0.0.1/LICENSE` & `servir-aces-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/PKG-INFO` & `servir-aces-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.1
+Version: 0.0.5
 Summary: Agricultural Classification and Estimation Service (ACES)
-Home-page: https://github.com/SERVIR/servir-aces
-Author: Biplov Bhandari
-Author-email: bb0134@uah.edu; bionicbiplov45@gmail.com
-License: GNU GPL v3.0
+Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
+License: GNU General Public License v3.0
+Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: tensorflow>=2.9.3
 Requires-Dist: apache-beam>=2.38.0
 Requires-Dist: earthengine-api
```

### Comparing `servir-aces-0.0.1/README.md` & `servir-aces-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/aces/config.py` & `servir-aces-0.0.5/aces/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 ACES Configuration Module
 This module provides the configuration settings for the ACES project.
 """
 
 from pathlib import Path
 import os
 import ast
-
 from dotenv import load_dotenv
-load_dotenv(".env")
 
 
 class Config:
     """
     ACES Configuration Class
 
     This class contains the configuration settings for the ACES project. These are generated from the .env file.
@@ -92,185 +90,123 @@
         GCS_VERTEX_CONTAINER_IMAGE (str): The Google Cloud Storage Vertex AI container image.
         # AI platform expects a need a serialized model, this parameter does this.
         # See its uses in `data_processor.py` and `model_training.py`
         USE_AI_PLATFORM (bool): Flag to use Google Cloud AI Platform.
         # Get machine type here: https://cloud.google.com/vertex-ai/docs/predictions/configure-compute
         GCP_MACHINE_TYPE (str): The Google Cloud Platform machine type.
     """
-    BASEDIR = Path(os.getenv("BASEDIR"))
-    DATADIR = BASEDIR / os.getenv("DATADIR")
-
-    TRAINING_DIR = DATADIR / "training"
-    TESTING_DIR = DATADIR / "testing"
-    VALIDATION_DIR= DATADIR / "validation"
-
-    OUTPUT_DIR = BASEDIR / os.getenv("OUTPUT_DIR")
-
-    MODEL_NAME = os.getenv("MODEL_NAME")
-    MODEL_CHECKPOINT_NAME = os.getenv("MODEL_CHECKPOINT_NAME")
-
-    MODEL_DIR_NAME = os.getenv("MODEL_DIR_NAME")
-
-    MODEL_DIR = OUTPUT_DIR / MODEL_DIR_NAME
 
-    AUTO_MODEL_DIR_NAME = os.getenv("AUTO_MODEL_DIR_NAME") == "True"
-    SCALE = int(os.getenv("SCALE"))
+    def __init__(self, config_file) -> None:
 
-    FEATURES = os.getenv("FEATURES").split("\n")
-    ADDED_FEATURES = os.getenv("ADDED_FEATURES").split("\n")
-    USE_ELEVATION = os.getenv("USE_ELEVATION") == "True"
-    USE_S1 = os.getenv("USE_S1") == "True"
-    LABELS = ast.literal_eval(os.getenv("LABELS"))
+        load_dotenv(config_file)
 
-    USE_SEED = os.getenv("USE_SEED") == "True"
-    SEED = int(os.getenv("SEED"))
+        self.BASEDIR = Path(os.getenv("BASEDIR"))
+        _DATADIR = os.getenv("DATADIR")
+        if _DATADIR.startswith("gs://"):
+            self.DATADIR = _DATADIR
+            self.TRAINING_DIR = f"{self.DATADIR}/training"
+            self.TESTING_DIR = f"{self.DATADIR}/testing"
+            self.VALIDATION_DIR = f"{self.DATADIR}/validation"
+        else:
+            self.DATADIR = self.BASEDIR / os.getenv("DATADIR")
+            self.TRAINING_DIR = self.DATADIR / "training"
+            self.TESTING_DIR = self.DATADIR / "testing"
+            self.VALIDATION_DIR= self.DATADIR / "validation"
 
-    # patch size for training
-    PATCH_SHAPE = ast.literal_eval(os.getenv("PATCH_SHAPE"))
-    PATCH_SHAPE_SINGLE = PATCH_SHAPE[0]
-    KERNEL_BUFFER = os.getenv("KERNEL_BUFFER")
-    if KERNEL_BUFFER == "0":
-        KERNEL_BUFFER = None
-    else:
-        KERNEL_BUFFER = ast.literal_eval(KERNEL_BUFFER)
+        print(f"BASEDIR: {self.BASEDIR}")
+        print(f"DATADIR: {self.DATADIR}")
 
-    # Sizes of the testing, and evaluation datasets
-    TRAIN_SIZE = int(os.getenv("TRAIN_SIZE"))
-    TEST_SIZE = int(os.getenv("TEST_SIZE"))
-    VAL_SIZE = int(os.getenv("VAL_SIZE"))
+        self.OUTPUT_DIR = self.BASEDIR / os.getenv("OUTPUT_DIR")
 
-    MODEL_TYPE = os.getenv("MODEL_TYPE")
-    IS_DNN = True if MODEL_TYPE == "dnn" else False
+        self.MODEL_NAME = os.getenv("MODEL_NAME")
+        self.MODEL_CHECKPOINT_NAME = os.getenv("MODEL_CHECKPOINT_NAME")
 
-    BATCH_SIZE = int(os.getenv("BATCH_SIZE"))
-    EPOCHS = int(os.getenv("EPOCHS"))
-    RAMPUP_EPOCHS = int(os.getenv("RAMPUP_EPOCHS"))
-    SUSTAIN_EPOCHS = int(os.getenv("SUSTAIN_EPOCHS"))
+        self.MODEL_DIR_NAME = os.getenv("MODEL_DIR_NAME")
 
-    USE_ADJUSTED_LR = os.getenv("USE_ADJUSTED_LR") == "True"
-    MAX_LR = float(os.getenv("MAX_LR"))
-    MID_LR = float(os.getenv("MID_LR"))
-    MIN_LR = float(os.getenv("MIN_LR"))
-    DROPOUT_RATE = float(os.getenv("DROPOUT_RATE"))
+        self.MODEL_DIR = self.OUTPUT_DIR / self.MODEL_DIR_NAME
 
-    LOSS = os.getenv("LOSS")
+        self.AUTO_MODEL_DIR_NAME = os.getenv("AUTO_MODEL_DIR_NAME") == "True"
+        self.SCALE = int(os.getenv("SCALE"))
 
-    OPTIMIZER = os.getenv("OPTIMIZER")
+        self.FEATURES = os.getenv("FEATURES").split("\n")
+        self.ADDED_FEATURES = os.getenv("ADDED_FEATURES").split("\n")
+        self.USE_ELEVATION = os.getenv("USE_ELEVATION") == "True"
+        self.USE_S1 = os.getenv("USE_S1") == "True"
+        self.LABELS = ast.literal_eval(os.getenv("LABELS"))
 
-    OUT_CLASS_NUM = int(os.getenv("OUT_CLASS_NUM"))
+        if self.USE_ELEVATION:
+                self.FEATURES.extend(["elevation", "slope"])
 
-    USE_BEST_MODEL_FOR_INFERENCE = os.getenv("USE_BEST_MODEL_FOR_INFERENCE") == "True"
+        if self.USE_S1:
+            self.FEATURES.extend(["vv_asc_before", "vh_asc_before", "vv_asc_during", "vh_asc_during",
+                                  "vv_desc_before", "vh_desc_before", "vv_desc_during", "vh_desc_during"])
 
-    ACTIVATION_FN = "sigmoid" if OUT_CLASS_NUM == 1 else "softmax"
-    CALLBACK_PARAMETER = os.getenv("CALLBACK_PARAMETER")
+        print(f"using features: {self.FEATURES}")
+        print(f"using labels: {self.LABELS}")
 
-    EARLY_STOPPING = os.getenv("EARLY_STOPPING") == "True"
-    TRANSFORM_DATA = os.getenv("TRANSFORM_DATA") == "True"
-    DERIVE_FEATURES = os.getenv("DERIVE_FEATURES") == "True"
+        self.USE_SEED = os.getenv("USE_SEED") == "True"
+        self.SEED = int(os.getenv("SEED"))
 
-    # EE settings
-    USE_SERVICE_ACCOUNT = os.getenv("USE_SERVICE_ACCOUNT") == "True"
-    EE_SERVICE_CREDENTIALS = os.getenv("EE_SERVICE_CREDENTIALS")
-    EE_USER = os.getenv("EE_USER")
-    EE_OUTPUT_ASSET = os.getenv("EE_OUTPUT_ASSET")
-    OUTPUT_NAME = os.getenv("OUTPUT_NAME")
+        self.PRINT_INFO = os.getenv("USE_SEED") == "True"
 
-    # cloud stuff
-    GCS_PROJECT = os.getenv("GCS_PROJECT")
-    GCS_BUCKET = os.getenv("GCS_BUCKET")
-    GCS_IMAGE_DIR = os.getenv("GCS_IMAGE_DIR")
-    GCS_IMAGE_PREFIX = os.getenv("GCS_IMAGE_PREFIX")
-    GCS_VERTEX_MODEL_SAVE_DIR = os.getenv("GCS_VERTEX_MODEL_SAVE_DIR")
-    GCS_REGION = os.getenv("GCS_REGION")
-    GCS_VERTEX_CONTAINER_IMAGE = os.getenv("GCS_VERTEX_CONTAINER_IMAGE")
+        # patch size for training
+        self.PATCH_SHAPE = ast.literal_eval(os.getenv("PATCH_SHAPE"))
+        self.PATCH_SHAPE_SINGLE = self.PATCH_SHAPE[0]
+        KERNEL_BUFFER = os.getenv("KERNEL_BUFFER")
+        if KERNEL_BUFFER == "0":
+            self.KERNEL_BUFFER = None
+        else:
+            self.KERNEL_BUFFER = ast.literal_eval(KERNEL_BUFFER)
 
-    USE_AI_PLATFORM = os.getenv("USE_AI_PLATFORM") == "True"
+        # Sizes of the testing, and evaluation datasets
+        self.TRAIN_SIZE = int(os.getenv("TRAIN_SIZE"))
+        self.TEST_SIZE = int(os.getenv("TEST_SIZE"))
+        self.VAL_SIZE = int(os.getenv("VAL_SIZE"))
 
-    GCP_MACHINE_TYPE = os.getenv("GCP_MACHINE_TYPE")
+        self.MODEL_TYPE = os.getenv("MODEL_TYPE")
+        self.IS_DNN = True if self.MODEL_TYPE == "dnn" else False
 
-    def __init__(self) -> None:
-        self.BASEDIR = Config.BASEDIR
-        self.DATADIR = Config.DATADIR
+        self.BATCH_SIZE = int(os.getenv("BATCH_SIZE"))
+        self.EPOCHS = int(os.getenv("EPOCHS"))
+        self.RAMPUP_EPOCHS = int(os.getenv("RAMPUP_EPOCHS"))
+        self.SUSTAIN_EPOCHS = int(os.getenv("SUSTAIN_EPOCHS"))
 
-        self.TRAINING_DIR = Config.TRAINING_DIR
-        print(f"TRAINING_DIR: {self.TRAINING_DIR}")
-        self.TESTING_DIR = Config.TESTING_DIR
-        self.VALIDATION_DIR = Config.VALIDATION_DIR
+        self.USE_ADJUSTED_LR = os.getenv("USE_ADJUSTED_LR") == "True"
+        self.MAX_LR = float(os.getenv("MAX_LR"))
+        self.MID_LR = float(os.getenv("MID_LR"))
+        self.MIN_LR = float(os.getenv("MIN_LR"))
+        self.DROPOUT_RATE = float(os.getenv("DROPOUT_RATE"))
 
-        self.OUTPUT_DIR = Config.OUTPUT_DIR
+        self.LOSS = os.getenv("LOSS")
 
-        self.MODEL_NAME = Config.MODEL_NAME
-        self.MODEL_CHECKPOINT_NAME = Config.MODEL_CHECKPOINT_NAME
-        self.MODEL_DIR_NAME = Config.MODEL_DIR_NAME
-        self.MODEL_DIR = Config.MODEL_DIR
-        self.AUTO_MODEL_DIR_NAME = Config.AUTO_MODEL_DIR_NAME
+        self.OPTIMIZER = os.getenv("OPTIMIZER")
 
-        self.SCALE = Config.SCALE
+        self.OUT_CLASS_NUM = int(os.getenv("OUT_CLASS_NUM"))
 
-        self.FEATURES = Config.FEATURES
-        self.ADDED_FEATURES = Config.ADDED_FEATURES
-        self.USE_ELEVATION = Config.USE_ELEVATION
-        self.USE_S1 = Config.USE_S1
-        self.LABELS = Config.LABELS
+        self.USE_BEST_MODEL_FOR_INFERENCE = os.getenv("USE_BEST_MODEL_FOR_INFERENCE") == "True"
 
-        self.USE_SEED = Config.USE_SEED
-        self.SEED = Config.SEED
+        self.ACTIVATION_FN = "sigmoid" if self.OUT_CLASS_NUM == 1 else "softmax"
+        self.CALLBACK_PARAMETER = os.getenv("CALLBACK_PARAMETER")
 
-        # patch size for training
-        self.PATCH_SHAPE = Config.PATCH_SHAPE
-        self.PATCH_SHAPE_SINGLE = Config.PATCH_SHAPE_SINGLE
-        self.KERNEL_BUFFER = Config.KERNEL_BUFFER
-
-        # Sizes of the testing, and evaluation datasets
-        self.TRAIN_SIZE = Config.TRAIN_SIZE
-        self.TEST_SIZE = Config.TEST_SIZE
-        self.VAL_SIZE = Config.VAL_SIZE
-
-        self.MODEL_TYPE = Config.MODEL_TYPE
-        self.IS_DNN = Config.IS_DNN
-
-        self.BATCH_SIZE = Config.BATCH_SIZE
-        print(f"BATCH_SIZE: {self.BATCH_SIZE}")
-        self.EPOCHS = Config.EPOCHS
-        self.RAMPUP_EPOCHS = Config.RAMPUP_EPOCHS
-        self.SUSTAIN_EPOCHS = Config.SUSTAIN_EPOCHS
-
-        self.USE_ADJUSTED_LR = Config.USE_ADJUSTED_LR
-        self.MAX_LR = Config.MAX_LR
-        self.MID_LR = Config.MID_LR
-        self.MIN_LR = Config.MIN_LR
-        self.DROPOUT_RATE = Config.DROPOUT_RATE
-
-        self.LOSS = Config.LOSS
-        self.OPTIMIZER = Config.OPTIMIZER
-
-        self.OUT_CLASS_NUM = Config.OUT_CLASS_NUM
-
-        self.USE_BEST_MODEL_FOR_INFERENCE = Config.USE_BEST_MODEL_FOR_INFERENCE
-
-        self.ACTIVATION_FN = Config.ACTIVATION_FN
-        self.CALLBACK_PARAMETER = Config.CALLBACK_PARAMETER
-
-        self.EARLY_STOPPING = Config.EARLY_STOPPING
-        self.TRANSFORM_DATA = Config.TRANSFORM_DATA
-        self.DERIVE_FEATURES = Config.DERIVE_FEATURES
+        self.EARLY_STOPPING = os.getenv("EARLY_STOPPING") == "True"
+        self.TRANSFORM_DATA = os.getenv("TRANSFORM_DATA") == "True"
+        self.DERIVE_FEATURES = os.getenv("DERIVE_FEATURES") == "True"
 
         # EE settings
-        self.USE_SERVICE_ACCOUNT = Config.USE_SERVICE_ACCOUNT
-        self.EE_SERVICE_CREDENTIALS = Config.EE_SERVICE_CREDENTIALS
-        self.EE_USER = Config.EE_USER
-        self.EE_OUTPUT_ASSET = Config.EE_OUTPUT_ASSET
-        self.OUTPUT_NAME = Config.OUTPUT_NAME
+        self.USE_SERVICE_ACCOUNT = os.getenv("USE_SERVICE_ACCOUNT") == "True"
+        self.EE_SERVICE_CREDENTIALS = os.getenv("EE_SERVICE_CREDENTIALS")
+        self.EE_USER = os.getenv("EE_USER")
+        self.EE_OUTPUT_ASSET = os.getenv("EE_OUTPUT_ASSET")
+        self.OUTPUT_NAME = os.getenv("OUTPUT_NAME")
 
         # cloud stuff
-        self.GCS_PROJECT = Config.GCS_PROJECT
-        self.GCS_BUCKET = Config.GCS_BUCKET
-        self.GCS_IMAGE_DIR = Config.GCS_IMAGE_DIR
-        self.GCS_IMAGE_PREFIX = Config.GCS_IMAGE_PREFIX
-
-        self.GCS_VERTEX_MODEL_SAVE_DIR = Config.GCS_VERTEX_MODEL_SAVE_DIR
-        self.GCS_REGION = Config.GCS_REGION
-        self.GCS_VERTEX_CONTAINER_IMAGE = Config.GCS_VERTEX_CONTAINER_IMAGE
+        self.GCS_PROJECT = os.getenv("GCS_PROJECT")
+        self.GCS_BUCKET = os.getenv("GCS_BUCKET")
+        self.GCS_IMAGE_DIR = os.getenv("GCS_IMAGE_DIR")
+        self.GCS_IMAGE_PREFIX = os.getenv("GCS_IMAGE_PREFIX")
+        self.GCS_VERTEX_MODEL_SAVE_DIR = os.getenv("GCS_VERTEX_MODEL_SAVE_DIR")
+        self.GCS_REGION = os.getenv("GCS_REGION")
+        self.GCS_VERTEX_CONTAINER_IMAGE = os.getenv("GCS_VERTEX_CONTAINER_IMAGE")
 
-        self.USE_AI_PLATFORM = Config.USE_AI_PLATFORM
+        self.USE_AI_PLATFORM = os.getenv("USE_AI_PLATFORM") == "True"
 
-        self.GCP_MACHINE_TYPE = Config.GCP_MACHINE_TYPE
+        self.GCP_MACHINE_TYPE = os.getenv("GCP_MACHINE_TYPE")
```

### Comparing `servir-aces-0.0.1/aces/data_processor.py` & `servir-aces-0.0.5/aces/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,29 @@
         """
         return tf.data.TFRecordDataset(filename, compression_type="GZIP")
 
     @staticmethod
     @tf.autograph.experimental.do_not_convert
     def get_sum_tensor(records):
         """
-        Get a single sample from a dataset.
+        Gets the total number of tensor record by mapping through them.
 
         Parameters:
 
         * records: The input tensor records.
 
         Returns:
 
-        * tf.Tensor: The single sample.
+        * tf.Tensor: The total number of tensor records.
         """
-        tensors = records.map(lambda x: tf.numpy_function(lambda _: 1, inp=[x], Tout=tf.int64), num_parallel_calls=tf.data.AUTOTUNE)
-        n_tensors = tensors.reduce(np.int64(0), lambda x, y: x + y).numpy()
+        dataset = records.map(lambda x, y: tf.constant(1, dtype=tf.int64), num_parallel_calls=tf.data.AUTOTUNE)
+        # ignores any error encountered while reading the records
+        # works with v2.x
+        dataset = dataset.apply(tf.data.experimental.ignore_errors())
+        n_tensors = dataset.reduce(np.int64(0), lambda x, y: x + y).numpy()
         return n_tensors
 
     @staticmethod
     def calculate_n_samples(**config):
         """
         Calculate the number of samples in the training, testing, and validation datasets.
 
@@ -70,36 +73,39 @@
         * int: The number of training samples.
 
         * int: The number of testing samples.
 
         * int: The number of validation samples.
 
         """
-        parser = partial(DataProcessor.parse_tfrecord_multi_label,
+        parser_tupler = partial(DataProcessor.parse_tfrecord,
                          patch_size=config.get("PATCH_SHAPE_SINGLE"),
                          features=config.get("FEATURES"),
-                         labels=config.get("LABELS"))
-        tupler = partial(DataProcessor.to_tuple_multi_label, depth=config.get("OUT_CLASS_NUM"), x_only=True)
+                         labels=config.get("LABELS"),
+                         x_only=False,
+                         depth=config.get("OUT_CLASS_NUM"))
 
         tf_training_records = tf.data.Dataset.list_files(f"{str(config.get('TRAINING_DIR'))}/*")\
                                              .interleave(DataProcessor.create_tfrecord_from_file, num_parallel_calls=tf.data.AUTOTUNE)
-        tf_training_records = tf_training_records.map(parser, num_parallel_calls=tf.data.AUTOTUNE)
-        tf_training_records = tf_training_records.map(tupler, num_parallel_calls=tf.data.AUTOTUNE)
+        tf_training_records = tf_training_records.map(parser_tupler, num_parallel_calls=tf.data.AUTOTUNE)
+
+
+        if config.get("PRINT_DATASET", False):
+            DataProcessor.print_dataset_info(tf_training_records, "Training")
+
         n_training_records = DataProcessor.get_sum_tensor(tf_training_records)
 
         tf_testing_records = tf.data.Dataset.list_files(f"{str(config.get('TESTING_DIR'))}/*")\
                                             .interleave(DataProcessor.create_tfrecord_from_file, num_parallel_calls=tf.data.AUTOTUNE)
-        tf_testing_records = tf_testing_records.map(parser, num_parallel_calls=tf.data.AUTOTUNE)
-        tf_testing_records = tf_testing_records.map(tupler, num_parallel_calls=tf.data.AUTOTUNE)
+        tf_testing_records = tf_testing_records.map(parser_tupler, num_parallel_calls=tf.data.AUTOTUNE)
         n_testing_records = DataProcessor.get_sum_tensor(tf_testing_records)
 
         tf_validation_records = tf.data.Dataset.list_files(f"{str(config.get('VALIDATION_DIR'))}/*")\
                                                .interleave(DataProcessor.create_tfrecord_from_file, num_parallel_calls=tf.data.AUTOTUNE)
-        tf_validation_records = tf_validation_records.map(parser, num_parallel_calls=tf.data.experimental.AUTOTUNE)
-        tf_validation_records = tf_validation_records.map(tupler, num_parallel_calls=tf.data.AUTOTUNE)
+        tf_validation_records = tf_validation_records.map(parser_tupler, num_parallel_calls=tf.data.AUTOTUNE)
         n_validation_records = DataProcessor.get_sum_tensor(tf_validation_records)
 
         return n_training_records, n_testing_records, n_validation_records
 
     @staticmethod
     def print_dataset_info(dataset: tf.data.Dataset, dataset_name: str) -> None:
         """
@@ -192,16 +198,16 @@
         ]
         proto_struct = dict(zip(keys, columns))
         inputs = tf.io.parse_single_example(example_proto, proto_struct)
         inputs_list = [inputs.get(key) for key in keys]
         stacked = tf.stack(inputs_list, axis=0)
         stacked = tf.transpose(stacked, [1, 2, 0])
         label = stacked[:, :, len(features):]
-        x = tf.one_hot(tf.cast(label[:, :, -1], tf.uint8), depth)
-        return stacked[:, :, :len(features)], x
+        y = tf.one_hot(tf.cast(label[:, :, -1], tf.uint8), depth)
+        return stacked[:, :, :len(features)], y
 
     @staticmethod
     @tf.function
     def to_tuple(dataset: tf.Tensor, n_features: int = None, inverse_labels: bool = False) -> tuple:
         """
         Convert a dataset to a tuple of features and labels.
 
@@ -531,15 +537,14 @@
 
         if kwargs.get("USE_AI_PLATFORM", False):
             parser = partial(DataProcessor.parse_tfrecord_multi_label, patch_size=patch_size, features=features, labels=labels)
             tupler = partial(DataProcessor.to_tuple_multi_label_ai_platform, depth=n_classes)
             parser_tupler = None
         else:
             parser_tupler = partial(DataProcessor.parse_tfrecord, patch_size=patch_size, features=features, labels=labels, depth=n_classes)
-            print(f'parser_tupler: {parser_tupler}')
 
         if parser_tupler is not None:
             dataset = dataset.map(parser_tupler, num_parallel_calls=tf.data.AUTOTUNE)
         else:
             dataset = dataset.map(parser, num_parallel_calls=tf.data.AUTOTUNE)
             dataset = dataset.map(tupler, num_parallel_calls=tf.data.AUTOTUNE)
```

### Comparing `servir-aces-0.0.1/aces/ee_utils.py` & `servir-aces-0.0.5/aces/ee_utils.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/aces/metrics.py` & `servir-aces-0.0.5/aces/metrics.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/aces/model_builder.py` & `servir-aces-0.0.5/aces/model_builder.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/aces/model_trainer.py` & `servir-aces-0.0.5/aces/model_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             # producable results
             import random
             logging.info(f"Using seed: {self.seed}")
             tf.random.set_seed(self.seed)
             np.random.seed(self.seed)
             random.seed(2)
 
+        # @ToDO: Create a way to autoload loss function from the list without if else
         if self.config.LOSS == "custom_focal_tversky_loss":
             self.config.LOSS = Metrics.focal_tversky_loss
             self.LOSS_TXT = Metrics.focal_tversky_loss.__func__.__name__ # "focal_tversky_loss"
         else:
             self.config.LOSS_TXT = self.config.LOSS
 
         self.model_builder = ModelBuilder(
@@ -96,15 +97,15 @@
         keras.backend.clear_session()
         logging.info("****************************************************************************")
         print(f"****************************** Configure memory growth... ************************")
         physical_devices = TFUtils.configure_memory_growth()
         self.config.physical_devices = physical_devices
         logging.info("****************************************************************************")
         logging.info("****************************** creating datasets... ************************")
-        self.create_datasets(print_info=True)
+        self.create_datasets(print_info=self.config.PRINT_INFO)
 
         if self.config.USE_AI_PLATFORM:
             logging.info("****************************************************************************")
             logging.info("******* building and compiling model for ai platform... ********************")
             self.build_and_compile_model_ai_platform()
         else:
             logging.info("****************************************************************************")
```

### Comparing `servir-aces-0.0.1/aces/remote_sensing.py` & `servir-aces-0.0.5/aces/remote_sensing.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/aces/utils.py` & `servir-aces-0.0.5/aces/utils.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.1/examples/count_sample_size.py` & `servir-aces-0.0.5/examples/count_sample_size.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,12 +13,17 @@
 
     from aces.config import Config
     from aces.data_processor import DataProcessor
 
 
 
 if __name__ == "__main__":
-    config = Config()
-    n_training_records, n_testing_records, n_validation_records = DataProcessor.calculate_n_samples(**config.__dict__)
+    config_file = "config.env"
+    config = Config(config_file)
+    # expand the config
+    additional_config = {
+        "PRINT_DATASET": True
+    }
+    n_training_records, n_testing_records, n_validation_records = DataProcessor.calculate_n_samples(**{**config.__dict__, **additional_config})
     logging.info(f"no of training records: {n_training_records}")
     logging.info(f"no of testing records: {n_testing_records}")
     logging.info(f"no of validation records: {n_validation_records}")
```

### Comparing `servir-aces-0.0.1/examples/run_model_example.py` & `servir-aces-0.0.5/examples/run_model_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 
     from aces.config import Config
     from aces.model_trainer import ModelTrainer
 
 
 
 if __name__ == "__main__":
-    config = Config()
+    config_file = "config.env"
+    config = Config(config_file)
     trainer = ModelTrainer(config)
     trainer.train_model()
```

### Comparing `servir-aces-0.0.1/servir_aces.egg-info/PKG-INFO` & `servir-aces-0.0.5/servir_aces.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.1
+Version: 0.0.5
 Summary: Agricultural Classification and Estimation Service (ACES)
-Home-page: https://github.com/SERVIR/servir-aces
-Author: Biplov Bhandari
-Author-email: bb0134@uah.edu; bionicbiplov45@gmail.com
-License: GNU GPL v3.0
+Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
+License: GNU General Public License v3.0
+Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: tensorflow>=2.9.3
 Requires-Dist: apache-beam>=2.38.0
 Requires-Dist: earthengine-api
```

