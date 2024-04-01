# Comparing `tmp/tensorneko-0.3.8.tar.gz` & `tmp/tensorneko-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko-0.3.8.tar", last modified: Mon Feb  5 02:39:46 2024, max compression
+gzip compressed data, was "tensorneko-0.3.9.tar", last modified: Mon Feb 19 00:53:59 2024, max compression
```

## Comparing `tensorneko-0.3.8.tar` & `tensorneko-0.3.9.tar`

### file list

```diff
@@ -1,120 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-05 02:37:47.000000 tensorneko-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-02-05 02:39:46.573598 tensorneko-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-02-05 02:37:47.000000 tensorneko-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 02:39:46.573598 tensorneko-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-05 02:37:47.000000 tensorneko-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.561598 tensorneko-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.561598 tensorneko-0.3.8/src/tensorneko/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/arch/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/binary_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/arch/wgan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/callback/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/display_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/earlystop_lr.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/epoch_num_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/epoch_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/gpu_stats_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/lr_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/nil_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/callback/system_stats_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/nested_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/round_robin_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/dataset/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/dataset/sampler/sequential_iter_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/debug/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/secs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/evaluation/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.565598 tensorneko-0.3.8/src/tensorneko/io/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/mesh/mesh_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/mesh/mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/layer/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/masked_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/layer/vector_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/module/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/inception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/module/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/neko_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/neko_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/neko_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/optim/lr_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.569598 tensorneko-0.3.8/src/tensorneko/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/preprocess/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/src/tensorneko/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/string_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/util/type.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/src/tensorneko/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/src/tensorneko/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/visualization/log_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/visualization/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/src/tensorneko/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-05 02:37:47.000000 tensorneko-0.3.8/src/tensorneko/visualization/watcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.561598 tensorneko-0.3.8/src/tensorneko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-05 02:39:46.000000 tensorneko-0.3.8/src/tensorneko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 02:39:46.573598 tensorneko-0.3.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-05 02:37:47.000000 tensorneko-0.3.8/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-05 02:37:47.000000 tensorneko-0.3.8/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-19 00:51:56.000000 tensorneko-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-02-19 00:53:59.116953 tensorneko-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-02-19 00:51:56.000000 tensorneko-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 00:53:59.116953 tensorneko-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-19 00:51:56.000000 tensorneko-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.104952 tensorneko-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/binary_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/arch/wgan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/display_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/earlystop_lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/epoch_num_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/epoch_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/gpu_stats_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/lr_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/nil_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/callback/system_stats_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/nested_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/round_robin_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/dataset/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/dataset/sampler/sequential_iter_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.112953 tensorneko-0.3.9/src/tensorneko/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/secs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/evaluation/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.112953 tensorneko-0.3.9/src/tensorneko/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.112953 tensorneko-0.3.9/src/tensorneko/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/mesh/mesh_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/mesh/mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.112953 tensorneko-0.3.9/src/tensorneko/io/weight/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/weight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/weight/weight_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/weight/weight_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.112953 tensorneko-0.3.9/src/tensorneko/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/masked_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/layer/vector_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/inception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/module/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/neko_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/neko_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/neko_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/optim/lr_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/preprocess/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/string_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/visualization/log_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/visualization/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/src/tensorneko/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-19 00:51:56.000000 tensorneko-0.3.9/src/tensorneko/visualization/watcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.108953 tensorneko-0.3.9/src/tensorneko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 00:53:59.000000 tensorneko-0.3.9/src/tensorneko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 00:53:59.116953 tensorneko-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-19 00:51:56.000000 tensorneko-0.3.9/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-19 00:51:56.000000 tensorneko-0.3.9/test/test_version.py
```

### Comparing `tensorneko-0.3.8/LICENSE` & `tensorneko-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/PKG-INFO` & `tensorneko-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.8/README.md` & `tensorneko-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/setup.py` & `tensorneko-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/__init__.py` & `tensorneko-0.3.9/src/tensorneko/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os.path
 
