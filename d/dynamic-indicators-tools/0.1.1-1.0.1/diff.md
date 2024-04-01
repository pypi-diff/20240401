# Comparing `tmp/dynamic_indicators_tools-0.1.1.tar.gz` & `tmp/dynamic_indicators_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_indicators_tools-0.1.1.tar", last modified: Mon Sep 11 23:23:50 2023, max compression
+gzip compressed data, was "dynamic_indicators_tools-1.0.1.tar", last modified: Mon Apr  1 21:00:55 2024, max compression
```

## Comparing `dynamic_indicators_tools-0.1.1.tar` & `dynamic_indicators_tools-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,57 @@
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1072 2023-09-08 10:49:06.000000 dynamic_indicators_tools-0.1.1/LICENSE
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/PKG-INFO
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6746 2023-09-11 23:15:55.000000 dynamic_indicators_tools-0.1.1/README.md
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       38 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/setup.cfg
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      862 2023-09-11 23:22:22.000000 dynamic_indicators_tools-0.1.1/setup.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.881036 dynamic_indicators_tools-0.1.1/src/
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.881036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/__init__.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.881036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/config_files/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/config_files/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    11052 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/config_files/get_params_config.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1829 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13378 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5769 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    18268 2023-09-11 23:15:55.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17903 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13790 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4033 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      842 2023-09-11 23:15:55.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/main_dynamic_indicators_process.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6398 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3329 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/integrators.py
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.881036 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2023-09-11 23:23:50.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/PKG-INFO
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1674 2023-09-11 23:23:50.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        1 2023-09-11 23:23:50.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       40 2023-09-11 23:23:50.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/requires.txt
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       31 2023-09-11 23:23:50.000000 dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/top_level.txt
-drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-11 23:23:50.885036 dynamic_indicators_tools-0.1.1/src/tests/
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/__init__.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4672 2023-09-08 13:53:43.000000 dynamic_indicators_tools-0.1.1/src/tests/test_config_files.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2378 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/test_data_transformations.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7833 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/test_diff_systems.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5757 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/test_differentiation.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1058 2023-09-11 23:15:55.000000 dynamic_indicators_tools-0.1.1/src/tests/test_dynamic_indicators_process.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     8670 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/test_finite_time_lyapunov_exponents.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3036 2023-09-08 10:50:04.000000 dynamic_indicators_tools-0.1.1/src/tests/test_lagrangian_descriptors.py
--rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4426 2023-09-08 11:19:22.000000 dynamic_indicators_tools-0.1.1/src/tests/test_system_black_hole_schwarzchids.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1072 2023-09-08 10:49:06.000000 dynamic_indicators_tools-1.0.1/LICENSE
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/PKG-INFO
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6746 2023-09-11 23:29:58.000000 dynamic_indicators_tools-1.0.1/README.md
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       38 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/setup.cfg
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      862 2024-04-01 20:59:24.000000 dynamic_indicators_tools-1.0.1/setup.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/__init__.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1829 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13333 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5769 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1863 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3431 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17262 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3097 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    17540 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6506 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      927 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    13642 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    10224 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/params_methods.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4748 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6358 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1842 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)    19000 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)      796 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/main_dynamic_indicators_process.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     6398 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3329 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/integrators.py
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.965436 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7232 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2606 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        1 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       40 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/requires.txt
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)       31 2024-04-01 21:00:55.000000 dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/top_level.txt
+drwxrwxr-x   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2024-04-01 21:00:55.969436 dynamic_indicators_tools-1.0.1/src/tests/
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)        0 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/__init__.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     2378 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_data_transformations.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     7833 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_diff_systems.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     5757 2023-09-08 10:50:04.000000 dynamic_indicators_tools-1.0.1/src/tests/test_differentiation.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     1938 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_dynamic_indicators_process.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     8630 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_finite_time_lyapunov_exponents.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     3045 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_lagrangian_descriptors.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4785 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_params_method.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4244 2024-04-01 20:57:01.000000 dynamic_indicators_tools-1.0.1/src/tests/test_poincare_map.py
+-rw-rw-r--   0 santhiperbolico  (1000) santhiperbolico  (1000)     4426 2023-09-08 11:19:22.000000 dynamic_indicators_tools-1.0.1/src/tests/test_system_black_hole_schwarzchids.py
```

### Comparing `dynamic_indicators_tools-0.1.1/LICENSE` & `dynamic_indicators_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/PKG-INFO` & `dynamic_indicators_tools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic_indicators_tools
-Version: 0.1.1
+Version: 1.0.1
 Summary: Repositorio que recoge herramientas para el análisis de sistemas dinámicos
 Home-page: https://github.com/santhiperbolico/dynamic_indicators_tools
 Author: Santiago Arranz Sanz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dynamic_indicators_tools-0.1.1/README.md` & `dynamic_indicators_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/setup.py` & `dynamic_indicators_tools-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dynamic_indicators_tools",
