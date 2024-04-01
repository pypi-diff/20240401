# Comparing `tmp/fdasrsf-2.5.8.tar.gz` & `tmp/fdasrsf-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdasrsf-2.5.8.tar", last modified: Wed Feb 14 13:09:40 2024, max compression
+gzip compressed data, was "fdasrsf-2.5.9.tar", last modified: Tue Feb 27 15:14:00 2024, max compression
```

## Comparing `fdasrsf-2.5.8.tar` & `fdasrsf-2.5.9.tar`

### file list

```diff
@@ -1,737 +1,737 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.847266 fdasrsf-2.5.8/bin/
--rw-r--r--   0 runner    (1001) docker     (127)  2156461 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/bin/MPEG7.npz
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/bin/ex_srsf_align.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/bin/simu_data.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.843266 fdasrsf-2.5.8/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.843266 fdasrsf-2.5.8/doc/build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.847266 fdasrsf-2.5.8/doc/build/man/
--rw-r--r--   0 runner    (1001) docker     (127)    98266 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/doc/build/man/fdasrsf.1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.851266 fdasrsf-2.5.8/fdasrsf/
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/bayesian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/boxplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    28664 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/curve_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/curve_pcr_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    36298 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/curve_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/curve_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/elastic_changepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/elastic_glm_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/fPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/fPLS.py
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/geodesic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/gp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/image_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/interparc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)    27597 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/pcr_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/plot_style.py
--rw-r--r--   0 runner    (1001) docker     (127)    20132 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/rbfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    71647 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/time_warping.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/umap_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    31991 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/fdasrsf/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/fdasrsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/fdasrsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25491 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/fdasrsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/fdasrsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/fdasrsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/fdasrsf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.855266 fdasrsf-2.5.8/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   515522 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/notebooks/example_curve.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   775961 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/notebooks/example_mvwarping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  2208768 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/notebooks/example_warping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.867267 fdasrsf-2.5.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/DP.c
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/DP.h
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/DynamicProgrammingQ2.c
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/DynamicProgrammingQ2.h
--rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/ImageRegister.h
--rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/UnitSquareImage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/UnitSquareImage.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.867267 fdasrsf-2.5.8/src/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-14 13:09:40.000000 fdasrsf-2.5.8/src/__pycache__/dp_build.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    33028 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/src/armadillo_bits/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/BaseCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/BaseCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Base_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Base_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Col_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    39469 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Col_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/CubeToMatOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/CubeToMatOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28666 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Cube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   128598 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Cube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/GenCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/GenCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Gen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Gen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/GlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/GlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Glue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Glue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/MapMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/MapMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    46136 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   207713 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/OpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/OpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Op_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Op_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    94856 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/ProxyCube.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Row_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    39413 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/Row_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SizeCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SizeCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SizeMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SizeMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpBase_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18862 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpBase_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpCol_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpCol_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    35787 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpMat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    25196 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpMat_iterators_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   148452 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpMat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpProxy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpRow_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpRow_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpSubview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpSubview_col_list_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14234 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpSubview_col_list_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31949 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpSubview_iterators_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    40563 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpSubview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpToDGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpToDGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpToDOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpToDOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpValProxy_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/SpValProxy_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/access.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_cmath.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_forward.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_ostream_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28965 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_ostream_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_rel_comparators.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23840 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_rng.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_rng_cxx03.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_static_check.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_str.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arma_version.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arrayops_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19641 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/arrayops_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20199 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/auxlib_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   200024 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/auxlib_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/band_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/compiler_check.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/compiler_setup.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/compiler_setup_post.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/cond_rel_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/cond_rel_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/config.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/config.hpp.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/constants.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/constants_old.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/csv_name.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/debug.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_arpack.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_atlas.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_blas.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   115263 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_lapack.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/def_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/diagmat_proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/diagview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22511 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/diagview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/diskio_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   131536 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/diskio_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/distr_param.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eGlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eGlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eOpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eOpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eglue_core_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    46921 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eglue_core_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eop_aux.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eop_core_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/eop_core_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fft_engine_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fft_engine_kissfft.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/field_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    62261 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/field_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fill.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23665 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_accu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_all.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_any.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_approx_equal.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_as_scalar.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_chi2rnd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_chol.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_clamp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cond_rcond.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_conv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_conv_to.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cross.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cumprod.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_cumsum.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_det.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_diagmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_diags_spdiags.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_diagvec.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_diff.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_dot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eig_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eig_pair.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eig_sym.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eigs_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eigs_sym.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_elem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eps.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_expmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_eye.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_fft.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_fft2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_find.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_find_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_flip.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_hess.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_hist.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_histc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_index_max.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_index_min.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_inplace_strans.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_inplace_trans.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_interp1.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_interp2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_intersect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_inv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_inv_sympd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_join.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_kmeans.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_kron.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_log_det.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_log_normpdf.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_logmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_lu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_max.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_mean.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_median.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_min.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_mvnrnd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_n_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_nonzeros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_norm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_normalise.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_normcdf.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_normpdf.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_numel.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_ones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_orth_null.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_pinv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_polyfit.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_polyval.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_powext.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_powmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_princomp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_prod.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_qr.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_quantile.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_qz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_randg.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_randi.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_randn.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_randperm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_randu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_range.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_rank.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_regspace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_repelem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_repmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_reshape.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_resize.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_reverse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_roots.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_shift.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_shuffle.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_size.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_solve.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sort.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sort_index.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_speye.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_spones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sprandn.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sprandu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_spsolve.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sqrtmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_stddev.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_strans.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sum.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_svd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_svds.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_sylvester.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_symmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_toeplitz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16300 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trans.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trapz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trig.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trimat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trimat_ind.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trunc_exp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_trunc_log.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_unique.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_var.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_vecnorm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_vectorise.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_wishrnd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/fn_zeros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_affmul_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_affmul_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_atan2_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_atan2_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_conv_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_conv_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cor_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cor_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cov_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cov_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cross_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_cross_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_hist_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_hist_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_histc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_histc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_hypot_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_hypot_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_intersect_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_intersect_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_join_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_join_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_kron_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_kron_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_mixed_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_mixed_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_mvnrnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_mvnrnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_polyfit_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_polyfit_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_polyval_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_polyval_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_powext_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_powext_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_quantile_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_quantile_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_solve_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20198 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_solve_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_times_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_times_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_times_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16965 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_times_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_toeplitz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_toeplitz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_trapz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/glue_trapz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_diag_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    66061 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_diag_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_full_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    68553 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_full_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/gmm_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/hdf5_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/hdf5_name.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/include_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/include_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/injector_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/injector_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/memory.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mp_misc.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtGlueCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtGlueCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtOpCube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtOpCube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtSpGlue_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtSpGlue_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtSpOp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mtSpOp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mul_gemm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mul_gemm_mixed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mul_gemv.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mul_herk.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/mul_syrk.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_EigsSelect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SortEigenvalue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenRealShiftSolve_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenRealShiftSolve_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsShiftSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsShiftSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_TridiagEigen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_TridiagEigen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/newarp_cx_attrib.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_all_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_all_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_any_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_any_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_chi2rnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_chi2rnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_chol_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_chol_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_clamp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_clamp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_col_as_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_col_as_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cond_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cond_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cor_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cor_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cov_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cov_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cumprod_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cumprod_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cumsum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cumsum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cx_scalar_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_cx_scalar_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_det_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_det_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diagmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diagmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diagvec_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diagvec_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diff_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_diff_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_dot_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_dot_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_dotext_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_dotext_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_expmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_expmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_fft_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_fft_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_find_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_find_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_find_unique_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_find_unique_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_flip_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_flip_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_hist_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_hist_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_htrans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_index_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_index_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_index_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_index_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_inv_gen_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_inv_gen_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_inv_spd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_inv_spd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_log_det_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_log_det_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_logmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_logmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27955 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_mean_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_mean_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_median_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_median_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27955 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_nonzeros_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_nonzeros_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_norm2est_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_norm2est_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_norm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17945 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_norm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_normalise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_normalise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_orth_null_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_orth_null_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_pinv_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_pinv_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_powmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_powmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_princomp_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_princomp_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_prod_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_prod_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_range_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_range_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_rank_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_rank_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_rcond_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_rcond_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_repelem_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_repelem_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_repmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_repmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_reshape_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_reshape_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_resize_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_resize_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_reverse_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_reverse_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_roots_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_roots_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_row_as_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_row_as_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_shift_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_shift_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_shuffle_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_shuffle_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sort_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sort_index_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sort_index_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sort_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sp_minus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sp_minus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sp_plus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sp_plus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sqrtmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sqrtmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_stddev_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_stddev_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_strans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_strans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_sum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_symmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_symmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_toeplitz_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_toeplitz_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_trimat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_trimat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_unique_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_unique_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_var_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_var_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_vecnorm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_vecnorm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_vectorise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_vectorise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_wishrnd_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/op_wishrnd_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_div.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_minus.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_plus.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_relational.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_cube_times.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_div.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_minus.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_ostream.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_plus.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_relational.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_schur.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/operator_times.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/podarray_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/podarray_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/promote_type.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/rbfgs.h
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/restrictors.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/running_stat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/running_stat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/running_stat_vec_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14471 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/running_stat_vec_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/sp_auxlib_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    89069 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/sp_auxlib_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/span.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spdiagview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spdiagview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_join_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_join_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_kron_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_kron_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_merge_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_merge_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_minus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_minus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_plus_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_plus_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_relational_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_relational_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_schur_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_schur_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_times_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spglue_times_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_diagmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_diagmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_htrans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_max_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_max_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_mean_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_mean_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_min_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_min_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_misc_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_misc_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_norm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_norm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_normalise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_normalise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_repmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_repmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_reverse_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_reverse_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_strans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_strans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_sum_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_sum_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_symmat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_symmat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_trimat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_trimat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_var_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_var_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_vecnorm_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_vecnorm_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_vectorise_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spop_vectorise_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spsolve_factoriser_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/spsolve_factoriser_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/strip.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24982 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_each_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_each_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    68242 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_slices_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_cube_slices_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_each_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30688 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_each_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_elem1_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_elem1_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_elem2_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21411 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_elem2_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_field_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_field_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)   109736 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/subview_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/sym_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30226 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_arpack.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_atlas.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_blas.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_fftw3.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    84711 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_lapack.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/translate_superlu.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/trimat_helper.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/typedef_elem.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/typedef_elem_check.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/typedef_mat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/typedef_mat_fixed.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    77808 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/unwrap.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/unwrap_cube.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/unwrap_spmat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/upgrade_val.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/wall_clock_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/wall_clock_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/xtrans_mat_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/xtrans_mat_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/xvec_htrans_bones.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/armadillo_bits/xvec_htrans_meat.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/bayesian.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/bayesian.h
--rw-r--r--   0 runner    (1001) docker     (127)    86846 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/c8lib.c
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/c8lib.h
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cDP.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cDPQ.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cUnitSquareImage.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cbayesian.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cbayesian.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cfPLS.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cmlogit.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/coclogit.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cocmlogit.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/crbfgs.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/crbfgs.pyx
--rwxr-xr-x   0 runner    (1001) docker     (127)     5186 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cyarma.pxd
--rwxr-xr-x   0 runner    (1001) docker     (127)     9637 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/cyarma.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/dp_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/dp_grid.c
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/dp_grid.h
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/dp_nbhd.c
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/dp_nbhd.h
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/fpls_warp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/fpls_warp_grad.c
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/fpls_warp_grad.h
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/imagecpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/matrix_exponential.c
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/matrix_exponential.h
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/misc_funcs.c
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/misc_funcs.h
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/mlogit_warp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/mlogit_warp_grad.c
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/mlogit_warp_grad.h
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/myVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/myVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/oclogit_warp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/oclogit_warp_grad.c
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/oclogit_warp_grad.h
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/ocmlogit_warp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/ocmlogit_warp_grad.c
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/ocmlogit_warp_grad.h
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/optimum_reparamN2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/optimum_reparam_N.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   832370 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/r8lib.c
--rw-r--r--   0 runner    (1001) docker     (127)    32641 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/r8lib.h
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/rbfgs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/src/rbfgs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:09:40.963267 fdasrsf-2.5.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-02-14 13:09:27.000000 fdasrsf-2.5.8/test/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.390827 fdasrsf-2.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-02-27 15:14:00.390827 fdasrsf-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.278828 fdasrsf-2.5.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)  2156461 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/bin/MPEG7.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/bin/ex_srsf_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/bin/simu_data.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.274828 fdasrsf-2.5.9/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.274828 fdasrsf-2.5.9/doc/build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.278828 fdasrsf-2.5.9/doc/build/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    98266 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/doc/build/man/fdasrsf.1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.282828 fdasrsf-2.5.9/fdasrsf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/bayesian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/boxplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28686 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/curve_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/curve_pcr_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36298 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/curve_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/curve_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/elastic_changepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/elastic_glm_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23141 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/fPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/fPLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/geodesic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/image_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/interparc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/pcr_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/plot_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20132 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/rbfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71647 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/time_warping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/umap_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31991 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/fdasrsf/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.386827 fdasrsf-2.5.9/fdasrsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-02-27 15:14:00.000000 fdasrsf-2.5.9/fdasrsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25491 2024-02-27 15:14:00.000000 fdasrsf-2.5.9/fdasrsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 15:14:00.000000 fdasrsf-2.5.9/fdasrsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-27 15:14:00.000000 fdasrsf-2.5.9/fdasrsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-27 15:14:00.000000 fdasrsf-2.5.9/fdasrsf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.282828 fdasrsf-2.5.9/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   515522 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/notebooks/example_curve.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   775961 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/notebooks/example_mvwarping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2208768 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/notebooks/example_warping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-27 15:14:00.390827 fdasrsf-2.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.294828 fdasrsf-2.5.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/DP.c
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/DP.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/DynamicProgrammingQ2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/DynamicProgrammingQ2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/ImageRegister.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/UnitSquareImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/UnitSquareImage.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.294828 fdasrsf-2.5.9/src/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-27 15:13:59.000000 fdasrsf-2.5.9/src/__pycache__/dp_build.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)    33028 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.386827 fdasrsf-2.5.9/src/armadillo_bits/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/BaseCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/BaseCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Base_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Base_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Col_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39469 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Col_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/CubeToMatOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/CubeToMatOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28666 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Cube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   128598 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Cube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/GenCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/GenCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Gen_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Gen_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/GlueCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/GlueCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Glue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Glue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/MapMat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/MapMat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46136 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Mat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   207713 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Mat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/OpCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/OpCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Op_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Op_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    94856 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Proxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/ProxyCube.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Row_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    39413 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/Row_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SizeCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SizeCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SizeMat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SizeMat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpBase_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18862 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpBase_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpCol_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpCol_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpGlue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpGlue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35787 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpMat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25196 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpMat_iterators_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   148452 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpMat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpProxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpRow_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpRow_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpSubview_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpSubview_col_list_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14234 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpSubview_col_list_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31949 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpSubview_iterators_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40563 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpSubview_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpToDGlue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpToDGlue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpToDOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpToDOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpValProxy_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/SpValProxy_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/access.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_cmath.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_forward.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_ostream_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28965 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_ostream_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_rel_comparators.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23840 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_rng.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_rng_cxx03.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_static_check.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_str.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arma_version.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arrayops_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19641 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/arrayops_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20199 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/auxlib_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   200024 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/auxlib_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/band_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/compiler_check.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/compiler_setup.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/compiler_setup_post.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/cond_rel_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/cond_rel_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12563 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/config.hpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    10926 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/constants_old.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/csv_name.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/debug.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_arpack.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_atlas.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_blas.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_fftw3.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   115263 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_lapack.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/def_superlu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/diagmat_proxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/diagview_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22511 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/diagview_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/diskio_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   131536 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/diskio_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/distr_param.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eGlueCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eGlueCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eGlue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eGlue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eOpCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eOpCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eglue_core_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46921 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eglue_core_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eop_aux.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eop_core_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30632 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/eop_core_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fft_engine_fftw3.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fft_engine_kissfft.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/field_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    62261 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/field_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fill.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23665 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_accu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_all.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_any.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_approx_equal.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_as_scalar.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_chi2rnd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_chol.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_clamp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cond_rcond.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_conv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_conv_to.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cross.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cumprod.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_cumsum.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_det.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_diagmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_diags_spdiags.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_diagvec.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_diff.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_dot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eig_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eig_pair.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eig_sym.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eigs_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eigs_sym.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_elem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eps.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_expmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_eye.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_fft.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_fft2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_find.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_find_unique.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_flip.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_hess.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_hist.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_histc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_index_max.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_index_min.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_inplace_strans.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_inplace_trans.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_interp1.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_interp2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_intersect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_inv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_inv_sympd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_join.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_kmeans.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_kron.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_log_det.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_log_normpdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_logmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_lu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_max.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_mean.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_median.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_min.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_mvnrnd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_n_unique.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_nonzeros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_norm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_normalise.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_normcdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_normpdf.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_numel.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_ones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_orth_null.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_pinv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_polyfit.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_polyval.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_powext.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_powmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_princomp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_prod.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_qr.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_quantile.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_qz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_randg.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_randi.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_randn.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_randperm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_randu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_range.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_rank.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_regspace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_repelem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_repmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_reshape.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_resize.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_reverse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_roots.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_schur.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_shift.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_shuffle.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_size.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_solve.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sort.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sort_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_speye.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_spones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sprandn.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sprandu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_spsolve.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sqrtmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_stddev.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_strans.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sum.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_svd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_svds.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_sylvester.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_symmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_toeplitz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16300 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trans.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trapz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trig.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trimat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trimat_ind.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trunc_exp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_trunc_log.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_unique.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_var.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8626 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_vecnorm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_vectorise.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_wishrnd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/fn_zeros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_affmul_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_affmul_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_atan2_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_atan2_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_conv_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_conv_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cor_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cor_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cov_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cov_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cross_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_cross_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_hist_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_hist_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_histc_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_histc_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_hypot_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_hypot_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_intersect_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_intersect_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_join_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_join_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_kron_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_kron_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_max_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_max_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_min_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_min_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_mixed_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_mixed_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_mvnrnd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_mvnrnd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_polyfit_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_polyfit_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_polyval_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_polyval_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_powext_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_powext_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_quantile_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_quantile_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_relational_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_relational_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_solve_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20198 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_solve_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_times_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_times_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_times_misc_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16965 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_times_misc_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_toeplitz_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_toeplitz_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_trapz_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/glue_trapz_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_diag_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    66061 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_diag_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_full_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    68553 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_full_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_misc_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/gmm_misc_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/hdf5_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/hdf5_name.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/include_hdf5.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/include_superlu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/injector_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/injector_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/memory.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mp_misc.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtGlueCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtGlueCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtGlue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtGlue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtOpCube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtOpCube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtSpGlue_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtSpGlue_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtSpOp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mtSpOp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mul_gemm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mul_gemm_mixed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mul_gemv.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mul_herk.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/mul_syrk.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_EigsSelect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SortEigenvalue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenRealShiftSolve_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenRealShiftSolve_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsShiftSolver_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsShiftSolver_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_TridiagEigen_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_TridiagEigen_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/newarp_cx_attrib.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_all_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_all_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_any_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_any_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_chi2rnd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_chi2rnd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_chol_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_chol_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_clamp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_clamp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_col_as_mat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_col_as_mat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cond_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cond_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cor_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cor_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cov_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cov_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cumprod_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cumprod_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cumsum_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cumsum_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cx_scalar_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_cx_scalar_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_det_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_det_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diagmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20265 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diagmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diagvec_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diagvec_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diff_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_diff_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_dot_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_dot_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_dotext_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_dotext_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_expmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_expmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_fft_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_fft_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_find_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_find_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_find_unique_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_find_unique_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_flip_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_flip_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_hist_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_hist_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_htrans_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_htrans_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_index_max_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_index_max_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_index_min_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_index_min_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_inv_gen_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_inv_gen_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_inv_spd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_inv_spd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_log_det_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_log_det_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_logmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_logmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_max_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27955 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_max_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_mean_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_mean_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_median_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_median_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_min_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27955 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_min_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_misc_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_misc_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_nonzeros_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_nonzeros_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_norm2est_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_norm2est_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_norm_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17945 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_norm_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_normalise_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_normalise_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_orth_null_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_orth_null_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_pinv_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_pinv_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_powmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_powmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_princomp_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_princomp_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_prod_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_prod_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_range_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_range_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_rank_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_rank_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_rcond_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_rcond_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_relational_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_relational_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_repelem_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_repelem_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_repmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_repmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_reshape_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_reshape_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_resize_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_resize_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_reverse_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_reverse_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_roots_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_roots_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_row_as_mat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_row_as_mat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_shift_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_shift_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_shuffle_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_shuffle_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sort_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sort_index_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sort_index_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sort_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sp_minus_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sp_minus_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sp_plus_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sp_plus_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sqrtmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sqrtmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_stddev_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_stddev_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_strans_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_strans_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sum_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_sum_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_symmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_symmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_toeplitz_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_toeplitz_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_trimat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_trimat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_unique_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_unique_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_var_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_var_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_vecnorm_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_vecnorm_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_vectorise_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_vectorise_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_wishrnd_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/op_wishrnd_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_div.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_minus.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_plus.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_relational.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_schur.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_cube_times.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_div.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_minus.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_ostream.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_plus.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_relational.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_schur.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/operator_times.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/podarray_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/podarray_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14372 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/promote_type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/rbfgs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/restrictors.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/running_stat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/running_stat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/running_stat_vec_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14471 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/running_stat_vec_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9582 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/sp_auxlib_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    89069 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/sp_auxlib_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/span.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spdiagview_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23126 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spdiagview_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_join_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_join_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_kron_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_kron_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_max_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_max_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_merge_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_merge_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_min_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_min_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_minus_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_minus_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_plus_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_plus_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_relational_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_relational_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_schur_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_schur_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_times_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spglue_times_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_diagmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_diagmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_htrans_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_htrans_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_max_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_max_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_mean_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_mean_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_min_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_min_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_misc_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_misc_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_norm_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_norm_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_normalise_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_normalise_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_repmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_repmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_reverse_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_reverse_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_strans_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_strans_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_sum_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_sum_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_symmat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_symmat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_trimat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_trimat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_var_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_var_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_vecnorm_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_vecnorm_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_vectorise_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spop_vectorise_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spsolve_factoriser_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/spsolve_factoriser_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/strip.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    24982 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_each_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_each_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    68242 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_slices_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11878 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_cube_slices_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_each_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30688 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_each_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_elem1_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_elem1_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_elem2_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21411 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_elem2_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_field_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_field_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)   109736 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/subview_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12640 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/sym_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30226 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_arpack.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_atlas.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_blas.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_fftw3.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    84711 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_lapack.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/translate_superlu.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/trimat_helper.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/typedef_elem.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/typedef_elem_check.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/typedef_mat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/typedef_mat_fixed.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    77808 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/unwrap.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/unwrap_cube.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/unwrap_spmat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/upgrade_val.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/wall_clock_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/wall_clock_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/xtrans_mat_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/xtrans_mat_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/xvec_htrans_bones.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/armadillo_bits/xvec_htrans_meat.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/bayesian.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/bayesian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    86846 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/c8lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/c8lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cDP.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cDPQ.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cUnitSquareImage.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cbayesian.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cbayesian.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cfPLS.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cmlogit.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/coclogit.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cocmlogit.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/crbfgs.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/crbfgs.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5186 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cyarma.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9637 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/cyarma.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/dp_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/dp_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/dp_grid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/dp_nbhd.c
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/dp_nbhd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/fpls_warp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/fpls_warp_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/fpls_warp_grad.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/imagecpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/matrix_exponential.c
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/matrix_exponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/misc_funcs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/misc_funcs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/mlogit_warp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/mlogit_warp_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/mlogit_warp_grad.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/myVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/myVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/oclogit_warp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/oclogit_warp_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/oclogit_warp_grad.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/ocmlogit_warp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/ocmlogit_warp_grad.c
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/ocmlogit_warp_grad.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/optimum_reparamN2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/optimum_reparam_N.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   832370 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/r8lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    32641 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/r8lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/rbfgs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/src/rbfgs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:14:00.386827 fdasrsf-2.5.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-02-27 15:13:47.000000 fdasrsf-2.5.9/test/test_all.py
```

### Comparing `fdasrsf-2.5.8/LICENSE.txt` & `fdasrsf-2.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/PKG-INFO` & `fdasrsf-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdasrsf
-Version: 2.5.8
+Version: 2.5.9
 Summary: functional data analysis using the square root slope framework
 Home-page: http://research.tetonedge.net
 Author: J. Derek Tucker
 Author-email: "J. Derek Tucker" <jdtuck@sandia.gov>
 License: BSD 3-Clause
 Project-URL: homepage, http://research.tetonedge.net
 Project-URL: repository, https://github.com/jdtuck/fdasrsf_python