-from tensorneko_util import io
 from . import backend
 from . import callback
 from . import dataset
 from . import debug
 from . import evaluation
+from . import io
 from . import layer
 from . import module
 from . import notebook
 from . import optim
 from . import preprocess
 from . import util
 from . import visualization
+from .io import read, write
 from .neko_model import NekoModel
 from .neko_module import NekoModule
 from .neko_trainer import NekoTrainer
 
+__version__ = io.read.text(os.path.join(util.get_tensorneko_path(), "version.txt"))
+
 __all__ = [
     "callback",
     "dataset",
     "backend",
     "evaluation",
     "io",
     "layer",
@@ -29,11 +32,13 @@
     "optim",
     "preprocess",
     "util",
     "visualization",
     "debug",
     "NekoModel",
     "NekoTrainer",
-    "NekoModule"
+    "NekoModule",
+    "read",
+    "write",
 ]
 
-__version__ = io.read.text(os.path.join(util.get_tensorneko_path(), "version.txt"))
+
```

### Comparing `tensorneko-0.3.8/src/tensorneko/arch/auto_encoder.py` & `tensorneko-0.3.9/src/tensorneko/arch/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/arch/binary_classifier.py` & `tensorneko-0.3.9/src/tensorneko/arch/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/arch/gan.py` & `tensorneko-0.3.9/src/tensorneko/arch/gan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/arch/vqvae.py` & `tensorneko-0.3.9/src/tensorneko/arch/vqvae.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/arch/wgan.py` & `tensorneko-0.3.9/src/tensorneko/arch/wgan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/__init__.py` & `tensorneko-0.3.9/src/tensorneko/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/earlystop_lr.py` & `tensorneko-0.3.9/src/tensorneko/callback/earlystop_lr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/epoch_time_logger.py` & `tensorneko-0.3.9/src/tensorneko/callback/epoch_time_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/gpu_stats_logger.py` & `tensorneko-0.3.9/src/tensorneko/callback/gpu_stats_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/lr_logger.py` & `tensorneko-0.3.9/src/tensorneko/callback/lr_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/callback/system_stats_logger.py` & `tensorneko-0.3.9/src/tensorneko/callback/system_stats_logger.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/dataset/list_dataset.py` & `tensorneko-0.3.9/src/tensorneko/dataset/list_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/dataset/nested_dataset.py` & `tensorneko-0.3.9/src/tensorneko/dataset/nested_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/dataset/round_robin_dataset.py` & `tensorneko-0.3.9/src/tensorneko/dataset/round_robin_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/dataset/sampler/sequential_iter_sampler.py` & `tensorneko-0.3.9/src/tensorneko/dataset/sampler/sequential_iter_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/evaluation/fid.py` & `tensorneko-0.3.9/src/tensorneko/evaluation/fid.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from torch import Tensor
 from torch.types import Device
 from torch.utils.data import IterableDataset
 from torchmetrics.image.fid import FrechetInceptionDistance
 from torchvision.transforms.functional import resize
 
 from tensorneko_util.backend import VisualLib
-from tensorneko_util.backend._tqdm import import_tqdm_auto
+from tensorneko_util.backend.tqdm import import_tqdm_auto
 
 try:
     from typing import Literal
     TypeOption = Literal["video", "image"]
 except ImportError:
