# Comparing `tmp/pytorch-ignite-0.5.0.post2.tar.gz` & `tmp/pytorch-ignite-0.6.0.dev20240401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.5.0.post2.tar", last modified: Mon Apr  1 12:21:49 2024, max compression
+gzip compressed data, was "pytorch-ignite-0.6.0.dev20240401.tar", last modified: Mon Apr  1 00:14:22 2024, max compression
```

## Comparing `pytorch-ignite-0.5.0.post2.tar` & `pytorch-ignite-0.6.0.dev20240401.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.138738 pytorch-ignite-0.5.0.post2/
--rw-rw-r--   0 root         (0) root         (0)     1527 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    27822 2024-04-01 12:21:49.138738 pytorch-ignite-0.5.0.post2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    27322 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.114739 pytorch-ignite-0.5.0.post2/ignite/
--rw-rw-r--   0 root         (0) root         (0)      188 2024-04-01 10:58:38.000000 pytorch-ignite-0.5.0.post2/ignite/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      182 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.114739 pytorch-ignite-0.5.0.post2/ignite/base/
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-28 23:43:55.000000 pytorch-ignite-0.5.0.post2/ignite/base/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      991 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/base/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.114739 pytorch-ignite-0.5.0.post2/ignite/contrib/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-28 23:43:55.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.114739 pytorch-ignite-0.5.0.post2/ignite/contrib/engines/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/engines/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28430 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/engines/common.py
--rw-rw-r--   0 root         (0) root         (0)     4508 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.114739 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/
--rw-rw-r--   0 root         (0) root         (0)     1073 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1182 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/base_logger.py
--rw-rw-r--   0 root         (0) root         (0)     1409 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/clearml_logger.py
--rw-rw-r--   0 root         (0) root         (0)      702 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/lr_finder.py
--rw-rw-r--   0 root         (0) root         (0)      940 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/mlflow_logger.py
--rw-rw-r--   0 root         (0) root         (0)     1319 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/neptune_logger.py
--rw-rw-r--   0 root         (0) root         (0)     1517 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/param_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)      962 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/polyaxon_logger.py
--rw-rw-r--   0 root         (0) root         (0)     1388 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/tensorboard_logger.py
--rw-rw-r--   0 root         (0) root         (0)      846 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/time_profilers.py
--rw-rw-r--   0 root         (0) root         (0)      703 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/tqdm_logger.py
--rw-rw-r--   0 root         (0) root         (0)     1212 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/visdom_logger.py
--rw-rw-r--   0 root         (0) root         (0)      929 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.118739 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/
--rw-rw-r--   0 root         (0) root         (0)      414 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      759 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/average_precision.py
--rw-rw-r--   0 root         (0) root         (0)      692 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/cohen_kappa.py
--rw-rw-r--   0 root         (0) root         (0)      659 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/gpu_info.py
--rw-rw-r--   0 root         (0) root         (0)      956 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.122738 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/
--rw-rw-r--   0 root         (0) root         (0)     2581 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2268 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/_base.py
--rw-rw-r--   0 root         (0) root         (0)      818 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/canberra_metric.py
--rw-rw-r--   0 root         (0) root         (0)      924 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)      818 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/fractional_bias.py
--rw-rw-r--   0 root         (0) root         (0)      964 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     1059 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)      851 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-rw-r--   0 root         (0) root         (0)      891 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)      953 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-rw-r--   0 root         (0) root         (0)      763 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_error.py
--rw-rw-r--   0 root         (0) root         (0)      869 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-rw-r--   0 root         (0) root         (0)      880 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)      997 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-rw-r--   0 root         (0) root         (0)      975 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)      741 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/r2_score.py
--rw-rw-r--   0 root         (0) root         (0)      869 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-rw-r--   0 root         (0) root         (0)      687 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.122738 pytorch-ignite-0.5.0.post2/ignite/distributed/
--rw-r--r--   0 root         (0) root         (0)      181 2022-11-28 23:43:55.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15401 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/auto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.122738 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/
--rw-rw-r--   0 root         (0) root         (0)     1357 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14021 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/base.py
--rw-rw-r--   0 root         (0) root         (0)     8143 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/horovod.py
--rw-rw-r--   0 root         (0) root         (0)    27705 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/native.py
--rw-rw-r--   0 root         (0) root         (0)     6174 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/xla.py
--rw-rw-r--   0 root         (0) root         (0)    13492 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/launcher.py
--rw-rw-r--   0 root         (0) root         (0)    22608 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/distributed/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.122738 pytorch-ignite-0.5.0.post2/ignite/engine/
--rw-rw-r--   0 root         (0) root         (0)    36118 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/engine/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11632 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/engine/deterministic.py
--rw-rw-r--   0 root         (0) root         (0)    54690 2024-04-01 10:58:38.000000 pytorch-ignite-0.5.0.post2/ignite/engine/engine.py
--rw-rw-r--   0 root         (0) root         (0)    21106 2024-04-01 10:58:38.000000 pytorch-ignite-0.5.0.post2/ignite/engine/events.py
--rw-rw-r--   0 root         (0) root         (0)     1073 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/engine/utils.py
--rw-r--r--   0 root         (0) root         (0)      150 2022-11-28 23:43:55.000000 pytorch-ignite-0.5.0.post2/ignite/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.126739 pytorch-ignite-0.5.0.post2/ignite/handlers/
--rw-rw-r--   0 root         (0) root         (0)     2641 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11793 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/base_logger.py
--rw-rw-r--   0 root         (0) root         (0)    44882 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)    37473 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/clearml_logger.py
--rw-rw-r--   0 root         (0) root         (0)     4139 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/early_stopping.py
--rw-rw-r--   0 root         (0) root         (0)    11854 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/ema_handler.py
--rw-rw-r--   0 root         (0) root         (0)     6781 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/fbresearch_logger.py
--rw-rw-r--   0 root         (0) root         (0)    22092 2024-04-01 10:58:38.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/lr_finder.py
--rw-rw-r--   0 root         (0) root         (0)    12315 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/mlflow_logger.py
--rw-rw-r--   0 root         (0) root         (0)    27366 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/neptune_logger.py
--rw-rw-r--   0 root         (0) root         (0)    68285 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/param_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)    12056 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/polyaxon_logger.py
--rw-rw-r--   0 root         (0) root         (0)    20745 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/state_param_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)     2616 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/stores.py
--rw-rw-r--   0 root         (0) root         (0)    26381 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/tensorboard_logger.py
--rw-rw-r--   0 root         (0) root         (0)     2103 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/terminate_on_nan.py
--rw-rw-r--   0 root         (0) root         (0)     1567 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/time_limit.py
--rw-rw-r--   0 root         (0) root         (0)    30228 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/time_profilers.py
--rw-rw-r--   0 root         (0) root         (0)     4705 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/timing.py
--rw-rw-r--   0 root         (0) root         (0)    13040 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/tqdm_logger.py
--rw-rw-r--   0 root         (0) root         (0)      872 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/utils.py
--rw-rw-r--   0 root         (0) root         (0)    21551 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/visdom_logger.py
--rw-rw-r--   0 root         (0) root         (0)    14346 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/handlers/wandb_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.134739 pytorch-ignite-0.5.0.post2/ignite/metrics/
--rw-rw-r--   0 root         (0) root         (0)     2713 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10988 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/accumulation.py
--rw-rw-r--   0 root         (0) root         (0)     9603 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/accuracy.py
--rw-rw-r--   0 root         (0) root         (0)     3231 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/average_precision.py
--rw-rw-r--   0 root         (0) root         (0)     5988 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/classification_report.py
--rw-rw-r--   0 root         (0) root         (0)     3594 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/cohen_kappa.py
--rw-rw-r--   0 root         (0) root         (0)    17742 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/confusion_matrix.py
--rw-rw-r--   0 root         (0) root         (0)     3977 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/cosine_similarity.py
--rw-rw-r--   0 root         (0) root         (0)     4016 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/entropy.py
--rw-rw-r--   0 root         (0) root         (0)     6882 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/epoch_metric.py
--rw-rw-r--   0 root         (0) root         (0)     6428 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/fbeta.py
--rw-rw-r--   0 root         (0) root         (0)     2966 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/frequency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.134739 pytorch-ignite-0.5.0.post2/ignite/metrics/gan/
--rw-rw-r--   0 root         (0) root         (0)      149 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/gan/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9978 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/gan/fid.py
--rw-rw-r--   0 root         (0) root         (0)     5565 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/gan/inception_score.py
--rw-rw-r--   0 root         (0) root         (0)     3988 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/gan/utils.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/gpu_info.py
--rw-rw-r--   0 root         (0) root         (0)     4425 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/loss.py
--rw-rw-r--   0 root         (0) root         (0)     3312 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/mean_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     3661 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/mean_pairwise_distance.py
--rw-rw-r--   0 root         (0) root         (0)     3296 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/mean_squared_error.py
--rw-rw-r--   0 root         (0) root         (0)    32127 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/metric.py
--rw-rw-r--   0 root         (0) root         (0)     7309 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/metrics_lambda.py
--rw-rw-r--   0 root         (0) root         (0)     6899 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/multilabel_confusion_matrix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.134739 pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/
--rw-rw-r--   0 root         (0) root         (0)      168 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11424 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/bleu.py
--rw-rw-r--   0 root         (0) root         (0)    15364 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/rouge.py
--rw-rw-r--   0 root         (0) root         (0)     2353 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/utils.py
--rw-rw-r--   0 root         (0) root         (0)    18160 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/precision.py
--rw-rw-r--   0 root         (0) root         (0)     5641 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/precision_recall_curve.py
--rw-rw-r--   0 root         (0) root         (0)     5073 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/psnr.py
--rw-rw-r--   0 root         (0) root         (0)     9484 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/recall.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.138738 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/
--rw-rw-r--   0 root         (0) root         (0)     1308 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2242 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/_base.py
--rw-rw-r--   0 root         (0) root         (0)     3077 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/canberra_metric.py
--rw-rw-r--   0 root         (0) root         (0)     3259 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/fractional_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     3172 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/fractional_bias.py
--rw-rw-r--   0 root         (0) root         (0)     3195 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/geometric_mean_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     4265 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     2788 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/manhattan_distance.py
--rw-rw-r--   0 root         (0) root         (0)     3009 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/maximum_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     3464 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_absolute_relative_error.py
--rw-rw-r--   0 root         (0) root         (0)     2957 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_error.py
--rw-rw-r--   0 root         (0) root         (0)     3167 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_normalized_bias.py
--rw-rw-r--   0 root         (0) root         (0)     2619 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     2745 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_absolute_percentage_error.py
--rw-rw-r--   0 root         (0) root         (0)     2749 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_relative_absolute_error.py
--rw-rw-r--   0 root         (0) root         (0)     4873 2024-03-31 20:18:42.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/pearson_correlation.py
--rw-rw-r--   0 root         (0) root         (0)     3404 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/r2_score.py
--rw-rw-r--   0 root         (0) root         (0)     2792 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/regression/wave_hedges_distance.py
--rw-rw-r--   0 root         (0) root         (0)     8164 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/roc_auc.py
--rw-rw-r--   0 root         (0) root         (0)     2520 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/root_mean_squared_error.py
--rw-rw-r--   0 root         (0) root         (0)    10859 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/running_average.py
--rw-rw-r--   0 root         (0) root         (0)     9312 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/ssim.py
--rw-rw-r--   0 root         (0) root         (0)     4254 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/metrics/top_k_categorical_accuracy.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/py.typed
--rw-rw-r--   0 root         (0) root         (0)    13624 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/ignite/utils.py
--rw-rw-r--   0 root         (0) root         (0)      762 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:21:49.138738 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/
--rw-r--r--   0 root         (0) root         (0)    27822 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5554 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-01 12:21:49.000000 pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      817 2024-04-01 12:21:49.138738 pytorch-ignite-0.5.0.post2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1310 2024-03-31 19:44:43.000000 pytorch-ignite-0.5.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.793318 pytorch-ignite-0.6.0.dev20240401/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-01 00:14:22.793318 pytorch-ignite-0.6.0.dev20240401/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.769317 pytorch-ignite-0.6.0.dev20240401/ignite/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 00:12:05.000000 pytorch-ignite-0.6.0.dev20240401/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.773317 pytorch-ignite-0.6.0.dev20240401/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.773317 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.773317 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28430 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.773317 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.773317 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.777318 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.777318 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.777318 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14021 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.781318 pytorch-ignite-0.6.0.dev20240401/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56579 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.785318 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44882 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37473 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/fbresearch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27366 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68285 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12056 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26381 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30228 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21551 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14346 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.789318 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10988 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.789318 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9978 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/multilabel_confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.789318 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/recall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.793318 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/pearson_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:14:22.793318 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27828 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 00:14:22.000000 pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 00:14:22.793318 pytorch-ignite-0.6.0.dev20240401/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 00:11:44.000000 pytorch-ignite-0.6.0.dev20240401/setup.py
```

### Comparing `pytorch-ignite-0.5.0.post2/LICENSE` & `pytorch-ignite-0.6.0.dev20240401/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/PKG-INFO` & `pytorch-ignite-0.6.0.dev20240401/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.post2
+Version: 0.6.0.dev20240401
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.post2/README.md` & `pytorch-ignite-0.6.0.dev20240401/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/base/mixins.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/engines/common.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/auto.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/launcher.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/distributed/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/engine/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/engine/deterministic.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/engine/engine.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import logging
+import math
 import time
 import warnings
 import weakref
 from collections import defaultdict, OrderedDict
 from collections.abc import Mapping
 from typing import Any, Callable, Dict, Generator, Iterable, Iterator, List, Optional, Tuple, Union
 