@@ -47,15 +47,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.5.8 is on pip and can be installed using
+v2.5.9 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.5.8/README.md` & `fdasrsf-2.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.5.8 is on pip and can be installed using
+v2.5.9 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.5.8/bin/MPEG7.npz` & `fdasrsf-2.5.9/bin/MPEG7.npz`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/bin/simu_data.npz` & `fdasrsf-2.5.9/bin/simu_data.npz`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/doc/build/man/fdasrsf.1` & `fdasrsf-2.5.9/doc/build/man/fdasrsf.1`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/__init__.py` & `fdasrsf-2.5.9/fdasrsf/__init__.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/bayesian_functions.py` & `fdasrsf-2.5.9/fdasrsf/bayesian_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/boxplots.py` & `fdasrsf-2.5.9/fdasrsf/boxplots.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/curve_functions.py` & `fdasrsf-2.5.9/fdasrsf/curve_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     """
     n, T = beta.shape
     v = gradient(beta, 1.0 / (T - 1))
     v = v[1]
 
     q = zeros((n, T))
-    lenb = sqrt(innerprod_q2(v, v))
+    lenb = sqrt(innerprod_q2(sqrt(abs(v)), sqrt(abs(v))))
     for i in range(0, T):
         L = sqrt(norm(v[:, i]))
         if L > 0.0001:
             q[:, i] = v[:, i] / L
         else:
             q[:, i] = v[:, i] * 0.0001
```

