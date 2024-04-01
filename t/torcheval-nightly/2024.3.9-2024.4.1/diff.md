# Comparing `tmp/torcheval-nightly-2024.3.9.tar.gz` & `tmp/torcheval-nightly-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torcheval-nightly-2024.3.9.tar", last modified: Sat Mar  9 12:08:03 2024, max compression
+gzip compressed data, was "torcheval-nightly-2024.4.1.tar", last modified: Mon Apr  1 12:09:17 2024, max compression
```

## Comparing `torcheval-nightly-2024.3.9.tar` & `torcheval-nightly-2024.4.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.057208 torcheval-nightly-2024.3.9/torcheval/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.057208 torcheval-nightly-2024.3.9/torcheval/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.057208 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/min.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.057208 torcheval-nightly-2024.3.9/torcheval/metrics/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/audio/fad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.061208 torcheval-nightly-2024.3.9/torcheval/metrics/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.061208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.061208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/throughput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.065208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_auprc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.065208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/image/psnr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.065208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/num_collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.065208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.065208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_information_preserved.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/image/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/reciprocal_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/retrieval_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/retrieval_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/ranking/weighted_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/regression/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/regression/r2_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/statistical/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/statistical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/statistical/wasserstein.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/synclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.069208 torcheval-nightly-2024.3.9/torcheval/metrics/text/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/word_information_lost.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/text/word_information_preserved.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/torcheval/metrics/window/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/click_through_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/normalized_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/metrics/window/weighted_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/torcheval/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/utils/random_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/torcheval/utils/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/utils/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/utils/test_utils/dummy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/utils/test_utils/metric_class_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-09 12:01:07.000000 torcheval-nightly-2024.3.9/torcheval/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 12:08:03.073207 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 12:08:03.000000 torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.771779 torcheval-nightly-2024.4.1/torcheval/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.771779 torcheval-nightly-2024.4.1/torcheval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.771779 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.771779 torcheval-nightly-2024.4.1/torcheval/metrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/audio/fad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.775779 torcheval-nightly-2024.4.1/torcheval/metrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.775779 torcheval-nightly-2024.4.1/torcheval/metrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.775779 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/throughput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_auprc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24115 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/image/psnr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/num_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.779780 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_information_preserved.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/reciprocal_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8728 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/retrieval_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/retrieval_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/ranking/weighted_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/regression/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/regression/r2_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/statistical/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/statistical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/statistical/wasserstein.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/synclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/word_information_lost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/text/word_information_preserved.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.783779 torcheval-nightly-2024.4.1/torcheval/metrics/window/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/click_through_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/normalized_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/metrics/window/weighted_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/torcheval/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/utils/random_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/torcheval/utils/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/utils/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/utils/test_utils/dummy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/utils/test_utils/metric_class_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 12:02:13.000000 torcheval-nightly-2024.4.1/torcheval/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:09:17.787779 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:09:17.000000 torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/zip-safe
```

### Comparing `torcheval-nightly-2024.3.9/LICENSE` & `torcheval-nightly-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/PKG-INFO` & `torcheval-nightly-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.3.9
+Version: 2024.4.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.3.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.4.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval-nightly-2024.3.9/README.md` & `torcheval-nightly-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/setup.py` & `torcheval-nightly-2024.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/auc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/auc.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar
 
 import torch
 