@@ -726,21 +727,22 @@
                     "If epoch is provided in the state dict, epoch_length should not be None. "
                     f"Input state_dict: {state_dict}"
                 )
             self.state.iteration = self.state.epoch_length * self.state.epoch
 
     @staticmethod
     def _is_done(state: State) -> bool:
+        is_done_iters = state.max_iters is not None and state.iteration >= state.max_iters
         is_done_count = (
             state.epoch_length is not None
             and state.max_epochs is not None
             and state.iteration >= state.epoch_length * state.max_epochs
         )
         is_done_epochs = state.max_epochs is not None and state.epoch >= state.max_epochs
-        return is_done_count or is_done_epochs
+        return is_done_iters or is_done_count or is_done_epochs
 
     def set_data(self, data: Union[Iterable, DataLoader]) -> None:
         """Method to set data. After calling the method the next batch passed to `processing_function` is
         from newly provided data. Please, note that epoch length is not modified.
 
         Args:
             data: Collection of batches allowing repeated iteration (e.g., list or `DataLoader`).
@@ -774,21 +776,22 @@
         self.state.dataloader = data
         self._dataloader_iter = iter(self.state.dataloader)
 
     def run(
         self,
         data: Optional[Iterable] = None,
         max_epochs: Optional[int] = None,
+        max_iters: Optional[int] = None,
         epoch_length: Optional[int] = None,
     ) -> State:
         """Runs the ``process_function`` over the passed data.
 
         Engine has a state and the following logic is applied in this function:
 
