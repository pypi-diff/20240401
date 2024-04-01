# Comparing `tmp/lm-buddy-0.4.0.tar.gz` & `tmp/lm-buddy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm-buddy-0.4.0.tar", last modified: Mon Mar 18 19:38:23 2024, max compression
+gzip compressed data, was "lm-buddy-0.4.1.tar", last modified: Mon Apr  1 21:22:26 2024, max compression
```

## Comparing `lm-buddy-0.4.0.tar` & `lm-buddy-0.4.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.101427 lm-buddy-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.101427 lm-buddy-0.4.0/src/lm_buddy/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/buddy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.105427 lm-buddy-0.4.0/src/lm_buddy/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/cli/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/cli/finetune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.105427 lm-buddy-0.4.0/src/lm_buddy/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.105427 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/adapter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/asset_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/tokenizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/trainer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.105427 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/run_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.105427 lm-buddy-0.4.0/src/lm_buddy/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/lm_harness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/lm_harness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/jobs/configs/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/src/lm_buddy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/src/lm_buddy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18119 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 19:38:23.000000 lm-buddy-0.4.0/src/lm_buddy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:38:23.109427 lm-buddy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-18 19:38:19.000000 lm-buddy-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.679905 lm-buddy-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.683905 lm-buddy-0.4.1/src/lm_buddy/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/buddy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.683905 lm-buddy-0.4.1/src/lm_buddy/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/adapter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/asset_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/tokenizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/trainer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.687904 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/lm_harness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/lm_harness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/jobs/configs/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/src/lm_buddy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/src/lm_buddy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18120 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 21:22:26.000000 lm-buddy-0.4.1/src/lm_buddy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:22:26.691905 lm-buddy-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-01 21:22:17.000000 lm-buddy-0.4.1/tests/test_utils.py
```

### Comparing `lm-buddy-0.4.0/LICENSE.md` & `lm-buddy-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/PKG-INFO` & `lm-buddy-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-buddy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Ray-centric library for finetuning and evaluation of (large) language models.
 Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -283,15 +283,15 @@
 Currently, we are utilizing Ray clusters running Python 3.10.8.
 In order to avoid dependency/syntax errors when executing LM Buddy on Ray,
 installation of this package requires Python between `[3.10, 3.11)`.
 
 ## CLI usage
 
 LM Buddy exposes a CLI with a few commands, one for each type of job.
-To see all available job commands, run `lm_buddy run --help`
+You can explore the CLI options by running `lm-buddy --help`.
 
 Once LM Buddy is installed in your local Python environment, usage is as follows:
 ```
 # LLM finetuning
 lm_buddy finetune --config finetuning_config.yaml
 
 # LLM evaluation
```

### Comparing `lm-buddy-0.4.0/README.md` & `lm-buddy-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Currently, we are utilizing Ray clusters running Python 3.10.8.
 In order to avoid dependency/syntax errors when executing LM Buddy on Ray,
 installation of this package requires Python between `[3.10, 3.11)`.
 
 ## CLI usage
 
 LM Buddy exposes a CLI with a few commands, one for each type of job.
-To see all available job commands, run `lm_buddy run --help`
+You can explore the CLI options by running `lm-buddy --help`.
 
 Once LM Buddy is installed in your local Python environment, usage is as follows:
 ```
 # LLM finetuning
 lm_buddy finetune --config finetuning_config.yaml
 
 # LLM evaluation
```

### Comparing `lm-buddy-0.4.0/pyproject.toml` & `lm-buddy-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lm-buddy"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     { name = "Sean Friedowitz", email = "sean@mozilla.ai" },
     { name = "Aaron Gonzales", email = "aaron@mozilla.ai" },
     { name = "Vicki Boykis", email = "vicki@mozilla.ai" },
     { name = "Davide Eynard", email = "davide@mozilla.ai" },
 ]
 description = "Ray-centric library for finetuning and evaluation of (large) language models."
```

### Comparing `lm-buddy-0.4.0/src/lm_buddy/buddy.py` & `lm-buddy-0.4.1/src/lm_buddy/buddy.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/adapter_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/adapter_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/asset_loader.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/asset_loader.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/dataset_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/dataset_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/quantization_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/quantization_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/huggingface/trainer_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/huggingface/trainer_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/vllm.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/vllm.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_loader.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_loader.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/artifact_utils.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/run_config.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_config.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/integrations/wandb/run_utils.py` & `lm-buddy-0.4.1/src/lm_buddy/integrations/wandb/run_utils.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/finetuning.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/finetuning.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/lm_harness.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/lm_harness.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/_entrypoints/prometheus.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/_entrypoints/prometheus.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/common.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/common.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/configs/__init__.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/configs/base.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/base.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/configs/finetuning.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/finetuning.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/configs/lm_harness.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/lm_harness.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/jobs/configs/prometheus.py` & `lm-buddy-0.4.1/src/lm_buddy/jobs/configs/prometheus.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/paths.py` & `lm-buddy-0.4.1/src/lm_buddy/paths.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy/types.py` & `lm-buddy-0.4.1/src/lm_buddy/types.py`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/src/lm_buddy.egg-info/PKG-INFO` & `lm-buddy-0.4.1/src/lm_buddy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-buddy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Ray-centric library for finetuning and evaluation of (large) language models.
 Author-email: Sean Friedowitz <sean@mozilla.ai>, Aaron Gonzales <aaron@mozilla.ai>, Vicki Boykis <vicki@mozilla.ai>, Davide Eynard <davide@mozilla.ai>
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -283,15 +283,15 @@
 Currently, we are utilizing Ray clusters running Python 3.10.8.
 In order to avoid dependency/syntax errors when executing LM Buddy on Ray,
 installation of this package requires Python between `[3.10, 3.11)`.
 
 ## CLI usage
 
 LM Buddy exposes a CLI with a few commands, one for each type of job.
-To see all available job commands, run `lm_buddy run --help`
+You can explore the CLI options by running `lm-buddy --help`.
 
 Once LM Buddy is installed in your local Python environment, usage is as follows:
 ```
 # LLM finetuning
 lm_buddy finetune --config finetuning_config.yaml
 
 # LLM evaluation
```

### Comparing `lm-buddy-0.4.0/src/lm_buddy.egg-info/SOURCES.txt` & `lm-buddy-0.4.1/src/lm_buddy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 src/lm_buddy.egg-info/dependency_links.txt
 src/lm_buddy.egg-info/entry_points.txt
 src/lm_buddy.egg-info/requires.txt
 src/lm_buddy.egg-info/top_level.txt
 src/lm_buddy/cli/__init__.py
 src/lm_buddy/cli/evaluate.py
 src/lm_buddy/cli/finetune.py
+src/lm_buddy/cli/utils.py
 src/lm_buddy/integrations/__init__.py
 src/lm_buddy/integrations/vllm.py
 src/lm_buddy/integrations/huggingface/__init__.py
 src/lm_buddy/integrations/huggingface/adapter_config.py
 src/lm_buddy/integrations/huggingface/asset_loader.py
 src/lm_buddy/integrations/huggingface/dataset_config.py
 src/lm_buddy/integrations/huggingface/model_config.py
```

### Comparing `lm-buddy-0.4.0/src/lm_buddy.egg-info/requires.txt` & `lm-buddy-0.4.1/src/lm_buddy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lm-buddy-0.4.0/tests/test_utils.py` & `lm-buddy-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

