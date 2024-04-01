# Comparing `tmp/aitk-1.0.9-py3-none-any.whl.zip` & `tmp/aitk-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,125 @@
-Zip file size: 1306 bytes, number of entries: 4
--rw-rw-r--  2.0 unx      988 b- defN 21-Jun-09 01:43 aitk-1.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Jun-09 01:43 aitk-1.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 21-Jun-09 01:43 aitk-1.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      284 b- defN 21-Jun-09 01:43 aitk-1.0.9.dist-info/RECORD
-4 files, 1365 bytes uncompressed, 748 bytes compressed:  45.2%
+Zip file size: 329015 bytes, number of entries: 123
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-01 14:41 aitk/__init__.py
+-rw-rw-r--  2.0 unx      372 b- defN 24-Apr-01 14:41 aitk/_version.py
+-rw-rw-r--  2.0 unx      381 b- defN 24-Apr-01 14:41 aitk/algorithms/__init__.py
+-rw-rw-r--  2.0 unx    13343 b- defN 24-Apr-01 14:41 aitk/algorithms/ga.py
+-rw-rw-r--  2.0 unx     4674 b- defN 24-Apr-01 14:41 aitk/algorithms/novelty.py
+-rw-rw-r--  2.0 unx      853 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/__init__.py
+-rw-rw-r--  2.0 unx     3518 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/activations.py
+-rw-rw-r--  2.0 unx     2216 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/aggregations.py
+-rw-rw-r--  2.0 unx     5957 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/attributes.py
+-rw-rw-r--  2.0 unx     3378 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/checkpoint.py
+-rw-rw-r--  2.0 unx     8889 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/config.py
+-rw-rw-r--  2.0 unx    22798 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/distributed.py
+-rw-rw-r--  2.0 unx     4439 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/genes.py
+-rw-rw-r--  2.0 unx    24666 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/genome.py
+-rw-rw-r--  2.0 unx     3535 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/graphs.py
+-rw-rw-r--  2.0 unx     1197 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/math_util.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/parallel.py
+-rw-rw-r--  2.0 unx     5951 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/population.py
+-rw-rw-r--  2.0 unx     5776 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/reporting.py
+-rw-rw-r--  2.0 unx     8010 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/reproduction.py
+-rw-rw-r--  2.0 unx     5283 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/species.py
+-rw-rw-r--  2.0 unx     3344 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/stagnation.py
+-rw-rw-r--  2.0 unx     5084 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/statistics.py
+-rw-rw-r--  2.0 unx     2941 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/threaded.py
+-rw-rw-r--  2.0 unx     5915 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/visualize.py
+-rw-rw-r--  2.0 unx     4538 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/ctrnn/__init__.py
+-rw-rw-r--  2.0 unx     7189 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/iznn/__init__.py
+-rw-rw-r--  2.0 unx      105 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/nn/__init__.py
+-rw-rw-r--  2.0 unx     2271 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/nn/feed_forward.py
+-rw-rw-r--  2.0 unx     5610 b- defN 24-Apr-01 14:41 aitk/algorithms/neat/nn/recurrent.py
+-rw-rw-r--  2.0 unx      818 b- defN 24-Apr-01 14:41 aitk/keras/__init__.py
+-rw-rw-r--  2.0 unx     7902 b- defN 24-Apr-01 14:41 aitk/keras/callbacks.py
+-rw-rw-r--  2.0 unx     1765 b- defN 24-Apr-01 14:41 aitk/keras/metrics.py
+-rw-rw-r--  2.0 unx       27 b- defN 24-Apr-01 14:41 aitk/keras/activations/__init__.py
+-rw-rw-r--  2.0 unx    18370 b- defN 24-Apr-01 14:41 aitk/keras/activations/activations.py
+-rw-rw-r--  2.0 unx       51 b- defN 24-Apr-01 14:41 aitk/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     2798 b- defN 24-Apr-01 14:41 aitk/keras/datasets/boston_housing.py
+-rw-rw-r--  2.0 unx     1341 b- defN 24-Apr-01 14:41 aitk/keras/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3418 b- defN 24-Apr-01 14:41 aitk/keras/datasets/cifar10.py
+-rw-rw-r--  2.0 unx     3256 b- defN 24-Apr-01 14:41 aitk/keras/datasets/cifar100.py
+-rw-rw-r--  2.0 unx     3314 b- defN 24-Apr-01 14:41 aitk/keras/datasets/fashion_mnist.py
+-rw-rw-r--  2.0 unx     7307 b- defN 24-Apr-01 14:41 aitk/keras/datasets/imdb.py
+-rw-rw-r--  2.0 unx     5734 b- defN 24-Apr-01 14:41 aitk/keras/datasets/mnist.py
+-rw-rw-r--  2.0 unx     6374 b- defN 24-Apr-01 14:41 aitk/keras/datasets/reuters.py
+-rw-rw-r--  2.0 unx    26340 b- defN 24-Apr-01 14:41 aitk/keras/datasets/utils.py
+-rw-rw-r--  2.0 unx       28 b- defN 24-Apr-01 14:41 aitk/keras/initializers/__init__.py
+-rw-rw-r--  2.0 unx     8684 b- defN 24-Apr-01 14:41 aitk/keras/initializers/initializers.py
+-rw-rw-r--  2.0 unx   152310 b- defN 24-Apr-01 14:41 aitk/keras/layers/__init__.py
+-rw-rw-r--  2.0 unx      155 b- defN 24-Apr-01 14:41 aitk/keras/losses/__init__.py
+-rw-rw-r--  2.0 unx    34365 b- defN 24-Apr-01 14:41 aitk/keras/losses/losses.py
+-rw-rw-r--  2.0 unx    21288 b- defN 24-Apr-01 14:41 aitk/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    16882 b- defN 24-Apr-01 14:41 aitk/keras/models/vae.py
+-rw-rw-r--  2.0 unx    18495 b- defN 24-Apr-01 14:41 aitk/keras/models/w2v.py
+-rw-rw-r--  2.0 unx    18570 b- defN 24-Apr-01 14:41 aitk/keras/models/wgan_gp.py
+-rw-rw-r--  2.0 unx       23 b- defN 24-Apr-01 14:41 aitk/keras/modules/__init__.py
+-rw-rw-r--  2.0 unx    53276 b- defN 24-Apr-01 14:41 aitk/keras/modules/modules.py
+-rw-rw-r--  2.0 unx      148 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/__init__.py
+-rw-rw-r--  2.0 unx    18443 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/data_structures.py
+-rw-rw-r--  2.0 unx     3159 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/distance_metrics.py
+-rw-rw-r--  2.0 unx    11505 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/graphs.py
+-rw-rw-r--  2.0 unx    11972 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/kernels.py
+-rw-rw-r--  2.0 unx     4503 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/testing.py
+-rw-rw-r--  2.0 unx     5113 b- defN 24-Apr-01 14:41 aitk/keras/numpy_ml_utils/windows.py
+-rw-rw-r--  2.0 unx       26 b- defN 24-Apr-01 14:41 aitk/keras/optimizers/__init__.py
+-rw-rw-r--  2.0 unx    18787 b- defN 24-Apr-01 14:41 aitk/keras/optimizers/optimizers.py
+-rw-rw-r--  2.0 unx       58 b- defN 24-Apr-01 14:41 aitk/keras/preprocessing/__init__.py
+-rw-rw-r--  2.0 unx    29314 b- defN 24-Apr-01 14:41 aitk/keras/preprocessing/dsp.py
+-rw-rw-r--  2.0 unx    12952 b- defN 24-Apr-01 14:41 aitk/keras/preprocessing/general.py
+-rw-rw-r--  2.0 unx    35922 b- defN 24-Apr-01 14:41 aitk/keras/preprocessing/nlp.py
+-rw-rw-r--  2.0 unx       26 b- defN 24-Apr-01 14:41 aitk/keras/schedulers/__init__.py
+-rw-rw-r--  2.0 unx    12389 b- defN 24-Apr-01 14:41 aitk/keras/schedulers/schedulers.py
+-rw-rw-r--  2.0 unx      196 b- defN 24-Apr-01 14:41 aitk/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx    37052 b- defN 24-Apr-01 14:41 aitk/keras/utils/utils.py
+-rw-rw-r--  2.0 unx     8675 b- defN 24-Apr-01 14:41 aitk/keras/wrappers/__init__.py
+-rw-rw-r--  2.0 unx      363 b- defN 24-Apr-01 14:41 aitk/networks/__init__.py
+-rw-rw-r--  2.0 unx     4294 b- defN 24-Apr-01 14:41 aitk/networks/callbacks.py
+-rw-rw-r--  2.0 unx   105211 b- defN 24-Apr-01 14:41 aitk/networks/network.py
+-rw-rw-r--  2.0 unx    14268 b- defN 24-Apr-01 14:41 aitk/networks/utils.py
+-rw-rw-r--  2.0 unx     7235 b- defN 24-Apr-01 14:41 aitk/networks/watchers.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-01 14:41 aitk/robots/__init__.py
+-rw-rw-r--  2.0 unx     5615 b- defN 24-Apr-01 14:41 aitk/robots/cart.py
+-rw-rw-r--  2.0 unx     1538 b- defN 24-Apr-01 14:41 aitk/robots/config.py
+-rw-rw-r--  2.0 unx      870 b- defN 24-Apr-01 14:41 aitk/robots/hit.py
+-rw-rw-r--  2.0 unx    47654 b- defN 24-Apr-01 14:41 aitk/robots/robot.py
+-rw-rw-r--  2.0 unx    20638 b- defN 24-Apr-01 14:41 aitk/robots/utils.py
+-rw-rw-r--  2.0 unx    22209 b- defN 24-Apr-01 14:41 aitk/robots/watchers.py
+-rw-rw-r--  2.0 unx    52755 b- defN 24-Apr-01 14:41 aitk/robots/world.py
+-rw-rw-r--  2.0 unx     1514 b- defN 24-Apr-01 14:41 aitk/robots/backends/__init__.py
+-rw-rw-r--  2.0 unx     7350 b- defN 24-Apr-01 14:41 aitk/robots/backends/base.py
+-rw-rw-r--  2.0 unx     1676 b- defN 24-Apr-01 14:41 aitk/robots/backends/canvas.py
+-rw-rw-r--  2.0 unx     6508 b- defN 24-Apr-01 14:41 aitk/robots/backends/debug.py
+-rw-rw-r--  2.0 unx     8342 b- defN 24-Apr-01 14:41 aitk/robots/backends/pil.py
+-rw-rw-r--  2.0 unx     7108 b- defN 24-Apr-01 14:41 aitk/robots/backends/svg.py
+-rw-rw-r--  2.0 unx      716 b- defN 24-Apr-01 14:41 aitk/robots/datasets/__init__.py
+-rw-rw-r--  2.0 unx     1054 b- defN 24-Apr-01 14:41 aitk/robots/datasets/coil100.py
+-rw-rw-r--  2.0 unx     1115 b- defN 24-Apr-01 14:41 aitk/robots/datasets/coil20.py
+-rw-rw-r--  2.0 unx     9362 b- defN 24-Apr-01 14:41 aitk/robots/datasets/utils.py
+-rw-rw-r--  2.0 unx      627 b- defN 24-Apr-01 14:41 aitk/robots/devices/__init__.py
+-rw-rw-r--  2.0 unx      562 b- defN 24-Apr-01 14:41 aitk/robots/devices/base.py
+-rw-rw-r--  2.0 unx     6921 b- defN 24-Apr-01 14:41 aitk/robots/devices/beacon.py
+-rw-rw-r--  2.0 unx     8413 b- defN 24-Apr-01 14:41 aitk/robots/devices/bulbs.py
+-rw-rw-r--  2.0 unx    31507 b- defN 24-Apr-01 14:41 aitk/robots/devices/cameras.py
+-rw-rw-r--  2.0 unx     7608 b- defN 24-Apr-01 14:41 aitk/robots/devices/compass.py
+-rw-rw-r--  2.0 unx     7976 b- defN 24-Apr-01 14:41 aitk/robots/devices/lightsensors.py
+-rw-rw-r--  2.0 unx    12530 b- defN 24-Apr-01 14:41 aitk/robots/devices/rangesensors.py
+-rw-rw-r--  2.0 unx     5127 b- defN 24-Apr-01 14:41 aitk/robots/devices/smellsensors.py
+-rw-rw-r--  2.0 unx     1557 b- defN 24-Apr-01 14:41 aitk/utils/__init__.py
+-rw-rw-r--  2.0 unx    36202 b- defN 24-Apr-01 14:41 aitk/utils/colors.py
+-rw-rw-r--  2.0 unx     4340 b- defN 24-Apr-01 14:41 aitk/utils/grid.py
+-rw-rw-r--  2.0 unx     2576 b- defN 24-Apr-01 14:41 aitk/utils/joypad.py
+-rw-rw-r--  2.0 unx     7522 b- defN 24-Apr-01 14:41 aitk/utils/joystick.py
+-rw-rw-r--  2.0 unx     9332 b- defN 24-Apr-01 14:41 aitk/utils/utils.py
+-rw-rw-r--  2.0 unx     2648 b- defN 24-Apr-01 14:41 aitk/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx     1465 b- defN 24-Apr-01 14:41 aitk/utils/datasets/cmu_faces.py
+-rw-rw-r--  2.0 unx     1352 b- defN 24-Apr-01 14:41 aitk/utils/datasets/digits6x6.py
+-rw-rw-r--  2.0 unx     1921 b- defN 24-Apr-01 14:41 aitk/utils/datasets/dogs_vs_cats.py
+-rw-rw-r--  2.0 unx      650 b- defN 24-Apr-01 14:41 aitk/utils/datasets/dogs_vs_cats_100.py
+-rw-rw-r--  2.0 unx    13430 b- defN 24-Apr-01 14:41 aitk/utils/datasets/utils.py
+-rw-rw-r--  2.0 unx     1326 b- defN 24-Apr-01 14:41 aitk/utils/datasets/validate_6x6.py
+-rw-rw-r--  2.0 unx     4414 b- defN 24-Apr-01 18:56 aitk-2.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-01 18:56 aitk-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-01 18:56 aitk-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    10620 b- defN 24-Apr-01 18:56 aitk-2.0.0.dist-info/RECORD
+123 files, 1295576 bytes uncompressed, 312313 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,13 +1,370 @@
-Filename: aitk-1.0.9.dist-info/METADATA
+Filename: aitk/__init__.py
 Comment: 
 
