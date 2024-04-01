# Comparing `tmp/efficientvit-gml-0.1.3.tar.gz` & `tmp/efficientvit-gml-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficientvit-gml-0.1.3.tar", last modified: Mon Apr  1 16:12:00 2024, max compression
+gzip compressed data, was "efficientvit-gml-0.1.4.tar", last modified: Mon Apr  1 16:49:05 2024, max compression
```

## Comparing `efficientvit-gml-0.1.3.tar` & `efficientvit-gml-0.1.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.404379 efficientvit-gml-0.1.3/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    11341 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/LICENSE
--rw-r--r--   0 michelle  (1001) michelle  (1001)    13707 2024-04-01 16:12:00.404379 efficientvit-gml-0.1.3/PKG-INFO
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5633 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/README.md
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.392378 efficientvit-gml-0.1.3/demo/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/demo/sam/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     9056 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/gradio_web_server.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/demo/sam/helpers/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3580 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/auto_mask_generator.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/demo/sam/helpers/predictors/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       66 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/predictors/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3894 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_onnx.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4478 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_pytorch.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5855 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_tensorrt.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      115 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3409 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_onnx.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3938 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_pytorch.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5259 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_tensorrt.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5257 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/helpers/utils.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1972 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/demo/sam/process_prompts.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/deployment/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/deployment/sam/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/deployment/sam/onnx/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       85 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/onnx/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     6119 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/onnx/export_decoder.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4178 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/onnx/export_encoder.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     9867 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/onnx/inference.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/deployment/sam/tensorrt/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       25 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/tensorrt/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     9235 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/deployment/sam/tensorrt/inference.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/efficientvit/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/efficientvit/apps/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      271 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.396378 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      240 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      786 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/bbox.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2523 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/color_aug.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     7784 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/base.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      273 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    75054 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/_data_loader.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    13589 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/_data_worker.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2973 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/controller.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4537 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/setup.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/apps/trainer/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      241 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/trainer/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    10759 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/trainer/base.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4245 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/trainer/run_config.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/apps/utils/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      355 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1872 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/dist.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1520 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/ema.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1385 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/export.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2628 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/init.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1610 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/lr.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1193 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/metric.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3325 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/misc.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1137 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/apps/utils/opt.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3096 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/cls_model_zoo.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/clscore/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/clscore/data_provider/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      219 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/data_provider/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4403 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/data_provider/imagenet.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      252 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      529 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/cls_run_config.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     9198 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/cls_trainer.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      266 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      678 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/label_smooth.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      750 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/metric.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1897 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/mixup.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/models/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/__init__.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      276 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    12527 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/backbone.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     4714 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/cls.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    23011 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/sam.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    10590 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/efficientvit/seg.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.400378 efficientvit-gml-0.1.3/efficientvit/models/nn/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      273 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/nn/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      818 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/nn/act.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2923 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/nn/drop.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5098 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/nn/norm.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)    16077 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/nn/ops.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.404379 efficientvit-gml-0.1.3/efficientvit/models/utils/
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      260 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/utils/__init__.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1378 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/utils/list.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2219 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/utils/network.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2143 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/models/utils/random.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     1715 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/sam_model_zoo.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     2455 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/efficientvit/seg_model_zoo.py
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       22 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit/version.py
-drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:12:00.404379 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/
--rw-r--r--   0 michelle  (1001) michelle  (1001)    13707 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/PKG-INFO
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     3179 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/SOURCES.txt
--rw-rw-r--   0 michelle  (1001) michelle  (1001)        1 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/dependency_links.txt
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      292 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/requires.txt
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       29 2024-04-01 16:12:00.000000 efficientvit-gml-0.1.3/efficientvit_gml.egg-info/top_level.txt
--rw-rw-r--   0 michelle  (1001) michelle  (1001)      298 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.3/pyproject.toml
--rw-rw-r--   0 michelle  (1001) michelle  (1001)       38 2024-04-01 16:12:00.404379 efficientvit-gml-0.1.3/setup.cfg
--rw-rw-r--   0 michelle  (1001) michelle  (1001)     5168 2024-04-01 16:11:05.000000 efficientvit-gml-0.1.3/setup.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    11341 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/LICENSE
+-rw-r--r--   0 michelle  (1001) michelle  (1001)    13707 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/PKG-INFO
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5633 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/README.md
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/demo/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/demo/sam/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     9056 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/gradio_web_server.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/demo/sam/helpers/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3580 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/auto_mask_generator.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/demo/sam/helpers/predictors/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       66 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/predictors/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3894 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_onnx.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4478 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_pytorch.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5855 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_tensorrt.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      115 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3409 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_onnx.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3938 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_pytorch.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5259 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_tensorrt.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5257 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/helpers/utils.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1972 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/demo/sam/process_prompts.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/deployment/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/deployment/sam/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.422113 efficientvit-gml-0.1.4/deployment/sam/onnx/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       85 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/onnx/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     6119 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/onnx/export_decoder.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4178 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/onnx/export_encoder.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     9867 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/onnx/inference.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/deployment/sam/tensorrt/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       25 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/tensorrt/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     9235 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/deployment/sam/tensorrt/inference.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      271 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      240 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      786 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/bbox.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2523 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/color_aug.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     7784 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/base.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      273 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    75054 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/_data_loader.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    13589 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/_data_worker.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2973 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/controller.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4537 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/setup.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/trainer/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      241 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/trainer/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    10759 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/trainer/base.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4245 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/trainer/run_config.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/apps/utils/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      355 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1872 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/dist.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1520 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/ema.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1385 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/export.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2628 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/init.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1610 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/lr.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1193 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/metric.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3325 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/misc.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1137 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/apps/utils/opt.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3096 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/cls_model_zoo.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/clscore/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.426113 efficientvit-gml-0.1.4/efficientvit/clscore/data_provider/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      219 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/data_provider/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4403 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/data_provider/imagenet.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      252 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      529 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/cls_run_config.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     9198 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/cls_trainer.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      266 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      678 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/label_smooth.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      750 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/metric.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1897 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/mixup.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/models/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        0 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/__init__.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      276 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    12527 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/backbone.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     4714 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/cls.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    23011 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/sam.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    10590 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/efficientvit/seg.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/models/nn/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      273 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/nn/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      818 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/nn/act.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2923 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/nn/drop.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5098 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/nn/norm.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)    16077 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/nn/ops.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit/models/utils/
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      260 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/utils/__init__.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1378 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/utils/list.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2219 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/utils/network.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2143 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/models/utils/random.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     1715 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/sam_model_zoo.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     2455 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/efficientvit/seg_model_zoo.py
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       22 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit/version.py
+drwxrwxr-x   0 michelle  (1001) michelle  (1001)        0 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/
+-rw-r--r--   0 michelle  (1001) michelle  (1001)    13707 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/PKG-INFO
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     3179 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/SOURCES.txt
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)        1 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/dependency_links.txt
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      292 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/requires.txt
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       29 2024-04-01 16:49:05.000000 efficientvit-gml-0.1.4/efficientvit_gml.egg-info/top_level.txt
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)      298 2024-04-01 05:12:15.000000 efficientvit-gml-0.1.4/pyproject.toml
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)       38 2024-04-01 16:49:05.430113 efficientvit-gml-0.1.4/setup.cfg
+-rw-rw-r--   0 michelle  (1001) michelle  (1001)     5168 2024-04-01 16:38:45.000000 efficientvit-gml-0.1.4/setup.py
```

### Comparing `efficientvit-gml-0.1.3/LICENSE` & `efficientvit-gml-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/PKG-INFO` & `efficientvit-gml-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficientvit-gml
-Version: 0.1.3
+Version: 0.1.4
 Summary: open-set object detector
 Home-page: https://github.com/mit-han-lab/efficientvit
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `efficientvit-gml-0.1.3/README.md` & `efficientvit-gml-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/gradio_web_server.py` & `efficientvit-gml-0.1.4/demo/sam/gradio_web_server.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/auto_mask_generator.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/auto_mask_generator.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_onnx.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_onnx.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_pytorch.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_pytorch.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/predictors/effvit_sam_tensorrt.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/predictors/effvit_sam_tensorrt.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_onnx.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_onnx.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_pytorch.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_pytorch.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/segmentation/process_prompts_tensorrt.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/segmentation/process_prompts_tensorrt.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/helpers/utils.py` & `efficientvit-gml-0.1.4/demo/sam/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/demo/sam/process_prompts.py` & `efficientvit-gml-0.1.4/demo/sam/process_prompts.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/deployment/sam/onnx/export_decoder.py` & `efficientvit-gml-0.1.4/deployment/sam/onnx/export_decoder.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/deployment/sam/onnx/export_encoder.py` & `efficientvit-gml-0.1.4/deployment/sam/onnx/export_encoder.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/deployment/sam/onnx/inference.py` & `efficientvit-gml-0.1.4/deployment/sam/onnx/inference.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/deployment/sam/tensorrt/inference.py` & `efficientvit-gml-0.1.4/deployment/sam/tensorrt/inference.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/bbox.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/bbox.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/augment/color_aug.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/augment/color_aug.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/base.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/base.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/_data_loader.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/_data_loader.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/_data_worker.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/_data_worker.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/data_provider/random_resolution/controller.py` & `efficientvit-gml-0.1.4/efficientvit/apps/data_provider/random_resolution/controller.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/setup.py` & `efficientvit-gml-0.1.4/efficientvit/apps/setup.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/trainer/base.py` & `efficientvit-gml-0.1.4/efficientvit/apps/trainer/base.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/trainer/run_config.py` & `efficientvit-gml-0.1.4/efficientvit/apps/trainer/run_config.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/dist.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/dist.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/ema.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/ema.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/export.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/export.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/init.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/init.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/lr.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/lr.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/metric.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/metric.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/misc.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/misc.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/apps/utils/opt.py` & `efficientvit-gml-0.1.4/efficientvit/apps/utils/opt.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/cls_model_zoo.py` & `efficientvit-gml-0.1.4/efficientvit/cls_model_zoo.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/data_provider/imagenet.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/data_provider/imagenet.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/trainer/cls_run_config.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/trainer/cls_run_config.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/trainer/cls_trainer.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/trainer/cls_trainer.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/label_smooth.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/label_smooth.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/metric.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/metric.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/clscore/trainer/utils/mixup.py` & `efficientvit-gml-0.1.4/efficientvit/clscore/trainer/utils/mixup.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/efficientvit/backbone.py` & `efficientvit-gml-0.1.4/efficientvit/models/efficientvit/backbone.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/efficientvit/cls.py` & `efficientvit-gml-0.1.4/efficientvit/models/efficientvit/cls.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/efficientvit/sam.py` & `efficientvit-gml-0.1.4/efficientvit/models/efficientvit/sam.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/efficientvit/seg.py` & `efficientvit-gml-0.1.4/efficientvit/models/efficientvit/seg.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/nn/act.py` & `efficientvit-gml-0.1.4/efficientvit/models/nn/act.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/nn/drop.py` & `efficientvit-gml-0.1.4/efficientvit/models/nn/drop.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/nn/norm.py` & `efficientvit-gml-0.1.4/efficientvit/models/nn/norm.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/nn/ops.py` & `efficientvit-gml-0.1.4/efficientvit/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/utils/list.py` & `efficientvit-gml-0.1.4/efficientvit/models/utils/list.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/utils/network.py` & `efficientvit-gml-0.1.4/efficientvit/models/utils/network.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/models/utils/random.py` & `efficientvit-gml-0.1.4/efficientvit/models/utils/random.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/sam_model_zoo.py` & `efficientvit-gml-0.1.4/efficientvit/sam_model_zoo.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit/seg_model_zoo.py` & `efficientvit-gml-0.1.4/efficientvit/seg_model_zoo.py`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/efficientvit_gml.egg-info/PKG-INFO` & `efficientvit-gml-0.1.4/efficientvit_gml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficientvit-gml
-Version: 0.1.3
+Version: 0.1.4
 Summary: open-set object detector
 Home-page: https://github.com/mit-han-lab/efficientvit
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `efficientvit-gml-0.1.3/efficientvit_gml.egg-info/SOURCES.txt` & `efficientvit-gml-0.1.4/efficientvit_gml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efficientvit-gml-0.1.3/setup.py` & `efficientvit-gml-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import os
 import subprocess
 import sys
 
 from setuptools import find_packages, setup
 
 # groundingdino version info
-version = "0.1.3"
+version = "0.1.4"
 package_name = "efficientvit-gml"
 cwd = os.path.dirname(os.path.abspath(__file__))
 
 
 def write_version_file():
     version_path = os.path.join(cwd, "efficientvit", "version.py")
     with open(version_path, "w") as f:
```