### Comparing `fdasrsf-2.5.8/fdasrsf/curve_pcr_regression.py` & `fdasrsf-2.5.9/fdasrsf/curve_pcr_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/curve_regression.py` & `fdasrsf-2.5.9/fdasrsf/curve_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/curve_stats.py` & `fdasrsf-2.5.9/fdasrsf/curve_stats.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/elastic_changepoint.py` & `fdasrsf-2.5.9/fdasrsf/elastic_changepoint.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/elastic_glm_regression.py` & `fdasrsf-2.5.9/fdasrsf/elastic_glm_regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/fPCA.py` & `fdasrsf-2.5.9/fdasrsf/fPCA.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         c = np.zeros((N2, no))
         for k in range(0, no):
             for l in range(0, N2):
                 c[l, k] = sum((np.append(qn[:, l], m_new[l]) - mqn) * U[:, k])
 
         if var_exp is not None:
             cumm_coef = np.cumsum(s) / sum(s)
-            no = np.argwhere(cumm_coef <= var_exp)[-1]
+            no = int(np.argwhere(cumm_coef <= var_exp)[-1])
 
         self.q_pca = q_pca
         self.f_pca = f_pca
         self.latent = s[0:no]
         self.coef = c[:, 0:no]
         self.U = U[:, 0:no]
         self.id = mididx