-Filename: aitk-1.0.9.dist-info/WHEEL
+Filename: aitk/_version.py
 Comment: 
 
-Filename: aitk-1.0.9.dist-info/top_level.txt
+Filename: aitk/algorithms/__init__.py
 Comment: 
 
-Filename: aitk-1.0.9.dist-info/RECORD
+Filename: aitk/algorithms/ga.py
+Comment: 
+
+Filename: aitk/algorithms/novelty.py
+Comment: 
+
+Filename: aitk/algorithms/neat/__init__.py
+Comment: 
+
+Filename: aitk/algorithms/neat/activations.py
+Comment: 
+
+Filename: aitk/algorithms/neat/aggregations.py
+Comment: 
+
+Filename: aitk/algorithms/neat/attributes.py
+Comment: 
+
+Filename: aitk/algorithms/neat/checkpoint.py
+Comment: 
+
+Filename: aitk/algorithms/neat/config.py
+Comment: 
+
+Filename: aitk/algorithms/neat/distributed.py
+Comment: 
+
+Filename: aitk/algorithms/neat/genes.py
+Comment: 
+
+Filename: aitk/algorithms/neat/genome.py
+Comment: 
+
+Filename: aitk/algorithms/neat/graphs.py
+Comment: 
+
+Filename: aitk/algorithms/neat/math_util.py
+Comment: 
+
+Filename: aitk/algorithms/neat/parallel.py
+Comment: 
+
+Filename: aitk/algorithms/neat/population.py
+Comment: 
+
+Filename: aitk/algorithms/neat/reporting.py
+Comment: 
+
+Filename: aitk/algorithms/neat/reproduction.py
+Comment: 
+
+Filename: aitk/algorithms/neat/species.py
+Comment: 
+
+Filename: aitk/algorithms/neat/stagnation.py
+Comment: 
+
+Filename: aitk/algorithms/neat/statistics.py
+Comment: 
+
+Filename: aitk/algorithms/neat/threaded.py
+Comment: 
+
+Filename: aitk/algorithms/neat/visualize.py
+Comment: 
+
+Filename: aitk/algorithms/neat/ctrnn/__init__.py
+Comment: 
+
+Filename: aitk/algorithms/neat/iznn/__init__.py
+Comment: 
+
+Filename: aitk/algorithms/neat/nn/__init__.py
+Comment: 
+
+Filename: aitk/algorithms/neat/nn/feed_forward.py
+Comment: 
+
+Filename: aitk/algorithms/neat/nn/recurrent.py
+Comment: 
+
+Filename: aitk/keras/__init__.py
+Comment: 
+
+Filename: aitk/keras/callbacks.py
+Comment: 
+
+Filename: aitk/keras/metrics.py
+Comment: 
+
+Filename: aitk/keras/activations/__init__.py
+Comment: 
+
+Filename: aitk/keras/activations/activations.py
+Comment: 
+
+Filename: aitk/keras/datasets/__init__.py
+Comment: 
+
+Filename: aitk/keras/datasets/boston_housing.py
+Comment: 
+
+Filename: aitk/keras/datasets/cifar.py
+Comment: 
+
+Filename: aitk/keras/datasets/cifar10.py
+Comment: 
+
+Filename: aitk/keras/datasets/cifar100.py
+Comment: 
+
+Filename: aitk/keras/datasets/fashion_mnist.py
+Comment: 
+
+Filename: aitk/keras/datasets/imdb.py
+Comment: 
+
+Filename: aitk/keras/datasets/mnist.py
+Comment: 
+
+Filename: aitk/keras/datasets/reuters.py
+Comment: 
+
+Filename: aitk/keras/datasets/utils.py
+Comment: 
+
+Filename: aitk/keras/initializers/__init__.py
+Comment: 
+
+Filename: aitk/keras/initializers/initializers.py
+Comment: 
+
+Filename: aitk/keras/layers/__init__.py
+Comment: 
+
+Filename: aitk/keras/losses/__init__.py
+Comment: 
+
+Filename: aitk/keras/losses/losses.py
+Comment: 
+
+Filename: aitk/keras/models/__init__.py
+Comment: 
+
+Filename: aitk/keras/models/vae.py
+Comment: 
+
+Filename: aitk/keras/models/w2v.py
+Comment: 
+
+Filename: aitk/keras/models/wgan_gp.py
+Comment: 
+
+Filename: aitk/keras/modules/__init__.py
+Comment: 
+
+Filename: aitk/keras/modules/modules.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/__init__.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/data_structures.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/distance_metrics.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/graphs.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/kernels.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/testing.py
+Comment: 
+
+Filename: aitk/keras/numpy_ml_utils/windows.py
+Comment: 
+
+Filename: aitk/keras/optimizers/__init__.py
+Comment: 
+
+Filename: aitk/keras/optimizers/optimizers.py
+Comment: 
+
+Filename: aitk/keras/preprocessing/__init__.py
+Comment: 
+
+Filename: aitk/keras/preprocessing/dsp.py
+Comment: 
+
+Filename: aitk/keras/preprocessing/general.py
+Comment: 
+
+Filename: aitk/keras/preprocessing/nlp.py
+Comment: 
+
+Filename: aitk/keras/schedulers/__init__.py
+Comment: 
+
+Filename: aitk/keras/schedulers/schedulers.py
+Comment: 
+
+Filename: aitk/keras/utils/__init__.py
+Comment: 
+
+Filename: aitk/keras/utils/utils.py
+Comment: 
+
+Filename: aitk/keras/wrappers/__init__.py
+Comment: 
+
+Filename: aitk/networks/__init__.py
+Comment: 
+
+Filename: aitk/networks/callbacks.py
+Comment: 
+
+Filename: aitk/networks/network.py
+Comment: 
+
+Filename: aitk/networks/utils.py
+Comment: 
+
+Filename: aitk/networks/watchers.py
+Comment: 
+
+Filename: aitk/robots/__init__.py
+Comment: 
+
+Filename: aitk/robots/cart.py
+Comment: 
+
+Filename: aitk/robots/config.py
+Comment: 
+
+Filename: aitk/robots/hit.py
+Comment: 
+
+Filename: aitk/robots/robot.py
+Comment: 
+
+Filename: aitk/robots/utils.py
+Comment: 
+
+Filename: aitk/robots/watchers.py
+Comment: 
+
+Filename: aitk/robots/world.py
+Comment: 
+
+Filename: aitk/robots/backends/__init__.py
+Comment: 
+
+Filename: aitk/robots/backends/base.py
+Comment: 
+
+Filename: aitk/robots/backends/canvas.py
+Comment: 
+
+Filename: aitk/robots/backends/debug.py
+Comment: 
+
+Filename: aitk/robots/backends/pil.py
+Comment: 
+
+Filename: aitk/robots/backends/svg.py
+Comment: 
+
+Filename: aitk/robots/datasets/__init__.py
+Comment: 
+
+Filename: aitk/robots/datasets/coil100.py
+Comment: 
+
+Filename: aitk/robots/datasets/coil20.py
+Comment: 
+
+Filename: aitk/robots/datasets/utils.py
+Comment: 
+
+Filename: aitk/robots/devices/__init__.py
+Comment: 
+
+Filename: aitk/robots/devices/base.py
+Comment: 
+
+Filename: aitk/robots/devices/beacon.py
+Comment: 
+
+Filename: aitk/robots/devices/bulbs.py
+Comment: 
+
+Filename: aitk/robots/devices/cameras.py
+Comment: 
+
+Filename: aitk/robots/devices/compass.py
+Comment: 
+
+Filename: aitk/robots/devices/lightsensors.py
+Comment: 
+
+Filename: aitk/robots/devices/rangesensors.py
+Comment: 
+
+Filename: aitk/robots/devices/smellsensors.py
+Comment: 
+
+Filename: aitk/utils/__init__.py
+Comment: 
+
+Filename: aitk/utils/colors.py
+Comment: 
+
+Filename: aitk/utils/grid.py
+Comment: 
+
+Filename: aitk/utils/joypad.py
+Comment: 
+
+Filename: aitk/utils/joystick.py
+Comment: 
+
+Filename: aitk/utils/utils.py
+Comment: 
+
+Filename: aitk/utils/datasets/__init__.py
+Comment: 
+
+Filename: aitk/utils/datasets/cmu_faces.py
+Comment: 
+
+Filename: aitk/utils/datasets/digits6x6.py
+Comment: 
+
+Filename: aitk/utils/datasets/dogs_vs_cats.py
+Comment: 
+
+Filename: aitk/utils/datasets/dogs_vs_cats_100.py
+Comment: 
+
+Filename: aitk/utils/datasets/utils.py
+Comment: 
+
+Filename: aitk/utils/datasets/validate_6x6.py
+Comment: 
+
+Filename: aitk-2.0.0.dist-info/METADATA
+Comment: 
+
+Filename: aitk-2.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: aitk-2.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: aitk-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