+    Literal = None
     TypeOption = str
 
 
 class FID:
     """
     Calculate Fréchet inception distance based on torchmetrics. Require library "torch-fidelity".
```

### Comparing `tensorneko-0.3.8/src/tensorneko/evaluation/iou.py` & `tensorneko-0.3.9/src/tensorneko/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/evaluation/psnr.py` & `tensorneko-0.3.9/src/tensorneko/evaluation/psnr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/evaluation/secs.py` & `tensorneko-0.3.9/src/tensorneko/evaluation/secs.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/evaluation/ssim.py` & `tensorneko-0.3.9/src/tensorneko/evaluation/ssim.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/io/reader.py` & `tensorneko-0.3.9/src/tensorneko/io/reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from __future__ import annotations
 from typing import Type
 
 from tensorneko_util.io.reader import Reader as BaseReader
+from .weight import WeightReader
 
 try:
     from .mesh import MeshReader
     pytorch3d_available = True
 except ImportError:
     MeshReader = object
     pytorch3d_available = False
 
 
 class Reader(BaseReader):
 
     def __init__(self):
         super().__init__()
+        self.weight = WeightReader
         self._mesh = None
 
     @property
     def mesh(self) -> Type[MeshReader]:
         if pytorch3d_available:
             if self._mesh is None:
                 from .mesh import MeshReader
```

### Comparing `tensorneko-0.3.8/src/tensorneko/io/writer.py` & `tensorneko-0.3.9/src/tensorneko/io/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 from typing import Type
 
 from tensorneko_util.io.writer import Writer as BaseWriter
+from .weight import WeightWriter
 
 try:
     from .mesh import MeshWriter
     pytorch3d_available = True
 except ImportError:
     MeshWriter = object
     pytorch3d_available = False
 
 
 class Writer(BaseWriter):
 
     def __init__(self):
         super().__init__()
+        self.weight = WeightWriter
         self._mesh = None
 
     @property
     def mesh(self) -> Type[MeshWriter]:
         if pytorch3d_available:
             if self._mesh is None:
                 from .mesh import MeshWriter
```

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/__init__.py` & `tensorneko-0.3.9/src/tensorneko/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/aggregation.py` & `tensorneko-0.3.9/src/tensorneko/layer/aggregation.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/attention.py` & `tensorneko-0.3.9/src/tensorneko/layer/attention.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/concatenate.py` & `tensorneko-0.3.9/src/tensorneko/layer/concatenate.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/conv.py` & `tensorneko-0.3.9/src/tensorneko/layer/conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/linear.py` & `tensorneko-0.3.9/src/tensorneko/layer/linear.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/log.py` & `tensorneko-0.3.9/src/tensorneko/layer/log.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/masked_conv2d.py` & `tensorneko-0.3.9/src/tensorneko/layer/masked_conv2d.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/noise.py` & `tensorneko-0.3.9/src/tensorneko/layer/noise.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         device (:class:`~tensorneko.util.type.Device`): The model running device. Default ``"cuda"``.
 
     References:
         Writing a simple Gaussian noise layer in Pytorch. (2017). Retrieved
         from https://discuss.pytorch.org/t/writing-a-simple-gaussian-noise-layer-in-pytorch/4694/3
     """
 
-    def __init__(self, sigma=0.1, device: Union[Device, str] = "cuda"):
+    def __init__(self, sigma=0.1, device: Device = "cuda"):
         super().__init__()
         self.sigma = sigma
         self.noise = torch.tensor(0.).to(device)
 
     def forward(self, x):
         if self.training and self.sigma != 0:
             scale = self.sigma * x.detach()