+# pyre-fixme[21]: Could not find module `torcheval.metrics.functional.aggregation.auc`.
 from torcheval.metrics.functional.aggregation.auc import (
     _auc_compute,
     _auc_update_input_check,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/cat.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/cat.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/max.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/max.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/mean.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/mean.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 import logging
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module `torcheval.metrics.functional.aggregation.mean`.
 from torcheval.metrics.functional.aggregation.mean import _mean_update
 from torcheval.metrics.metric import Metric
 
 TMean = TypeVar("TMean")
 
 
 class Mean(Metric[torch.Tensor]):
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/min.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/min.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/sum.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/sum.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module `torcheval.metrics.functional.aggregation.sum`.
 from torcheval.metrics.functional.aggregation.sum import _sum_update
 from torcheval.metrics.metric import Metric
 
 TSum = TypeVar("TSum")
 
 
 class Sum(Metric[torch.Tensor]):
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/aggregation/throughput.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/audio/fad.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/audio/fad.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/accuracy.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/auprc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/auroc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/binary_normalized_entropy.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/binary_normalized_entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.classification.binary_normalized_entropy`.
 from torcheval.metrics.functional.classification.binary_normalized_entropy import (
     _baseline_update,
     _binary_normalized_entropy_update,
 )
 from torcheval.metrics.metric import Metric
 
 TNormalizedEntropy = TypeVar("TNormalizedEntropy")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_auprc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_auroc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/confusion_matrix.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/f1_score.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/precision_recall_curve.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/recall.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/auc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/auc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/mean.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/mean.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/sum.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/sum.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/aggregation/throughput.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/aggregation/throughput.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     multilabel_auprc,
 )
 
 from torcheval.metrics.functional.classification.auroc import (
     binary_auroc,
     multiclass_auroc,
 )
+
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.classification.binary_normalized_entropy`.
 from torcheval.metrics.functional.classification.binary_normalized_entropy import (
     binary_normalized_entropy,
 )
 from torcheval.metrics.functional.classification.binned_auprc import (
     binary_binned_auprc,
     multiclass_binned_auprc,
     multilabel_binned_auprc,
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/accuracy.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/auprc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/auroc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binary_normalized_entropy.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binary_normalized_entropy.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_auprc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_auprc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_auroc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/binned_precision_recall_curve.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/binned_precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/confusion_matrix.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/f1_score.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/f1_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/precision_recall_curve.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/recall.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/classification/recall_at_fixed_precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/classification/recall_at_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/image/psnr.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/click_through_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/click_through_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/frequency.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/frequency.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/hit_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/num_collisions.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/num_collisions.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/reciprocal_rank.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/retrieval_precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/retrieval_precision.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/retrieval_recall.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/retrieval_recall.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/ranking/weighted_calibration.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/ranking/weighted_calibration.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 # pyre-strict
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.regression.mean_squared_error`.
 from torcheval.metrics.functional.regression.mean_squared_error import (
     mean_squared_error,
 )
+
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.regression.r2_score`.
 from torcheval.metrics.functional.regression.r2_score import r2_score
 
 __all__ = ["mean_squared_error", "r2_score"]
 __doc_name__ = "Regression Metrics"
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/mean_squared_error.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/regression/r2_score.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/statistical/wasserstein.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/tensor_utils.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/bleu.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/bleu.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 ) -> torch.Tensor:
     if weights is not None and n_gram != weights.size(dim=0):
         raise ValueError(
             f"the length of weights should equal n_gram, got len(weights)={weights.size(dim=0)}, n_gram={n_gram}"
         )
 
     if weights is None:
-        weights = torch.tensor([1 / n_gram] * n_gram)
+        weights = torch.tensor([1 / n_gram] * n_gram, device=input_len.device)
 
     precisions = matches_by_order / possible_matches_by_order
     geometric_mean = torch.exp(torch.sum(weights * torch.log(precisions)))
 
     brevity_penalty = _calc_brevity_penalty(input_len, target_len)
 
     return brevity_penalty * geometric_mean
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/helper.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/perplexity.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_error_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_information_lost.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_information_lost.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/functional/text/word_information_preserved.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/functional/text/word_information_preserved.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/image/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/image/fid.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/image/fid.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/image/psnr.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/image/ssim.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/metric.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/click_through_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/click_through_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.click_through_rate`.
 from torcheval.metrics.functional.ranking.click_through_rate import (
     _click_through_rate_compute,
     _click_through_rate_update,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/hit_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/reciprocal_rank.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/retrieval_precision.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/retrieval_precision.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.retrieval_precision`.
 from torcheval.metrics.functional.ranking.retrieval_precision import (
     _retrieval_precision_param_check,
     _retrieval_precision_update_input_check,
     get_topk,
     retrieval_precision,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/retrieval_recall.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/retrieval_recall.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.retrieval_recall`.
 from torcheval.metrics.functional.ranking.retrieval_recall import (
     _retrieval_recall_param_check,
     _retrieval_recall_update_input_check,
     get_topk,
     retrieval_recall,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/ranking/weighted_calibration.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/ranking/weighted_calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 # pyre-strict
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar, Union
 
 import torch
+
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.weighted_calibration`.
 from torcheval.metrics.functional.ranking.weighted_calibration import (
     _weighted_calibration_update,
 )
 from torcheval.metrics.metric import Metric
 
 TWeightedCalibration = TypeVar("TWeightedCalibration")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/regression/mean_squared_error.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/regression/mean_squared_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.regression.mean_squared_error`.
 from torcheval.metrics.functional.regression.mean_squared_error import (
     _mean_squared_error_compute,
     _mean_squared_error_param_check,
     _mean_squared_error_update,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/regression/r2_score.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/regression/r2_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.regression.r2_score`.
 from torcheval.metrics.functional.regression.r2_score import (
     _r2_score_compute,
     _r2_score_param_check,
     _r2_score_update,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/statistical/wasserstein.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/statistical/wasserstein.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/synclib.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/synclib.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/bleu.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/perplexity.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/perplexity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, TypeVar
 
 import torch
 
+# pyre-fixme[21]: Could not find module `torcheval.metrics.functional.text.perplexity`.
 from torcheval.metrics.functional.text.perplexity import (
     _perplexity_compute,
     _perplexity_update,
 )
 from torcheval.metrics.metric import Metric
 
 TPerplexity = TypeVar("TPerplexity")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/word_error_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/word_error_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, List, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.text.word_error_rate`.
 from torcheval.metrics.functional.text.word_error_rate import (
     _word_error_rate_compute,
     _word_error_rate_update,
 )
 from torcheval.metrics.metric import Metric
 
 TWordErrorRate = TypeVar("TWordErrorRate")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/word_information_lost.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/word_information_lost.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, List, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.text.word_information_lost`.
 from torcheval.metrics.functional.text.word_information_lost import (
     _wil_compute,
     _wil_update,
 )
 
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/text/word_information_preserved.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/text/word_information_preserved.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, List, Optional, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.text.word_information_preserved`.
 from torcheval.metrics.functional.text.word_information_preserved import (
     _word_information_preserved_compute,
     _word_information_preserved_update,
 )
 from torcheval.metrics.metric import Metric
 
 TWordInformationPreserved = TypeVar("TWordInformationPreserved")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/toolkit.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/toolkit.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/__init__.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/__init__.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/auroc.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/auroc.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/click_through_rate.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/click_through_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, Tuple, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.click_through_rate`.
 from torcheval.metrics.functional.ranking.click_through_rate import (
     _click_through_rate_compute,
     _click_through_rate_update,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/mean_squared_error.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/mean_squared_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, Tuple, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.regression.mean_squared_error`.
 from torcheval.metrics.functional.regression.mean_squared_error import (
     _mean_squared_error_compute,
     _mean_squared_error_param_check,
     _mean_squared_error_update,
 )
 from torcheval.metrics.metric import Metric
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/normalized_entropy.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/normalized_entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, Tuple, TypeVar, Union
 
 import torch
 
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.classification.binary_normalized_entropy`.
 from torcheval.metrics.functional.classification.binary_normalized_entropy import (
     _baseline_update,
     _binary_normalized_entropy_update,
 )
 from torcheval.metrics.metric import Metric
 
 TWindowedNormalizedEntropy = TypeVar("TWindowedNormalizedEntropy")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/metrics/window/weighted_calibration.py` & `torcheval-nightly-2024.4.1/torcheval/metrics/window/weighted_calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 # pyre-strict
 
 # pyre-ignore-all-errors[16]: Undefined attribute of metric states.
 
 from typing import Iterable, Optional, Tuple, TypeVar, Union
 
 import torch
+
+# pyre-fixme[21]: Could not find module
+#  `torcheval.metrics.functional.ranking.weighted_calibration`.
 from torcheval.metrics.functional.ranking.weighted_calibration import (
     _weighted_calibration_update,
 )
 from torcheval.metrics.metric import Metric
 
 TWindowedWeightedCalibration = TypeVar("TWindowedWeightedCalibration")
```

### Comparing `torcheval-nightly-2024.3.9/torcheval/utils/random_data.py` & `torcheval-nightly-2024.4.1/torcheval/utils/random_data.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/utils/test_utils/dummy_metric.py` & `torcheval-nightly-2024.4.1/torcheval/utils/test_utils/dummy_metric.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/utils/test_utils/metric_class_tester.py` & `torcheval-nightly-2024.4.1/torcheval/utils/test_utils/metric_class_tester.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval/version.py` & `torcheval-nightly-2024.4.1/torcheval/version.py`

 * *Files identical despite different names*

### Comparing `torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/PKG-INFO` & `torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torcheval-nightly
-Version: 2024.3.9
+Version: 2024.4.1
 Summary: A library for providing a simple interface to create new metrics and an easy-to-use toolkit for metric computations and checkpointing.
 Home-page: https://github.com/pytorch/torcheval
 Author: torcheval team
 Author-email: yicongd@fb.com
 License: BSD-3
 Keywords: pytorch,evaluation,metrics
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.3.9 Summary: A
+Metadata-Version: 2.1 Name: torcheval-nightly Version: 2024.4.1 Summary: A
 library for providing a simple interface to create new metrics and an easy-to-
 use toolkit for metric computations and checkpointing. Home-page: https://
 github.com/pytorch/torcheval Author: torcheval team Author-email:
 yicongd@fb.com License: BSD-3 Keywords: pytorch,evaluation,metrics Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torcheval-nightly-2024.3.9/torcheval_nightly.egg-info/SOURCES.txt` & `torcheval-nightly-2024.4.1/torcheval_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