@@ -332,15 +332,15 @@
         c = np.zeros((N2, no))
         for k in range(0, no):
             for i in range(0, N2):
                 c[i, k] = np.dot(vec[:, i] - vm, U[:, k])
 
         if var_exp is not None:
             cumm_coef = np.cumsum(s) / sum(s)
-            no = np.argwhere(cumm_coef <= var_exp)[-1]
+            no = int(np.argwhere(cumm_coef <= var_exp)[-1])
 
         self.gam_pca = gam_pca
         self.psi_pca = psi_pca
         self.U = U[:, 0:no]
         self.coef = c[:, 0:no]
         self.latent = s[0:no]
         self.gam_mu = gam_mu
@@ -566,15 +566,15 @@
                 f_pca[:, l, k] = uf.warp_f_gamma(np.linspace(0, 1, M), fhat, gamhat)
                 q_pca[:, l, k] = uf.warp_q_gamma(
                     np.linspace(0, 1, M), qhat[0:M], gamhat
                 )
 
         if var_exp is not None:
             cumm_coef = np.cumsum(s) / s.sum()
-            no = np.argwhere(cumm_coef >= var_exp)[0][0]
+            no = int(np.argwhere(cumm_coef >= var_exp)[0][0])
 
         self.q_pca = q_pca
         self.f_pca = f_pca
         self.latent = s[0:no]
         self.coef = a[:, 0:no]
         self.U = U[:, 0:no]
         self.mu_psi = mu_psi