```

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/patching.py` & `tensorneko-0.3.9/src/tensorneko/layer/patching.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/positional_embedding.py` & `tensorneko-0.3.9/src/tensorneko/layer/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/reshape.py` & `tensorneko-0.3.9/src/tensorneko/layer/reshape.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/stack.py` & `tensorneko-0.3.9/src/tensorneko/layer/stack.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/layer/vector_quantizer.py` & `tensorneko-0.3.9/src/tensorneko/layer/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/dense.py` & `tensorneko-0.3.9/src/tensorneko/module/dense.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/gated_conv.py` & `tensorneko-0.3.9/src/tensorneko/module/gated_conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/inception.py` & `tensorneko-0.3.9/src/tensorneko/module/inception.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/mlp.py` & `tensorneko-0.3.9/src/tensorneko/module/mlp.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/residual.py` & `tensorneko-0.3.9/src/tensorneko/module/residual.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/module/transformer.py` & `tensorneko-0.3.9/src/tensorneko/module/transformer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/neko_model.py` & `tensorneko-0.3.9/src/tensorneko/neko_model.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/neko_module.py` & `tensorneko-0.3.9/src/tensorneko/neko_module.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/neko_trainer.py` & `tensorneko-0.3.9/src/tensorneko/neko_trainer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/preprocess/__init__.py` & `tensorneko-0.3.9/src/tensorneko/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/preprocess/crop.py` & `tensorneko-0.3.9/src/tensorneko/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/preprocess/enum.py` & `tensorneko-0.3.9/src/tensorneko/preprocess/enum.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/preprocess/pad.py` & `tensorneko-0.3.9/src/tensorneko/preprocess/pad.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/preprocess/resize.py` & `tensorneko-0.3.9/src/tensorneko/preprocess/resize.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/__init__.py` & `tensorneko-0.3.9/src/tensorneko/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/configuration.py` & `tensorneko-0.3.9/src/tensorneko/util/configuration.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/dispatched_misc.py` & `tensorneko-0.3.9/src/tensorneko/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/misc.py` & `tensorneko-0.3.9/src/tensorneko/util/misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/reproducibility.py` & `tensorneko-0.3.9/src/tensorneko/util/reproducibility.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/string_getter.py` & `tensorneko-0.3.9/src/tensorneko/util/string_getter.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/util/type.py` & `tensorneko-0.3.9/src/tensorneko/util/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from tensorneko_util.util.type import T, R, E, P, T1, T2, T3
 
 ModuleFactory = Union[Callable[[], Module], Callable[[int], Module]]
 """The module builder type of ``() -> torch.nn.Module | (int) -> torch.nn.Module``"""
 
 
-Device = device
+Device = Union[str, device]
 """Device type of :class:`torch.device`"""
 
 
 Shape = Union[Size, List[int], Tuple[int, ...]]
 """Shape type. Normally is ``List[int]``, ``Tuple[int, ...]`` or :class:`torch.Size`"""
```

### Comparing `tensorneko-0.3.8/src/tensorneko/visualization/__init__.py` & `tensorneko-0.3.9/src/tensorneko/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/visualization/log_graph.py` & `tensorneko-0.3.9/src/tensorneko/visualization/log_graph.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko/visualization/matplotlib.py` & `tensorneko-0.3.9/src/tensorneko/visualization/matplotlib.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.3.8/src/tensorneko.egg-info/PKG-INFO` & `tensorneko-0.3.9/src/tensorneko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.3.8
+Version: 0.3.9
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
```

### Comparing `tensorneko-0.3.8/src/tensorneko.egg-info/SOURCES.txt` & `tensorneko-0.3.9/src/tensorneko.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 src/tensorneko/evaluation/ssim.py
 src/tensorneko/io/__init__.py
 src/tensorneko/io/reader.py
 src/tensorneko/io/writer.py
 src/tensorneko/io/mesh/__init__.py
 src/tensorneko/io/mesh/mesh_reader.py
 src/tensorneko/io/mesh/mesh_writer.py
+src/tensorneko/io/weight/__init__.py
+src/tensorneko/io/weight/weight_reader.py
+src/tensorneko/io/weight/weight_writer.py
 src/tensorneko/layer/__init__.py
 src/tensorneko/layer/aggregation.py
 src/tensorneko/layer/attention.py
 src/tensorneko/layer/concatenate.py
 src/tensorneko/layer/conv.py
 src/tensorneko/layer/linear.py
 src/tensorneko/layer/log.py
```

### Comparing `tensorneko-0.3.8/test/test_version.py` & `tensorneko-0.3.9/test/test_version.py`

 * *Files identical despite different names*

