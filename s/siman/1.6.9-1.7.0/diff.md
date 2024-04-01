# Comparing `tmp/siman-1.6.9.tar.gz` & `tmp/siman-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.6.9.tar", last modified: Wed Mar 13 12:47:03 2024, max compression
+gzip compressed data, was "dist/siman-1.7.0.tar", last modified: Mon Apr  1 11:29:22 2024, max compression
```

## Comparing `siman-1.6.9.tar` & `siman-1.7.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.713402 siman-1.6.9/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.6.9/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.6.9/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-03-13 12:47:03.713402 siman-1.6.9/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.6.9/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2024-03-13 12:47:03.713402 siman-1.6.9/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2024-03-13 12:47:02.000000 siman-1.6.9/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.711402 siman-1.6.9/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.6.9/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3215 2023-12-17 17:36:40.000000 siman-1.6.9/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.6.9/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50716 2024-02-01 17:56:50.000000 siman-1.6.9/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.6.9/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.711402 siman-1.6.9/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.6.9/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.6.9/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.6.9/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.6.9/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   121473 2024-03-04 08:14:56.000000 siman-1.6.9/siman/calc_manage (2).py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   122774 2024-01-18 17:24:59.000000 siman-1.6.9/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.6.9/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.712402 siman-1.6.9/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.6.9/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.6.9/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.6.9/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.6.9/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    57149 2024-01-18 16:57:55.000000 siman-1.6.9/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.6.9/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.712402 siman-1.6.9/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.6.9/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.6.9/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.6.9/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.6.9/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.712402 siman-1.6.9/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.6.9/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53522 2024-03-07 15:18:22.000000 siman-1.6.9/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.6.9/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    34063 2023-11-29 19:26:59.000000 siman-1.6.9/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.6.9/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.6.9/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120871 2024-01-20 16:12:25.000000 siman-1.6.9/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.6.9/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.6.9/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.6.9/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2024-03-07 15:17:14.000000 siman-1.6.9/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.6.9/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28322 2023-12-17 17:36:40.000000 siman-1.6.9/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   115020 2024-02-26 14:49:15.000000 siman-1.6.9/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16799 2024-01-19 17:40:37.000000 siman-1.6.9/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.6.9/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.6.9/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    90186 2024-03-13 12:46:54.000000 siman-1.6.9/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.6.9/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.713402 siman-1.6.9/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.6.9/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.6.9/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.6.9/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.6.9/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.6.9/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31738 2023-12-07 16:24:27.000000 siman-1.6.9/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.6.9/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50674 2023-11-01 19:53:34.000000 siman-1.6.9/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.6.9/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.6.9/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.6.9/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.6.9/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194864 2023-12-24 13:06:44.000000 siman-1.6.9/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.6.9/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.6.9/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.6.9/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31129 2024-01-22 17:42:09.000000 siman-1.6.9/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.6.9/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.6.9/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6875 2023-11-01 20:00:05.000000 siman-1.6.9/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.6.9/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.6.9/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.6.9/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.6.9/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-03-13 12:47:03.711402 siman-1.6.9/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-03-13 12:47:03.000000 siman-1.6.9/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1702 2024-03-13 12:47:03.000000 siman-1.6.9/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2024-03-13 12:47:03.000000 siman-1.6.9/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2024-03-13 12:47:03.000000 siman-1.6.9/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2024-03-13 12:47:03.000000 siman-1.6.9/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.7.0/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.7.0/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-04-01 11:29:22.738325 siman-1.7.0/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.7.0/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2024-04-01 11:29:22.738325 siman-1.7.0/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2024-04-01 11:29:18.000000 siman-1.7.0/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.7.0/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3215 2024-04-01 10:39:48.000000 siman-1.7.0/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.7.0/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50716 2024-04-01 10:39:48.000000 siman-1.7.0/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.7.0/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.7.0/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.7.0/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.7.0/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   121473 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calc_manage (2).py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   122774 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.7.0/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.737325 siman-1.7.0/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    57149 2024-04-01 10:39:48.000000 siman-1.7.0/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.7.0/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.737325 siman-1.7.0/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.7.0/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.7.0/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53522 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.7.0/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    34063 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3783 2023-07-26 16:52:32.000000 siman-1.7.0/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.7.0/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120871 2024-04-01 10:39:48.000000 siman-1.7.0/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.7.0/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.7.0/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.7.0/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2024-04-01 10:39:48.000000 siman-1.7.0/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.7.0/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28322 2024-04-01 10:39:48.000000 siman-1.7.0/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   115084 2024-04-01 10:39:48.000000 siman-1.7.0/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16831 2024-04-01 10:39:48.000000 siman-1.7.0/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.7.0/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.7.0/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    90186 2024-04-01 10:39:48.000000 siman-1.7.0/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.7.0/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.738325 siman-1.7.0/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.7.0/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.7.0/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.7.0/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.7.0/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.7.0/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31738 2024-04-01 10:39:48.000000 siman-1.7.0/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.7.0/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50674 2023-11-01 19:53:34.000000 siman-1.7.0/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.7.0/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.7.0/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194864 2024-04-01 10:39:48.000000 siman-1.7.0/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.7.0/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31133 2024-04-01 10:39:48.000000 siman-1.7.0/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.7.0/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.7.0/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6875 2023-11-01 20:00:05.000000 siman-1.7.0/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.7.0/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.7.0/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.7.0/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.7.0/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2024-04-01 11:29:22.736325 siman-1.7.0/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1702 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2024-04-01 11:29:22.000000 siman-1.7.0/siman.egg-info/top_level.txt
```

### Comparing `siman-1.6.9/LICENSE` & `siman-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/PKG-INFO` & `siman-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.6.9
+Version: 1.7.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.6.9/setup.py` & `siman-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.6.9",
+    version="1.7.0",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.6.9/siman/3d_plot.py` & `siman-1.7.0/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/SSHTools.py` & `siman-1.7.0/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/analysis.py` & `siman-1.7.0/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/analysis_functions.py` & `siman-1.7.0/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/analyze/segregation.py` & `siman-1.7.0/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/approximation.py` & `siman-1.7.0/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/bands.py` & `siman-1.7.0/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calc_manage (2).py` & `siman-1.7.0/siman/calc_manage (2).py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calc_manage.py` & `siman-1.7.0/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calcul.py` & `siman-1.7.0/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calculators/aims.py` & `siman-1.7.0/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calculators/gaussian.py` & `siman-1.7.0/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calculators/qe.py` & `siman-1.7.0/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calculators/vasp.py` & `siman-1.7.0/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/calculators/vasp_old.py` & `siman-1.7.0/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/chg/chg_func.py` & `siman-1.7.0/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/chg/vasputil_chgarith_module.py` & `siman-1.7.0/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/classes.py` & `siman-1.7.0/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/calculation.py` & `siman-1.7.0/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/calculation_old.py` & `siman-1.7.0/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/cluster_batch_script.py` & `siman-1.7.0/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/cluster_run_script.py` & `siman-1.7.0/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/molecule.py` & `siman-1.7.0/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/core/structure.py` & `siman-1.7.0/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/database.py` & `siman-1.7.0/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/default_project_conf.py` & `siman-1.7.0/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/dev_functions.py` & `siman-1.7.0/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/dos_functions.py` & `siman-1.7.0/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/fit_hex.py` & `siman-1.7.0/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/functions.py` & `siman-1.7.0/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/geo.py` & `siman-1.7.0/siman/geo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2880,18 +2880,20 @@
             return st_ads_pack
 
 
 
 def best_miller(hkl):
     #find best integer representation of float hkl
     #returns float
