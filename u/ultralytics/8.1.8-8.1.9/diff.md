# Comparing `tmp/ultralytics-8.1.8.tar.gz` & `tmp/ultralytics-8.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultralytics-8.1.8.tar", last modified: Tue Jan 30 00:07:57 2024, max compression
+gzip compressed data, was "ultralytics-8.1.9.tar", last modified: Thu Feb  1 22:36:55 2024, max compression
```

## Comparing `ultralytics-8.1.8.tar` & `ultralytics-8.1.9.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.380210 ultralytics-8.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-30 00:06:29.000000 ultralytics-8.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-01-30 00:07:57.380210 ultralytics-8.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36735 2024-01-30 00:06:29.000000 ultralytics-8.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-01-30 00:06:29.000000 ultralytics-8.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 00:07:57.380210 ultralytics-8.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.344210 ultralytics-8.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-01-30 00:06:29.000000 ultralytics-8.1.8/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.344210 ultralytics-8.1.8/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.348210 ultralytics-8.1.8/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.348210 ultralytics-8.1.8/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.352210 ultralytics-8.1.8/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.340210 ultralytics-8.1.8/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.352210 ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.352210 ultralytics-8.1.8/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.352210 ultralytics-8.1.8/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.352210 ultralytics-8.1.8/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.356210 ultralytics-8.1.8/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.356210 ultralytics-8.1.8/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.356210 ultralytics-8.1.8/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    52000 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.356210 ultralytics-8.1.8/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.356210 ultralytics-8.1.8/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51992 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    37636 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17832 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34307 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16190 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.360210 ultralytics-8.1.8/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29136 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.364210 ultralytics-8.1.8/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.368210 ultralytics-8.1.8/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.368210 ultralytics-8.1.8/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.368210 ultralytics-8.1.8/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.368210 ultralytics-8.1.8/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.368210 ultralytics-8.1.8/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38765 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.372210 ultralytics-8.1.8/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.372210 ultralytics-8.1.8/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.372210 ultralytics-8.1.8/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.376210 ultralytics-8.1.8/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    36882 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.376210 ultralytics-8.1.8/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    27665 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21189 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53361 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-01-30 00:06:29.000000 ultralytics-8.1.8/ultralytics/utils/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 00:07:57.376210 ultralytics-8.1.8/ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 00:07:57.000000 ultralytics-8.1.8/ultralytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.298454 ultralytics-8.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-01 22:35:40.000000 ultralytics-8.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-02-01 22:36:55.298454 ultralytics-8.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36735 2024-02-01 22:35:40.000000 ultralytics-8.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-02-01 22:35:40.000000 ultralytics-8.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 22:36:55.298454 ultralytics-8.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.258454 ultralytics-8.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-02-01 22:35:40.000000 ultralytics-8.1.9/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.258454 ultralytics-8.1.9/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.262454 ultralytics-8.1.9/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.262454 ultralytics-8.1.9/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.254454 ultralytics-8.1.9/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.266454 ultralytics-8.1.9/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.270454 ultralytics-8.1.9/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52000 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51992 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37636 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17832 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34306 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.274454 ultralytics-8.1.9/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16190 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.278454 ultralytics-8.1.9/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.282454 ultralytics-8.1.9/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38765 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.286454 ultralytics-8.1.9/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.290454 ultralytics-8.1.9/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.290454 ultralytics-8.1.9/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    36882 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27665 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21189 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53358 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25143 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-02-01 22:35:40.000000 ultralytics-8.1.9/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:36:55.294454 ultralytics-8.1.9/ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-01 22:36:55.000000 ultralytics-8.1.9/ultralytics.egg-info/top_level.txt
```

### Comparing `ultralytics-8.1.8/LICENSE` & `ultralytics-8.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/PKG-INFO` & `ultralytics-8.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.1.8
+Version: 8.1.9
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.1.8 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.1.9 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.1.8/README.md` & `ultralytics-8.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/pyproject.toml` & `ultralytics-8.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_cli.py` & `ultralytics-8.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_cuda.py` & `ultralytics-8.1.9/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_engine.py` & `ultralytics-8.1.9/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_explorer.py` & `ultralytics-8.1.9/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_integrations.py` & `ultralytics-8.1.9/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/tests/test_python.py` & `ultralytics-8.1.9/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/__init__.py` & `ultralytics-8.1.9/ultralytics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.1.8"
+__version__ = "8.1.9"
 
 from ultralytics.data.explorer.explorer import Explorer
 from ultralytics.models import RTDETR, SAM, YOLO
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS as settings
 from ultralytics.utils.checks import check_yolo as checks