-    version="0.1.1",
+    version="1.0.1",
     author="Santiago Arranz Sanz",
     description="Repositorio que recoge herramientas para el análisis de sistemas dinámicos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     url="https://github.com/santhiperbolico/dynamic_indicators_tools",
     classifiers=[
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/data_transformations.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/diff_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -290,37 +290,37 @@
             Diccionario con los parámetros del solver.
         """
         return self.solver_method, self.args_func, self.params_solver
 
     def flow_grid(
         self,
         t: Union[int, float],
-        x0_min_grid: np.ndarray,
-        x0_max_grid: np.ndarray,
-        nx_grid: Union[int, np.ndarray],
+        x0_min: np.ndarray,
+        x0_max: np.ndarray,
+        n_xgrid: Union[int, np.ndarray],
         n_jobs: int = 1,
         projection_config: Dict[int, Projection] = None,
     ) -> Tuple[Union[Sequence[np.ndarray], str], np.ndarray]:
         """
         Método que crea una malla de condiciones iniciales, donde los
         limítes están definidos por x0_min_grid y x0_max_grid y la cantidad
         de puntos son nx_grid^(numero de variables), y calcula el valor del
         flujo para estos puntos.
 
         Parameters
         ----------
         t: Union[int, float]
             Valor del tiempo.
-        x0_min_grid: np.ndarray
+        x0_min: np.ndarray
             Array de dimensión (n_variables,) que indica el valor inferior
             de la malla.
-        x0_max_grid: np.ndarray
+        x0_max: np.ndarray
             Array de dimensión (n_variables,) que indica el valor superior
             de la malla.
-        nx_grid: Union[int, np.ndarray]
+        n_xgrid: Union[int, np.ndarray]
             Número de puntos generados por variable, donde el número
             total de puntos será nx_grid^(n_variables.). Si pasamos
             un entero se aplicará a todas las dimensiones. Si es una
             secuencia se aplicará según el orden de las dimensiones.
         n_jobs: int, default 1
             Número máximo de jobs en la paralelización.
         projection_config: Dict[int, Projection], default None
@@ -331,27 +331,27 @@
         grid_points: Sequence[np.ndarray]
             Lista con la malla para cada dimensión. Cada elemento
             es n array de dimensión (nx_grid,..., <n_variables>, ...,nx_grid).
         zz: np.ndarray:
             Array con el valor del flujo para cada punto de la malla. Este
             array es de dimensión (nx_grid,..., <n_variables>, ...,nx_grid, n_variables).
         """
-        n_var = x0_max_grid.size
-        if isinstance(nx_grid, int):
-            nx_grid = np.ones(n_var).astype(int) * nx_grid
-        if x0_min_grid.shape != x0_max_grid.shape:
+        n_var = x0_max.size
+        if isinstance(n_xgrid, int):
+            n_xgrid = np.ones(n_var).astype(int) * n_xgrid
+        if x0_min.shape != x0_max.shape:
             raise DoesntCoincideDimension(
                 "La dimensión de x0_min_grid y x0_max_grid" " deben ser iguales."
             )
-        if nx_grid.size != n_var:
+        if n_xgrid.size != n_var:
             raise DoesntCoincideDimension(
                 "La dimensión de nx_grid no coincide con el número de variables."
             )
         grid_points = np.meshgrid(
-            *[np.linspace(x0_min_grid[i], x0_max_grid[i], nx_grid[i]) for i in range(n_var)]
+            *[np.linspace(x0_min[i], x0_max[i], n_xgrid[i]) for i in range(n_var)]
         )
         grid_points = project_grid_data(grid_points, projection_config)
         flow = np.zeros(grid_points[0].shape + (n_var,))
         it = np.nditer(grid_points[0], flags=["multi_index"])
 
         with ThreadPoolExecutor(max_workers=n_jobs) as executor:
             futures = []
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/differentials_systems/solver_integrators.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,449 +1,420 @@
 import logging
 import os
-from abc import ABC, abstractmethod
-from typing import Any, Dict
-from warnings import warn
+from typing import Any, Dict, List
 
 import numpy as np
 from attr import attrs
 
-from dynamic_indicators_tools.config_files.get_params_config import format_symbolic_number
-from dynamic_indicators_tools.differentials_systems.diff_system import (
-    DiffSystem,
-    DiffVariable,
-    FlowMap,
+from .ftle_params import FTLE_ELEMENT_WISE_PARAMS, FTLE_GRID_PARAMS, FTLE_VARIATIONAL_EQUATIONS
+from .ftle_utils import ftl_variational_equations, ftle_element_wise, ftle_grid
+from dynamic_indicators_tools.dynamic_indicators.dynamic_indicators_process import (
+    DynamicIndicator,
+    create_system,
 )
-from dynamic_indicators_tools.dynamic_indicators.finite_time_lyapunov_exponents import (
-    ftl_variational_equations,
-    ftle_element_wise,
-    ftle_grid,
-)
-from dynamic_indicators_tools.dynamic_indicators.lagrangian_descriptors import (
-    lagrangian_descriptors,
-)
-from dynamic_indicators_tools.dynamic_indicators.plot_descriptors import (
-    plot_descriptors_map,
-    plot_extremals_solutions,
+from dynamic_indicators_tools.dynamic_indicators.params_methods import (
+    Param,
+    ParamProcessor,
+    ParamType,
 )
+from dynamic_indicators_tools.dynamic_indicators.plot_descriptors import plot_descriptors_map
 
 
-def create_system(system: Dict[str, Any], system_params: Dict[str, Any]) -> FlowMap:
+@attrs
+class FtleElementWise(DynamicIndicator):
     """
-    Función que devueve el FlowMap asociado a la función de systems.
-
-    Parameters
-    ----------
-    system: Dict[str, Any]
-        Diccionario con las funciones del sistema diferencial
-    system_params: Dict[str, Any]
-        Diccionario con los parámetros generales de los indicadores y del sistema.
-
-    Returns
-    -------
-    flow_map: FlowMap
-        FlowMap asociado al sistema diferencial que define systems.
+    Proceso que recoge el indicador dinámico de los exponentes de
+    Lyapunov en tiempos finitos calculado elemento a elemento.
     """
-    function_system = system["function"]
-    system_name = system_params.get("system_name")
-    args_system = system_params.get("args_system")
-    t0 = system_params.get("t0")
-    solver_method = system_params.get("solver_method")
-
-    logging.info("\t - Creando el sistema %s" % system_name)
-    x = DiffVariable("x")
-    flow_map = FlowMap(diff_system=DiffSystem(x, function_system), t0=t0)
-    flow_map.set_params_fun_solver(solver_method=solver_method, args_func=args_system)
-    return flow_map
 
+    name_dynamic_indicator: str = "ftle_element_wise"
+    default_params: List[Param] = FTLE_ELEMENT_WISE_PARAMS
 
-class DynamicIndicatorNotExist(Exception):
-    pass
+    def create_params_processor(self, params: Dict[str, Any] = None) -> ParamProcessor:
+        """
+        Método que crea el params processor para el método de FtleElementWise.
 
+        Parameters
+        ----------
+        params: Dict[str, Any], default None
+            Diccionario con los parámetros del indicador dinámico.
 
-@attrs
-class DynamicIndicator(ABC):
-    @abstractmethod
-    def process(
-        self,
-        system: Dict[str, Any],
-        system_params: Dict[str, Any],
-        dynamic_indicators_params: Dict[str, Any],
-    ) -> None:
-        """
-        Proceso que ejecuta el indicador dinámico
-        """
-        pass
+        Returns
+        -------
+        param_processor: ParamProcessor
+            ParamProcessor del indicador dinámico.
 
+        """
+        params_indicator = {}
+        if params is None:
+            params = {}
+        params_indicator.update(params.get("system_params"))
+        params_indicator.update(params.get(self.name_dynamic_indicator, {}))
+        params_processor = ParamProcessor(self.default_params, params_indicator)
+        h_steps = params_processor.get_param("h_steps")
+        n_xgrid = params_processor.get_param("n_xgrid")
 
-@attrs
-class FtleElementWise(DynamicIndicator):
-    """
-    Proceso que recoge el indicador dinámico de los exponentes de
-    Lyapunov en tiempos finitos calculado elemento a elemento.
-    """
+        if h_steps is None:
+            x_max = params_processor.get_param("x0_max")
+            x_min = params_processor.get_param("x0_min")
+            params_processor.update_param("h_steps", (x_max - x_min) / (n_xgrid - 1))
+        return params_processor
 
-    def process(
-        self,
-        system: Dict[str, Any],
-        system_params: Dict[str, Any],
-        dynamic_indicators_params: Dict[str, Any],
-    ) -> None:
+    def load_params(self, params: Dict[str, Any]) -> ParamProcessor:
         """
-        Proceso que ejecuta el indicador dinámico para una malla de puntos sacando
-        una gráfica en el plano indicado dentro de system_params con los valores del
-        indicador en colores. Guarda las gráficas en la ruta especificada.
+        Método que carga los parámetros a un objeto param processor.
 
         Parameters
         ----------
-        system: Dict[str, Any]
-            Diccionario con las funciones del sistema diferencial
-        system_params: Dict[str, Any]
-            Diccionario con los parámetros generales de los indicadores y del sistema.
-        dynamic_indicators_params: Dict[str, Any]
-            Diccionario con los parámetros del indicador. Debe aparecer un parámetro
-            "execute" que indica si se quiere procesar dicho indicador, por defecto lo
-            toma como False.
+        params: Dict[str, Any]
+            Diccionario con los parámetros del proceso.
+
+        Returns
+        -------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del método del indicador dinámico.
+
         """
         logging.info("-- Cargando parámetros.")
-        path_fig = system_params.get("path", ".")
-        axis_data = system_params["axis"]
-        system_name = system_params.get("system_name")
-        t1 = format_symbolic_number(system_params.get("t1"))
-        n_xgrid = system_params.get("n_xgrid")
-        x_min = system_params.get("x_min")
-        x_max = system_params.get("x_max")
-        n_jobs = system_params.get("n_jobs")
-        projection_config = system_params.get("projection_config")
-        flow_map = create_system(system, system_params)
-        h_steps = dynamic_indicators_params.get("h_steps")
-        params_time_close = dynamic_indicators_params.get("params_t_close")
-
+        params_processor = self.create_params_processor(params)
+        n_xgrid = params_processor.get_param("n_xgrid")
         n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
-        if h_steps is None:
-            h_steps = (x_max - x_min) / (n_xgrid - 1)
+        system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+        params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
         logging.info("-- Parámetros del proceso:")
-        logging.info("\t T=%i" % t1)
+        logging.info("\t T=%i" % params_indicator.get("t"))
         logging.info("\t Número de puntos =%i" % n_xgrid_total)
-        logging.info("\t Paso de la integración = %s " % (str(h_steps)))
-        logging.info("\t Solver usado = %s " % flow_map.solver_method)
-        logging.info("\t Límite inferior de la malla = %s " % (str(list(x_min))))
-        logging.info("\t Límite superior de la malla = %s " % (str(list(x_max))))
-        logging.info("\t Número máximo de hilos = %i" % n_jobs)
+        logging.info("\t Paso de la integración = %s " % (str(params_indicator.get("h_steps"))))
+        logging.info("\t Solver usado = %s " % system_params.get("solver_method"))
+        logging.info(
+            "\t Límite inferior de la malla = %s " % (str(list(params_indicator.get("x0_min"))))
+        )
+        logging.info(
+            "\t Límite superior de la malla = %s " % (str(list(params_indicator.get("x0_max"))))
+        )
+        logging.info("\t Número máximo de hilos = %i" % params_indicator.get("n_jobs"))
+        return params_processor
 
-        logging.info("-- Ejecutando el cálculo punto a punto.")
-        fname = f"{system_name}_element_wise_t_{t1:.0f}_nx_grid_{n_xgrid_total:.0f}"
+    def create_file_name_process(self, params_processor: ParamProcessor) -> str:
+        """
+        Método que crea el título del indicador dinámico con los procesos.
+
+        Parameters
+        ----------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del proceso.
+
+        Returns
+        -------
+        fname: str
+            Nombre asociado al indicador con los prámetros y problema utilizado.
+
+        """
+
+        n_xgrid = params_processor.get_param("n_xgrid")
+        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
+        system_name = params_processor.get_param("system_name")
+        h_steps = params_processor.get_param("h_steps")
+        t = params_processor.get_param("t")
+        fname = (
+            f"{system_name}_{self.name_dynamic_indicator}_t_{t:.0f}_nx_grid_{n_xgrid_total:.0f}"
+        )
         if isinstance(h_steps, np.ndarray):
             logging.info("\t -Paso de la derivada = %.4f" % h_steps.max())
             fname = f"{fname}_h_{h_steps.max():.4f}"
         if isinstance(h_steps, float):
             logging.info("\t -Paso de la derivada = %.4f" % h_steps)
             fname = f"{fname}_h_{h_steps:.4f}"
-        filename = os.path.join(path_fig, fname + ".png")
-        grid_points, zz = ftle_element_wise(
-            flow_map,
-            t1,
-            x_min,
-            x_max,
-            n_xgrid,
-            h_steps=h_steps,
-            n_jobs=n_jobs,
-            params_t_close=params_time_close,
-            projection_config=projection_config,
-        )
-        _, _ = plot_descriptors_map(
-            grid_points[axis_data[0]],
-            grid_points[axis_data[1]],
-            values=zz,
-            filename=filename,
-            axis=axis_data,
-        )
-
+        return fname
 
-@attrs
-class FtleGrid(DynamicIndicator):
-    def process(
-        self,
-        system: Dict[str, Any],
-        system_params: Dict[str, Any],
-        dynamic_indicators_params: Dict[str, Any],
-    ) -> None:
+    def process(self, params: Dict[str, Any]) -> None:
         """
         Proceso que ejecuta el indicador dinámico para una malla de puntos sacando
         una gráfica en el plano indicado dentro de system_params con los valores del
         indicador en colores. Guarda las gráficas en la ruta especificada.
 
         Parameters
         ----------
-        system: Dict[str, Any]
-            Diccionario con las funciones del sistema diferencial
-        system_params: Dict[str, Any]
-            Diccionario con los parámetros generales de los indicadores y del sistema.
-        dynamic_indicators_params: Dict[str, Any]
-            Diccionario con los parámetros del indicador. Debe aparecer un parámetro
-            "execute" que indica si se quiere procesar dicho indicador, por defecto lo
-            toma como False.
+        params: Dict[str, Any]
+            Parámetros del indicador dinámico.
         """
-        logging.info("-- Cargando parámetros.")
-        path_fig = system_params.get("path", ".")
-        axis_data = system_params["axis"]
-        system_name = system_params.get("system_name")
-        t1 = format_symbolic_number(system_params.get("t1"))
-        n_xgrid = system_params.get("n_xgrid")
-        x_min = system_params.get("x_min")
-        x_max = system_params.get("x_max")
-        n_jobs = system_params.get("n_jobs")
-        projection_config = system_params.get("projection_config")
-        flow_map = create_system(system, system_params)
-        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
-
-        logging.info("-- Parámetros del proceso:")
-        logging.info("\t T=%i" % t1)
-        logging.info("\t Número de puntos =%i" % n_xgrid_total)
-        logging.info("\t Solver usado = %s " % flow_map.solver_method)
-        logging.info("\t Límite inferior de la malla = %s " % (str(list(x_min))))
-        logging.info("\t Límite superior de la malla = %s " % (str(list(x_max))))
-        logging.info("\t Número máximo de hilos = %i" % n_jobs)
-
-        logging.info("-- Ejecutando el cálculo de malla.")
-        grid_points, diff_f = ftle_grid(
-            flow_map, t1, x_min, x_max, n_xgrid, n_jobs, projection_config=projection_config
-        )
-        fname = f"{system_name}_grid_t_{t1:.0f}_nx_grid_{n_xgrid_total:.0f}.png"
-        filename = os.path.join(path_fig, fname)
-        _, _ = plot_descriptors_map(
-            grid_points[axis_data[0]],
-            grid_points[axis_data[1]],
-            values=diff_f,
-            filename=filename,
-            axis=axis_data,
-        )
+        execute = params.get(self.name_dynamic_indicator, {}).get("execute", False)
+        if execute:
+            logging.info(f"Ejecutando {self.name_dynamic_indicator}")
+            params_processor = self.load_params(params)
+            system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+            params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
+            flow_map = create_system(system_params)
+            fname = self.create_file_name_process(params_processor)
+            path_fig = params_processor.get_param("path")
+            filename = os.path.join(path_fig, fname + ".png")
+            axis_data = params_processor.get_param("axis")
+            logging.info("-- Ejecutando el cálculo punto a punto.")
+            grid_points, zz = ftle_element_wise(flow_map, **params_indicator)
+            _, _ = plot_descriptors_map(
+                grid_points[axis_data[0]],
+                grid_points[axis_data[1]],
+                values=zz,
+                filename=filename,
+                axis=axis_data,
+            )
+            logging.info(f"- Campo FTLE guardado en {filename}.")
+            logging.info(f"- Fin del proceso de {self.name_dynamic_indicator}")
 
 
 @attrs
-class FtleVariationalEquations(DynamicIndicator):
-    def process(
-        self,
-        system: Dict[str, Any],
-        system_params: Dict[str, Any],
-        dynamic_indicators_params: Dict[str, Any],
-    ) -> None:
+class FtleGrid(DynamicIndicator):
+    """
+    Proceso que recoge el indicador dinámico de los exponentes de
+    Lyapunov en tiempos finitos calculado en malla.
+    """
+
+    name_dynamic_indicator: str = "ftle_grid"
+    default_params: List[Param] = FTLE_GRID_PARAMS
+
+    def create_params_processor(self, params: Dict[str, Any] = None) -> ParamProcessor:
         """
-        Proceso que ejecuta el indicador dinámico para una malla de puntos sacando
-        una gráfica en el plano indicado dentro de system_params con los valores del
-        indicador en colores. En vez de calcular la jacobiana numéricamente la incluye
-        en el sistema diferencial en forma de ecuaciones variacionales.
+        Método que crea el params processor para el método de FtleElementWise.
 
         Parameters
         ----------
-        system: Dict[str, Any]
-            Diccionario con las funciones del sistema diferencial
-        system_params: Dict[str, Any]
-            Diccionario con los parámetros generales de los indicadores y del sistema.
-        dynamic_indicators_params: Dict[str, Any]
-            Diccionario con los parámetros del indicador. Debe aparecer un parámetro
-            "execute" que indica si se quiere procesar dicho indicador, por defecto lo
-            toma como False.
+        params: Dict[str, Any], default None
+            Diccionario con los parámetros del indicador dinámico.
+
+        Returns
+        -------
+        param_processor: ParamProcessor
+            ParamProcessor del indicador dinámico.
+
+        """
+        params_indicator = {}
+        if params is None:
+            params = {}
+        params_indicator.update(params.get("system_params"))
+        params_indicator.update(params.get(self.name_dynamic_indicator, {}))
+        params_processor = ParamProcessor(self.default_params, params_indicator)
+        return params_processor
+
+    def load_params(self, params: Dict[str, Any]) -> ParamProcessor:
+        """
+        Método que carga los parámetros a un objeto param processor.
+
+        Parameters
+        ----------
+        params: Dict[str, Any]
+            Diccionario con los parámetros del proceso.
+
+        Returns
+        -------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del método del indicador dinámico.
+
         """
         logging.info("-- Cargando parámetros.")
-        path_fig = system_params.get("path", ".")
-        axis_data = system_params["axis"]
-        system_name = system_params.get("system_name")
-        t1 = format_symbolic_number(system_params.get("t1"))
-        n_xgrid = system_params.get("n_xgrid")
-        x_min = system_params.get("x_min")
-        x_max = system_params.get("x_max")
-        n_jobs = system_params.get("n_jobs")
-        projection_config = system_params.get("projection_config")
-        system_ve = system.copy()
-        system_ve["function"] = dynamic_indicators_params.get("system")
-        flow_map = create_system(system_ve, system_params)
+        params_processor = self.create_params_processor(params)
+        n_xgrid = params_processor.get_param("n_xgrid")
         n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
-
+        system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+        params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
         logging.info("-- Parámetros del proceso:")
-        logging.info("\t T=%i" % t1)
+        logging.info("\t T=%i" % params_indicator.get("t"))
         logging.info("\t Número de puntos =%i" % n_xgrid_total)
-        logging.info("\t Solver usado = %s " % flow_map.solver_method)
-        logging.info("\t Límite inferior de la malla = %s " % (str(list(x_min))))
-        logging.info("\t Límite superior de la malla = %s " % (str(list(x_max))))
-        logging.info("\t Número máximo de hilos = %i" % n_jobs)
-
-        logging.info("-- Ejecutando el cálculo de malla con ecuaciones variacionales.")
-        grid_points, diff_f = ftl_variational_equations(
-            flow_map, t1, x_min, x_max, n_xgrid, n_jobs, projection_config=projection_config
+        logging.info("\t Solver usado = %s " % system_params.get("solver_method"))
+        logging.info(
+            "\t Límite inferior de la malla = %s " % (str(list(params_indicator.get("x0_min"))))
         )
-        fname = f"{system_name}_variational_equations_t_{t1:.0f}_nx_grid_{n_xgrid_total:.0f}.png"
-        filename = os.path.join(path_fig, fname)
-        _, _ = plot_descriptors_map(
-            grid_points[axis_data[0]],
-            grid_points[axis_data[1]],
-            values=diff_f,
-            filename=filename,
-            axis=axis_data,
+        logging.info(
+            "\t Límite superior de la malla = %s " % (str(list(params_indicator.get("x0_max"))))
         )
+        logging.info("\t Número máximo de hilos = %i" % params_indicator.get("n_jobs"))
+        return params_processor
 
+    def create_file_name_process(self, params_processor: ParamProcessor) -> str:
+        """
+        Método que crea el título del indicador dinámico con los procesos.
+
+        Parameters
+        ----------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del proceso.
+
+        Returns
+        -------
+        fname: str
+            Nombre asociado al indicador con los prámetros y problema utilizado.
 
-@attrs
-class LagrangianDescriptor(DynamicIndicator):
-    def process(
-        self,
-        system: Dict[str, Any],
-        system_params: Dict[str, Any],
-        dynamic_indicators_params: Dict[str, Any],
-    ):
+        """
+
+        n_xgrid = params_processor.get_param("n_xgrid")
+        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
+        system_name = params_processor.get_param("system_name")
+        t = params_processor.get_param("t")
+        fname = (
+            f"{system_name}_{self.name_dynamic_indicator}_t_{t:.0f}_nx_grid_{n_xgrid_total:.0f}"
+        )
+        return fname
+
+    def process(self, params: Dict[str, Any]) -> None:
         """
         Proceso que ejecuta el indicador dinámico para una malla de puntos sacando
         una gráfica en el plano indicado dentro de system_params con los valores del
         indicador en colores. Guarda las gráficas en la ruta especificada.
 
         Parameters
         ----------
-        system: Dict[str, Any]
-            Diccionario con las funciones del sistema diferencial
-        system_params: Dict[str, Any]
-            Diccionario con los parámetros generales de los indicadores y del sistema.
-        dynamic_indicators_params: Dict[str, Any]
-            Diccionario con los parámetros del indicador. Debe aparecer un parámetro
-            "execute" que indica si se quiere procesar dicho indicador, por defecto lo
-            toma como False.
+        params: Dict[str, Any]
+            Parámetros del indicador dinámico.
         """
-        logging.info("-- Cargando parámetros.")
-        path_fig = system_params.get("path", ".")
-        axis_data = system_params["axis"]
-        system_name = system_params.get("system_name")
-        t1 = format_symbolic_number(system_params.get("t1"))
-        n_xgrid = system_params.get("n_xgrid")
-        x_min = system_params.get("x_min")
-        x_max = system_params.get("x_max")
-        n_jobs = system_params.get("n_jobs")
-        projection_config = system_params.get("projection_config")
-        flow_map = create_system(system, system_params)
-        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
+        execute = params.get(self.name_dynamic_indicator, {}).get("execute", False)
+        if execute:
+            logging.info(f"Ejecutando {self.name_dynamic_indicator}")
+            params_processor = self.load_params(params)
+            fname = self.create_file_name_process(params_processor)
+            system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+            params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
+            flow_map = create_system(system_params)
+            path_fig = params_processor.get_param("path")
+            filename = os.path.join(path_fig, fname + ".png")
+            axis_data = params_processor.get_param("axis")
+            logging.info("-- Ejecutando el cálculo de malla.")
+            grid_points, diff_f = ftle_grid(flow_map, **params_indicator)
+            _, _ = plot_descriptors_map(
+                grid_points[axis_data[0]],
+                grid_points[axis_data[1]],
+                values=diff_f,
+                filename=filename,
+                axis=axis_data,
+            )
+            logging.info(f"- Campo FTLE guardado en {filename}.")
+            logging.info(f"- Fin del proceso de {self.name_dynamic_indicator}")
+
+
+@attrs
+class FtleVariationalEquations(DynamicIndicator):
+    """
+    Proceso que recoge el indicador dinámico de los exponentes de
+    Lyapunov en tiempos finitos calculado punto a punto a través
+    de las ecuaciones diferenciales variacionales.
+    """
+
+    name_dynamic_indicator: str = "ftle_variational_equations"
+    default_params: List[Param] = FTLE_VARIATIONAL_EQUATIONS
+
+    def create_params_processor(self, params: Dict[str, Any] = None) -> ParamProcessor:
+        """
+        Método que crea el params processor para el método de FtleElementWise.
+
+        Parameters
+        ----------
+        params: Dict[str, Any], default None
+            Diccionario con los parámetros del indicador dinámico.
+
+        Returns
+        -------
+        param_processor: ParamProcessor
+            ParamProcessor del indicador dinámico.
+
+        """
+        params_indicator = {}
+        if params is None:
+            params = {}
+        params_indicator.update(params.get("system_params"))
+        params_indicator.update(params.get(self.name_dynamic_indicator, {}))
+        if "var_system" in params_indicator.keys():
+            params_indicator.update({"function": params_indicator.get("var_system")})
+        params_processor = ParamProcessor(self.default_params, params_indicator)
+        return params_processor
 
-        tau = dynamic_indicators_params.get("tau")
-        method_integrate = dynamic_indicators_params.get("method_integrate")
-        log_scale = dynamic_indicators_params.get("log_scale_color", False)
-        plot_orbits = dynamic_indicators_params.get("plot_orbits")
-        params_solver = {
-            "solver_method": flow_map.solver_method,
-            "t0": flow_map.t0,
-            "args": flow_map.args_func,
-        }
+    def load_params(self, params: Dict[str, Any]) -> ParamProcessor:
+        """
+        Método que carga los parámetros a un objeto param processor.
+
+        Parameters
+        ----------
+        params: Dict[str, Any]
+            Diccionario con los parámetros del proceso.
 
+        Returns
+        -------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del método del indicador dinámico.
+
+        """
+        logging.info("-- Cargando parámetros.")
+        params_processor = self.create_params_processor(params)
+        n_xgrid = params_processor.get_param("n_xgrid")
+        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
+        system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+        params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
         logging.info("-- Parámetros del proceso:")
-        logging.info("\t - T=%i" % t1)
-        logging.info("\t - Número de puntos =%i" % n_xgrid_total)
-        logging.info("\t - Intervalo Tau usado = %s " % (str(tau)))
-        logging.info("\t - Método de integración usado = %s " % method_integrate)
-        logging.info("\t - Solver usado = %s " % flow_map.solver_method)
-        logging.info("\t - Límite inferior de la malla = %s " % (str(list(x_min))))
-        logging.info("\t - Límite superior de la malla = %s " % (str(list(x_max))))
-        logging.info("\t - Número máximo de hilos = %i" % n_jobs)
-
-        logging.info("-- Ejecutando descriptores Lagrangianos punto a punto.")
-        grid_points, zz = lagrangian_descriptors(
-            flow_map.diff_system,
-            t1,
-            x_min,
-            x_max,
-            n_xgrid,
-            tau=tau,
-            method_integrate=method_integrate,
-            n_jobs=n_jobs,
-            opts_integrate={"args_func": flow_map.args_func},
-            projection_config=projection_config,
-            params_solver=params_solver,
+        logging.info("\t T=%i" % params_indicator.get("t"))
+        logging.info("\t Número de puntos =%i" % n_xgrid_total)
+        logging.info("\t Solver usado = %s " % system_params.get("solver_method"))
+        logging.info(
+            "\t Límite inferior de la malla = %s " % (str(list(params_indicator.get("x0_min"))))
         )
-
-        fname = f"{system_name}_lag_desc_t_{t1:.0f}_nx_grid_{n_xgrid_total:.0f}.png"
-        filename = os.path.join(path_fig, fname)
-        fig, ax = plot_descriptors_map(
-            grid_points[axis_data[0]],
-            grid_points[axis_data[1]],
-            values=zz,
-            filename=filename,
-            axis=axis_data,
-            log_scale=log_scale,
+        logging.info(
+            "\t Límite superior de la malla = %s " % (str(list(params_indicator.get("x0_max"))))
         )
-        if plot_orbits:
-            _ = plot_extremals_solutions(
-                ax=ax,
-                extremals_functionals=system["extremals"],
-                args_func=flow_map.args_func,
-                x_min=x_min,
-                x_max=x_max,
-                t1=t1,
-                diff_system=flow_map.diff_system,
-                solver_method=flow_map.solver_method,
-            )
-            fig.savefig(filename)
+        logging.info("\t Número máximo de hilos = %i" % params_indicator.get("n_jobs"))
+        return params_processor
 
+    def create_file_name_process(self, params_processor: ParamProcessor) -> str:
+        """
+        Método que crea el título del indicador dinámico con los procesos.
 
-DynamicIndicatorDict = {
-    "ftle_element_wise": FtleElementWise,
-    "ftle_grid": FtleGrid,
-    "lagrangian_descriptors": LagrangianDescriptor,
-    "ftle_variational_equations": FtleVariationalEquations,
-}
+        Parameters
+        ----------
+        params_processor: ParamProcessor
+            Objeto paramprocessor con los parámetros del proceso.
 
+        Returns
+        -------
+        fname: str
+            Nombre asociado al indicador con los prámetros y problema utilizado.
 
-def get_dynamic_indicator(dynamic_indicator_name: str) -> DynamicIndicator:
-    """
-    Función que dado un nombre del indicador devuelve el objeto DynamicIndicator
-    correspondiente si existe. En caso de que no devuelve un error DynamicIndicatorNotExist
+        """
 
-    Parameters
-    ----------
-    dynamic_indicator_name: str
-        Nombre del indicador
-
-    Returns
-    -------
-    dynamic_indicators_object: DynamicIndicator
-        Objeto instanciado del indicador.
-    """
-    try:
-        return DynamicIndicatorDict[dynamic_indicator_name]()
-    except KeyError:
-        raise DynamicIndicatorNotExist(
-            f"El indicador {dynamic_indicator_name} no existe."
-            f" Pruebe con {list(DynamicIndicatorDict.keys())}"
+        n_xgrid = params_processor.get_param("n_xgrid")
+        n_xgrid_total = np.prod(n_xgrid) if isinstance(n_xgrid, np.ndarray) else n_xgrid
+        system_name = params_processor.get_param("system_name")
+        t = params_processor.get_param("t")
+        fname = (
+            f"{system_name}_{self.name_dynamic_indicator}_t_{t:.0f}_nx_grid_{n_xgrid_total:.0f}"
         )
+        return fname
 
+    def process(self, params: Dict[str, Any]) -> None:
+        """
+        Proceso que ejecuta el indicador dinámico para una malla de puntos sacando
+        una gráfica en el plano indicado dentro de system_params con los valores del
+        indicador en colores. En vez de calcular la jacobiana numéricamente la incluye
+        en el sistema diferencial en forma de ecuaciones variacionales.
 
-def main_process_di(
-    system: Dict[str, Any], system_params: Dict[str, Any], dynamic_indicators: Dict[str, Any]
-) -> None:
-    """
-    Función que crea las gráficas de indicadores dinámicos para el problema
-    configurado a través de los parámetros system y system_params. Cada indicador dinámico
-    está especificado en dynamic_indicators donde la key es el nombre y los valores
-    un diccionario con los parámetros del indicador. En ese diccionario debe aparecer
-    un parámetro "execute" que indica si se quiere procesar dicho indicador, por defecto
-    lo toma como False.
-
-    Parameters
-    ----------
-    system: Dict[str, Any]
-        Diccionario con las funciones del sistema diferencial
-    system_params: Dict[str, Any]
-        Diccionario con los parámetros generales de los indicadores y del sistema.
-    dynamic_indicators: Dict[str, Any]
-        Diccionario donde Cada indicador dinámico está especificado con la key como el nombre
-        y los valores como un diccionario con los parámetros del indicador. En ese diccionario
-        debe aparecer un parámetro "execute" que indica si se quiere procesar dicho indicador,
-        por defecto lo toma como False.
-    """
-    for dynamic_indicator_name, dynamic_indicator_params in dynamic_indicators.items():
-        try:
-            dynamic_indicator_object = get_dynamic_indicator(dynamic_indicator_name)
-        except DynamicIndicatorNotExist:
-            warn(
-                f"El indicador {dynamic_indicator_name} no existe. "
-                "Se continua con el siguiente indicador."
+        Parameters
+        ----------
+        params: Dict[str, Any]
+            Parámetros del indicador dinámico.
+        """
+        execute = params.get(self.name_dynamic_indicator, {}).get("execute", False)
+        if execute:
+            logging.info(f"Ejecutando {self.name_dynamic_indicator}")
+            params_processor = self.load_params(params)
+            fname = self.create_file_name_process(params_processor)
+            system_params = params_processor.get_params_by_type(ParamType.SYSTEM)
+            params_indicator = params_processor.get_params_by_type(ParamType.INDICATOR)
+            flow_map = create_system(system_params)
+            path_fig = params_processor.get_param("path")
+            filename = os.path.join(path_fig, fname + ".png")
+            axis_data = params_processor.get_param("axis")
+
+            logging.info("-- Ejecutando el cálculo de malla con ecuaciones variacionales.")
+            grid_points, diff_f = ftl_variational_equations(flow_map, **params_indicator)
+            _, _ = plot_descriptors_map(
+                grid_points[axis_data[0]],
+                grid_points[axis_data[1]],
+                values=diff_f,
+                filename=filename,
+                axis=axis_data,
             )
-            continue
-        if dynamic_indicator_params.pop("execute", False):
-            logging.info(f"Ejecutando {dynamic_indicator_name}")
-            dynamic_indicator_object.process(system, system_params, dynamic_indicator_params)
-            logging.info(f"- Fin del proceso de {dynamic_indicator_name}")
-            logging.info("----------------------------------------------")
+            logging.info(f"- Campo FTLE guardado en {filename}.")
+            logging.info(f"- Fin del proceso de {self.name_dynamic_indicator}")
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     cauchy_green = np.dot(jacobian.T, jacobian)
     return np.log(np.max(np.linalg.eig(cauchy_green)[0])) / 2 / delta_t
 
 
 def ftle_element_wise(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    n_grid_x: Union[int, np.ndarray],
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: Union[int, np.ndarray],
     h_steps: Union[int, float, np.ndarray] = None,
     params_t_close: Dict[str, Any] = None,
     n_jobs: int = -1,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultFtleMethods:
     """
     Función que calcula los FTLE punto por punto para una malla de puntos delimitada por
@@ -99,18 +99,18 @@
 
     Parameters
     ----------
     flow: FlowMap
         Flujo del cual se calcula los ftle.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
     nx_grid: Union[int, np.ndarray]
         Número de puntos generados por variable, donde el número
         total de puntos será nx_grid^(n_variables.).  Si pasamos
         un entero se aplicará a todas las dimensiones. Si es una
         secuencia se aplicará según el orden de las dimensiones.
@@ -122,87 +122,79 @@
     projection_config: Dict[int, Projection], default None
             Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultFtleMethods
     """
-    n_var = x0_max_grid.size
-    if isinstance(n_grid_x, int):
-        n_grid_x = np.ones(n_var).astype(int) * n_grid_x
-    if x0_min_grid.size != n_var:
+    n_var = x0_max.size
+    if isinstance(n_xgrid, int):
+        n_xgrid = np.ones(n_var).astype(int) * n_xgrid
+    if x0_min.size != n_var:
         raise DoesntCoincideDimension(
             "La dimensión de x0_min_grid y x0_max_grid" " deben ser iguales."
         )
-    if n_grid_x.size != n_var:
+    if n_xgrid.size != n_var:
         raise DoesntCoincideDimension(
             "La dimensión de nx_grid no coincide con el número de variables."
         )
     if params_t_close is None:
         params_t_close = {}
 
     if h_steps is None:
-        h_steps = (x0_max_grid - x0_min_grid) / n_grid_x
+        h_steps = (x0_max - x0_min) / n_xgrid
     if n_jobs < 2:
         return _ftle_map_non_paralelizable(
-            flow, t, x0_min_grid, x0_max_grid, n_grid_x, h_steps, params_t_close, projection_config
+            flow, t, x0_min, x0_max, n_xgrid, h_steps, params_t_close, projection_config
         )
     return _ftle_map_paralelizable(
-        flow,
-        t,
-        x0_min_grid,
-        x0_max_grid,
-        n_grid_x,
-        h_steps,
-        params_t_close,
-        n_jobs,
-        projection_config,
+        flow, t, x0_min, x0_max, n_xgrid, h_steps, params_t_close, n_jobs, projection_config
     )
 
 
 def _ftle_map_non_paralelizable(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: np.ndarray,
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: np.ndarray,
     h_steps: Union[int, float, np.ndarray],
     params_t_close: Dict[str, Any] = None,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultFtleMethods:
     """
     Método no paralelizable de ftle_element_wise
 
     Parameters
     ----------
     flow: FlowMap
         Flujo del cual se calcula los ftle.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: np.ndarray
+    n_xgrid: np.ndarray
         Array con el número de puntos generados por variable.
     h_steps: Union[int, float, np.ndarray], default None
         Array que indica el paso de las derivadas numéticas para cada dimensión
         de la variable. En el caso de indicar None se usará el paso de la malla.
     projection_config: Dict[int, Projection], default None
             Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultFtleMethods
     """
-    n_var = x0_max_grid.size
+    n_var = x0_max.size
     grid_points = np.meshgrid(
-        *[np.linspace(x0_min_grid[i], x0_max_grid[i], nx_grid[i]) for i in range(n_var)]
+        *[np.linspace(x0_min[i], x0_max[i], n_xgrid[i]) for i in range(n_var)]
     )
     grid_points = project_grid_data(grid_points, projection_config)
     ftle_grid = np.zeros(grid_points[0].shape)
     it = np.nditer(grid_points[0], flags=["multi_index"])
     pbar = tqdm(total=grid_points[0].size)
     while not it.finished:
         x0 = np.array([gp[it.multi_index] for gp in grid_points])
@@ -215,54 +207,54 @@
     result = ResultFtleMethods(grid_points, ftle_grid)
     return result
 
 
 def _ftle_map_paralelizable(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: np.ndarray,
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: np.ndarray,
     h_steps: Union[int, float, np.ndarray],
     params_t_close: Dict[str, Any],
     n_jobs: int,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultFtleMethods:
     """
     Método paralelizable de ftle_element_wise
 
     Parameters
     ----------
     flow: FlowMap
         Flujo del cual se calcula los ftle.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: np.ndarray
+    n_xgrid: np.ndarray
          Array con el número de puntos generados por variable.
     h_steps: Union[int, float, np.ndarray], default None
         Array que indica el paso de las derivadas numéticas para cada dimensión
         de la variable. En el caso de indicar None se usará el paso de la malla.
     n_jobs: int
         Número máximo de jobs en la paralelización.
     projection_config: Dict[int, Projection], default None
             Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultFtleMethods
     """
-    n_var = x0_max_grid.size
+    n_var = x0_max.size
     grid_points = np.meshgrid(
-        *[np.linspace(x0_min_grid[i], x0_max_grid[i], nx_grid[i]) for i in range(n_var)]
+        *[np.linspace(x0_min[i], x0_max[i], n_xgrid[i]) for i in range(n_var)]
     )
     grid_points = project_grid_data(grid_points, projection_config)
     ftle_grid = np.zeros(grid_points[0].shape)
     it = np.nditer(grid_points[0], flags=["multi_index"])
     with ThreadPoolExecutor(max_workers=n_jobs) as executor:
         futures = []
         multi_index_list: List[Sequence[int]] = []
@@ -280,17 +272,17 @@
     result = ResultFtleMethods(grid_points, ftle_grid)
     return result
 
 
 def diff_flow_grid(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: Union[int, np.ndarray],
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: Union[int, np.ndarray],
     n_jobs: int = -1,
     projection_config: Dict[int, Projection] = None,
 ) -> Tuple[Union[Sequence[np.ndarray], str], Sequence[np.ndarray]]:
     """
     Método que crea una malla de condiciones iniciales, donde los
     limítes están definidos por x0_min_grid y x0_max_grid y la cantidad
     de puntos son nx_grid^(numero de variables), y calcula el valor de las
@@ -300,21 +292,21 @@
 
     Parameters
     ----------
     flow: FlowMap
         Flujo el cual queremos calcular las derivadas parciales.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: Union[int, Sequence[int]]
+    n_xgrid: Union[int, Sequence[int]]
         Número de puntos generados por variable, donde el número
         total de puntos será nx_grid^(n_variables.).  Si pasamos
         un entero se aplicará a todas las dimensiones. Si es una
         secuencia se aplicará según el orden de las dimensiones.
     n_jobs: int, default 0
         Número máximo de jobs en la paralelización.
     projection_config: Dict[int, Projection], default None
@@ -326,43 +318,43 @@
         Lista con la malla para cada dimensión. Cada elemento
         es n array de dimensión (nx_grid,..., <n_variables>, ...,nx_grid).
     list_df: List[np.ndarray]:
         Lista de arrays de dimensión (nx_grid,..., <n_variables>, ...,nx_grid, n_variables),
         donde el elemento i de la lista representa el valor de la dereivada parcial de la
         variable x_i.
     """
-    n_var = x0_max_grid.size
-    if x0_min_grid.shape != x0_max_grid.shape:
+    n_var = x0_max.size
+    if x0_min.shape != x0_max.shape:
         raise DoesntCoincideDimension(
             "La dimensión de x0_min_grid y x0_max_grid" " deben ser iguales."
         )
-    if isinstance(nx_grid, int):
-        nx_grid = np.ones(n_var).astype(int) * nx_grid
-    nx_grid_1 = nx_grid == 1
-    h = (x0_max_grid - x0_min_grid) / (nx_grid - 1)
-    h[nx_grid_1] = (x0_max_grid[nx_grid_1] - x0_min_grid[nx_grid_1]) / (nx_grid[nx_grid_1])
+    if isinstance(n_xgrid, int):
+        n_xgrid = np.ones(n_var).astype(int) * n_xgrid
+    nx_grid_1 = n_xgrid == 1
+    h = (x0_max - x0_min) / (n_xgrid - 1)
+    h[nx_grid_1] = (x0_max[nx_grid_1] - x0_min[nx_grid_1]) / (n_xgrid[nx_grid_1])
     grid_points, zz = flow.flow_grid(
         t=t,
-        x0_min_grid=x0_min_grid - h,
-        x0_max_grid=x0_max_grid + h,
-        nx_grid=nx_grid + 2,
+        x0_min=x0_min - h,
+        x0_max=x0_max + h,
+        n_xgrid=n_xgrid + 2,
         n_jobs=n_jobs,
         projection_config=projection_config,
     )
     diff_partials = diff_partials_grid(zz, n_var, h, edge_remove=True)
     mask = (np.s_[1:-1],) * n_var
     return [gp[mask] for gp in grid_points], diff_partials
 
 
 def ftle_grid(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: Union[int, np.ndarray],
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: Union[int, np.ndarray],
     n_jobs: int = -1,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultFtleMethods:
     """
     Función que crea una malla de condiciones iniciales, donde los
     limítes están definidos por x0_min_grid y x0_max_grid y la cantidad
     de puntos son nx_grid^(numero de variables), y calcula el valor de las
@@ -371,36 +363,36 @@
 
     Parameters
     ----------
     flow: FlowMap
         Flujo del cual se calcula los ftle.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: Union[int, Sequence[int]]
+    n_xgrid: Union[int, Sequence[int]]
         Número de puntos generados por variable, donde el número
         total de puntos será nx_grid^(n_variables.). Si pasamos
         un entero se aplicará a todas las dimensiones. Si es una
         secuencia se aplicará según el orden de las dimensiones.
     n_jobs: int, default 0
         Número máximo de jobs en la paralelización.
     projection_config: Dict[int, Projection], default None
             Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultFtleMethods
     """
     grid_points, diff_flow = diff_flow_grid(
-        flow, t, x0_min_grid, x0_max_grid, nx_grid, n_jobs, projection_config
+        flow, t, x0_min, x0_max, n_xgrid, n_jobs, projection_config
     )
     ftle_grid = np.zeros(diff_flow[0].shape[:-1])
     delta_t = abs(t - flow.t0)
     for index in np.ndindex(diff_flow[0].shape[:-1]):
         jacobian = np.concatenate([di[index].reshape(1, -1) for di in diff_flow], 0)
         cauchy_green = np.dot(jacobian.T, jacobian)
         if np.isnan(jacobian).any():
@@ -410,17 +402,17 @@
     result = ResultFtleMethods(grid_points, ftle_grid)
     return result
 
 
 def ftl_variational_equations(
     flow: FlowMap,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: Union[int, np.ndarray],
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: Union[int, np.ndarray],
     n_jobs: int = -1,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultFtleMethods:
     """
     Función que crea una malla de condiciones iniciales, donde los
     limítes están definidos por x0_min_grid y x0_max_grid y la cantidad
     de puntos son nx_grid^(numero de variables), y calcula el valor de las
@@ -429,50 +421,50 @@
 
     Parameters
     ----------
     flow: FlowMap
         Flujo del cual se calcula los ftle.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: Union[int, Sequence[int]]
+    n_xgrid: Union[int, Sequence[int]]
         Número de puntos generados por variable, donde el número
         total de puntos será nx_grid^(n_variables.). Si pasamos
         un entero se aplicará a todas las dimensiones. Si es una
         secuencia se aplicará según el orden de las dimensiones.
     n_jobs: int, default 0
         Número máximo de jobs en la paralelización.
     projection_config: Dict[int, Projection], default None
             Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultFtleMethods
     """
-    n_var = x0_max_grid.size
-    if x0_min_grid.shape != x0_max_grid.shape:
+    n_var = x0_max.size
+    if x0_min.shape != x0_max.shape:
         raise DoesntCoincideDimension(
             "La dimensión de x0_min_grid y x0_max_grid" " deben ser iguales."
         )
-    if isinstance(nx_grid, int):
-        nx_grid = np.ones(n_var).astype(int) * nx_grid
+    if isinstance(n_xgrid, int):
+        n_xgrid = np.ones(n_var).astype(int) * n_xgrid
 
-    x_min_grid = np.concatenate((x0_min_grid, np.eye(n_var).reshape(n_var**2)))
-    x_max_grid = np.concatenate((x0_max_grid, np.eye(n_var).reshape(n_var**2)))
-    nx_grid = np.concatenate((nx_grid, np.ones(n_var**2))).astype(int)
+    x_min_grid = np.concatenate((x0_min, np.eye(n_var).reshape(n_var**2)))
+    x_max_grid = np.concatenate((x0_max, np.eye(n_var).reshape(n_var**2)))
+    n_xgrid = np.concatenate((n_xgrid, np.ones(n_var**2))).astype(int)
     grid_points, flow_points = flow.flow_grid(
         t=t,
-        x0_min_grid=x_min_grid,
-        x0_max_grid=x_max_grid,
-        nx_grid=nx_grid,
+        x0_min=x_min_grid,
+        x0_max=x_max_grid,
+        n_xgrid=n_xgrid,
         n_jobs=n_jobs,
         projection_config=projection_config,
     )
     ftle_grid = np.zeros(flow_points.shape[:n_var])
     delta_t = abs(t - flow.t0)
     for index in np.ndindex(flow_points.shape[:n_var]):
         jacobian = flow_points[index].reshape(n_var + n_var**2)
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -124,17 +124,17 @@
     mean_velocity = length_value / delta_t
     return mean_velocity, error_length
 
 
 def lagrangian_descriptors(
     diff_system: DiffSystem,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    n_grid_x: Union[int, np.ndarray],
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: Union[int, np.ndarray],
     tau: Union[float, int, Tuple[float, float]],
     method_integrate: str,
     params_solver: Dict[str, Any] = None,
     opts_integrate: Dict[str, Any] = None,
     n_jobs: int = -1,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultLDMethods:
@@ -146,21 +146,21 @@
 
     Parameters
     ----------
     diff_system: DiffSystem
         Sistema diferencial para integrar.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    n_grid_x: Union[int, np.ndarray]
+    n_xgrid: Union[int, np.ndarray]
         Número de puntos generados por variable, donde el número
         total de puntos será nx_grid^(n_variables.).  Si pasamos
         un entero se aplicará a todas las dimensiones. Si es una
         secuencia se aplicará según el orden de las dimensiones.
     tau: Union[float, int, Tuple[float, float]]
         Valor utilizado para construir el intervalo de integración.
         Si es int o float el intervalo se calcula como [t-tau, t+tau].
@@ -180,60 +180,60 @@
     projection_config: Dict[int, Projection], default None
         Diccionario que recoge las proyecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultLDMethods
     """
-    n_var = x0_max_grid.size
-    if isinstance(n_grid_x, int):
-        n_grid_x = np.ones(n_var).astype(int) * n_grid_x
-    if x0_min_grid.size != n_var:
+    n_var = x0_max.size
+    if isinstance(n_xgrid, int):
+        n_xgrid = np.ones(n_var).astype(int) * n_xgrid
+    if x0_min.size != n_var:
         raise DoesntCoincideDimension(
             "La dimensión de x0_min_grid y x0_max_grid" " deben ser iguales."
         )
-    if n_grid_x.size != n_var:
+    if n_xgrid.size != n_var:
         raise DoesntCoincideDimension(
             "La dimensión de nx_grid no coincide con el número de variables."
         )
 
     if n_jobs < 2:
         return _lagrangian_descriptors_non_paralelizable(
             diff_system=diff_system,
             t=t,
-            x0_min_grid=x0_min_grid,
-            x0_max_grid=x0_max_grid,
-            nx_grid=n_grid_x,
+            x0_min=x0_min,
+            x0_max=x0_max,
+            n_xgrid=n_xgrid,
             tau=tau,
-            params_solver=params_solver,
             method_integrate=method_integrate,
+            params_solver=params_solver,
             opts_integrate=opts_integrate,
             projection_config=projection_config,
         )
     return _lagrangian_descriptors_paralelizable(
         diff_system=diff_system,
         t=t,
-        x0_min_grid=x0_min_grid,
-        x0_max_grid=x0_max_grid,
-        nx_grid=n_grid_x,
+        x0_min=x0_min,
+        x0_max=x0_max,
+        n_xgrid=n_xgrid,
         tau=tau,
-        params_solver=params_solver,
         method_integrate=method_integrate,
+        params_solver=params_solver,
         opts_integrate=opts_integrate,
         n_jobs=n_jobs,
         projection_config=projection_config,
     )
 
 
 def _lagrangian_descriptors_non_paralelizable(
     diff_system: DiffSystem,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: np.ndarray,
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: np.ndarray,
     tau: Union[float, int, Tuple[float, float]],
     method_integrate: str,
     params_solver: Dict[str, Any] = None,
     opts_integrate: Dict[str, Any] = None,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultLDMethods:
     """
@@ -241,21 +241,21 @@
 
     Parameters
     ----------
     diff_system: DiffSystem
         Sistema diferencial para integrar.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: np.ndarray
+    n_xgrid: np.ndarray
         Array con el número de puntos generados por variable.
     method_integrate: str, default "quad"
         Nombre del método de integración utilizado.
         Ver get_method_integrate, por defecto se utiliza
         scipy.integrate.quad.
     params_solver: Dict[str, Any], default None
         Diccionario con los parámetros del solver del sistema diferencial.
@@ -266,17 +266,17 @@
     projection_config: Dict[int, Projection], default None
         Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultLDMethods
     """
-    n_var = x0_max_grid.size
+    n_var = x0_max.size
     grid_points = np.meshgrid(
-        *[np.linspace(x0_min_grid[i], x0_max_grid[i], nx_grid[i]) for i in range(n_var)]
+        *[np.linspace(x0_min[i], x0_max[i], n_xgrid[i]) for i in range(n_var)]
     )
     grid_points = project_grid_data(grid_points, projection_config)
     lag_grid = np.zeros(grid_points[0].shape)
     it = np.nditer(grid_points[0], flags=["multi_index"])
     pbar = tqdm(total=grid_points[0].size)
 
     while not it.finished:
@@ -292,17 +292,17 @@
     result = ResultLDMethods(grid_points, lag_grid)
     return result
 
 
 def _lagrangian_descriptors_paralelizable(
     diff_system: DiffSystem,
     t: Union[int, float],
-    x0_min_grid: np.ndarray,
-    x0_max_grid: np.ndarray,
-    nx_grid: np.ndarray,
+    x0_min: np.ndarray,
+    x0_max: np.ndarray,
+    n_xgrid: np.ndarray,
     tau: Union[float, int, Tuple[float, float]],
     method_integrate: str,
     params_solver: Dict[str, Any] = None,
     opts_integrate: Dict[str, Any] = None,
     n_jobs: int = 2,
     projection_config: Dict[int, Projection] = None,
 ) -> ResultLDMethods:
@@ -311,21 +311,21 @@
 
     Parameters
     ----------
     diff_system: DiffSystem
         Sistema diferencial para integrar.
     t: Union[int, float]
         Valor del tiempo.
-    x0_min_grid: np.ndarray
+    x0_min: np.ndarray
         Array de dimensión (n_variables,) que indica el valor inferior
         de la malla.
-    x0_max_grid: np.ndarray
+    x0_max: np.ndarray
         Array de dimensión (n_variables,) que indica el valor superior
         de la malla.
-    nx_grid: np.ndarray
+    n_xgrid: np.ndarray
          Array con el número de puntos generados por variable.
     method_integrate: str, default "quad"
         Nombre del método de integración utilizado.
         Ver get_method_integrate, por defecto se utiliza
         scipy.integrate.quad.
     params_solver: Dict[str, Any], default None
         Diccionario con los parámetros del solver del sistema diferencial.
@@ -338,17 +338,17 @@
     projection_config: Dict[int, Projection], default None
         Diccionario que recoge las projecciones que se hagan en cada dimensión.
 
     Returns
     -------
     result: ResultLDMethods
     """
-    n_var = x0_max_grid.size
+    n_var = x0_max.size
     grid_points = np.meshgrid(
-        *[np.linspace(x0_min_grid[i], x0_max_grid[i], nx_grid[i]) for i in range(n_var)]
+        *[np.linspace(x0_min[i], x0_max[i], n_xgrid[i]) for i in range(n_var)]
     )
     grid_points = project_grid_data(grid_points, projection_config)
     lag_grid = np.zeros(grid_points[0].shape)
     it = np.nditer(grid_points[0], flags=["multi_index"])
     with ThreadPoolExecutor(max_workers=n_jobs) as executor:
         futures = []
         multi_index_list: List[Sequence[int]] = []
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Sequence, Tuple, Union
+from typing import Any, Callable, List, Sequence, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.colors import Normalize
 
 from dynamic_indicators_tools.differentials_systems.diff_system import DiffSystem
 
@@ -117,7 +117,34 @@
         )
         t_ar = np.linspace(0, 2 * t1, 200)
         sol = ds.variable(t_ar).T
         ax.plot(sol[:, 0], sol[:, 1])
     ax.set_xlim(left=x_min[0], right=x_max[0])
     ax.set_ylim(bottom=x_min[1], top=x_max[1])
     return ax
+
+
+def plot_poincare_sections(
+    values: Union[np.ndarray, List[np.ndarray]],
+    title_map: str = None,
+    filename: str = None,
+    axis: Tuple[int, int] = None,
+) -> plt.Figure:
+    if isinstance(values, np.ndarray):
+        values = [values]
+    if axis is None:
+        axis = (0, 1)
+
+    title = ""
+    if isinstance(filename, str):
+        title = filename.split("/")[-1].split(".")[0]
+    title = title_map or title
+    fig = plt.figure()
+    plt.title(title)
+    for i, var in enumerate(values):
+        x = var[:, axis[0]]
+        y = var[:, axis[1]]
+        plt.scatter(x, y, s=3)
+    plt.xlabel(f"x{axis[0]}-values")
+    plt.ylabel(f"x{axis[1]}-values")
+    plt.savefig(filename)
+    return fig
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/differentiation.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools/numercial_methods/integrators.py` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools/numercial_methods/integrators.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/PKG-INFO` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-indicators-tools
-Version: 0.1.1
+Version: 1.0.1
 Summary: Repositorio que recoge herramientas para el análisis de sistemas dinámicos
 Home-page: https://github.com/santhiperbolico/dynamic_indicators_tools
 Author: Santiago Arranz Sanz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dynamic_indicators_tools-0.1.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt` & `dynamic_indicators_tools-1.0.1/src/dynamic_indicators_tools.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,41 @@
 src/dynamic_indicators_tools/__init__.py
 src/dynamic_indicators_tools/main_dynamic_indicators_process.py
 src/dynamic_indicators_tools.egg-info/PKG-INFO
 src/dynamic_indicators_tools.egg-info/SOURCES.txt
 src/dynamic_indicators_tools.egg-info/dependency_links.txt
 src/dynamic_indicators_tools.egg-info/requires.txt
 src/dynamic_indicators_tools.egg-info/top_level.txt
-src/dynamic_indicators_tools/config_files/__init__.py
-src/dynamic_indicators_tools/config_files/get_params_config.py
 src/dynamic_indicators_tools/differentials_systems/__init__.py
 src/dynamic_indicators_tools/differentials_systems/data_transformations.py
 src/dynamic_indicators_tools/differentials_systems/diff_system.py
 src/dynamic_indicators_tools/differentials_systems/solver_integrators.py
 src/dynamic_indicators_tools/dynamic_indicators/__init__.py
 src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_process.py
-src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents.py
-src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors.py
+src/dynamic_indicators_tools/dynamic_indicators/dynamic_indicators_utils.py
+src/dynamic_indicators_tools/dynamic_indicators/params_methods.py
 src/dynamic_indicators_tools/dynamic_indicators/plot_descriptors.py
+src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/__init__.py
+src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_indicator.py
+src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_params.py
+src/dynamic_indicators_tools/dynamic_indicators/finite_time_lyapunov_exponents/ftle_utils.py
+src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/__init__.py
+src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_indicator.py
+src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_params.py
+src/dynamic_indicators_tools/dynamic_indicators/lagrangian_descriptors/ld_utils.py
+src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/__init__.py
+src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_indicator.py
+src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_params.py
+src/dynamic_indicators_tools/dynamic_indicators/poincare_maps/poincare_utils.py
 src/dynamic_indicators_tools/numercial_methods/__init__.py
 src/dynamic_indicators_tools/numercial_methods/differentiation.py
 src/dynamic_indicators_tools/numercial_methods/integrators.py
 src/tests/__init__.py
-src/tests/test_config_files.py
 src/tests/test_data_transformations.py
 src/tests/test_diff_systems.py
 src/tests/test_differentiation.py
 src/tests/test_dynamic_indicators_process.py
 src/tests/test_finite_time_lyapunov_exponents.py
 src/tests/test_lagrangian_descriptors.py
+src/tests/test_params_method.py
+src/tests/test_poincare_map.py
 src/tests/test_system_black_hole_schwarzchids.py
```

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_config_files.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_params_method.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import numpy as np
 import pytest
 
-from dynamic_indicators_tools.config_files.get_params_config import (
-    format_symbolic_number,
-    get_main_params,
-)
+from dynamic_indicators_tools.dynamic_indicators.params_methods import format_symbolic_number
 
 
 @pytest.mark.parametrize(
     "symbol, expected",
     [
         ("-_pi", -np.pi),
         ("2_-_pi", 2 - np.pi),
@@ -31,81 +28,82 @@
 
 
 @pytest.fixture
 def config_main_test():
     return "tests/config_files/config_main_test_system.json"
 
 
-def test_get_main_params_system_params(config_main_test):
-    system, system_params, dynamic_indicators = get_main_params(config_main_test)
-
-    expected_system_params = {
-        "path": "tests/systems/test_plots/",
-        "system_name": "test_system_2",
-        "args_system": [2],
-        "t0": 0,
-        "t1": 10,
-        "x_min": np.array([-np.pi, -3.0, 0.0]),
-        "x_max": np.array([np.pi, 3.0, 1.0]),
-        "n_xgrid": 10,
-        "solver_method": "solve_ivp",
-        "n_jobs": 1,
-    }
-
-    assert expected_system_params["path"] == system_params["path"]
-    assert expected_system_params["system_name"] == system_params["system_name"]
-    assert expected_system_params["args_system"] == system_params["args_system"]
-    assert expected_system_params["t0"] == system_params["t0"]
-    assert (expected_system_params["x_min"] == system_params["x_min"]).all()
-    assert (expected_system_params["x_min"] == system_params["x_min"]).all()
-    assert expected_system_params["n_xgrid"] == system_params["n_xgrid"]
-    assert expected_system_params["solver_method"] == system_params["solver_method"]
-    assert expected_system_params["n_jobs"] == system_params["n_jobs"]
-
-
-def test_get_main_params_dynamic_params(config_main_test):
-    system, system_params, dynamic_indicators = get_main_params(config_main_test)
-
-    expected_dynamic = {
-        "ftle_element_wise": {
-            "execute": True,
-            "h_steps": 0.01,
-            "t_close": True,
-            "params_t_close": {
-                "time_delta": 0.2,
-                "dimensions_close": [True, False, False],
-                "mod_solution": 2 * np.pi,
-            },
-        },
-        "ftle_grid": {"execute": True},
-        "lagrangian_descriptors": {
-            "execute": True,
-            "tau": 5,
-            "method_integrate": "fixed_quad",
-            "plot_orbits": True,
-        },
-    }
-    execute_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["execute"]
-    h_steps_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["h_steps"]
-    t_close_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["t_close"]
-    time_delta = dynamic_indicators["ftle_element_wise"]["params_t_close"]["time_delta"]
-    dim_c = dynamic_indicators["ftle_element_wise"]["params_t_close"]["dimensions_close"]
-    mod_solution = dynamic_indicators["ftle_element_wise"]["params_t_close"]["mod_solution"]
-
-    execute_ftle_grid = dynamic_indicators["ftle_grid"]["execute"]
-    tau_lagrangian_descriptors = dynamic_indicators["lagrangian_descriptors"]["tau"]
-    execute_lagrangian_descriptors = dynamic_indicators["lagrangian_descriptors"]["execute"]
-    method_integrate = dynamic_indicators["lagrangian_descriptors"]["method_integrate"]
-    plot_orbits = dynamic_indicators["lagrangian_descriptors"]["plot_orbits"]
-
-    assert expected_dynamic["ftle_element_wise"]["execute"] == execute_ftle_element_wise
-    assert expected_dynamic["ftle_element_wise"]["h_steps"] == h_steps_ftle_element_wise
-    assert expected_dynamic["ftle_element_wise"]["t_close"] == t_close_ftle_element_wise
-    assert expected_dynamic["ftle_element_wise"]["params_t_close"]["time_delta"] == time_delta
-    assert expected_dynamic["ftle_element_wise"]["params_t_close"]["dimensions_close"] == dim_c
-    assert expected_dynamic["ftle_element_wise"]["params_t_close"]["mod_solution"] == mod_solution
-
-    assert expected_dynamic["ftle_grid"]["execute"] == execute_ftle_grid
-    assert expected_dynamic["lagrangian_descriptors"]["execute"] == execute_lagrangian_descriptors
-    assert expected_dynamic["lagrangian_descriptors"]["tau"] == tau_lagrangian_descriptors
-    assert expected_dynamic["lagrangian_descriptors"]["method_integrate"] == method_integrate
-    assert expected_dynamic["lagrangian_descriptors"]["plot_orbits"] == plot_orbits
+#
+# def test_get_main_params_system_params(config_main_test):
+#     system, system_params, dynamic_indicators = get_main_params(config_main_test)
+#
+#     expected_system_params = {
+#         "path": "tests/systems/test_plots/",
+#         "system_name": "test_system_2",
+#         "args_system": [2],
+#         "t0": 0,
+#         "t1": 10,
+#         "x_min": np.array([-np.pi, -3.0, 0.0]),
+#         "x_max": np.array([np.pi, 3.0, 1.0]),
+#         "n_xgrid": 10,
+#         "solver_method": "solve_ivp",
+#         "n_jobs": 1,
+#     }
+#
+#     assert expected_system_params["path"] == system_params["path"]
+#     assert expected_system_params["system_name"] == system_params["system_name"]
+#     assert expected_system_params["args_system"] == system_params["args_system"]
+#     assert expected_system_params["t0"] == system_params["t0"]
+#     assert (expected_system_params["x_min"] == system_params["x_min"]).all()
+#     assert (expected_system_params["x_min"] == system_params["x_min"]).all()
+#     assert expected_system_params["n_xgrid"] == system_params["n_xgrid"]
+#     assert expected_system_params["solver_method"] == system_params["solver_method"]
+#     assert expected_system_params["n_jobs"] == system_params["n_jobs"]
+#
+#
+# def test_get_main_params_dynamic_params(config_main_test):
+#     system, system_params, dynamic_indicators = get_main_params(config_main_test)
+#
+#     expected_dynamic = {
+#         "ftle_element_wise": {
+#             "execute": True,
+#             "h_steps": 0.01,
+#             "t_close": True,
+#             "params_t_close": {
+#                 "time_delta": 0.2,
+#                 "dimensions_close": [True, False, False],
+#                 "mod_solution": 2 * np.pi,
+#             },
+#         },
+#         "ftle_grid": {"execute": True},
+#         "lagrangian_descriptors": {
+#             "execute": True,
+#             "tau": 5,
+#             "method_integrate": "fixed_quad",
+#             "plot_orbits": True,
+#         },
+#     }
+#     execute_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["execute"]
+#     h_steps_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["h_steps"]
+#     t_close_ftle_element_wise = dynamic_indicators["ftle_element_wise"]["t_close"]
+#     time_delta = dynamic_indicators["ftle_element_wise"]["params_t_close"]["time_delta"]
+#     dim_c = dynamic_indicators["ftle_element_wise"]["params_t_close"]["dimensions_close"]
+#     mod_solution = dynamic_indicators["ftle_element_wise"]["params_t_close"]["mod_solution"]
+#
+#     execute_ftle_grid = dynamic_indicators["ftle_grid"]["execute"]
+#     tau_lagrangian_descriptors = dynamic_indicators["lagrangian_descriptors"]["tau"]
+#     execute_lagrangian_descriptors = dynamic_indicators["lagrangian_descriptors"]["execute"]
+#     method_integrate = dynamic_indicators["lagrangian_descriptors"]["method_integrate"]
+#     plot_orbits = dynamic_indicators["lagrangian_descriptors"]["plot_orbits"]
+#
+#     assert expected_dynamic["ftle_element_wise"]["execute"] == execute_ftle_element_wise
+#     assert expected_dynamic["ftle_element_wise"]["h_steps"] == h_steps_ftle_element_wise
+#     assert expected_dynamic["ftle_element_wise"]["t_close"] == t_close_ftle_element_wise
+#     assert expected_dynamic["ftle_element_wise"]["params_t_close"]["time_delta"] == time_delta
+#     assert expected_dynamic["ftle_element_wise"]["params_t_close"]["dimensions_close"] == dim_c
+#    assert expected_dynamic["ftle_element_wise"]["params_t_close"]["mod_solution"] == mod_solution
+#
+#     assert expected_dynamic["ftle_grid"]["execute"] == execute_ftle_grid
+#    assert expected_dynamic["lagrangian_descriptors"]["execute"] == execute_lagrangian_descriptors
+#     assert expected_dynamic["lagrangian_descriptors"]["tau"] == tau_lagrangian_descriptors
+#     assert expected_dynamic["lagrangian_descriptors"]["method_integrate"] == method_integrate
+#     assert expected_dynamic["lagrangian_descriptors"]["plot_orbits"] == plot_orbits
```

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_data_transformations.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_diff_systems.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_diff_systems.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_differentiation.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_differentiation.py`

 * *Files identical despite different names*

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_finite_time_lyapunov_exponents.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_finite_time_lyapunov_exponents.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 
 from dynamic_indicators_tools.differentials_systems.diff_system import (
     DiffSystem,
     DiffVariable,
     FlowMap,
 )
-from dynamic_indicators_tools.dynamic_indicators.finite_time_lyapunov_exponents import (
+from dynamic_indicators_tools.dynamic_indicators.finite_time_lyapunov_exponents.ftle_utils import (
     diff_flow_grid,
     ftl_variational_equations,
     ftle_element_wise,
     ftle_fun,
     ftle_grid,
 )
 
@@ -103,20 +103,15 @@
     n_jobs = 1
 
     dx, _ = get_diff_system()
     flow_x = FlowMap(dx, 0)
     x_min_grid = np.array([0] * dimension)
     x_max_grid = np.array([10] * dimension)
     grid_points, diff_f = diff_flow_grid(
-        flow=flow_x,
-        t=t,
-        x0_min_grid=x_min_grid,
-        x0_max_grid=x_max_grid,
-        nx_grid=nx_grid,
-        n_jobs=n_jobs,
+        flow=flow_x, t=t, x0_min=x_min_grid, x0_max=x_max_grid, n_xgrid=nx_grid, n_jobs=n_jobs
     )
     for i in range(len(diff_f)):
         dfxi = diff_f[i]
         gradient = np.zeros(dimension)
         gradient[i] = np.exp((-1) ** i * t)
         expected_val = gradient.reshape((1, 1, -1)).repeat(nx_grid, axis=0).repeat(nx_grid, axis=1)
         error_max = np.abs(expected_val - dfxi).max()
```

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_lagrangian_descriptors.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_lagrangian_descriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Tuple, Union
 
 import numpy as np
 import pytest
 
 from dynamic_indicators_tools.differentials_systems.diff_system import DiffSystem, DiffVariable
-from dynamic_indicators_tools.dynamic_indicators.lagrangian_descriptors import (
+from dynamic_indicators_tools.dynamic_indicators.lagrangian_descriptors.ld_utils import (
     integrate_func_diff_system,
 )
 from dynamic_indicators_tools.numercial_methods.integrators import DoesntExistIntegrator
 
 TimeType = Union[int, float, np.ndarray]
 SolutionSystem = Callable[[TimeType, np.ndarray], np.ndarray]
```

### Comparing `dynamic_indicators_tools-0.1.1/src/tests/test_system_black_hole_schwarzchids.py` & `dynamic_indicators_tools-1.0.1/src/tests/test_system_black_hole_schwarzchids.py`

 * *Files identical despite different names*