+
     if min(hkl) == 0: 
         n = abs(max(hkl))
     else:
         n = abs(min(hkl)) 
+    hkl = np.array(hkl)
     hkl = hkl/n
 
     d_m = 100
     for mul in range(1,10):
         hklm = hkl*mul
         hkli = hklm.round(0).astype(int)
         d = np.linalg.norm(hkli-hklm)
@@ -2925,16 +2927,19 @@
     ghkl = np.dot(hkl, recip) # convert to cartesian
     # print('hkl', hkl)
     # print('ghkl', ghkl)
     grprimd = np.asarray( np.matrix(rprimd).I.T ) #Transpose of the inverse matrix of rprimd
     uvw = np.dot(grprimd, ghkl )
     # print('uvw', uvw)
     m = np.linalg.norm(uvw)
+    # print(uvw)
+    
     uvw = uvw/m # normalize
     # uvw = uvw.round(0).astype(int)
+    # print(uvw)
     uvwo = best_miller(uvw)
 
 
     return uvwo
 
 def uvw2hkl(uvw, rprimd):
     #convert,
```

### Comparing `siman-1.6.9/siman/header.py` & `siman-1.7.0/siman/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 override_cluster_address = 0 # 1 or 0, override read calculations to header.CLUSTERS[cluster]['address'], usefull when switching between proxy and back of the same cluster
 pymatgen_flag = None
 open_terminal = False #used in runBash
 siman_run = False #
 PATH2SHELVE_DBSUP = 'calc.gdbm3' # supporting database
 PATH2SHELVE_DB = 'only_calc.gdbm3' # name for calculation database, db dict
 PATH2HISTORYFILE = 'history' 