```

### Comparing `ultralytics-8.1.8/ultralytics/assets/bus.jpg` & `ultralytics-8.1.9/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/assets/zidane.jpg` & `ultralytics-8.1.9/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/__init__.py` & `ultralytics-8.1.9/ultralytics/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/Argoverse.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/DOTAv1.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/ImageNet.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/Objects365.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/SKU-110K.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/VOC.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/VisDrone.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/carparts-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco-pose.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco128-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco128.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco8-pose.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco8-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/coco8.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/crack-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/dota8.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/open-images-v7.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/package-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/tiger-pose.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/datasets/xView.yaml` & `ultralytics-8.1.9/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/default.yaml` & `ultralytics-8.1.9/ultralytics/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v3/yolov3.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v5/yolov5.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v6/yolov6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/models/v8/yolov8.yaml` & `ultralytics-8.1.9/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/trackers/botsort.yaml` & `ultralytics-8.1.9/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/cfg/trackers/bytetrack.yaml` & `ultralytics-8.1.9/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/annotator.py` & `ultralytics-8.1.9/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/augment.py` & `ultralytics-8.1.9/ultralytics/data/augment.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/base.py` & `ultralytics-8.1.9/ultralytics/data/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/build.py` & `ultralytics-8.1.9/ultralytics/data/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/converter.py` & `ultralytics-8.1.9/ultralytics/data/converter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/dataset.py` & `ultralytics-8.1.9/ultralytics/data/dataset.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/explorer/explorer.py` & `ultralytics-8.1.9/ultralytics/data/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/explorer/gui/dash.py` & `ultralytics-8.1.9/ultralytics/data/explorer/gui/dash.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/explorer/utils.py` & `ultralytics-8.1.9/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/loaders.py` & `ultralytics-8.1.9/ultralytics/data/loaders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/split_dota.py` & `ultralytics-8.1.9/ultralytics/data/split_dota.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/data/utils.py` & `ultralytics-8.1.9/ultralytics/data/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/exporter.py` & `ultralytics-8.1.9/ultralytics/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/model.py` & `ultralytics-8.1.9/ultralytics/engine/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/predictor.py` & `ultralytics-8.1.9/ultralytics/engine/predictor.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/results.py` & `ultralytics-8.1.9/ultralytics/engine/results.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/trainer.py` & `ultralytics-8.1.9/ultralytics/engine/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
                             dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                             self.stop = broadcast_list[0]
                         if self.stop:  # training time exceeded
                             break
 
                 # Log
                 mem = f"{torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0:.3g}G"  # (GB)
-                loss_len = self.tloss.shape[0] if len(self.tloss.size()) else 1
+                loss_len = self.tloss.shape[0] if len(self.tloss.shape) else 1
                 losses = self.tloss if loss_len > 1 else torch.unsqueeze(self.tloss, 0)
                 if RANK in (-1, 0):
                     pbar.set_description(
                         ("%11s" * 2 + "%11.4g" * (2 + loss_len))
                         % (f"{epoch + 1}/{self.epochs}", mem, *losses, batch["cls"].shape[0], batch["img"].shape[-1])
                     )
                     self.run_callbacks("on_batch_end")
