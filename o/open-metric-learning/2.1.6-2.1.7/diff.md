# Comparing `tmp/open-metric-learning-2.1.6.tar.gz` & `tmp/open-metric-learning-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-2.1.6.tar", last modified: Sun Feb  4 10:39:06 2024, max compression
+gzip compressed data, was "dist/open-metric-learning-2.1.7.tar", last modified: Mon Apr  1 16:12:26 2024, max compression
```

## Comparing `open-metric-learning-2.1.6.tar` & `open-metric-learning-2.1.7.tar`

### file list

```diff
@@ -1,225 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    32375 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30550 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.340588 open-metric-learning-2.1.6/oml/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.344588 open-metric-learning-2.1.6/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.344588 open-metric-learning-2.1.6/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.344588 open-metric-learning-2.1.6/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/extractor/vit_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/extractor/vit_unicom.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.344588 open-metric-learning-2.1.6/oml/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/logger/neptune.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/logger/tensorboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/logger/wandb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.344588 open-metric-learning-2.1.6/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.348588 open-metric-learning-2.1.6/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.348588 open-metric-learning-2.1.6/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.348588 open-metric-learning-2.1.6/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.348588 open-metric-learning-2.1.6/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.348588 open-metric-learning-2.1.6/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.352588 open-metric-learning-2.1.6/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/configs/transforms/unicom_transforms.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.352588 open-metric-learning-2.1.6/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.352588 open-metric-learning-2.1.6/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/ddp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.352588 open-metric-learning-2.1.6/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.352588 open-metric-learning-2.1.6/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9509 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.356588 open-metric-learning-2.1.6/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/meta/siamese.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/resnet/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/resnet/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/vit_clip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_clip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/vit_clip/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_clip/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_clip/external/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_clip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/vit_dino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_dino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/vit_dino/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_dino/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_dino/external/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_dino/external/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_dino/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.360588 open-metric-learning-2.1.6/oml/models/vit_unicom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_unicom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/models/vit_unicom/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_unicom/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_unicom/external/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_unicom/external/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/models/vit_unicom/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.364588 open-metric-learning-2.1.6/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32375 2024-02-04 10:39:06.000000 open-metric-learning-2.1.6/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-02-04 10:39:06.000000 open-metric-learning-2.1.6/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 10:39:06.000000 open-metric-learning-2.1.6/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-04 10:39:06.000000 open-metric-learning-2.1.6/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-04 10:39:06.000000 open-metric-learning-2.1.6/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-04 10:39:06.372588 open-metric-learning-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:39:06.368588 open-metric-learning-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-02-04 10:38:53.000000 open-metric-learning-2.1.6/tests/test_outdated_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33670 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.986306 open-metric-learning-2.1.7/oml/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.986306 open-metric-learning-2.1.7/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit_unicom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/mlflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/neptune.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/tensorboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/wandb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/unicom_transforms.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/siamese.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/vit_clip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/vit_clip/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/vision_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_unicom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_unicom/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33670 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-2.1.6/LICENSE` & `open-metric-learning-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/PKG-INFO` & `open-metric-learning-2.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 2.1.6
+Version: 2.1.7
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -57,15 +57,16 @@
 ### Trusted by
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
-<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>
+<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -289,15 +290,15 @@
 
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 
 * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 * **TUTORIAL TO START WITH:**
 [English](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Russian](https://habr.com/ru/company/ods/blog/695380/) |
-[Chinese](https://blog.csdn.net/fermion0217/article/details/127932087)
+[Chinese](https://zhuanlan.zhihu.com/p/683102241)
 
 ---
 * The
 [DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
 for our paper
 [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
 
@@ -428,15 +429,15 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -449,23 +450,26 @@
 
 # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
 val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
 metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
 
 # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".")
+logger = TensorBoardPipelineLogger(".")
 
 # 2) Logging with Neptune
-# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)
+# logger = NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False)
 
 # 3) Logging with Weights and Biases
 # import os
 # os.environ["WANDB_API_KEY"] = ""
-# logger = WandbLogger(project="test_project", log_model=False)
+# logger = WandBPipelineLogger(project="test_project", log_model=False)
+
+# 4) Logging with MLFlow locally
+# logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
@@ -545,15 +549,16 @@
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 Models, trained by other researchers.
-The metrics below are for **224 x 224** images:
+Note, that some metrics on particular benchmarks are so high because they were part of the training dataset (for example `unicom`).
+The metrics below are for 224 x 224 images:
 
 |                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
 |:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
 |    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
 |    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
 |    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
 | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
@@ -563,14 +568,20 @@
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
 |        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
 |         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
 |        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
 |         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|       `ViTExtractor.from_pretrained("vits14_dinov2")`        |          0.566           |       0.334        |    0.797     |  0.503   |
+|     `ViTExtractor.from_pretrained("vits14_reg_dinov2")`      |          0.566           |       0.332        |    0.795     |  0.740   |
+|       `ViTExtractor.from_pretrained("vitb14_dinov2")`        |          0.565           |       0.342        |    0.842     |  0.644   |
+|     `ViTExtractor.from_pretrained("vitb14_reg_dinov2")`      |          0.557           |       0.324        |    0.833     |  0.828   |
+|       `ViTExtractor.from_pretrained("vitl14_dinov2")`        |          0.576           |       0.352        |    0.844     |  0.692   |
+|     `ViTExtractor.from_pretrained("vitl14_reg_dinov2")`      |          0.571           |       0.340        |    0.840     |  0.871   |
 |    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
 | `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
 
 **The metrics may be different from the ones reported by papers,
 because the version of train/val split and usage of bounding boxes may differ.*
 
 ### How to use models from Zoo?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.6 Summary: OML is
+Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.7 Summary: OML is
 a PyTorch-based framework to train and validate the models producing high-
 quality embeddings. Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei Author-email: shabanoff.aleksei@gmail.com License:
 Apache License 2.0 Project-URL: Homepage, https://github.com/OML-Team/open-
 metric-learning Project-URL: Bug Tracker, https://github.com/OML-Team/open-
 metric-learning/issues Keywords: data-science,computer-vision,deep-
 learning,pytorch,metric-learning,representation-learning,pytorch-lightning
@@ -41,15 +41,16 @@
  framework to train and validate the models producing high-quality embeddings.
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
-_r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]_[_h_t_t_p_s_:_/_/
+ _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
+ _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
  _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
 _d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
    number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
 www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
  github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
  (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
               github.com/nik-fedorov/term_paper_metric_learning)
@@ -200,23 +201,22 @@
 their real-world projects. Unfortunately, we don't have ready-to-use tutorials
 for this kind of usage at the moment.
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/
 index.html) * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/
 en/latest/index.html) * **TUTORIAL TO START WITH:** [English](https://
 medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) | [Russian]
 (https://habr.com/ru/company/ods/blog/695380/) | [Chinese](https://
-blog.csdn.net/fermion0217/article/details/127932087) --- * The [DEMO](https://
-dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our
-paper [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://
-arxiv.org/abs/2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost]
-(https://www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-
-based-python-framework-to-train-and-validate-the-deep-learning-models-
-producing-high-quality-embeddings/) * The report for Berlin-based meetup:
-"Computer Vision in production". November, 2022. [Link](https://
-drive.google.com/drive/folders/
+zhuanlan.zhihu.com/p/683102241) --- * The [DEMO](https://dapladoc-oml-
+postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our paper [STIR:
+Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/
+2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost](https://
+www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-based-
+python-framework-to-train-and-validate-the-deep-learning-models-producing-high-
+quality-embeddings/) * The report for Berlin-based meetup: "Computer Vision in
+production". November, 2022. [Link](https://drive.google.com/drive/folders/
 1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link) ## [Installation](https://
 open-metric-learning.readthedocs.io/en/latest/oml/installation.html) OML is
 available in PyPI: ```shell pip install -U open-metric-learning ``` You can
 also pull the prepared image from DockerHub... ```shell docker pull omlteam/
 oml:gpu docker pull omlteam/oml:cpu ``` ## [Examples](https://open-metric-
 learning.readthedocs.io/en/latest/feature_extraction/python_examples.html#)
 Training
@@ -266,31 +266,34 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+oml.lightning.pipelines.logging import NeptunePipelineLogger,
+TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
 (dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
 normalise_features=False) # train optimizer = torch.optim.SGD
 (extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
 dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
 miner=AllTripletsMiner()) batch_sampler = BalanceSampler
 (train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
 torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
 = torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
 MetricValCallback(metric=EmbeddingMetrics(extra_keys=
 [train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".") # 2) Logging with Neptune # logger =
-NeptuneLogger(api_key="", project="", log_model_checkpoints=False) # 3) Logging
-with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = "" # logger
-= WandbLogger(project="test_project", log_model=False) # run pl_model =
+logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
+Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
+# logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
+Logging with MLFlow locally # logger = MLFlowPipelineLogger
+(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
 ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
 (max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
@@ -348,63 +351,71 @@
 ("vits16_cars")` | 0.907 | CARS 196 | [link](https://drive.google.com/drive/
 folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
 features_extraction/extractor_cars) | | `ViTExtractor.from_pretrained
 ("vits16_cub")` | 0.837 | CUB 200 2011 | [link](https://drive.google.com/drive/
 folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
-features_extraction/extractor_cub) | Models, trained by other researchers. The
-metrics below are for **224 x 224** images: | model | Stanford Online Products
-| DeepFashion InShop | CUB 200 2011 | CARS 196 | |:----------------------------
---------------------------------:|:------------------------:|:-----------------
--:|:------------:|:--------:| | `ViTUnicomExtractor.from_pretrained
-("vitb16_unicom")` | 0.700 | 0.734 | 0.847 | 0.916 | |
-`ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690 | 0.722 | 0.796 |
-0.893 | | `ViTUnicomExtractor.from_pretrained("vitl14_unicom")` | 0.726 | 0.790
-| 0.868 | 0.922 | | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`
-| 0.745 | 0.810 | 0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained
-("sber_vitb32_224")` | 0.547 | 0.514 | 0.448 | 0.618 | |
-`ViTCLIPExtractor.from_pretrained("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 |
-0.648 | | `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555
-| 0.606 | 0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` |
-0.612 | 0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
+features_extraction/extractor_cub) | Models, trained by other researchers.
+Note, that some metrics on particular benchmarks are so high because they were
+part of the training dataset (for example `unicom`). The metrics below are for
+224 x 224 images: | model | Stanford Online Products | DeepFashion InShop | CUB
+200 2011 | CARS 196 | |:-------------------------------------------------------
+-----:|:------------------------:|:------------------:|:------------:|:-------
+-:| | `ViTUnicomExtractor.from_pretrained("vitb16_unicom")` | 0.700 | 0.734 |
+0.847 | 0.916 | | `ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690
+| 0.722 | 0.796 | 0.893 | | `ViTUnicomExtractor.from_pretrained
+("vitl14_unicom")` | 0.726 | 0.790 | 0.868 | 0.922 | |
+`ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")` | 0.745 | 0.810 |
+0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")` | 0.547
+| 0.514 | 0.448 | 0.618 | | `ViTCLIPExtractor.from_pretrained
+("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 | 0.648 | |
+`ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555 | 0.606 |
+0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` | 0.612 |
+0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
 ("openai_vitb16_224")` | 0.648 | 0.606 | 0.665 | 0.767 | |
 `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")` | 0.670 | 0.675 | 0.745
 | 0.844 | | `ViTExtractor.from_pretrained("vits16_dino")` | 0.648 | 0.509 |
 0.627 | 0.265 | | `ViTExtractor.from_pretrained("vits8_dino")` | 0.651 | 0.524
 | 0.661 | 0.315 | | `ViTExtractor.from_pretrained("vitb16_dino")` | 0.658 |
 0.514 | 0.541 | 0.288 | | `ViTExtractor.from_pretrained("vitb8_dino")` | 0.689
-| 0.599 | 0.506 | 0.313 | | `ResnetExtractor.from_pretrained
-("resnet50_moco_v2")` | 0.493 | 0.267 | 0.264 | 0.149 | |
-`ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` | 0.515 | 0.284 |
-0.455 | 0.247 | **The metrics may be different from the ones reported by
-papers, because the version of train/val split and usage of bounding boxes may
-differ.* ### How to use models from Zoo? [comment]:zoo-start ```python from
-oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR from
-oml.models import ViTExtractor from oml.registry.transforms import
-get_transforms_for_pretrained model = ViTExtractor.from_pretrained
-("vits16_dino") transforms, im_reader = get_transforms_for_pretrained
-("vits16_dino") img = im_reader(DATA_DIR / "images" / "circle_1.jpg") # put
-path to your image here img_tensor = transforms(img) # img_tensor = transforms
-(image=img)["image"] # for transforms from Albumentations features = model
-(img_tensor.unsqueeze(0)) # Check other available models: print(list
-(ViTExtractor.pretrained_models.keys())) # Load checkpoint saved on a disk:
-model_ = ViTExtractor(weights=CKPT_DIR / "vits16_dino.ckpt", arch="vits16",
-normalise_features=False) ``` [comment]:zoo-end ## [Contributing guide](https:/
-/open-metric-learning.readthedocs.io/en/latest/oml/contributing.html) We
-welcome new contributors! Please, see our: * [Contributing guide](https://open-
-metric-learning.readthedocs.io/en/latest/oml/contributing.html) * [Kanban
-board](https://github.com/OML-Team/open-metric-learning/projects/1) ##
-Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/
-_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was started in 2020 as a module for
-[Catalyst](https://github.com/catalyst-team/catalyst) library. I want to thank
-people who worked with me on that module: [Julia Shenshina](https://github.com/
-julia-shenshina), [Nikita Balagansky](https://github.com/elephantmipt), [Sergey
-Kolesnikov](https://github.com/Scitator) and others. I would like to thank
-people who continue working on this pipeline when it became a separe project:
-[Julia Shenshina](https://github.com/julia-shenshina), [Misha Kindulov](https:/
-/github.com/b0nce), [Aron Dik](https://github.com/dapladoc), [Aleksei Tarasov]
-(https://github.com/DaloroAT) and [Verkhovtsev Leonid](https://github.com/
-leoromanovich). _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
-_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since
-the part of functionality was developed (and used) by its computer vision team
-led by me.
+| 0.599 | 0.506 | 0.313 | | `ViTExtractor.from_pretrained("vits14_dinov2")` |
+0.566 | 0.334 | 0.797 | 0.503 | | `ViTExtractor.from_pretrained
+("vits14_reg_dinov2")` | 0.566 | 0.332 | 0.795 | 0.740 | |
+`ViTExtractor.from_pretrained("vitb14_dinov2")` | 0.565 | 0.342 | 0.842 | 0.644
+| | `ViTExtractor.from_pretrained("vitb14_reg_dinov2")` | 0.557 | 0.324 | 0.833
+| 0.828 | | `ViTExtractor.from_pretrained("vitl14_dinov2")` | 0.576 | 0.352 |
+0.844 | 0.692 | | `ViTExtractor.from_pretrained("vitl14_reg_dinov2")` | 0.571 |
+0.340 | 0.840 | 0.871 | | `ResnetExtractor.from_pretrained("resnet50_moco_v2")`
+| 0.493 | 0.267 | 0.264 | 0.149 | | `ResnetExtractor.from_pretrained
+("resnet50_imagenet1k_v1")` | 0.515 | 0.284 | 0.455 | 0.247 | **The metrics may
+be different from the ones reported by papers, because the version of train/val
+split and usage of bounding boxes may differ.* ### How to use models from Zoo?
+[comment]:zoo-start ```python from oml.const import CKPT_SAVE_ROOT as CKPT_DIR,
+MOCK_DATASET_PATH as DATA_DIR from oml.models import ViTExtractor from
+oml.registry.transforms import get_transforms_for_pretrained model =
+ViTExtractor.from_pretrained("vits16_dino") transforms, im_reader =
+get_transforms_for_pretrained("vits16_dino") img = im_reader(DATA_DIR /
+"images" / "circle_1.jpg") # put path to your image here img_tensor =
+transforms(img) # img_tensor = transforms(image=img)["image"] # for transforms
+from Albumentations features = model(img_tensor.unsqueeze(0)) # Check other
+available models: print(list(ViTExtractor.pretrained_models.keys())) # Load
+checkpoint saved on a disk: model_ = ViTExtractor(weights=CKPT_DIR /
+"vits16_dino.ckpt", arch="vits16", normalise_features=False) ``` [comment]:zoo-
+end ## [Contributing guide](https://open-metric-learning.readthedocs.io/en/
+latest/oml/contributing.html) We welcome new contributors! Please, see our: *
+[Contributing guide](https://open-metric-learning.readthedocs.io/en/latest/oml/
+contributing.html) * [Kanban board](https://github.com/OML-Team/open-metric-
+learning/projects/1) ## Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was
+started in 2020 as a module for [Catalyst](https://github.com/catalyst-team/
+catalyst) library. I want to thank people who worked with me on that module:
+[Julia Shenshina](https://github.com/julia-shenshina), [Nikita Balagansky]
+(https://github.com/elephantmipt), [Sergey Kolesnikov](https://github.com/
+Scitator) and others. I would like to thank people who continue working on this
+pipeline when it became a separe project: [Julia Shenshina](https://github.com/
+julia-shenshina), [Misha Kindulov](https://github.com/b0nce), [Aron Dik](https:
+//github.com/dapladoc), [Aleksei Tarasov](https://github.com/DaloroAT) and
+[Verkhovtsev Leonid](https://github.com/leoromanovich). _[_h_t_t_p_s_:_/_/
+_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-
+_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since the part of
+functionality was developed (and used) by its computer vision team led by me.
```

### Comparing `open-metric-learning-2.1.6/README.md` & `open-metric-learning-2.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 ### Trusted by
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
-<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>
+<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -248,15 +249,15 @@
 
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 
 * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 * **TUTORIAL TO START WITH:**
 [English](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Russian](https://habr.com/ru/company/ods/blog/695380/) |
-[Chinese](https://blog.csdn.net/fermion0217/article/details/127932087)
+[Chinese](https://zhuanlan.zhihu.com/p/683102241)
 
 ---
 * The
 [DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
 for our paper
 [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
 
@@ -387,15 +388,15 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -408,23 +409,26 @@
 
 # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
 val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
 metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
 
 # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".")
+logger = TensorBoardPipelineLogger(".")
 
 # 2) Logging with Neptune
-# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)
+# logger = NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False)
 
 # 3) Logging with Weights and Biases
 # import os
 # os.environ["WANDB_API_KEY"] = ""
-# logger = WandbLogger(project="test_project", log_model=False)
+# logger = WandBPipelineLogger(project="test_project", log_model=False)
+
+# 4) Logging with MLFlow locally
+# logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
@@ -504,15 +508,16 @@
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 Models, trained by other researchers.
-The metrics below are for **224 x 224** images:
+Note, that some metrics on particular benchmarks are so high because they were part of the training dataset (for example `unicom`).
+The metrics below are for 224 x 224 images:
 
 |                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
 |:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
 |    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
 |    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
 |    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
 | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
@@ -522,14 +527,20 @@
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
 |        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
 |         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
 |        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
 |         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|       `ViTExtractor.from_pretrained("vits14_dinov2")`        |          0.566           |       0.334        |    0.797     |  0.503   |
+|     `ViTExtractor.from_pretrained("vits14_reg_dinov2")`      |          0.566           |       0.332        |    0.795     |  0.740   |
+|       `ViTExtractor.from_pretrained("vitb14_dinov2")`        |          0.565           |       0.342        |    0.842     |  0.644   |
+|     `ViTExtractor.from_pretrained("vitb14_reg_dinov2")`      |          0.557           |       0.324        |    0.833     |  0.828   |
+|       `ViTExtractor.from_pretrained("vitl14_dinov2")`        |          0.576           |       0.352        |    0.844     |  0.692   |
+|     `ViTExtractor.from_pretrained("vitl14_reg_dinov2")`      |          0.571           |       0.340        |    0.840     |  0.871   |
 |    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
 | `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
 
 **The metrics may be different from the ones reported by papers,
 because the version of train/val split and usage of bounding boxes may differ.*
 
 ### How to use models from Zoo?
```

#### html2text {}

```diff
@@ -16,15 +16,16 @@
  framework to train and validate the models producing high-quality embeddings.
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
-_r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]_[_h_t_t_p_s_:_/_/
+ _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
+ _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
  _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
 _d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
    number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
 www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
  github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
  (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
               github.com/nik-fedorov/term_paper_metric_learning)
@@ -175,23 +176,22 @@
 their real-world projects. Unfortunately, we don't have ready-to-use tutorials
 for this kind of usage at the moment.
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/
 index.html) * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/
 en/latest/index.html) * **TUTORIAL TO START WITH:** [English](https://
 medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) | [Russian]
 (https://habr.com/ru/company/ods/blog/695380/) | [Chinese](https://
-blog.csdn.net/fermion0217/article/details/127932087) --- * The [DEMO](https://
-dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our
-paper [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://
-arxiv.org/abs/2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost]
-(https://www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-
-based-python-framework-to-train-and-validate-the-deep-learning-models-
-producing-high-quality-embeddings/) * The report for Berlin-based meetup:
-"Computer Vision in production". November, 2022. [Link](https://
-drive.google.com/drive/folders/
+zhuanlan.zhihu.com/p/683102241) --- * The [DEMO](https://dapladoc-oml-
+postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our paper [STIR:
+Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/
+2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost](https://
+www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-based-
+python-framework-to-train-and-validate-the-deep-learning-models-producing-high-
+quality-embeddings/) * The report for Berlin-based meetup: "Computer Vision in
+production". November, 2022. [Link](https://drive.google.com/drive/folders/
 1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link) ## [Installation](https://
 open-metric-learning.readthedocs.io/en/latest/oml/installation.html) OML is
 available in PyPI: ```shell pip install -U open-metric-learning ``` You can
 also pull the prepared image from DockerHub... ```shell docker pull omlteam/
 oml:gpu docker pull omlteam/oml:cpu ``` ## [Examples](https://open-metric-
 learning.readthedocs.io/en/latest/feature_extraction/python_examples.html#)
 Training
@@ -241,31 +241,34 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+oml.lightning.pipelines.logging import NeptunePipelineLogger,
+TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
 (dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
 normalise_features=False) # train optimizer = torch.optim.SGD
 (extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
 dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
 miner=AllTripletsMiner()) batch_sampler = BalanceSampler
 (train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
 torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
 = torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
 MetricValCallback(metric=EmbeddingMetrics(extra_keys=
 [train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".") # 2) Logging with Neptune # logger =
-NeptuneLogger(api_key="", project="", log_model_checkpoints=False) # 3) Logging
-with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = "" # logger
-= WandbLogger(project="test_project", log_model=False) # run pl_model =
+logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
+Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
+# logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
+Logging with MLFlow locally # logger = MLFlowPipelineLogger
+(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
 ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
 (max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
@@ -323,63 +326,71 @@
 ("vits16_cars")` | 0.907 | CARS 196 | [link](https://drive.google.com/drive/
 folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
 features_extraction/extractor_cars) | | `ViTExtractor.from_pretrained
 ("vits16_cub")` | 0.837 | CUB 200 2011 | [link](https://drive.google.com/drive/
 folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
-features_extraction/extractor_cub) | Models, trained by other researchers. The
-metrics below are for **224 x 224** images: | model | Stanford Online Products
-| DeepFashion InShop | CUB 200 2011 | CARS 196 | |:----------------------------
---------------------------------:|:------------------------:|:-----------------
--:|:------------:|:--------:| | `ViTUnicomExtractor.from_pretrained
-("vitb16_unicom")` | 0.700 | 0.734 | 0.847 | 0.916 | |
-`ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690 | 0.722 | 0.796 |
-0.893 | | `ViTUnicomExtractor.from_pretrained("vitl14_unicom")` | 0.726 | 0.790
-| 0.868 | 0.922 | | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`
-| 0.745 | 0.810 | 0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained
-("sber_vitb32_224")` | 0.547 | 0.514 | 0.448 | 0.618 | |
-`ViTCLIPExtractor.from_pretrained("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 |
-0.648 | | `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555
-| 0.606 | 0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` |
-0.612 | 0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
+features_extraction/extractor_cub) | Models, trained by other researchers.
+Note, that some metrics on particular benchmarks are so high because they were
+part of the training dataset (for example `unicom`). The metrics below are for
+224 x 224 images: | model | Stanford Online Products | DeepFashion InShop | CUB
+200 2011 | CARS 196 | |:-------------------------------------------------------
+-----:|:------------------------:|:------------------:|:------------:|:-------
+-:| | `ViTUnicomExtractor.from_pretrained("vitb16_unicom")` | 0.700 | 0.734 |
+0.847 | 0.916 | | `ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690
+| 0.722 | 0.796 | 0.893 | | `ViTUnicomExtractor.from_pretrained
+("vitl14_unicom")` | 0.726 | 0.790 | 0.868 | 0.922 | |
+`ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")` | 0.745 | 0.810 |
+0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")` | 0.547
+| 0.514 | 0.448 | 0.618 | | `ViTCLIPExtractor.from_pretrained
+("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 | 0.648 | |
+`ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555 | 0.606 |
+0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` | 0.612 |
+0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
 ("openai_vitb16_224")` | 0.648 | 0.606 | 0.665 | 0.767 | |
 `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")` | 0.670 | 0.675 | 0.745
 | 0.844 | | `ViTExtractor.from_pretrained("vits16_dino")` | 0.648 | 0.509 |
 0.627 | 0.265 | | `ViTExtractor.from_pretrained("vits8_dino")` | 0.651 | 0.524
 | 0.661 | 0.315 | | `ViTExtractor.from_pretrained("vitb16_dino")` | 0.658 |
 0.514 | 0.541 | 0.288 | | `ViTExtractor.from_pretrained("vitb8_dino")` | 0.689
-| 0.599 | 0.506 | 0.313 | | `ResnetExtractor.from_pretrained
-("resnet50_moco_v2")` | 0.493 | 0.267 | 0.264 | 0.149 | |
-`ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` | 0.515 | 0.284 |
-0.455 | 0.247 | **The metrics may be different from the ones reported by
-papers, because the version of train/val split and usage of bounding boxes may
-differ.* ### How to use models from Zoo? [comment]:zoo-start ```python from
-oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR from
-oml.models import ViTExtractor from oml.registry.transforms import
-get_transforms_for_pretrained model = ViTExtractor.from_pretrained
-("vits16_dino") transforms, im_reader = get_transforms_for_pretrained
-("vits16_dino") img = im_reader(DATA_DIR / "images" / "circle_1.jpg") # put
-path to your image here img_tensor = transforms(img) # img_tensor = transforms
-(image=img)["image"] # for transforms from Albumentations features = model
-(img_tensor.unsqueeze(0)) # Check other available models: print(list
-(ViTExtractor.pretrained_models.keys())) # Load checkpoint saved on a disk:
-model_ = ViTExtractor(weights=CKPT_DIR / "vits16_dino.ckpt", arch="vits16",
-normalise_features=False) ``` [comment]:zoo-end ## [Contributing guide](https:/
-/open-metric-learning.readthedocs.io/en/latest/oml/contributing.html) We
-welcome new contributors! Please, see our: * [Contributing guide](https://open-
-metric-learning.readthedocs.io/en/latest/oml/contributing.html) * [Kanban
-board](https://github.com/OML-Team/open-metric-learning/projects/1) ##
-Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/
-_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was started in 2020 as a module for
-[Catalyst](https://github.com/catalyst-team/catalyst) library. I want to thank
-people who worked with me on that module: [Julia Shenshina](https://github.com/
-julia-shenshina), [Nikita Balagansky](https://github.com/elephantmipt), [Sergey
-Kolesnikov](https://github.com/Scitator) and others. I would like to thank
-people who continue working on this pipeline when it became a separe project:
-[Julia Shenshina](https://github.com/julia-shenshina), [Misha Kindulov](https:/
-/github.com/b0nce), [Aron Dik](https://github.com/dapladoc), [Aleksei Tarasov]
-(https://github.com/DaloroAT) and [Verkhovtsev Leonid](https://github.com/
-leoromanovich). _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
-_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since
-the part of functionality was developed (and used) by its computer vision team
-led by me.
+| 0.599 | 0.506 | 0.313 | | `ViTExtractor.from_pretrained("vits14_dinov2")` |
+0.566 | 0.334 | 0.797 | 0.503 | | `ViTExtractor.from_pretrained
+("vits14_reg_dinov2")` | 0.566 | 0.332 | 0.795 | 0.740 | |
+`ViTExtractor.from_pretrained("vitb14_dinov2")` | 0.565 | 0.342 | 0.842 | 0.644
+| | `ViTExtractor.from_pretrained("vitb14_reg_dinov2")` | 0.557 | 0.324 | 0.833
+| 0.828 | | `ViTExtractor.from_pretrained("vitl14_dinov2")` | 0.576 | 0.352 |
+0.844 | 0.692 | | `ViTExtractor.from_pretrained("vitl14_reg_dinov2")` | 0.571 |
+0.340 | 0.840 | 0.871 | | `ResnetExtractor.from_pretrained("resnet50_moco_v2")`
+| 0.493 | 0.267 | 0.264 | 0.149 | | `ResnetExtractor.from_pretrained
+("resnet50_imagenet1k_v1")` | 0.515 | 0.284 | 0.455 | 0.247 | **The metrics may
+be different from the ones reported by papers, because the version of train/val
+split and usage of bounding boxes may differ.* ### How to use models from Zoo?
+[comment]:zoo-start ```python from oml.const import CKPT_SAVE_ROOT as CKPT_DIR,
+MOCK_DATASET_PATH as DATA_DIR from oml.models import ViTExtractor from
+oml.registry.transforms import get_transforms_for_pretrained model =
+ViTExtractor.from_pretrained("vits16_dino") transforms, im_reader =
+get_transforms_for_pretrained("vits16_dino") img = im_reader(DATA_DIR /
+"images" / "circle_1.jpg") # put path to your image here img_tensor =
+transforms(img) # img_tensor = transforms(image=img)["image"] # for transforms
+from Albumentations features = model(img_tensor.unsqueeze(0)) # Check other
+available models: print(list(ViTExtractor.pretrained_models.keys())) # Load
+checkpoint saved on a disk: model_ = ViTExtractor(weights=CKPT_DIR /
+"vits16_dino.ckpt", arch="vits16", normalise_features=False) ``` [comment]:zoo-
+end ## [Contributing guide](https://open-metric-learning.readthedocs.io/en/
+latest/oml/contributing.html) We welcome new contributors! Please, see our: *
+[Contributing guide](https://open-metric-learning.readthedocs.io/en/latest/oml/
+contributing.html) * [Kanban board](https://github.com/OML-Team/open-metric-
+learning/projects/1) ## Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was
+started in 2020 as a module for [Catalyst](https://github.com/catalyst-team/
+catalyst) library. I want to thank people who worked with me on that module:
+[Julia Shenshina](https://github.com/julia-shenshina), [Nikita Balagansky]
+(https://github.com/elephantmipt), [Sergey Kolesnikov](https://github.com/
+Scitator) and others. I would like to thank people who continue working on this
+pipeline when it became a separe project: [Julia Shenshina](https://github.com/
+julia-shenshina), [Misha Kindulov](https://github.com/b0nce), [Aron Dik](https:
+//github.com/dapladoc), [Aleksei Tarasov](https://github.com/DaloroAT) and
+[Verkhovtsev Leonid](https://github.com/leoromanovich). _[_h_t_t_p_s_:_/_/
+_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-
+_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since the part of
+functionality was developed (and used) by its computer vision team led by me.
```

### Comparing `open-metric-learning-2.1.6/oml/const.py` & `open-metric-learning-2.1.7/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/datasets/base.py` & `open-metric-learning-2.1.7/oml/datasets/base.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/datasets/list_dataset.py` & `open-metric-learning-2.1.7/oml/datasets/list_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/datasets/pairs.py` & `open-metric-learning-2.1.7/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/datasets/triplet.py` & `open-metric-learning-2.1.7/oml/datasets/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/ddp/patching.py` & `open-metric-learning-2.1.7/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/ddp/utils.py` & `open-metric-learning-2.1.7/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/functional/label_smoothing.py` & `open-metric-learning-2.1.7/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/functional/losses.py` & `open-metric-learning-2.1.7/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/functional/metrics.py` & `open-metric-learning-2.1.7/oml/functional/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/inference/abstract.py` & `open-metric-learning-2.1.7/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/inference/flat.py` & `open-metric-learning-2.1.7/oml/inference/flat.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/inference/pairs.py` & `open-metric-learning-2.1.7/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/criterions.py` & `open-metric-learning-2.1.7/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/datasets.py` & `open-metric-learning-2.1.7/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/metrics.py` & `open-metric-learning-2.1.7/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/miners.py` & `open-metric-learning-2.1.7/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/models.py` & `open-metric-learning-2.1.7/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/retrieval.py` & `open-metric-learning-2.1.7/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/interfaces/samplers.py` & `open-metric-learning-2.1.7/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/lightning/callbacks/metric.py` & `open-metric-learning-2.1.7/oml/lightning/callbacks/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
+import warnings
 from math import ceil
 from typing import Any, Optional
 
 import matplotlib.pyplot as plt
-import numpy as np
 import pytorch_lightning as pl
 from pytorch_lightning import Callback
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader
 
 from oml.const import LOG_IMAGE_FOLDER
 from oml.ddp.patching import check_loaders_is_patched, patch_dataloader_to_ddp
+from oml.interfaces.loggers import IFigureLogger
 from oml.interfaces.metrics import IBasicMetric, IMetricDDP, IMetricVisualisable
 from oml.lightning.modules.ddp import ModuleDDP
-from oml.utils.images.images import figure_to_nparray
 from oml.utils.misc import flatten_dict
 
 
 class MetricValCallback(Callback):
     """
     This is a wrapper which allows to use IBasicMetric with PyTorch Lightning.
 
@@ -98,31 +97,24 @@
             if is_last_expected_batch:
                 self.calc_and_log_metrics(pl_module)
 
     def _log_images(self, pl_module: pl.LightningModule) -> None:
         if not isinstance(self.metric, IMetricVisualisable):
             return
 
+        if not isinstance(pl_module.logger, IFigureLogger):
+            warnings.warn(
+                f"Unexpected logger {pl_module.logger}. Figures have not been saved. "
+                f"Please, use a child of {IFigureLogger}."
+            )
+            return
+
         for fig, metric_log_str in zip(*self.metric.visualize()):
             log_str = f"{LOG_IMAGE_FOLDER}/{metric_log_str}"
-            if isinstance(pl_module.logger, NeptuneLogger):
-                from neptune.new.types import File  # this is the optional dependency
-
-                pl_module.logger.experiment[log_str].log(File.as_image(fig))
-            elif isinstance(pl_module.logger, WandbLogger):
-                fig_img = figure_to_nparray(fig)
-                pl_module.logger.log_image(images=[fig_img], key=metric_log_str)
-            elif isinstance(pl_module.logger, TensorBoardLogger):
-                fig_img = figure_to_nparray(fig)
-                pl_module.logger.experiment.add_image(
-                    log_str, np.transpose(fig_img, (2, 0, 1)), pl_module.current_epoch
-                )
-            else:
-                raise ValueError(f"Logging with {type(pl_module.logger)} is not supported yet.")
-
+            pl_module.logger.log_figure(fig=fig, title=log_str, idx=pl_module.current_epoch)
             plt.close(fig=fig)
 
     def on_validation_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         self._ready_to_accumulate = False
         if self._collected_samples != self._expected_samples:
             self._raise_computation_error()
```

### Comparing `open-metric-learning-2.1.6/oml/lightning/modules/ddp.py` & `open-metric-learning-2.1.7/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/lightning/modules/extractor.py` & `open-metric-learning-2.1.7/oml/lightning/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/lightning/modules/pairwise_postprocessing.py` & `open-metric-learning-2.1.7/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/lightning/pipelines/predict.py` & `open-metric-learning-2.1.7/oml/lightning/pipelines/predict.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/lightning/pipelines/train.py` & `open-metric-learning-2.1.7/oml/lightning/pipelines/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from oml.const import TCfg
 from oml.datasets.base import get_retrieval_datasets
 from oml.lightning.callbacks.metric import MetricValCallback, MetricValCallbackDDP
 from oml.lightning.modules.extractor import ExtractorModule, ExtractorModuleDDP
 from oml.lightning.pipelines.parser import (
     check_is_config_for_ddp,
-    initialize_logging,
     parse_ckpt_callback_from_config,
     parse_engine_params_from_config,
+    parse_logger_from_config,
     parse_sampler_from_config,
     parse_scheduler_from_config,
 )
 from oml.metrics.embeddings import EmbeddingMetrics, EmbeddingMetricsDDP
 from oml.registry.losses import get_criterion_by_cfg
 from oml.registry.models import get_extractor_by_cfg
 from oml.registry.optimizers import get_optimizer_by_cfg
@@ -66,15 +66,17 @@
     For more details look at ``pipelines/features_extraction/README.md``
 
     """
     set_global_seed(cfg["seed"])
 
     cfg = dictconfig_to_dict(cfg)
     pprint(cfg)
-    logger = initialize_logging(cfg)
+
+    logger = parse_logger_from_config(cfg)
+    logger.log_pipeline_info(cfg)
 
     trainer_engine_params = parse_engine_params_from_config(cfg)
     is_ddp = check_is_config_for_ddp(trainer_engine_params)
 
     loader_train, loaders_val = get_retrieval_loaders(cfg)
     extractor = get_extractor_by_cfg(cfg["extractor"])
     criterion = get_criterion_by_cfg(cfg["criterion"], **{"label2category": loader_train.dataset.get_label2category()})
```

### Comparing `open-metric-learning-2.1.6/oml/lightning/pipelines/train_postprocessor.py` & `open-metric-learning-2.1.7/oml/lightning/pipelines/train_postprocessor.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from oml.lightning.callbacks.metric import MetricValCallback, MetricValCallbackDDP
 from oml.lightning.modules.pairwise_postprocessing import (
     PairwiseModule,
     PairwiseModuleDDP,
 )
 from oml.lightning.pipelines.parser import (
     check_is_config_for_ddp,
-    initialize_logging,
     parse_ckpt_callback_from_config,
     parse_engine_params_from_config,
+    parse_logger_from_config,
     parse_sampler_from_config,
     parse_scheduler_from_config,
 )
 from oml.metrics.embeddings import EmbeddingMetrics, EmbeddingMetricsDDP
 from oml.miners.pairs import PairsMiner
 from oml.registry.models import get_extractor_by_cfg
 from oml.registry.optimizers import get_optimizer_by_cfg
@@ -114,15 +114,17 @@
     For more details look at ``pipelines/postprocessing/pairwise_postprocessing/README.md``
 
     """
     set_global_seed(cfg["seed"])
 
     cfg = dictconfig_to_dict(cfg)
     pprint(cfg)
-    logger = initialize_logging(cfg)
+
+    logger = parse_logger_from_config(cfg)
+    logger.log_pipeline_info(cfg)
 
     trainer_engine_params = parse_engine_params_from_config(cfg)
     is_ddp = check_is_config_for_ddp(trainer_engine_params)
 
     loader_train, loader_val = get_loaders_with_embeddings(cfg)
 
     postprocessor = None if not cfg.get("postprocessor", None) else get_postprocessor_by_cfg(cfg["postprocessor"])
```

### Comparing `open-metric-learning-2.1.6/oml/lightning/pipelines/validate.py` & `open-metric-learning-2.1.7/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/losses/arcface.py` & `open-metric-learning-2.1.7/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/losses/surrogate_precision.py` & `open-metric-learning-2.1.7/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/losses/triplet.py` & `open-metric-learning-2.1.7/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/metrics/accumulation.py` & `open-metric-learning-2.1.7/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/metrics/embeddings.py` & `open-metric-learning-2.1.7/oml/metrics/embeddings.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/metrics/triplets.py` & `open-metric-learning-2.1.7/oml/metrics/triplets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/cross_batch.py` & `open-metric-learning-2.1.7/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/inbatch_all_tri.py` & `open-metric-learning-2.1.7/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/inbatch_hard_cluster.py` & `open-metric-learning-2.1.7/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/inbatch_hard_tri.py` & `open-metric-learning-2.1.7/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/inbatch_nhard_tri.py` & `open-metric-learning-2.1.7/oml/miners/inbatch_nhard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/miner_with_bank.py` & `open-metric-learning-2.1.7/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/miners/pairs.py` & `open-metric-learning-2.1.7/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/meta/projection.py` & `open-metric-learning-2.1.7/oml/models/meta/projection.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/meta/siamese.py` & `open-metric-learning-2.1.7/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/resnet/extractor.py` & `open-metric-learning-2.1.7/oml/models/resnet/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/resnet/pooling.py` & `open-metric-learning-2.1.7/oml/models/resnet/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/utils.py` & `open-metric-learning-2.1.7/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_clip/external/model.py` & `open-metric-learning-2.1.7/oml/models/vit_clip/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_clip/extractor.py` & `open-metric-learning-2.1.7/oml/models/vit_clip/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_dino/external/hubconf.py` & `open-metric-learning-2.1.7/oml/models/vit_dino/external/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_dino/external/vision_transformer.py` & `open-metric-learning-2.1.7/oml/models/vit_dino/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_dino/extractor.py` & `open-metric-learning-2.1.7/oml/models/vit_dino/extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,47 @@
 )
 from oml.models.vit_dino.external.hubconf import (  # type: ignore
     dino_vitb8,
     dino_vitb16,
     dino_vits8,
     dino_vits16,
 )
+from oml.models.vit_dino.external_v2.hubconf import (  # type: ignore
+    dinov2_vitb14,
+    dinov2_vitb14_reg,
+    dinov2_vitl14,
+    dinov2_vitl14_reg,
+    dinov2_vits14,
+    dinov2_vits14_reg,
+)
 from oml.transforms.images.albumentations import get_normalisation_albu
 from oml.utils.io import download_checkpoint_one_of
 from oml.utils.misc_torch import normalise, temporary_setting_model_mode
 
 _FB_URL = "https://dl.fbaipublicfiles.com"
 
 
 class ViTExtractor(IExtractor):
     """
     The base class for the extractors that follow VisualTransformer architecture.
 
     """
 
-    constructors = {"vits8": dino_vits8, "vits16": dino_vits16, "vitb8": dino_vitb8, "vitb16": dino_vitb16}
+    constructors = {
+        "vits8": dino_vits8,
+        "vits16": dino_vits16,
+        "vitb8": dino_vitb8,
+        "vitb16": dino_vitb16,
+        "vits14": dinov2_vits14,
+        "vitb14": dinov2_vitb14,
+        "vitl14": dinov2_vitl14,
+        "vits14_reg": dinov2_vits14_reg,
+        "vitb14_reg": dinov2_vitb14_reg,
+        "vitl14_reg": dinov2_vitl14_reg,
+    }
 
     pretrained_models = {
         # checkpoints pretrained in DINO framework on ImageNet by MetaAI
         "vits16_dino": {
             "url": f"{_FB_URL}/dino/dino_deitsmall16_pretrain/dino_deitsmall16_pretrain.pth",
             "hash": "cf0f22",
             "fname": "vits16_dino.ckpt",
@@ -56,35 +75,83 @@
         },
         "vitb8_dino": {
             "url": f"{_FB_URL}/dino/dino_vitbase8_pretrain/dino_vitbase8_pretrain.pth",
             "hash": "556550",
             "fname": "vitb8_dino.ckpt",
             "init_args": {"arch": "vitb8", "normalise_features": False},
         },
+        "vits14_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vits14/dinov2_vits14_pretrain.pth",
+            "hash": "2e405c",
+            "fname": "dinov2_vits14.ckpt",
+            "init_args": {"arch": "vits14", "normalise_features": False},
+        },
+        "vits14_reg_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vits14/dinov2_vits14_reg4_pretrain.pth",
+            "hash": "2a50c5",
+            "fname": "dinov2_vits14_reg4.ckpt",
+            "init_args": {"arch": "vits14_reg", "normalise_features": False},
+        },
+        "vitb14_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vitb14/dinov2_vitb14_pretrain.pth",
+            "hash": "8635e7",
+            "fname": "dinov2_vitb14.ckpt",
+            "init_args": {"arch": "vitb14", "normalise_features": False},
+        },
+        "vitb14_reg_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vitb14/dinov2_vitb14_reg4_pretrain.pth",
+            "hash": "13d13c",
+            "fname": "dinov2_vitb14_reg4.ckpt",
+            "init_args": {"arch": "vitb14_reg", "normalise_features": False},
+        },
+        "vitl14_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vitl14/dinov2_vitl14_pretrain.pth",
+            "hash": "19a02c",
+            "fname": "dinov2_vitl14.ckpt",
+            "init_args": {"arch": "vitl14", "normalise_features": False},
+        },
+        "vitl14_reg_dinov2": {
+            "url": f"{_FB_URL}/dinov2/dinov2_vitl14/dinov2_vitl14_reg4_pretrain.pth",
+            "hash": "8b6364",
+            "fname": "dinov2_vitl14_reg4.ckpt",
+            "init_args": {"arch": "vitl14_reg", "normalise_features": False},
+        },
         # our pretrained checkpoints
         "vits16_inshop": {
-            "url": [f"{STORAGE_CKPTS}/inshop/vits16_inshop_a76b85.ckpt", "1niX-TC8cj6j369t7iU2baHQSVN3MVJbW"],
+            "url": [
+                f"{STORAGE_CKPTS}/inshop/vits16_inshop_a76b85.ckpt",
+                "1niX-TC8cj6j369t7iU2baHQSVN3MVJbW",
+            ],
             "hash": "a76b85",
             "fname": "vits16_inshop.ckpt",
             "init_args": {"arch": "vits16", "normalise_features": False},
         },
         "vits16_sop": {
-            "url": [f"{STORAGE_CKPTS}/sop/vits16_sop_21e743.ckpt", "1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A"],
+            "url": [
+                f"{STORAGE_CKPTS}/sop/vits16_sop_21e743.ckpt",
+                "1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A",
+            ],
             "hash": "21e743",
             "fname": "vits16_sop.ckpt",
             "init_args": {"arch": "vits16", "normalise_features": True},
         },
         "vits16_cub": {
-            "url": [f"{STORAGE_CKPTS}/cub/vits16_cub.ckpt", "1p2tUosFpGXh5sCCdzlXtjV87kCDfG34G"],
+            "url": [
+                f"{STORAGE_CKPTS}/cub/vits16_cub.ckpt",
+                "1p2tUosFpGXh5sCCdzlXtjV87kCDfG34G",
+            ],
             "hash": "e82633",
             "fname": "vits16_cub.ckpt",
             "init_args": {"arch": "vits16", "normalise_features": False},
         },
         "vits16_cars": {
-            "url": [f"{STORAGE_CKPTS}/cars/vits16_cars.ckpt", "1hcOxDRRXrKr6ZTCyBauaY8Ue-pok4Icg"],
+            "url": [
+                f"{STORAGE_CKPTS}/cars/vits16_cars.ckpt",
+                "1hcOxDRRXrKr6ZTCyBauaY8Ue-pok4Icg",
+            ],
             "hash": "9f1e59",
             "fname": "vits16_cars.ckpt",
             "init_args": {"arch": "vits16", "normalise_features": False},
         },
     }
 
     def __init__(
@@ -175,15 +242,18 @@
         Visualization of the multi-head attention on a particular image.
 
         """
         return vis_vit(vit=self, image=image)
 
 
 def vis_vit(
-    vit: ViTExtractor, image: Union[TPILImage, np.ndarray], mean: TNormParam = MEAN, std: TNormParam = STD
+    vit: ViTExtractor,
+    image: Union[TPILImage, np.ndarray],
+    mean: TNormParam = MEAN,
+    std: TNormParam = STD,
 ) -> np.ndarray:
     # this is the optional dependency
     from pytorch_grad_cam.utils.image import show_cam_on_image
 
     need_to_convert = not isinstance(image, np.ndarray)
 
     if need_to_convert:
```

### Comparing `open-metric-learning-2.1.6/oml/models/vit_unicom/external/model.py` & `open-metric-learning-2.1.7/oml/models/vit_unicom/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_unicom/external/vision_transformer.py` & `open-metric-learning-2.1.7/oml/models/vit_unicom/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/models/vit_unicom/extractor.py` & `open-metric-learning-2.1.7/oml/models/vit_unicom/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/__init__.py` & `open-metric-learning-2.1.7/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/loggers.py` & `open-metric-learning-2.1.7/oml/registry/loggers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import os
-from typing import Any, Dict, Union
-
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
-from pytorch_lightning.loggers.logger import Logger
+from typing import Any, Dict
 
 from oml.const import TCfg
+from oml.interfaces.loggers import IPipelineLogger
+from oml.lightning.pipelines.logging import (
+    MLFlowPipelineLogger,
+    NeptunePipelineLogger,
+    TensorBoardPipelineLogger,
+    WandBPipelineLogger,
+)
 from oml.utils.misc import dictconfig_to_dict
 
-LOGGERS_REGISTRY = {"wandb": WandbLogger, "neptune": NeptuneLogger, "tensorboard": TensorBoardLogger}
+LOGGERS_REGISTRY = {
+    "wandb": WandBPipelineLogger,
+    "neptune": NeptunePipelineLogger,
+    "tensorboard": TensorBoardPipelineLogger,
+    "mlflow": MLFlowPipelineLogger,
+}
 
 CLOUD_TOKEN_NAMES = {"wandb": "WANDB_API_KEY", "neptune": "NEPTUNE_API_TOKEN"}
 TOKEN_ERROR_MESSAGE = (
     "{} logger is specified in your config file, "
     "but <{}> is not provided as a global environment variable."
     "Please, execute `export {}=your_token` before running the script."
 )
 
 
-def get_logger(name: str, **kwargs: Dict[str, Any]) -> Logger:
+def get_logger(name: str, **kwargs: Dict[str, Any]) -> IPipelineLogger:
     if (name in CLOUD_TOKEN_NAMES) and (CLOUD_TOKEN_NAMES[name] not in os.environ):
         token_name = CLOUD_TOKEN_NAMES[name]
         raise ValueError(TOKEN_ERROR_MESSAGE.format(name.upper(), token_name, token_name))
 
-    return LOGGERS_REGISTRY[name](**kwargs)
+    return LOGGERS_REGISTRY[name](**kwargs)  # type: ignore
 
 
-def get_logger_by_cfg(cfg: TCfg) -> Union[bool, Logger]:
+def get_logger_by_cfg(cfg: TCfg) -> IPipelineLogger:
     cfg = dictconfig_to_dict(cfg)
     logger = get_logger(cfg["name"], **cfg["args"])
     return logger
 
 
 __all__ = ["LOGGERS_REGISTRY", "get_logger", "get_logger_by_cfg"]
```

### Comparing `open-metric-learning-2.1.6/oml/registry/losses.py` & `open-metric-learning-2.1.7/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/miners.py` & `open-metric-learning-2.1.7/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/models.py` & `open-metric-learning-2.1.7/oml/registry/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/optimizers.py` & `open-metric-learning-2.1.7/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/postprocessors.py` & `open-metric-learning-2.1.7/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/samplers.py` & `open-metric-learning-2.1.7/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/schedulers.py` & `open-metric-learning-2.1.7/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/registry/transforms.py` & `open-metric-learning-2.1.7/oml/registry/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,20 @@
     "resnet50_imagenet1k_v1": get_normalisation_resize_hypvit(im_size=256, crop_size=224),
     "resnet101_imagenet1k_v1": get_normalisation_resize_hypvit(im_size=256, crop_size=224),
     "resnet152_imagenet1k_v1": get_normalisation_resize_hypvit(im_size=256, crop_size=224),
     "vitb8_dino": get_normalisation_resize_torch(im_size=224),
     "vitb16_dino": get_normalisation_resize_torch(im_size=224),
     "vits8_dino": get_normalisation_resize_torch(im_size=224),
     "vits16_dino": get_normalisation_resize_torch(im_size=224),
+    "vitb14_dinov2": get_normalisation_resize_hypvit(im_size=224),
+    "vitb14_reg_dinov2": get_normalisation_resize_hypvit(im_size=224),
+    "vitl14_dinov2": get_normalisation_resize_hypvit(im_size=224),
+    "vitl14_reg_dinov2": get_normalisation_resize_hypvit(im_size=224),
+    "vits14_dinov2": get_normalisation_resize_hypvit(im_size=224),
+    "vits14_reg_dinov2": get_normalisation_resize_hypvit(im_size=224),
     "sber_vitb32_224": get_normalisation_resize_albu_clip(im_size=224),
     "sber_vitb16_224": get_normalisation_resize_albu_clip(im_size=224),
     "sber_vitl14_224": get_normalisation_resize_albu_clip(im_size=224),
     "openai_vitb32_224": get_normalisation_resize_albu_clip(im_size=224),
     "openai_vitb16_224": get_normalisation_resize_albu_clip(im_size=224),
     "openai_vitl14_224": get_normalisation_resize_albu_clip(im_size=224),
     "vits16_inshop": get_normalisation_resize_hypvit(im_size=224, crop_size=224),
```

### Comparing `open-metric-learning-2.1.6/oml/retrieval/postprocessors/pairwise.py` & `open-metric-learning-2.1.7/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/samplers/balance.py` & `open-metric-learning-2.1.7/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/samplers/category_balance.py` & `open-metric-learning-2.1.7/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/samplers/distinct_category_balance.py` & `open-metric-learning-2.1.7/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/transforms/images/albumentations.py` & `open-metric-learning-2.1.7/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/transforms/images/torchvision.py` & `open-metric-learning-2.1.7/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/dataframe_format.py` & `open-metric-learning-2.1.7/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/download_mock_dataset.py` & `open-metric-learning-2.1.7/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/images/images.py` & `open-metric-learning-2.1.7/oml/utils/images/images.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/images/images_resize.py` & `open-metric-learning-2.1.7/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/io.py` & `open-metric-learning-2.1.7/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/misc.py` & `open-metric-learning-2.1.7/oml/utils/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 from typing import Any, Dict, Hashable, Iterable, List, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 from omegaconf import DictConfig, OmegaConf
 
-from oml.const import DOTENV_PATH, TCfg
+from oml.const import TCfg
 
 
 def find_value_ids(it: Iterable[Any], value: Any) -> List[int]:
     """
     Args:
         it: List of any
         value: Query element
@@ -64,20 +64,14 @@
         if isinstance(v, dict):
             items.extend(flatten_dict(v, new_key, sep=sep, ignored_keys=ignored_keys).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 
-def load_dotenv() -> None:
-    import dotenv  # this is the optional dependency
-
-    dotenv.load_dotenv(DOTENV_PATH)
-
-
 def dictconfig_to_dict(cfg: TCfg) -> Dict[str, Any]:
     if isinstance(cfg, DictConfig):
         cfg = OmegaConf.to_container(cfg, resolve=True)
 
     ret = dict()
 
     for k in cfg.keys():
@@ -177,15 +171,14 @@
 
 
 __all__ = [
     "find_value_ids",
     "set_global_seed",
     "one_hot",
     "flatten_dict",
-    "load_dotenv",
     "dictconfig_to_dict",
     "smart_sample",
     "clip_max",
     "check_if_nonempty_positive_integers",
     "compare_dicts_recursively",
     "find_first_occurrences",
 ]
```

### Comparing `open-metric-learning-2.1.6/oml/utils/misc_torch.py` & `open-metric-learning-2.1.7/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/oml/utils/remote_storage.py` & `open-metric-learning-2.1.7/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/open_metric_learning.egg-info/PKG-INFO` & `open-metric-learning-2.1.7/open_metric_learning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 2.1.6
+Version: 2.1.7
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -57,15 +57,16 @@
 ### Trusted by
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
-<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>
+<a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -289,15 +290,15 @@
 
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 
 * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/en/latest/index.html)
 * **TUTORIAL TO START WITH:**
 [English](https://medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) |
 [Russian](https://habr.com/ru/company/ods/blog/695380/) |
-[Chinese](https://blog.csdn.net/fermion0217/article/details/127932087)
+[Chinese](https://zhuanlan.zhihu.com/p/683102241)
 
 ---
 * The
 [DEMO](https://dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/)
 for our paper
 [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/2304.13393)
 
@@ -428,15 +429,15 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -449,23 +450,26 @@
 
 # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root)
 val_loader = torch.utils.data.DataLoader(val_dataset, batch_size=4)
 metric_callback = MetricValCallback(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]), log_images=True)
 
 # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".")
+logger = TensorBoardPipelineLogger(".")
 
 # 2) Logging with Neptune
-# logger = NeptuneLogger(api_key="", project="", log_model_checkpoints=False)
+# logger = NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False)
 
 # 3) Logging with Weights and Biases
 # import os
 # os.environ["WANDB_API_KEY"] = ""
-# logger = WandbLogger(project="test_project", log_model=False)
+# logger = WandBPipelineLogger(project="test_project", log_model=False)
+
+# 4) Logging with MLFlow locally
+# logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
@@ -545,15 +549,16 @@
 |:-----------------------------------------------:|:-----:|:------------------------:|:-------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|
 | `ViTExtractor.from_pretrained("vits16_inshop")` | 0.921 |    DeepFashion Inshop    |    [link](https://drive.google.com/file/d/1niX-TC8cj6j369t7iU2baHQSVN3MVJbW/view?usp=sharing)     | [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_inshop) |
 |  `ViTExtractor.from_pretrained("vits16_sop")`   | 0.866 | Stanford Online Products |   [link](https://drive.google.com/file/d/1zuGRHvF2KHd59aw7i7367OH_tQNOGz7A/view?usp=sharing)      |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_sop)   |
 | `ViTExtractor.from_pretrained("vits16_cars")`   | 0.907 |         CARS 196         |   [link](https://drive.google.com/drive/folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cars)  |
 |  `ViTExtractor.from_pretrained("vits16_cub")`   | 0.837 |       CUB 200 2011       |   [link](https://drive.google.com/drive/folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing)    |  [link](https://github.com/OML-Team/open-metric-learning/tree/main/pipelines/features_extraction/extractor_cub)   |
 
 Models, trained by other researchers.
-The metrics below are for **224 x 224** images:
+Note, that some metrics on particular benchmarks are so high because they were part of the training dataset (for example `unicom`).
+The metrics below are for 224 x 224 images:
 
 |                            model                             | Stanford Online Products | DeepFashion InShop | CUB 200 2011 | CARS 196 |
 |:------------------------------------------------------------:|:------------------------:|:------------------:|:------------:|:--------:|
 |    `ViTUnicomExtractor.from_pretrained("vitb16_unicom")`     |          0.700           |       0.734        |    0.847     |  0.916   |
 |    `ViTUnicomExtractor.from_pretrained("vitb32_unicom")`     |          0.690           |       0.722        |    0.796     |  0.893   |
 |    `ViTUnicomExtractor.from_pretrained("vitl14_unicom")`     |          0.726           |       0.790        |    0.868     |  0.922   |
 | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`  |          0.745           |       0.810        |    0.875     |  0.924   |
@@ -563,14 +568,20 @@
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")`    |          0.612           |       0.491        |    0.560     |  0.693   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitb16_224")`    |          0.648           |       0.606        |    0.665     |  0.767   |
 |   `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")`    |          0.670           |       0.675        |    0.745     |  0.844   |
 |        `ViTExtractor.from_pretrained("vits16_dino")`         |          0.648           |       0.509        |    0.627     |  0.265   |
 |         `ViTExtractor.from_pretrained("vits8_dino")`         |          0.651           |       0.524        |    0.661     |  0.315   |
 |        `ViTExtractor.from_pretrained("vitb16_dino")`         |          0.658           |       0.514        |    0.541     |  0.288   |
 |         `ViTExtractor.from_pretrained("vitb8_dino")`         |          0.689           |       0.599        |    0.506     |  0.313   |
+|       `ViTExtractor.from_pretrained("vits14_dinov2")`        |          0.566           |       0.334        |    0.797     |  0.503   |
+|     `ViTExtractor.from_pretrained("vits14_reg_dinov2")`      |          0.566           |       0.332        |    0.795     |  0.740   |
+|       `ViTExtractor.from_pretrained("vitb14_dinov2")`        |          0.565           |       0.342        |    0.842     |  0.644   |
+|     `ViTExtractor.from_pretrained("vitb14_reg_dinov2")`      |          0.557           |       0.324        |    0.833     |  0.828   |
+|       `ViTExtractor.from_pretrained("vitl14_dinov2")`        |          0.576           |       0.352        |    0.844     |  0.692   |
+|     `ViTExtractor.from_pretrained("vitl14_reg_dinov2")`      |          0.571           |       0.340        |    0.840     |  0.871   |
 |    `ResnetExtractor.from_pretrained("resnet50_moco_v2")`     |          0.493           |       0.267        |    0.264     |  0.149   |
 | `ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")`  |          0.515           |       0.284        |    0.455     |  0.247   |
 
 **The metrics may be different from the ones reported by papers,
 because the version of train/val split and usage of bounding boxes may differ.*
 
 ### How to use models from Zoo?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.6 Summary: OML is
+Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.7 Summary: OML is
 a PyTorch-based framework to train and validate the models producing high-
 quality embeddings. Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei Author-email: shabanoff.aleksei@gmail.com License:
 Apache License 2.0 Project-URL: Homepage, https://github.com/OML-Team/open-
 metric-learning Project-URL: Bug Tracker, https://github.com/OML-Team/open-
 metric-learning/issues Keywords: data-science,computer-vision,deep-
 learning,pytorch,metric-learning,representation-learning,pytorch-lightning
@@ -41,15 +41,16 @@
  framework to train and validate the models producing high-quality embeddings.
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
-_r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]_[_h_t_t_p_s_:_/_/
+ _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
+ _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
  _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
 _d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
    number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
 www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
  github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
  (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
               github.com/nik-fedorov/term_paper_metric_learning)
@@ -200,23 +201,22 @@
 their real-world projects. Unfortunately, we don't have ready-to-use tutorials
 for this kind of usage at the moment.
 ## [Documentation](https://open-metric-learning.readthedocs.io/en/latest/
 index.html) * [**DOCUMENTATION**](https://open-metric-learning.readthedocs.io/
 en/latest/index.html) * **TUTORIAL TO START WITH:** [English](https://
 medium.com/@AlekseiShabanov/practical-metric-learning-b0410cda2201) | [Russian]
 (https://habr.com/ru/company/ods/blog/695380/) | [Chinese](https://
-blog.csdn.net/fermion0217/article/details/127932087) --- * The [DEMO](https://
-dapladoc-oml-postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our
-paper [STIR: Siamese Transformers for Image Retrieval Postprocessing](https://
-arxiv.org/abs/2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost]
-(https://www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-
-based-python-framework-to-train-and-validate-the-deep-learning-models-
-producing-high-quality-embeddings/) * The report for Berlin-based meetup:
-"Computer Vision in production". November, 2022. [Link](https://
-drive.google.com/drive/folders/
+zhuanlan.zhihu.com/p/683102241) --- * The [DEMO](https://dapladoc-oml-
+postprocessing-demo-srcappmain-pfh2g0.streamlit.app/) for our paper [STIR:
+Siamese Transformers for Image Retrieval Postprocessing](https://arxiv.org/abs/
+2304.13393) * Meet OpenMetricLearning (OML) on [Marktechpost](https://
+www.marktechpost.com/2023/12/26/meet-openmetriclearning-oml-a-pytorch-based-
+python-framework-to-train-and-validate-the-deep-learning-models-producing-high-
+quality-embeddings/) * The report for Berlin-based meetup: "Computer Vision in
+production". November, 2022. [Link](https://drive.google.com/drive/folders/
 1uHmLU8vMrMVMFodt36u0uXAgYjG_3D30?usp=share_link) ## [Installation](https://
 open-metric-learning.readthedocs.io/en/latest/oml/installation.html) OML is
 available in PyPI: ```shell pip install -U open-metric-learning ``` You can
 also pull the prepared image from DockerHub... ```shell docker pull omlteam/
 oml:gpu docker pull omlteam/oml:cpu ``` ## [Examples](https://open-metric-
 learning.readthedocs.io/en/latest/feature_extraction/python_examples.html#)
 Training
@@ -266,31 +266,34 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-pytorch_lightning.loggers import NeptuneLogger, TensorBoardLogger, WandbLogger
+oml.lightning.pipelines.logging import NeptunePipelineLogger,
+TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
 dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
 (dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
 normalise_features=False) # train optimizer = torch.optim.SGD
 (extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
 dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
 miner=AllTripletsMiner()) batch_sampler = BalanceSampler
 (train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
 torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
 val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
 = torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
 MetricValCallback(metric=EmbeddingMetrics(extra_keys=
 [train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardLogger(".") # 2) Logging with Neptune # logger =
-NeptuneLogger(api_key="", project="", log_model_checkpoints=False) # 3) Logging
-with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = "" # logger
-= WandbLogger(project="test_project", log_model=False) # run pl_model =
+logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
+Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
+# logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
+Logging with MLFlow locally # logger = MLFlowPipelineLogger
+(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
 ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
 (max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
@@ -348,63 +351,71 @@
 ("vits16_cars")` | 0.907 | CARS 196 | [link](https://drive.google.com/drive/
 folders/17a4_fg94dox2sfkXmw-KCtiLBlx-ut-1?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
 features_extraction/extractor_cars) | | `ViTExtractor.from_pretrained
 ("vits16_cub")` | 0.837 | CUB 200 2011 | [link](https://drive.google.com/drive/
 folders/1TPCN-eZFLqoq4JBgnIfliJoEK48x9ozb?usp=sharing) | [link](https://
 github.com/OML-Team/open-metric-learning/tree/main/pipelines/
-features_extraction/extractor_cub) | Models, trained by other researchers. The
-metrics below are for **224 x 224** images: | model | Stanford Online Products
-| DeepFashion InShop | CUB 200 2011 | CARS 196 | |:----------------------------
---------------------------------:|:------------------------:|:-----------------
--:|:------------:|:--------:| | `ViTUnicomExtractor.from_pretrained
-("vitb16_unicom")` | 0.700 | 0.734 | 0.847 | 0.916 | |
-`ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690 | 0.722 | 0.796 |
-0.893 | | `ViTUnicomExtractor.from_pretrained("vitl14_unicom")` | 0.726 | 0.790
-| 0.868 | 0.922 | | `ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")`
-| 0.745 | 0.810 | 0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained
-("sber_vitb32_224")` | 0.547 | 0.514 | 0.448 | 0.618 | |
-`ViTCLIPExtractor.from_pretrained("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 |
-0.648 | | `ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555
-| 0.606 | 0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` |
-0.612 | 0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
+features_extraction/extractor_cub) | Models, trained by other researchers.
+Note, that some metrics on particular benchmarks are so high because they were
+part of the training dataset (for example `unicom`). The metrics below are for
+224 x 224 images: | model | Stanford Online Products | DeepFashion InShop | CUB
+200 2011 | CARS 196 | |:-------------------------------------------------------
+-----:|:------------------------:|:------------------:|:------------:|:-------
+-:| | `ViTUnicomExtractor.from_pretrained("vitb16_unicom")` | 0.700 | 0.734 |
+0.847 | 0.916 | | `ViTUnicomExtractor.from_pretrained("vitb32_unicom")` | 0.690
+| 0.722 | 0.796 | 0.893 | | `ViTUnicomExtractor.from_pretrained
+("vitl14_unicom")` | 0.726 | 0.790 | 0.868 | 0.922 | |
+`ViTUnicomExtractor.from_pretrained("vitl14_336px_unicom")` | 0.745 | 0.810 |
+0.875 | 0.924 | | `ViTCLIPExtractor.from_pretrained("sber_vitb32_224")` | 0.547
+| 0.514 | 0.448 | 0.618 | | `ViTCLIPExtractor.from_pretrained
+("sber_vitb16_224")` | 0.565 | 0.565 | 0.524 | 0.648 | |
+`ViTCLIPExtractor.from_pretrained("sber_vitl14_224")` | 0.512 | 0.555 | 0.606 |
+0.707 | | `ViTCLIPExtractor.from_pretrained("openai_vitb32_224")` | 0.612 |
+0.491 | 0.560 | 0.693 | | `ViTCLIPExtractor.from_pretrained
 ("openai_vitb16_224")` | 0.648 | 0.606 | 0.665 | 0.767 | |
 `ViTCLIPExtractor.from_pretrained("openai_vitl14_224")` | 0.670 | 0.675 | 0.745
 | 0.844 | | `ViTExtractor.from_pretrained("vits16_dino")` | 0.648 | 0.509 |
 0.627 | 0.265 | | `ViTExtractor.from_pretrained("vits8_dino")` | 0.651 | 0.524
 | 0.661 | 0.315 | | `ViTExtractor.from_pretrained("vitb16_dino")` | 0.658 |
 0.514 | 0.541 | 0.288 | | `ViTExtractor.from_pretrained("vitb8_dino")` | 0.689
-| 0.599 | 0.506 | 0.313 | | `ResnetExtractor.from_pretrained
-("resnet50_moco_v2")` | 0.493 | 0.267 | 0.264 | 0.149 | |
-`ResnetExtractor.from_pretrained("resnet50_imagenet1k_v1")` | 0.515 | 0.284 |
-0.455 | 0.247 | **The metrics may be different from the ones reported by
-papers, because the version of train/val split and usage of bounding boxes may
-differ.* ### How to use models from Zoo? [comment]:zoo-start ```python from
-oml.const import CKPT_SAVE_ROOT as CKPT_DIR, MOCK_DATASET_PATH as DATA_DIR from
-oml.models import ViTExtractor from oml.registry.transforms import
-get_transforms_for_pretrained model = ViTExtractor.from_pretrained
-("vits16_dino") transforms, im_reader = get_transforms_for_pretrained
-("vits16_dino") img = im_reader(DATA_DIR / "images" / "circle_1.jpg") # put
-path to your image here img_tensor = transforms(img) # img_tensor = transforms
-(image=img)["image"] # for transforms from Albumentations features = model
-(img_tensor.unsqueeze(0)) # Check other available models: print(list
-(ViTExtractor.pretrained_models.keys())) # Load checkpoint saved on a disk:
-model_ = ViTExtractor(weights=CKPT_DIR / "vits16_dino.ckpt", arch="vits16",
-normalise_features=False) ``` [comment]:zoo-end ## [Contributing guide](https:/
-/open-metric-learning.readthedocs.io/en/latest/oml/contributing.html) We
-welcome new contributors! Please, see our: * [Contributing guide](https://open-
-metric-learning.readthedocs.io/en/latest/oml/contributing.html) * [Kanban
-board](https://github.com/OML-Team/open-metric-learning/projects/1) ##
-Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/
-_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was started in 2020 as a module for
-[Catalyst](https://github.com/catalyst-team/catalyst) library. I want to thank
-people who worked with me on that module: [Julia Shenshina](https://github.com/
-julia-shenshina), [Nikita Balagansky](https://github.com/elephantmipt), [Sergey
-Kolesnikov](https://github.com/Scitator) and others. I would like to thank
-people who continue working on this pipeline when it became a separe project:
-[Julia Shenshina](https://github.com/julia-shenshina), [Misha Kindulov](https:/
-/github.com/b0nce), [Aron Dik](https://github.com/dapladoc), [Aleksei Tarasov]
-(https://github.com/DaloroAT) and [Verkhovtsev Leonid](https://github.com/
-leoromanovich). _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
-_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since
-the part of functionality was developed (and used) by its computer vision team
-led by me.
+| 0.599 | 0.506 | 0.313 | | `ViTExtractor.from_pretrained("vits14_dinov2")` |
+0.566 | 0.334 | 0.797 | 0.503 | | `ViTExtractor.from_pretrained
+("vits14_reg_dinov2")` | 0.566 | 0.332 | 0.795 | 0.740 | |
+`ViTExtractor.from_pretrained("vitb14_dinov2")` | 0.565 | 0.342 | 0.842 | 0.644
+| | `ViTExtractor.from_pretrained("vitb14_reg_dinov2")` | 0.557 | 0.324 | 0.833
+| 0.828 | | `ViTExtractor.from_pretrained("vitl14_dinov2")` | 0.576 | 0.352 |
+0.844 | 0.692 | | `ViTExtractor.from_pretrained("vitl14_reg_dinov2")` | 0.571 |
+0.340 | 0.840 | 0.871 | | `ResnetExtractor.from_pretrained("resnet50_moco_v2")`
+| 0.493 | 0.267 | 0.264 | 0.149 | | `ResnetExtractor.from_pretrained
+("resnet50_imagenet1k_v1")` | 0.515 | 0.284 | 0.455 | 0.247 | **The metrics may
+be different from the ones reported by papers, because the version of train/val
+split and usage of bounding boxes may differ.* ### How to use models from Zoo?
+[comment]:zoo-start ```python from oml.const import CKPT_SAVE_ROOT as CKPT_DIR,
+MOCK_DATASET_PATH as DATA_DIR from oml.models import ViTExtractor from
+oml.registry.transforms import get_transforms_for_pretrained model =
+ViTExtractor.from_pretrained("vits16_dino") transforms, im_reader =
+get_transforms_for_pretrained("vits16_dino") img = im_reader(DATA_DIR /
+"images" / "circle_1.jpg") # put path to your image here img_tensor =
+transforms(img) # img_tensor = transforms(image=img)["image"] # for transforms
+from Albumentations features = model(img_tensor.unsqueeze(0)) # Check other
+available models: print(list(ViTExtractor.pretrained_models.keys())) # Load
+checkpoint saved on a disk: model_ = ViTExtractor(weights=CKPT_DIR /
+"vits16_dino.ckpt", arch="vits16", normalise_features=False) ``` [comment]:zoo-
+end ## [Contributing guide](https://open-metric-learning.readthedocs.io/en/
+latest/oml/contributing.html) We welcome new contributors! Please, see our: *
+[Contributing guide](https://open-metric-learning.readthedocs.io/en/latest/oml/
+contributing.html) * [Kanban board](https://github.com/OML-Team/open-metric-
+learning/projects/1) ## Acknowledgments _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
+_c_a_t_a_l_y_s_t_-_t_e_a_m_/_c_a_t_a_l_y_s_t_-_p_i_c_s_/_m_a_s_t_e_r_/_p_i_c_s_/_c_a_t_a_l_y_s_t___l_o_g_o_._p_n_g_]The project was
+started in 2020 as a module for [Catalyst](https://github.com/catalyst-team/
+catalyst) library. I want to thank people who worked with me on that module:
+[Julia Shenshina](https://github.com/julia-shenshina), [Nikita Balagansky]
+(https://github.com/elephantmipt), [Sergey Kolesnikov](https://github.com/
+Scitator) and others. I would like to thank people who continue working on this
+pipeline when it became a separe project: [Julia Shenshina](https://github.com/
+julia-shenshina), [Misha Kindulov](https://github.com/b0nce), [Aron Dik](https:
+//github.com/dapladoc), [Aleksei Tarasov](https://github.com/DaloroAT) and
+[Verkhovtsev Leonid](https://github.com/leoromanovich). _[_h_t_t_p_s_:_/_/
+_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/_N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-
+_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]I also want to thank NewYorker, since the part of
+functionality was developed (and used) by its computer vision team led by me.
```

### Comparing `open-metric-learning-2.1.6/open_metric_learning.egg-info/SOURCES.txt` & `open-metric-learning-2.1.7/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
 oml/configs/extractor/extractor_with_mlp.yaml
 oml/configs/extractor/resnet.yaml
 oml/configs/extractor/vit.yaml
 oml/configs/extractor/vit_clip.yaml
 oml/configs/extractor/vit_unicom.yaml
+oml/configs/logger/mlflow.yaml
 oml/configs/logger/neptune.yaml
 oml/configs/logger/tensorboard.yaml
 oml/configs/logger/wandb.yaml
 oml/configs/miner/all_triplets.yaml
 oml/configs/miner/hard_cluster.yaml
 oml/configs/miner/hard_triplets.yaml
 oml/configs/miner/miner_with_bank.yaml
@@ -78,27 +79,29 @@
 oml/inference/__init__.py
 oml/inference/abstract.py
 oml/inference/flat.py
 oml/inference/pairs.py
 oml/interfaces/__init__.py
 oml/interfaces/criterions.py
 oml/interfaces/datasets.py
+oml/interfaces/loggers.py
 oml/interfaces/metrics.py
 oml/interfaces/miners.py
 oml/interfaces/models.py
 oml/interfaces/retrieval.py
 oml/interfaces/samplers.py
 oml/lightning/__init__.py
 oml/lightning/callbacks/__init__.py
 oml/lightning/callbacks/metric.py
 oml/lightning/modules/__init__.py
 oml/lightning/modules/ddp.py
 oml/lightning/modules/extractor.py
 oml/lightning/modules/pairwise_postprocessing.py
 oml/lightning/pipelines/__init__.py
+oml/lightning/pipelines/logging.py
 oml/lightning/pipelines/parser.py
 oml/lightning/pipelines/predict.py
 oml/lightning/pipelines/train.py
 oml/lightning/pipelines/train_postprocessor.py
 oml/lightning/pipelines/validate.py
 oml/losses/__init__.py
 oml/losses/arcface.py
@@ -129,14 +132,18 @@
 oml/models/vit_clip/external/__init__.py
 oml/models/vit_clip/external/model.py
 oml/models/vit_dino/__init__.py
 oml/models/vit_dino/extractor.py
 oml/models/vit_dino/external/__init__.py
 oml/models/vit_dino/external/hubconf.py
 oml/models/vit_dino/external/vision_transformer.py
+oml/models/vit_dino/external_v2/__init__.py
+oml/models/vit_dino/external_v2/config.py
+oml/models/vit_dino/external_v2/hubconf.py
+oml/models/vit_dino/external_v2/vision_transformer.py
 oml/models/vit_unicom/__init__.py
 oml/models/vit_unicom/extractor.py
 oml/models/vit_unicom/external/__init__.py
 oml/models/vit_unicom/external/model.py
 oml/models/vit_unicom/external/vision_transformer.py
 oml/registry/__init__.py
 oml/registry/loggers.py
```

### Comparing `open-metric-learning-2.1.6/setup.py` & `open-metric-learning-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/tests/test_build_readme.py` & `open-metric-learning-2.1.7/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/tests/test_imports.py` & `open-metric-learning-2.1.7/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.6/tests/test_outdated_docs.py` & `open-metric-learning-2.1.7/tests/test_outdated_docs.py`

 * *Files identical despite different names*

