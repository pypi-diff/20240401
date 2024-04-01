# Comparing `tmp/gwalk-2.1.2.tar.gz` & `tmp/gwalk-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwalk-2.1.2.tar", last modified: Tue Dec 12 01:59:12 2023, max compression
+gzip compressed data, was "gwalk-2.1.3.tar", last modified: Mon Apr  1 18:35:04 2024, max compression
```

## Comparing `gwalk-2.1.2.tar` & `gwalk-2.1.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.465577 gwalk-2.1.2/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      339 2023-12-12 01:57:59.000000 gwalk-2.1.2/MANIFEST.in
--rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2023-12-12 01:59:12.465470 gwalk-2.1.2/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.1.2/README.md
--rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2023-12-12 01:57:59.000000 gwalk-2.1.2/__version__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      515 2023-08-15 23:07:31.000000 gwalk-2.1.2/pyproject.toml
--rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2023-12-12 01:59:12.465852 gwalk-2.1.2/setup.cfg
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5617 2023-12-12 01:57:59.000000 gwalk-2.1.2/setup.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.444248 gwalk-2.1.2/src/
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.447812 gwalk-2.1.2/src/gwalk/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/__init__.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.449279 gwalk-2.1.2/src/gwalk/c_utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/c_utils/dbg.h
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.452142 gwalk-2.1.2/src/gwalk/catalog/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    29447 2023-05-02 15:45:34.000000 gwalk-2.1.2/src/gwalk/catalog/catalog.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/coordinates.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.453076 gwalk-2.1.2/src/gwalk/catalog/prior/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/prior/CIP_prior_functions.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/prior/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/prior/callister_prior.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/catalog/prior/prior_methods.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5712 2023-05-02 15:46:03.000000 gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:14.000000 gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_2.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3070 2023-05-02 15:46:22.000000 gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_2p1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:27.000000 gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_3.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.453584 gwalk-2.1.2/src/gwalk/density/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/density/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.1.2/src/gwalk/density/mesh.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.458106 gwalk-2.1.2/src/gwalk/multivariate_normal/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/_decomposition.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/_mahalanobis_distance.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/decomposition_numpy.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    35812 2023-12-12 01:57:59.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/pdf.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11686 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/multivariate_normal/utils.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6816 2023-12-12 01:57:59.000000 gwalk-2.1.2/src/gwalk/optimize_likelihood_grid.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.459577 gwalk-2.1.2/src/gwalk/plots/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/plots/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/plots/axis.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/plots/likelihood_corner.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/plots/percentile_levels.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/plots/walker_plot.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.462228 gwalk-2.1.2/src/gwalk/tools/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.1.2/src/gwalk/tools/NAL_event_pipeline.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/collect.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/example_script.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.1.2/src/gwalk/tools/fit_catalog_samples.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/tools/fit_likelihood_grid.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/load_best_fits.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/plot_mesh_norm_corner.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/tools/populate_nal_figures.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.1.2/src/gwalk/tools/test_catalog_samples.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.462872 gwalk-2.1.2/src/gwalk/utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/utils/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.1.2/src/gwalk/utils/hist.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-04-25 18:43:04.000000 gwalk-2.1.2/src/gwalk/utils/multivariate_normal.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.465108 gwalk-2.1.2/src/gwalk.egg-info/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2023-12-12 01:59:12.000000 gwalk-2.1.2/src/gwalk.egg-info/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2032 2023-12-12 01:59:12.000000 gwalk-2.1.2/src/gwalk.egg-info/SOURCES.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2023-12-12 01:59:12.000000 gwalk-2.1.2/src/gwalk.egg-info/dependency_links.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)      131 2023-12-12 01:59:12.000000 gwalk-2.1.2/src/gwalk.egg-info/requires.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2023-12-12 01:59:12.000000 gwalk-2.1.2/src/gwalk.egg-info/top_level.txt
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2023-12-12 01:59:12.464768 gwalk-2.1.2/tests/
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3984 2023-12-12 01:57:59.000000 gwalk-2.1.2/tests/test_dpgmm.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_grid.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_kl.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_maha.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13133 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-04-25 18:43:04.000000 gwalk-2.1.2/tests/test_pdf.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      339 2024-03-01 18:48:16.000000 gwalk-2.1.3/MANIFEST.in
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      932 2024-04-01 18:35:04.477428 gwalk-2.1.3/PKG-INFO
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     2029 2024-03-01 18:48:16.000000 gwalk-2.1.3/README.md
+-rw-r--r--   0 xevra     (1000) xevra     (1000)       20 2024-04-01 18:35:00.000000 gwalk-2.1.3/__version__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      515 2024-03-01 18:48:16.000000 gwalk-2.1.3/pyproject.toml
+-rw-r--r--   0 xevra     (1000) xevra     (1000)       63 2024-04-01 18:35:04.481428 gwalk-2.1.3/setup.cfg
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     5617 2024-03-01 18:48:16.000000 gwalk-2.1.3/setup.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.469428 gwalk-2.1.3/src/
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.469428 gwalk-2.1.3/src/gwalk/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      307 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)       20 2024-04-01 18:35:00.000000 gwalk-2.1.3/src/gwalk/__version__.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/c_utils/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     1236 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/c_utils/dbg.h
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/catalog/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)       23 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    29447 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/catalog.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    17506 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/coordinates.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/catalog/prior/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     4574 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/CIP_prior_functions.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    11432 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/callister_prior.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     4176 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/prior/prior_methods.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     5712 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_1.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3071 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3070 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2p1.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3071 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_3.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.473428 gwalk-2.1.3/src/gwalk/density/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)       23 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/density/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    50044 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/density/mesh.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/multivariate_normal/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      108 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    24841 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_decomposition.c
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     6289 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_mahalanobis_distance.c
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    25977 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    27446 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    17947 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    13587 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition_numpy.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    35820 2024-04-01 18:26:38.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/object.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    11599 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/pdf.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    11686 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/multivariate_normal/utils.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     6816 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/optimize_likelihood_grid.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/plots/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     7254 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/axis.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     8166 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/likelihood_corner.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     1578 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/percentile_levels.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      686 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/plots/walker_plot.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/tools/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     5546 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/NAL_event_pipeline.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     2937 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/collect.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    13900 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/example_script.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    13076 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/fit_catalog_samples.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     1681 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/fit_likelihood_grid.py
+-rwxr-xr-x   0 xevra     (1000) xevra     (1000)     5595 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/load_best_fits.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     4668 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/plot_mesh_norm_corner.py
+-rwxr-xr-x   0 xevra     (1000) xevra     (1000)     4068 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/populate_nal_figures.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    11425 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/tools/test_catalog_samples.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk/utils/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        0 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/__init__.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3186 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/hist.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      133 2024-03-01 18:48:16.000000 gwalk-2.1.3/src/gwalk/utils/multivariate_normal.py
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/src/gwalk.egg-info/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      932 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/PKG-INFO
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     2057 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/SOURCES.txt
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        1 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/dependency_links.txt
+-rw-r--r--   0 xevra     (1000) xevra     (1000)      131 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/requires.txt
+-rw-r--r--   0 xevra     (1000) xevra     (1000)        6 2024-04-01 18:35:04.000000 gwalk-2.1.3/src/gwalk.egg-info/top_level.txt
+drwxr-xr-x   0 xevra     (1000) xevra     (1000)        0 2024-04-01 18:35:04.477428 gwalk-2.1.3/tests/
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    13966 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_decomposition.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3984 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_dpgmm.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3304 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_grid.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     5810 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_kl.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     3882 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_maha.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)    13133 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_object.py
+-rw-r--r--   0 xevra     (1000) xevra     (1000)     4824 2024-03-01 18:48:16.000000 gwalk-2.1.3/tests/test_pdf.py
```

### Comparing `gwalk-2.1.2/PKG-INFO` & `gwalk-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.1.2
+Version: 2.1.3
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.1.2/README.md` & `gwalk-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/pyproject.toml` & `gwalk-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/setup.py` & `gwalk-2.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/c_utils/dbg.h` & `gwalk-2.1.3/src/gwalk/c_utils/dbg.h`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/catalog.py` & `gwalk-2.1.3/src/gwalk/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/coordinates.py` & `gwalk-2.1.3/src/gwalk/catalog/coordinates.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/prior/CIP_prior_functions.py` & `gwalk-2.1.3/src/gwalk/catalog/prior/CIP_prior_functions.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/prior/callister_prior.py` & `gwalk-2.1.3/src/gwalk/catalog/prior/callister_prior.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/prior/prior_methods.py` & `gwalk-2.1.3/src/gwalk/catalog/prior/prior_methods.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_1.py` & `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_1.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_2.py` & `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_2p1.py` & `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_2p1.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/catalog/read_catalog_GWTC_3.py` & `gwalk-2.1.3/src/gwalk/catalog/read_catalog_GWTC_3.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/density/mesh.py` & `gwalk-2.1.3/src/gwalk/density/mesh.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/_decomposition.c` & `gwalk-2.1.3/src/gwalk/multivariate_normal/_decomposition.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/_mahalanobis_distance.c` & `gwalk-2.1.3/src/gwalk/multivariate_normal/_mahalanobis_distance.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c` & `gwalk-2.1.3/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/bounded_multivariate_normal.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/bounded_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/decomposition.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/decomposition_numpy.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/decomposition_numpy.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/object.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         assert value.shape == (self.ndim,)
         # Check that std limits make sense
         if hasattr(self, "plimits") and not (self.plimits is None):
             assert all(value >= self.plimits[self.ndim + 1:2*self.ndim + 1, 0])
             assert all(value <= self.plimits[self.ndim + 1:2*self.ndim + 1, 1])
         self._std = value
         if hasattr(self, "_params"):
-            self._params[self.ndim + 1:2*self.ndim + 1]
+            self._params[self.ndim + 1:2*self.ndim + 1] = value
 
     #### eigvals property ####
     @property
     def eigvals(self):
         '''The eigvals of the Gaussian covariance'''
         return self._eigvals
```

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/pdf.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/pdf.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/multivariate_normal/utils.py` & `gwalk-2.1.3/src/gwalk/multivariate_normal/utils.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/optimize_likelihood_grid.py` & `gwalk-2.1.3/src/gwalk/optimize_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/plots/axis.py` & `gwalk-2.1.3/src/gwalk/plots/axis.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/plots/likelihood_corner.py` & `gwalk-2.1.3/src/gwalk/plots/likelihood_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/plots/percentile_levels.py` & `gwalk-2.1.3/src/gwalk/plots/percentile_levels.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/plots/walker_plot.py` & `gwalk-2.1.3/src/gwalk/plots/walker_plot.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/NAL_event_pipeline.py` & `gwalk-2.1.3/src/gwalk/tools/NAL_event_pipeline.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/collect.py` & `gwalk-2.1.3/src/gwalk/tools/collect.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/example_script.py` & `gwalk-2.1.3/src/gwalk/tools/example_script.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/fit_catalog_samples.py` & `gwalk-2.1.3/src/gwalk/tools/fit_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/fit_likelihood_grid.py` & `gwalk-2.1.3/src/gwalk/tools/fit_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/load_best_fits.py` & `gwalk-2.1.3/src/gwalk/tools/load_best_fits.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/plot_mesh_norm_corner.py` & `gwalk-2.1.3/src/gwalk/tools/plot_mesh_norm_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/populate_nal_figures.py` & `gwalk-2.1.3/src/gwalk/tools/populate_nal_figures.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/tools/test_catalog_samples.py` & `gwalk-2.1.3/src/gwalk/tools/test_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk/utils/hist.py` & `gwalk-2.1.3/src/gwalk/utils/hist.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/src/gwalk.egg-info/PKG-INFO` & `gwalk-2.1.3/src/gwalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.1.2
+Version: 2.1.3
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.1.2/src/gwalk.egg-info/SOURCES.txt` & `gwalk-2.1.3/src/gwalk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 __version__.py
 pyproject.toml
 setup.cfg
 setup.py
 src/gwalk/__init__.py
+src/gwalk/__version__.py
 src/gwalk/optimize_likelihood_grid.py
 src/gwalk.egg-info/PKG-INFO
 src/gwalk.egg-info/SOURCES.txt
 src/gwalk.egg-info/dependency_links.txt
 src/gwalk.egg-info/requires.txt
 src/gwalk.egg-info/top_level.txt
 src/gwalk/c_utils/dbg.h
```

### Comparing `gwalk-2.1.2/tests/test_decomposition.py` & `gwalk-2.1.3/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_dpgmm.py` & `gwalk-2.1.3/tests/test_dpgmm.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_grid.py` & `gwalk-2.1.3/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_kl.py` & `gwalk-2.1.3/tests/test_kl.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_maha.py` & `gwalk-2.1.3/tests/test_maha.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_object.py` & `gwalk-2.1.3/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.1.2/tests/test_pdf.py` & `gwalk-2.1.3/tests/test_pdf.py`

 * *Files identical despite different names*