```

### Comparing `ultralytics-8.1.8/ultralytics/engine/tuner.py` & `ultralytics-8.1.9/ultralytics/engine/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/engine/validator.py` & `ultralytics-8.1.9/ultralytics/engine/validator.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/hub/__init__.py` & `ultralytics-8.1.9/ultralytics/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/hub/auth.py` & `ultralytics-8.1.9/ultralytics/hub/auth.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/hub/session.py` & `ultralytics-8.1.9/ultralytics/hub/session.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/hub/utils.py` & `ultralytics-8.1.9/ultralytics/hub/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/fastsam/model.py` & `ultralytics-8.1.9/ultralytics/models/fastsam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/fastsam/predict.py` & `ultralytics-8.1.9/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/fastsam/prompt.py` & `ultralytics-8.1.9/ultralytics/models/fastsam/prompt.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/fastsam/utils.py` & `ultralytics-8.1.9/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/fastsam/val.py` & `ultralytics-8.1.9/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/nas/model.py` & `ultralytics-8.1.9/ultralytics/models/nas/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/nas/predict.py` & `ultralytics-8.1.9/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/nas/val.py` & `ultralytics-8.1.9/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/rtdetr/model.py` & `ultralytics-8.1.9/ultralytics/models/rtdetr/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/rtdetr/predict.py` & `ultralytics-8.1.9/ultralytics/models/rtdetr/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/rtdetr/train.py` & `ultralytics-8.1.9/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/rtdetr/val.py` & `ultralytics-8.1.9/ultralytics/models/rtdetr/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/amg.py` & `ultralytics-8.1.9/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/build.py` & `ultralytics-8.1.9/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/model.py` & `ultralytics-8.1.9/ultralytics/models/sam/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/modules/decoders.py` & `ultralytics-8.1.9/ultralytics/models/sam/modules/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         """
         Predicts masks.
 
         See 'forward' for more details.
         """
         # Concatenate output tokens
         output_tokens = torch.cat([self.iou_token.weight, self.mask_tokens.weight], dim=0)
-        output_tokens = output_tokens.unsqueeze(0).expand(sparse_prompt_embeddings.size(0), -1, -1)
+        output_tokens = output_tokens.unsqueeze(0).expand(sparse_prompt_embeddings.shape[0], -1, -1)
         tokens = torch.cat((output_tokens, sparse_prompt_embeddings), dim=1)
 
         # Expand per-image data in batch direction to be per-mask
         src = torch.repeat_interleave(image_embeddings, tokens.shape[0], dim=0)
         src = src + dense_prompt_embeddings
         pos_src = torch.repeat_interleave(image_pe, tokens.shape[0], dim=0)
         b, c, h, w = src.shape
```

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/modules/encoders.py` & `ultralytics-8.1.9/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/modules/sam.py` & `ultralytics-8.1.9/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/modules/tiny_encoder.py` & `ultralytics-8.1.9/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -728,15 +728,15 @@
 
         x = self.layers[0](x)
         start_i = 1
 
         for i in range(start_i, len(self.layers)):
             layer = self.layers[i]
             x = layer(x)
-        B, _, C = x.size()
+        B, _, C = x.shape
         x = x.view(B, 64, 64, C)
         x = x.permute(0, 3, 1, 2)
         return self.neck(x)
 
     def forward(self, x):
         """Executes a forward pass on the input tensor through the constructed model layers."""
         return self.forward_features(x)
```

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/modules/transformer.py` & `ultralytics-8.1.9/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/sam/predict.py` & `ultralytics-8.1.9/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/utils/loss.py` & `ultralytics-8.1.9/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/utils/ops.py` & `ultralytics-8.1.9/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/classify/predict.py` & `ultralytics-8.1.9/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/classify/train.py` & `ultralytics-8.1.9/ultralytics/models/yolo/classify/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/classify/val.py` & `ultralytics-8.1.9/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/detect/predict.py` & `ultralytics-8.1.9/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/detect/train.py` & `ultralytics-8.1.9/ultralytics/models/yolo/detect/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/detect/val.py` & `ultralytics-8.1.9/ultralytics/models/yolo/detect/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/model.py` & `ultralytics-8.1.9/ultralytics/models/yolo/model.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/obb/predict.py` & `ultralytics-8.1.9/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/obb/train.py` & `ultralytics-8.1.9/ultralytics/models/yolo/obb/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/obb/val.py` & `ultralytics-8.1.9/ultralytics/models/yolo/obb/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/pose/predict.py` & `ultralytics-8.1.9/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/pose/train.py` & `ultralytics-8.1.9/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/pose/val.py` & `ultralytics-8.1.9/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/segment/predict.py` & `ultralytics-8.1.9/ultralytics/models/yolo/segment/predict.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             classes=self.args.classes,
         )
 
         if not isinstance(orig_imgs, list):  # input images are a torch.Tensor, not a list
             orig_imgs = ops.convert_torch2numpy_batch(orig_imgs)
 
         results = []