```

### Comparing `fdasrsf-2.5.8/fdasrsf/fPLS.py` & `fdasrsf-2.5.9/fdasrsf/fPLS.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/geodesic.py` & `fdasrsf-2.5.9/fdasrsf/geodesic.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/geometry.py` & `fdasrsf-2.5.9/fdasrsf/geometry.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/gp.py` & `fdasrsf-2.5.9/fdasrsf/gp.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/image.py` & `fdasrsf-2.5.9/fdasrsf/image.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/image_functions.py` & `fdasrsf-2.5.9/fdasrsf/image_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/interparc.py` & `fdasrsf-2.5.9/fdasrsf/interparc.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/kmeans.py` & `fdasrsf-2.5.9/fdasrsf/kmeans.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/pcr_regression.py` & `fdasrsf-2.5.9/fdasrsf/pcr_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,26 +51,29 @@
         self.y = y
         self.time = time
 
     def calc_model(
         self,
         pca_method="combined",
         no=5,
+        var_exp=None,
         smooth_data=False,
         sparam=25,
         parallel=False,
         C=None,
     ):
         """
         This function identifies a regression model with phase-variability
         using elastic pca
 
         :param pca_method: string specifying pca method (options = "combined",
                         "vert", or "horiz", default = "combined")
         :param no: scalar specify number of principal components (default=5)
+        :param var_exp: compute no based on value percent variance explained
+                        (example: 0.95)
         :param smooth_data: smooth data using box filter (default = F)
         :param sparam: number of times to apply box filter (default = 25)
         :param parallel: run in parallel (default = F)
         :param C: scale balance parameter for combined method (default = None)
         """
 
         if smooth_data:
@@ -87,27 +90,29 @@
             self.pca = fpca.fdajpca(self.warp_data)
         elif pca_method == "vert":
             self.pca = fpca.fdavpca(self.warp_data)
         elif pca_method == "horiz":
             self.pca = fpca.fdahpca(self.warp_data)
         else:
             raise Exception("Invalid fPCA Method")
-        self.pca.calc_fpca(no)
+        self.pca.calc_fpca(no=no, var_exp=var_exp)
+
+        no = self.pca.no
 
         # OLS using PCA basis
         lam = 0
         R = 0
         Phi = np.ones((N1, no + 1))
-        Phi[:, 1 : (no + 1)] = self.pca.coef
+        Phi[:, 1:(no + 1)] = self.pca.coef
         xx = np.dot(Phi.T, Phi)
         inv_xx = inv(xx + lam * R)
         xy = np.dot(Phi.T, self.y)
         b = np.dot(inv_xx, xy)
         alpha = b[0]
-        b = b[1 : no + 1]
+        b = b[1:no + 1]
 
         # compute the SSE
         int_X = np.zeros(N1)
         for ii in range(0, N1):
             int_X[ii] = np.sum(self.pca.coef[ii, :] * b)
 
         y_pred = alpha + int_X
```

### Comparing `fdasrsf-2.5.8/fdasrsf/plot_style.py` & `fdasrsf-2.5.9/fdasrsf/plot_style.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/rbfgs.py` & `fdasrsf-2.5.9/fdasrsf/rbfgs.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/regression.py` & `fdasrsf-2.5.9/fdasrsf/regression.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/time_warping.py` & `fdasrsf-2.5.9/fdasrsf/time_warping.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/tolerance.py` & `fdasrsf-2.5.9/fdasrsf/tolerance.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/umap_metric.py` & `fdasrsf-2.5.9/fdasrsf/umap_metric.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf/utility_functions.py` & `fdasrsf-2.5.9/fdasrsf/utility_functions.py`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/fdasrsf.egg-info/PKG-INFO` & `fdasrsf-2.5.9/fdasrsf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdasrsf
-Version: 2.5.8
+Version: 2.5.9
 Summary: functional data analysis using the square root slope framework
 Home-page: http://research.tetonedge.net
 Author: J. Derek Tucker
 Author-email: "J. Derek Tucker" <jdtuck@sandia.gov>
 License: BSD 3-Clause
 Project-URL: homepage, http://research.tetonedge.net
 Project-URL: repository, https://github.com/jdtuck/fdasrsf_python
@@ -47,15 +47,15 @@
 A python package for functional data analysis using the square root
 slope framework and curves using the square root velocity framework
 which performs pair-wise and group-wise alignment as well as modeling
 using functional component analysis and regression. 
 
 ### Installation
 ------------------------------------------------------------------------------
-v2.5.8 is on pip and can be installed using
+v2.5.9 is on pip and can be installed using
 > `pip install fdasrsf`
 
 or conda
 
 > `conda install -c conda-forge fdasrsf`
 
 To install the most up to date version on github
```

### Comparing `fdasrsf-2.5.8/fdasrsf.egg-info/SOURCES.txt` & `fdasrsf-2.5.9/fdasrsf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/notebooks/example_curve.ipynb` & `fdasrsf-2.5.9/notebooks/example_curve.ipynb`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/notebooks/example_mvwarping.ipynb` & `fdasrsf-2.5.9/notebooks/example_mvwarping.ipynb`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/notebooks/example_warping.ipynb` & `fdasrsf-2.5.9/notebooks/example_warping.ipynb`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/pyproject.toml` & `fdasrsf-2.5.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fdasrsf"
-version = "2.5.8"
+version = "2.5.9"
 description = "functional data analysis using the square root slope framework"
 authors = [
 	{name = "J. Derek Tucker", email = "jdtuck@sandia.gov"}
 ]
 license = {text = "BSD 3-Clause"}
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `fdasrsf-2.5.8/setup.py` & `fdasrsf-2.5.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 ]
 
 
 setup(
     cmdclass={"build_ext": build_ext_with_blas, "build_docs": build_docs},
     ext_modules=extensions,
     name="fdasrsf",
-    version="2.5.8",
+    version="2.5.9",
     packages=["fdasrsf"],
     url="http://research.tetonedge.net",
     license="LICENSE.txt",
     author="J. Derek Tucker",
     author_email="jdtuck@sandia.gov",
     scripts=["bin/ex_srsf_align.py"],
     keywords=["functional data analysis"],
```