-        - At the first call, new state is defined by `max_epochs`, `epoch_length`, if provided.
+        - At the first call, new state is defined by `max_epochs`, `max_iters`, `epoch_length`, if provided.
           A timer for total and per-epoch time is initialized when Events.STARTED is handled.
         - If state is already defined such that there are iterations to run until `max_epochs` and no input arguments
           provided, state is kept and used in the function.
         - If state is defined and engine is "done" (no iterations to run until `max_epochs`), a new state is defined.
         - If state is defined, engine is NOT "done", then input arguments if provided override defined state.
 
         Args:
@@ -798,14 +801,17 @@
                 If a new state should be created (first run or run again from ended engine), it's default value is 1.
                 If run is resuming from a state, provided `max_epochs` will be taken into account and should be larger
                 than `engine.state.max_epochs`.
             epoch_length: Number of iterations to count as one epoch. By default, it can be set as
                 `len(data)`. If `data` is an iterator and `epoch_length` is not set, then it will be automatically
                 determined as the iteration on which data iterator raises `StopIteration`.
                 This argument should not change if run is resuming from a state.
+            max_iters: Number of iterations to run for.
+                `max_iters` and `max_epochs` are mutually exclusive; only one of the two arguments should be provided.
+
         Returns:
             State: output state.
 
         Note:
             User can dynamically preprocess input batch at :attr:`~ignite.engine.events.Events.ITERATION_STARTED` and
             store output batch in `engine.state.batch`. Latter is passed as usually to `process_function` as argument:
 