-        proto = preds[1][-1] if len(preds[1]) == 3 else preds[1]  # second output is len 3 if pt, but only 1 if exported
+        proto = preds[1][-1] if isinstance(preds[1], tuple) else preds[1]  # tuple if PyTorch model or array if exported
         for i, pred in enumerate(p):
             orig_img = orig_imgs[i]
             img_path = self.batch[0][i]
             if not len(pred):  # save empty boxes
                 masks = None
             elif self.args.retina_masks:
                 pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], orig_img.shape)
```

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/segment/train.py` & `ultralytics-8.1.9/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/models/yolo/segment/val.py` & `ultralytics-8.1.9/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/__init__.py` & `ultralytics-8.1.9/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/autobackend.py` & `ultralytics-8.1.9/ultralytics/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/__init__.py` & `ultralytics-8.1.9/ultralytics/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/block.py` & `ultralytics-8.1.9/ultralytics/nn/modules/block.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/conv.py` & `ultralytics-8.1.9/ultralytics/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/head.py` & `ultralytics-8.1.9/ultralytics/nn/modules/head.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/transformer.py` & `ultralytics-8.1.9/ultralytics/nn/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/modules/utils.py` & `ultralytics-8.1.9/ultralytics/nn/modules/utils.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/nn/tasks.py` & `ultralytics-8.1.9/ultralytics/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/solutions/ai_gym.py` & `ultralytics-8.1.9/ultralytics/solutions/ai_gym.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/solutions/distance_calculation.py` & `ultralytics-8.1.9/ultralytics/solutions/distance_calculation.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/solutions/heatmap.py` & `ultralytics-8.1.9/ultralytics/solutions/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,18 @@
 
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
+            self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
             if self.view_img and self.env_check:
                 self.display_frames()
-            return
+            return im0
         self.heatmap *= self.decay_factor  # decay factor
         self.extract_results(tracks)
         self.annotator = Annotator(self.im0, self.count_txt_thickness, None)
 
         if self.count_reg_pts is not None:
             # Draw counting region
             if self.view_in_counts or self.view_out_counts:
```

### Comparing `ultralytics-8.1.8/ultralytics/solutions/object_counter.py` & `ultralytics-8.1.9/ultralytics/solutions/object_counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0  # store image
 
         if tracks[0].boxes.id is None:
             if self.view_img:
                 self.display_frames()
-            return
+            return im0
         self.extract_and_process_tracks(tracks)
 
         if self.view_img:
             self.display_frames()
         return self.im0
```

### Comparing `ultralytics-8.1.8/ultralytics/solutions/speed_estimation.py` & `ultralytics-8.1.9/ultralytics/solutions/speed_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img and self.env_check:
                 self.display_frames()
-            return
+            return im0
         self.extract_tracks(tracks)
 
         self.annotator = Annotator(self.im0, line_width=2)
         self.annotator.draw_region(reg_pts=self.reg_pts, color=(255, 0, 0), thickness=self.region_thickness)
 
         for box, trk_id, cls in zip(self.boxes, self.trk_ids, self.clss):
             track = self.store_track_info(trk_id, box)
```

### Comparing `ultralytics-8.1.8/ultralytics/trackers/basetrack.py` & `ultralytics-8.1.9/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/trackers/bot_sort.py` & `ultralytics-8.1.9/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/trackers/byte_tracker.py` & `ultralytics-8.1.9/ultralytics/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/trackers/track.py` & `ultralytics-8.1.9/ultralytics/trackers/track.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/trackers/utils/gmc.py` & `ultralytics-8.1.9/ultralytics/trackers/utils/gmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         currPoints = np.array(currPoints)
 
         # Draw the keypoint matches on the output image
         # if False:
         #     import matplotlib.pyplot as plt
         #     matches_img = np.hstack((self.prevFrame, frame))
         #     matches_img = cv2.cvtColor(matches_img, cv2.COLOR_GRAY2BGR)
-        #     W = np.size(self.prevFrame, 1)
+        #     W = self.prevFrame.shape[1]
         #     for m in goodMatches:
         #         prev_pt = np.array(self.prevKeyPoints[m.queryIdx].pt, dtype=np.int_)
         #         curr_pt = np.array(keypoints[m.trainIdx].pt, dtype=np.int_)
         #         curr_pt[0] += W
         #         color = np.random.randint(0, 255, 3)
         #         color = (int(color[0]), int(color[1]), int(color[2]))
         #