### Comparing `fdasrsf-2.5.8/src/DP.c` & `fdasrsf-2.5.9/src/DP.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/DynamicProgrammingQ2.c` & `fdasrsf-2.5.9/src/DynamicProgrammingQ2.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/ImageRegister.h` & `fdasrsf-2.5.9/src/ImageRegister.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/UnitSquareImage.cpp` & `fdasrsf-2.5.9/src/UnitSquareImage.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/UnitSquareImage.h` & `fdasrsf-2.5.9/src/UnitSquareImage.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/__pycache__/dp_build.cpython-310.pyc` & `fdasrsf-2.5.9/src/__pycache__/dp_build.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Feb 14 13:09:27 2024 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 87bb cc65 3f01 0000  o..........e?...
+00000000: 6f0d 0d0a 0000 0000 2bfc dd65 3f01 0000  o.......+..e?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6501 8300 5a03 6504 6502 6a05 a006  Z.e...Z.e.e.j...
 00000050: 6502 6a05 a007 6508 a101 6403 a102 8301  e.j...e...d.....
 00000060: 8f0f 5a09 6503 a00a 6509 a00b a100 a101  ..Z.e...e.......
 00000070: 0100 5700 6402 0400 0400 8303 0100 6e08  ..W.d.........n.
```

### Comparing `fdasrsf-2.5.8/src/armadillo` & `fdasrsf-2.5.9/src/armadillo`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/BaseCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/BaseCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/BaseCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/BaseCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Base_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Base_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Base_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Base_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Col_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Col_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Col_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Col_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/CubeToMatOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/CubeToMatOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/CubeToMatOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/CubeToMatOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Cube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Cube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/GenCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/GenCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/GenCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/GenCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Gen_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Gen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Gen_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Gen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/GlueCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/GlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/GlueCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/GlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Glue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Glue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Glue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Glue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/MapMat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/MapMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/MapMat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/MapMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Mat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Mat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/OpCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/OpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/OpCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/OpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Op_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Op_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Op_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Op_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Proxy.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Proxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/ProxyCube.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/ProxyCube.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Row_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Row_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/Row_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/Row_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SizeCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SizeCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SizeCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SizeCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SizeMat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SizeMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SizeMat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SizeMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpBase_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpBase_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpBase_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpBase_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpCol_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpCol_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpCol_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpCol_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpGlue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpGlue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpMat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpMat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpMat_iterators_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpMat_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpMat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpMat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpProxy.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpProxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpRow_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpRow_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpRow_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpRow_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpSubview_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpSubview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpSubview_col_list_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpSubview_col_list_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpSubview_col_list_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpSubview_col_list_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpSubview_iterators_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpSubview_iterators_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpSubview_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpSubview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpToDGlue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpToDGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpToDGlue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpToDGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpToDOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpToDOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpToDOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpToDOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpValProxy_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpValProxy_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/SpValProxy_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/SpValProxy_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/access.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/access.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_cmath.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_cmath.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_config.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_config.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_forward.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_forward.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_ostream_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_ostream_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_ostream_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_ostream_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_rel_comparators.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_rel_comparators.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_rng.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_rng.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_rng_cxx03.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_rng_cxx03.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_static_check.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_static_check.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_str.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_str.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arma_version.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arma_version.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arrayops_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arrayops_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/arrayops_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/arrayops_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/auxlib_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/auxlib_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/band_helper.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/band_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/compiler_check.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/compiler_check.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/compiler_setup.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/compiler_setup.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/compiler_setup_post.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/compiler_setup_post.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/cond_rel_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/cond_rel_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/cond_rel_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/cond_rel_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/config.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/config.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/config.hpp.cmake` & `fdasrsf-2.5.9/src/armadillo_bits/config.hpp.cmake`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/constants.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/constants.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/constants_old.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/constants_old.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/csv_name.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/csv_name.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/debug.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/debug.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_arpack.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_arpack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_atlas.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_atlas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_blas.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_blas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_fftw3.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_fftw3.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_lapack.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_lapack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/def_superlu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/def_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/diagmat_proxy.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/diagmat_proxy.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/diagview_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/diagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/diagview_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/diagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/diskio_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/diskio_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/diskio_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/diskio_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/distr_param.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/distr_param.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eGlueCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eGlueCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eGlue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eGlue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eOpCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eOpCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eglue_core_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eglue_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eglue_core_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eglue_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eop_aux.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eop_aux.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eop_core_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eop_core_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/eop_core_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/eop_core_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fft_engine_fftw3.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fft_engine_fftw3.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fft_engine_kissfft.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fft_engine_kissfft.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/field_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/field_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/field_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/field_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fill.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fill.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_accu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_accu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_all.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_all.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_any.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_any.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_approx_equal.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_approx_equal.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_as_scalar.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_as_scalar.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_chi2rnd.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_chi2rnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_chol.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_chol.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_clamp.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_clamp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cond_rcond.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cond_rcond.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_conv.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_conv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_conv_to.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_conv_to.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cor.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cor.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cov.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cov.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cross.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cross.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cumprod.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cumprod.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_cumsum.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_cumsum.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_det.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_det.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_diagmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_diagmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_diags_spdiags.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_diags_spdiags.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_diagvec.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_diagvec.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_diff.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_diff.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_dot.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_dot.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eig_gen.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eig_gen.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eig_pair.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eig_pair.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eig_sym.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eig_sym.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eigs_gen.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eigs_gen.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eigs_sym.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eigs_sym.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_elem.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_elem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eps.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eps.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_expmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_expmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_eye.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_eye.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_fft.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_fft.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_fft2.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_fft2.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_find.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_find.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_find_unique.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_find_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_flip.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_flip.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_hess.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_hess.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_hist.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_hist.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_histc.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_histc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_index_max.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_index_max.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_index_min.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_index_min.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_inplace_strans.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_inplace_strans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_inplace_trans.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_inplace_trans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_interp1.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_interp1.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_interp2.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_interp2.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_intersect.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_intersect.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_inv.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_inv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_inv_sympd.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_inv_sympd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_join.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_join.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_kmeans.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_kmeans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_kron.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_kron.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_log_det.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_log_det.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_log_normpdf.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_log_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_logmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_logmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_lu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_lu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_max.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_max.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_mean.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_mean.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_median.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_median.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_min.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_min.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_misc.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_mvnrnd.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_mvnrnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_n_unique.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_n_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_nonzeros.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_nonzeros.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_norm.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_norm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_normalise.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_normalise.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_normcdf.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_normcdf.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_normpdf.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_normpdf.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_numel.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_numel.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_ones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_ones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_orth_null.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_orth_null.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_pinv.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_pinv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_polyfit.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_polyfit.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_polyval.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_polyval.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_powext.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_powext.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_powmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_powmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_princomp.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_princomp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_prod.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_prod.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_qr.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_qr.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_quantile.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_quantile.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_qz.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_qz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_randg.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_randg.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_randi.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_randi.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_randn.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_randn.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_randperm.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_randperm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_randu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_randu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_range.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_range.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_rank.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_rank.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_regspace.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_regspace.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_repelem.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_repelem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_repmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_repmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_reshape.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_reshape.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_resize.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_resize.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_reverse.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_reverse.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_roots.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_roots.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_schur.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_shift.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_shift.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_shuffle.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_shuffle.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_size.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_size.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_solve.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_solve.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sort.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sort.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sort_index.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sort_index.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_speye.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_speye.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_spones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_spones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sprandn.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sprandn.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sprandu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sprandu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_spsolve.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_spsolve.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sqrtmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sqrtmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_stddev.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_stddev.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_strans.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_strans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sum.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sum.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_svd.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_svd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_svds.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_svds.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_sylvester.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_sylvester.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_symmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_symmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_toeplitz.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_toeplitz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trace.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trace.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trans.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trans.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trapz.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trapz.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trig.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trig.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trimat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trimat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trimat_ind.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trimat_ind.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trunc_exp.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trunc_exp.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_trunc_log.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_trunc_log.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_unique.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_unique.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_var.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_var.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_vecnorm.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_vecnorm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_vectorise.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_vectorise.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_wishrnd.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_wishrnd.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/fn_zeros.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/fn_zeros.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_affmul_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_affmul_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_affmul_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_affmul_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_atan2_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_atan2_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_atan2_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_atan2_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_conv_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_conv_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_conv_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_conv_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cor_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cor_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cov_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cov_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cross_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cross_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_cross_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_cross_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_hist_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_hist_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_histc_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_histc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_histc_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_histc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_hypot_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_hypot_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_hypot_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_hypot_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_intersect_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_intersect_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_intersect_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_intersect_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_join_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_join_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_kron_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_kron_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_max_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_max_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_min_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_min_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_mixed_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_mixed_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_mixed_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_mixed_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_mvnrnd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_mvnrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_mvnrnd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_mvnrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_polyfit_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_polyfit_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_polyfit_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_polyfit_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_polyval_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_polyval_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_polyval_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_polyval_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_powext_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_powext_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_powext_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_powext_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_quantile_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_quantile_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_quantile_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_quantile_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_relational_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_relational_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_solve_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_solve_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_solve_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_solve_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_times_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_times_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_times_misc_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_times_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_times_misc_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_times_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_toeplitz_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_toeplitz_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_trapz_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_trapz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/glue_trapz_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/glue_trapz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_diag_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_diag_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_diag_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_diag_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_full_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_full_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_full_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_full_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_misc_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/gmm_misc_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/gmm_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/hdf5_misc.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/hdf5_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/hdf5_name.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/hdf5_name.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/include_hdf5.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/include_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/include_superlu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/include_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/injector_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/injector_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/injector_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/injector_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/memory.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/memory.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mp_misc.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mp_misc.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtGlueCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtGlueCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtGlueCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtGlueCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtGlue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtGlue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtOpCube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtOpCube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtOpCube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtOpCube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtSpGlue_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtSpGlue_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtSpGlue_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtSpGlue_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtSpOp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtSpOp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mtSpOp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mtSpOp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mul_gemm.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mul_gemm.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mul_gemm_mixed.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mul_gemm_mixed.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mul_gemv.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mul_gemv.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mul_herk.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mul_herk.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/mul_syrk.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/mul_syrk.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_DenseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_DenseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_DoubleShiftQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_DoubleShiftQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_EigsSelect.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_EigsSelect.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_GenEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_GenEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SortEigenvalue.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SortEigenvalue.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenMatProd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenMatProd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenRealShiftSolve_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenRealShiftSolve_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SparseGenRealShiftSolve_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SparseGenRealShiftSolve_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsShiftSolver_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsShiftSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsShiftSolver_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsShiftSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsSolver_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_SymEigsSolver_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_TridiagEigen_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_TridiagEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_TridiagEigen_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_TridiagEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergEigen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergEigen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergQR_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_UpperHessenbergQR_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/newarp_cx_attrib.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/newarp_cx_attrib.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_all_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_all_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_all_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_all_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_any_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_any_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_any_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_any_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_chi2rnd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_chi2rnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_chi2rnd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_chi2rnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_chol_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_chol_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_chol_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_chol_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_clamp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_clamp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_clamp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_clamp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_col_as_mat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_col_as_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_col_as_mat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_col_as_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cond_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cond_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cond_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cond_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cor_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cor_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cor_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cor_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cov_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cov_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cov_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cov_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cumprod_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cumprod_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cumprod_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cumprod_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cumsum_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cumsum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cumsum_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cumsum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cx_scalar_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cx_scalar_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_cx_scalar_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_cx_scalar_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_det_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_det_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_det_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_det_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diagmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diagmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diagvec_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diagvec_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diagvec_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diagvec_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diff_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diff_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_diff_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_diff_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_dot_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_dot_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_dot_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_dot_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_dotext_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_dotext_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_dotext_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_dotext_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_expmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_expmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_expmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_expmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_fft_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_fft_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_fft_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_fft_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_find_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_find_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_find_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_find_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_find_unique_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_find_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_find_unique_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_find_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_flip_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_flip_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_flip_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_flip_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_hist_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_hist_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_hist_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_hist_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_htrans_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_htrans_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_index_max_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_index_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_index_max_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_index_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_index_min_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_index_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_index_min_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_index_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_inv_gen_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_inv_gen_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_inv_gen_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_inv_gen_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_inv_spd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_inv_spd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_inv_spd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_inv_spd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_log_det_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_log_det_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_log_det_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_log_det_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_logmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_logmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_logmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_logmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_max_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_max_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_mean_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_mean_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_median_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_median_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_median_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_median_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_min_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_min_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_misc_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_misc_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_nonzeros_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_nonzeros_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_nonzeros_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_nonzeros_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_norm2est_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_norm2est_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_norm2est_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_norm2est_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_norm_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_norm_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_norm_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_norm_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_normalise_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_normalise_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_orth_null_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_orth_null_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_orth_null_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_orth_null_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_pinv_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_pinv_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_pinv_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_pinv_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_powmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_powmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_powmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_powmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_princomp_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_princomp_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_princomp_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_princomp_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_prod_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_prod_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_prod_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_prod_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_range_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_range_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_range_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_range_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_rank_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_rank_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_rank_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_rank_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_rcond_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_rcond_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_rcond_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_rcond_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_relational_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_relational_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_repelem_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_repelem_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_repelem_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_repelem_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_repmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_repmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_reshape_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_reshape_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_reshape_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_reshape_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_resize_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_resize_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_resize_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_resize_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_reverse_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_reverse_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_roots_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_roots_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_roots_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_roots_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_row_as_mat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_row_as_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_row_as_mat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_row_as_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_shift_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_shift_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_shift_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_shift_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_shuffle_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_shuffle_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_shuffle_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_shuffle_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sort_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sort_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sort_index_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sort_index_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sort_index_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sort_index_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sort_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sort_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sp_minus_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sp_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sp_minus_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sp_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sp_plus_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sp_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sp_plus_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sp_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sqrtmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sqrtmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sqrtmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sqrtmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_stddev_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_stddev_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_stddev_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_stddev_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_strans_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_strans_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sum_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_sum_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_symmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_symmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_toeplitz_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_toeplitz_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_toeplitz_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_toeplitz_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_trimat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_trimat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_unique_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_unique_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_unique_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_unique_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_var_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_var_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_vecnorm_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_vecnorm_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_vecnorm_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_vecnorm_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_vectorise_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_vectorise_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_wishrnd_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_wishrnd_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/op_wishrnd_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/op_wishrnd_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_div.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_div.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_minus.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_minus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_plus.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_plus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_relational.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_relational.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_schur.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_cube_times.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_cube_times.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_div.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_div.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_minus.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_minus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_ostream.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_ostream.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_plus.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_plus.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_relational.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_relational.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_schur.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_schur.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/operator_times.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/operator_times.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/podarray_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/podarray_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/podarray_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/podarray_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/promote_type.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/promote_type.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/restrictors.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/restrictors.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/running_stat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/running_stat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/running_stat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/running_stat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/running_stat_vec_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/running_stat_vec_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/running_stat_vec_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/running_stat_vec_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/sp_auxlib_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/sp_auxlib_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/sp_auxlib_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/sp_auxlib_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/span.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/span.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spdiagview_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spdiagview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spdiagview_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spdiagview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_join_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_join_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_join_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_join_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_kron_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_kron_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_kron_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_kron_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_max_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_max_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_merge_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_merge_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_merge_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_merge_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_min_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_min_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_minus_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_minus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_minus_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_minus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_plus_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_plus_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_plus_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_plus_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_relational_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_relational_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_relational_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_relational_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_schur_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_schur_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_schur_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_schur_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_times_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_times_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spglue_times_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spglue_times_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_diagmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_diagmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_diagmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_diagmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_htrans_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_htrans_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_max_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_max_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_max_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_max_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_mean_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_mean_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_mean_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_mean_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_min_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_min_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_min_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_min_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_misc_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_misc_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_misc_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_misc_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_norm_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_norm_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_norm_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_norm_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_normalise_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_normalise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_normalise_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_normalise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_repmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_repmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_repmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_repmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_reverse_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_reverse_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_reverse_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_reverse_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_strans_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_strans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_strans_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_strans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_sum_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_sum_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_sum_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_sum_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_symmat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_symmat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_symmat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_symmat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_trimat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_trimat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_trimat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_trimat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_var_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_var_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_var_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_var_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_vecnorm_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_vecnorm_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_vecnorm_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_vecnorm_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_vectorise_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_vectorise_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spop_vectorise_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spop_vectorise_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spsolve_factoriser_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spsolve_factoriser_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/spsolve_factoriser_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/spsolve_factoriser_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/strip.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/strip.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_each_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_each_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_slices_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_slices_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_cube_slices_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_cube_slices_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_each_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_each_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_each_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_each_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_elem1_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_elem1_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_elem1_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_elem1_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_elem2_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_elem2_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_elem2_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_elem2_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_field_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_field_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_field_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_field_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/subview_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/subview_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/sym_helper.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/sym_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/traits.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/traits.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_arpack.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_arpack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_atlas.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_atlas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_blas.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_blas.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_fftw3.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_fftw3.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_lapack.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_lapack.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/translate_superlu.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/translate_superlu.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/trimat_helper.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/trimat_helper.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/typedef_elem.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/typedef_elem.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/typedef_elem_check.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/typedef_elem_check.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/typedef_mat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/typedef_mat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/typedef_mat_fixed.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/typedef_mat_fixed.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/unwrap.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/unwrap.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/unwrap_cube.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/unwrap_cube.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/unwrap_spmat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/unwrap_spmat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/upgrade_val.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/upgrade_val.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/wall_clock_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/wall_clock_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/wall_clock_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/wall_clock_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/xtrans_mat_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/xtrans_mat_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/xtrans_mat_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/xtrans_mat_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/xvec_htrans_bones.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/xvec_htrans_bones.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/armadillo_bits/xvec_htrans_meat.hpp` & `fdasrsf-2.5.9/src/armadillo_bits/xvec_htrans_meat.hpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/bayesian.cpp` & `fdasrsf-2.5.9/src/bayesian.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/c8lib.c` & `fdasrsf-2.5.9/src/c8lib.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/c8lib.h` & `fdasrsf-2.5.9/src/c8lib.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/cbayesian.pyx` & `fdasrsf-2.5.9/src/cbayesian.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/crbfgs.pyx` & `fdasrsf-2.5.9/src/crbfgs.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     q1 = np.ascontiguousarray(q1)
     q2 = np.ascontiguousarray(q2)
     d = np.zeros(q1.shape[1])
     M = q1.shape[0]
     alpha = 0.5
     time = np.linspace(0, 1, M)
     for i in range(q1.shape[1]):