+PATH2DATABASE        = None # ?
 
 
 
 
 
 
 #1. Read default global settings for siman package
```

### Comparing `siman-1.6.9/siman/impurity.py` & `siman-1.7.0/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/inout.py` & `siman-1.7.0/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/kpoints_functions.py` & `siman-1.7.0/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/mat_prop/mat_prop.py` & `siman-1.7.0/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/matproj_functions.py` & `siman-1.7.0/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/monte.py` & `siman-1.7.0/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/monte_functions.py` & `siman-1.7.0/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/neb.py` & `siman-1.7.0/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/pairs.py` & `siman-1.7.0/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/picture_functions.py` & `siman-1.7.0/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/plot_functions.py` & `siman-1.7.0/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/polaron.py` & `siman-1.7.0/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/polaron_hop.py` & `siman-1.7.0/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/polaron_mod.py` & `siman-1.7.0/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/project_funcs.py` & `siman-1.7.0/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/properties_2d.py` & `siman-1.7.0/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/properties_energy.py` & `siman-1.7.0/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/properties_lattice.py` & `siman-1.7.0/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/set_functions.py` & `siman-1.7.0/siman/set_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1013,15 +1013,15 @@
             }
         s.vasp_params = s.params
         s.potdir = copy.deepcopy(header.nu_dict)
 
         s.update()
         header.varset[setname] = copy.deepcopy(s)
     
-    setname = 'static'
+    setname = 'static' #SP
     if init or setname not in varset: #init only once
         s = InputSet(setname, calculator = 'vasp') #default starting set without relaxation
         s.kpoints_file = True
         s.add_nbands = 1.5
         s.params = {
             'ISTART'    : 0,
             'NELM'      : 50,
```

### Comparing `siman-1.6.9/siman/simanrc.py` & `siman-1.7.0/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/small_functions.py` & `siman-1.7.0/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/structure_functions.py` & `siman-1.7.0/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/table_functions.py` & `siman-1.7.0/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/thermo.py` & `siman-1.7.0/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman/workflow_utilities.py` & `siman-1.7.0/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.6.9/siman.egg-info/PKG-INFO` & `siman-1.7.0/siman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.6.9
+Version: 1.7.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.6.9/siman.egg-info/SOURCES.txt` & `siman-1.7.0/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