@@ -271,15 +271,15 @@
         #         matches_img = cv2.circle(matches_img, curr_pt, 2, tuple(color), -1)
         #
         #     plt.figure()
         #     plt.imshow(matches_img)
         #     plt.show()
 
         # Find rigid matrix
-        if (np.size(prevPoints, 0) > 4) and (np.size(prevPoints, 0) == np.size(prevPoints, 0)):
+        if (prevPoints.shape[0] > 4) and (prevPoints.shape[0] == prevPoints.shape[0]):
             H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             # Handle downscale
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
@@ -339,15 +339,15 @@
                 prevPoints.append(self.prevKeyPoints[i])
                 currPoints.append(matchedKeypoints[i])
 
         prevPoints = np.array(prevPoints)
         currPoints = np.array(currPoints)
 
         # Find rigid matrix
-        if np.size(prevPoints, 0) > 4 and np.size(prevPoints, 0) == np.size(prevPoints, 0):
+        if (prevPoints.shape[0] > 4) and (prevPoints.shape[0] == prevPoints.shape[0]):
             H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
             LOGGER.warning("WARNING: not enough matching points")
```

### Comparing `ultralytics-8.1.8/ultralytics/trackers/utils/kalman_filter.py` & `ultralytics-8.1.9/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/trackers/utils/matching.py` & `ultralytics-8.1.9/ultralytics/trackers/utils/matching.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/__init__.py` & `ultralytics-8.1.9/ultralytics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/autobatch.py` & `ultralytics-8.1.9/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/benchmarks.py` & `ultralytics-8.1.9/ultralytics/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/base.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/clearml.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/comet.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/dvc.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/hub.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/mlflow.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/mlflow.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/neptune.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/raytune.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/raytune.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/tensorboard.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/callbacks/wb.py` & `ultralytics-8.1.9/ultralytics/utils/callbacks/wb.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/checks.py` & `ultralytics-8.1.9/ultralytics/utils/checks.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/dist.py` & `ultralytics-8.1.9/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/downloads.py` & `ultralytics-8.1.9/ultralytics/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/errors.py` & `ultralytics-8.1.9/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/files.py` & `ultralytics-8.1.9/ultralytics/utils/files.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/instance.py` & `ultralytics-8.1.9/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/loss.py` & `ultralytics-8.1.9/ultralytics/utils/loss.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/metrics.py` & `ultralytics-8.1.9/ultralytics/utils/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
 
         Args:
             detections (Array[N, 6]): Detected bounding boxes and their associated information.
                                       Each row should contain (x1, y1, x2, y2, conf, class).
             gt_bboxes (Array[M, 4]): Ground truth bounding boxes with xyxy format.
             gt_cls (Array[M]): The class labels.
         """
-        if gt_cls.size(0) == 0:  # Check if labels is empty
+        if gt_cls.shape[0] == 0:  # Check if labels is empty
             if detections is not None:
                 detections = detections[detections[:, 4] > self.conf]
                 detection_classes = detections[:, 5].int()
                 for dc in detection_classes:
                     self.matrix[dc, self.nc] += 1  # false positives
             return
         if detections is None:
@@ -697,25 +697,25 @@
 
     @property
     def map50(self):
         """
         Returns the mean Average Precision (mAP) at an IoU threshold of 0.5.
 
         Returns:
-            (float): The mAP50 at an IoU threshold of 0.5.
+            (float): The mAP at an IoU threshold of 0.5.
         """
         return self.all_ap[:, 0].mean() if len(self.all_ap) else 0.0
 
     @property
     def map75(self):
         """
         Returns the mean Average Precision (mAP) at an IoU threshold of 0.75.
 
         Returns:
-            (float): The mAP50 at an IoU threshold of 0.75.
+            (float): The mAP at an IoU threshold of 0.75.
         """
         return self.all_ap[:, 5].mean() if len(self.all_ap) else 0.0
 
     @property
     def map(self):
         """
         Returns the mean Average Precision (mAP) over IoU thresholds of 0.5 - 0.95 in steps of 0.05.