-        q1t = q1[:,1]
+        q1t = q1[:,i]
         q1t = np.ascontiguousarray(q1t)
         gam = rlbfgs(q1t, time, q2)
         # warp q
         gam_dev = np.gradient(gam, 1.0 / (M - 1))
         tmp = np.interp((time[-1] - time[0]) * gam + time[0], time, q2)
 
         qw = tmp * np.sqrt(gam_dev)
@@ -52,8 +52,8 @@
         Dx = np.real(np.arccos(q1dotq2))
 
         d[i] = alpha * Dy + (1-alpha) * Dx
     
     return d
         
         
-    
+
```

### Comparing `fdasrsf-2.5.8/src/cyarma.pxd` & `fdasrsf-2.5.9/src/cyarma.pxd`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/cyarma.pyx` & `fdasrsf-2.5.9/src/cyarma.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/dp_grid.c` & `fdasrsf-2.5.9/src/dp_grid.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/dp_grid.h` & `fdasrsf-2.5.9/src/dp_grid.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/dp_nbhd.c` & `fdasrsf-2.5.9/src/dp_nbhd.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/fpls_warp.pyx` & `fdasrsf-2.5.9/src/fpls_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/fpls_warp_grad.c` & `fdasrsf-2.5.9/src/fpls_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/imagecpp.pyx` & `fdasrsf-2.5.9/src/imagecpp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/matrix_exponential.c` & `fdasrsf-2.5.9/src/matrix_exponential.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/misc_funcs.c` & `fdasrsf-2.5.9/src/misc_funcs.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/misc_funcs.h` & `fdasrsf-2.5.9/src/misc_funcs.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/mlogit_warp.pyx` & `fdasrsf-2.5.9/src/mlogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/mlogit_warp_grad.c` & `fdasrsf-2.5.9/src/mlogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/myVector.cpp` & `fdasrsf-2.5.9/src/myVector.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/oclogit_warp.pyx` & `fdasrsf-2.5.9/src/oclogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/oclogit_warp_grad.c` & `fdasrsf-2.5.9/src/oclogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/ocmlogit_warp.pyx` & `fdasrsf-2.5.9/src/ocmlogit_warp.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/ocmlogit_warp_grad.c` & `fdasrsf-2.5.9/src/ocmlogit_warp_grad.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/optimum_reparamN2.pyx` & `fdasrsf-2.5.9/src/optimum_reparamN2.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/optimum_reparam_N.pyx` & `fdasrsf-2.5.9/src/optimum_reparam_N.pyx`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/r8lib.c` & `fdasrsf-2.5.9/src/r8lib.c`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/r8lib.h` & `fdasrsf-2.5.9/src/r8lib.h`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/src/rbfgs.cpp` & `fdasrsf-2.5.9/src/rbfgs.cpp`

 * *Files identical despite different names*

### Comparing `fdasrsf-2.5.8/test/test_all.py` & `fdasrsf-2.5.9/test/test_all.py`

 * *Files identical despite different names*