@@ -848,27 +854,38 @@
                     raise ValueError(
                         "Argument epoch_length should be same as in the state, "
                         f"but given {epoch_length} vs {self.state.epoch_length}"
                     )
 
         if self.state.max_epochs is None or (self._is_done(self.state) and self._internal_run_generator is None):
             # Create new state
-            if max_epochs is None:
-                max_epochs = 1
             if epoch_length is None:
                 if data is None:
                     raise ValueError("epoch_length should be provided if data is None")
 
                 epoch_length = self._get_data_length(data)
                 if epoch_length is not None and epoch_length < 1:
                     raise ValueError("Input data has zero size. Please provide non-empty data")
 
+            if max_iters is None:
+                if max_epochs is None:
+                    max_epochs = 1
+            else:
+                if max_epochs is not None:
+                    raise ValueError(
+                        "Arguments max_iters and max_epochs are mutually exclusive."
+                        "Please provide only max_epochs or max_iters."
+                    )
+                if epoch_length is not None:
+                    max_epochs = math.ceil(max_iters / epoch_length)
+
             self.state.iteration = 0
             self.state.epoch = 0
             self.state.max_epochs = max_epochs
+            self.state.max_iters = max_iters
             self.state.epoch_length = epoch_length
             # Reset generator if previously used
             self._internal_run_generator = None
             self.logger.info(f"Engine run starting with max_epochs={max_epochs}.")
         else:
             self.logger.info(
                 f"Engine run resuming from iteration {self.state.iteration}, "
@@ -1041,20 +1058,26 @@
                     iter_counter += 1
                     should_exit = False
                 except StopIteration:
                     # Define self.state.epoch_length if it is not yet set
                     if self.state.epoch_length is None:
                         # Define epoch length and stop the epoch
                         self.state.epoch_length = iter_counter
+                        if self.state.max_iters is not None:
+                            self.state.max_epochs = math.ceil(self.state.max_iters / self.state.epoch_length)
                         break
 
                     # Should exit while loop if we can not iterate
                     if should_exit:
-                        if not self._is_done(self.state) and self.state.max_epochs is not None:
-                            total_iters = self.state.epoch_length * self.state.max_epochs
+                        if not self._is_done(self.state):
+                            total_iters = (
+                                self.state.epoch_length * self.state.max_epochs
+                                if self.state.max_epochs is not None
+                                else self.state.max_iters
+                            )
 
                             warnings.warn(
                                 "Data iterator can not provide data anymore but required total number of "
                                 "iterations to run is not reached. "
                                 f"Current iteration: {self.state.iteration} vs Total iterations to run : {total_iters}"
                             )
                         break
@@ -1077,14 +1100,18 @@
                 self.state.output = self._process_function(self, self.state.batch)
                 self._fire_event(Events.ITERATION_COMPLETED)
                 yield from self._maybe_terminate_or_interrupt()
 
                 if self.state.epoch_length is not None and iter_counter == self.state.epoch_length:
                     break
 
+                if self.state.max_iters is not None and self.state.iteration == self.state.max_iters:
+                    self.should_terminate = True
+                    raise _EngineTerminateException()
+
         except _EngineTerminateSingleEpochException:
             self._fire_event(Events.TERMINATE_SINGLE_EPOCH, iter_counter=iter_counter)
             self.should_terminate_single_epoch = False
             self._setup_dataloader_iter()
 
         except _EngineTerminateException as e:
             # we need to reraise this exception such that it is not handled
@@ -1198,20 +1225,26 @@
                     iter_counter += 1
                     should_exit = False
                 except StopIteration:
                     # Define self.state.epoch_length if it is not yet set
                     if self.state.epoch_length is None:
                         # Define epoch length and stop the epoch
                         self.state.epoch_length = iter_counter
+                        if self.state.max_iters is not None:
+                            self.state.max_epochs = math.ceil(self.state.max_iters / self.state.epoch_length)
                         break
 
                     # Should exit while loop if we can not iterate
                     if should_exit:
-                        if not self._is_done(self.state) and self.state.max_epochs is not None:
-                            total_iters = self.state.epoch_length * self.state.max_epochs
+                        if not self._is_done(self.state):
+                            total_iters = (
+                                self.state.epoch_length * self.state.max_epochs
+                                if self.state.max_epochs is not None
+                                else self.state.max_iters
+                            )
 
                             warnings.warn(
                                 "Data iterator can not provide data anymore but required total number of "
                                 "iterations to run is not reached. "
                                 f"Current iteration: {self.state.iteration} vs Total iterations to run : {total_iters}"
                             )
                         break
@@ -1234,14 +1267,18 @@
                 self.state.output = self._process_function(self, self.state.batch)
                 self._fire_event(Events.ITERATION_COMPLETED)
                 self._maybe_terminate_legacy()
 
                 if self.state.epoch_length is not None and iter_counter == self.state.epoch_length:
                     break
 
+                if self.state.max_iters is not None and self.state.iteration == self.state.max_iters:
+                    self.should_terminate = True
+                    raise _EngineTerminateException()
+
         except _EngineTerminateSingleEpochException:
             self._fire_event(Events.TERMINATE_SINGLE_EPOCH, iter_counter=iter_counter)
             self.should_terminate_single_epoch = False
             self._setup_dataloader_iter()
 
         except _EngineTerminateException as e:
             # we need to reraise this exception such that it is not handled
```

### Comparing `pytorch-ignite-0.5.0.post2/ignite/engine/events.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/engine/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,14 +439,15 @@
 
         state.iteration         # 1-based, the first iteration is 1
         state.epoch             # 1-based, the first epoch is 1
         state.seed              # seed to set at each epoch
         state.dataloader        # data passed to engine
         state.epoch_length      # optional length of an epoch
         state.max_epochs        # number of epochs to run
+        state.max_iters         # number of iterations to run
         state.batch             # batch passed to `process_function`
         state.output            # output of `process_function` after a single iteration
         state.metrics           # dictionary with defined metrics if any
         state.times             # dictionary with total and per-epoch times fetched on
                                 # keys: Events.EPOCH_COMPLETED.name and Events.COMPLETED.name
 
     Args:
@@ -465,14 +466,15 @@
     }
 
     def __init__(self, **kwargs: Any) -> None:
         self.iteration = 0
         self.epoch = 0
         self.epoch_length: Optional[int] = None
         self.max_epochs: Optional[int] = None