```

### Comparing `ultralytics-8.1.8/ultralytics/utils/ops.py` & `ultralytics-8.1.9/ultralytics/utils/ops.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/patches.py` & `ultralytics-8.1.9/ultralytics/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/plotting.py` & `ultralytics-8.1.9/ultralytics/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/tal.py` & `ultralytics-8.1.9/ultralytics/utils/tal.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         Returns:
             target_labels (Tensor): shape(bs, num_total_anchors)
             target_bboxes (Tensor): shape(bs, num_total_anchors, 4)
             target_scores (Tensor): shape(bs, num_total_anchors, num_classes)
             fg_mask (Tensor): shape(bs, num_total_anchors)
             target_gt_idx (Tensor): shape(bs, num_total_anchors)
         """
-        self.bs = pd_scores.size(0)
-        self.n_max_boxes = gt_bboxes.size(1)
+        self.bs = pd_scores.shape[0]
+        self.n_max_boxes = gt_bboxes.shape[1]
 
         if self.n_max_boxes == 0:
             device = gt_bboxes.device
             return (
                 torch.full_like(pd_scores[..., 0], self.bg_idx).to(device),
                 torch.zeros_like(pd_bboxes).to(device),
                 torch.zeros_like(pd_scores).to(device),
```

### Comparing `ultralytics-8.1.8/ultralytics/utils/torch_utils.py` & `ultralytics-8.1.9/ultralytics/utils/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
     # Prepare filters
     w_conv = conv.weight.clone().view(conv.out_channels, -1)
     w_bn = torch.diag(bn.weight.div(torch.sqrt(bn.eps + bn.running_var)))
     fusedconv.weight.copy_(torch.mm(w_bn, w_conv).view(fusedconv.weight.shape))
 
     # Prepare spatial bias
-    b_conv = torch.zeros(conv.weight.size(0), device=conv.weight.device) if conv.bias is None else conv.bias
+    b_conv = torch.zeros(conv.weight.shape[0], device=conv.weight.device) if conv.bias is None else conv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fusedconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fusedconv
 
 
 def fuse_deconv_and_bn(deconv, bn):
@@ -217,15 +217,15 @@
 
     # Prepare filters
     w_deconv = deconv.weight.clone().view(deconv.out_channels, -1)
     w_bn = torch.diag(bn.weight.div(torch.sqrt(bn.eps + bn.running_var)))
     fuseddconv.weight.copy_(torch.mm(w_bn, w_deconv).view(fuseddconv.weight.shape))
 
     # Prepare spatial bias
-    b_conv = torch.zeros(deconv.weight.size(1), device=deconv.weight.device) if deconv.bias is None else deconv.bias
+    b_conv = torch.zeros(deconv.weight.shape[1], device=deconv.weight.device) if deconv.bias is None else deconv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fuseddconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fuseddconv
 
 
 def model_info(model, detailed=False, verbose=True, imgsz=640):
```

### Comparing `ultralytics-8.1.8/ultralytics/utils/triton.py` & `ultralytics-8.1.9/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics/utils/tuner.py` & `ultralytics-8.1.9/ultralytics/utils/tuner.py`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics.egg-info/PKG-INFO` & `ultralytics-8.1.9/ultralytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultralytics
-Version: 8.1.8
+Version: 8.1.9
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Author: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/ultralytics/ultralytics/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/ultralytics/ultralytics/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ultralytics Version: 8.1.8 Summary: Ultralytics
+Metadata-Version: 2.1 Name: ultralytics Version: 8.1.9 Summary: Ultralytics
 YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation,
 pose estimation and image classification. Author: Glenn Jocher, Ayush
 Chaurasia, Jing Qiu Maintainer: Glenn Jocher, Ayush Chaurasia, Jing Qiu
 License: AGPL-3.0 Project-URL: Bug Reports, https://github.com/ultralytics/
 ultralytics/issues Project-URL: Funding, https://ultralytics.com Project-URL:
 Source, https://github.com/ultralytics/ultralytics/ Keywords: machine-
 learning,deep-learning,computer-
```

### Comparing `ultralytics-8.1.8/ultralytics.egg-info/SOURCES.txt` & `ultralytics-8.1.9/ultralytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ultralytics-8.1.8/ultralytics.egg-info/requires.txt` & `ultralytics-8.1.9/ultralytics.egg-info/requires.txt`

 * *Files identical despite different names*