+        self.max_iters: Optional[int] = None
         self.output: Optional[int] = None
         self.batch: Optional[int] = None
         self.metrics: Dict[str, Any] = {}
         self.dataloader: Optional[Union[DataLoader, Iterable[Any]]] = None
         self.seed: Optional[int] = None
         self.times: Dict[str, Optional[float]] = {
             Events.EPOCH_COMPLETED.name: None,
```

### Comparing `pytorch-ignite-0.5.0.post2/ignite/engine/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/base_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/clearml_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/fbresearch_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/fbresearch_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/lr_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         # attach LRScheduler to trainer.
         if num_iter is None:
             num_iter = trainer.state.epoch_length * trainer.state.max_epochs
         else:
             max_iter = trainer.state.epoch_length * trainer.state.max_epochs  # type: ignore[operator]
             if max_iter < num_iter:
                 max_iter = num_iter
+                trainer.state.max_iters = num_iter
                 trainer.state.max_epochs = ceil(num_iter / trainer.state.epoch_length)  # type: ignore[operator]
 
         if not trainer.has_event_handler(self._reached_num_iterations):
             trainer.add_event_handler(Events.ITERATION_COMPLETED, self._reached_num_iterations, num_iter)
 
         # attach loss and lr logging
         if not trainer.has_event_handler(self._log_lr_and_loss):
```

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/mlflow_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/neptune_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/polyaxon_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/stores.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/tensorboard_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/time_limit.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/timing.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/tqdm_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/visdom_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/handlers/wandb_logger.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/accumulation.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/accuracy.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/average_precision.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/classification_report.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/cohen_kappa.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/cosine_similarity.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/entropy.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/fbeta.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/frequency.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/gpu_info.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/loss.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/metric.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/precision.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/precision_recall_curve.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/psnr.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/recall.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/__init__.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/_base.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/pearson_correlation.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/pearson_correlation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/r2_score.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/roc_auc.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/running_average.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/ssim.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/ignite/utils.py` & `pytorch-ignite-0.6.0.dev20240401/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/pyproject.toml` & `pytorch-ignite-0.6.0.dev20240401/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.post2
+Version: 0.6.0.dev20240401
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pytorch-ignite-0.5.0.post2/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.6.0.dev20240401/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/setup.cfg` & `pytorch-ignite-0.6.0.dev20240401/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.post2/setup.py` & `pytorch-ignite-0.6.0.dev20240401/setup.py`

 * *Files identical despite different names*

