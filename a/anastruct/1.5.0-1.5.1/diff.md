# Comparing `tmp/anastruct-1.5.0.tar.gz` & `tmp/anastruct-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastruct-1.5.0.tar", last modified: Mon Oct 30 11:40:01 2023, max compression
+gzip compressed data, was "anastruct-1.5.1.tar", last modified: Mon Apr  1 21:03:03 2024, max compression
```

## Comparing `anastruct-1.5.0.tar` & `anastruct-1.5.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.297856 anastruct-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35046 2023-10-30 11:38:46.000000 anastruct-1.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-30 11:38:46.000000 anastruct-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2023-10-30 11:40:01.297856 anastruct-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2023-10-30 11:38:46.000000 anastruct-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-10-30 11:38:46.000000 anastruct-1.5.0/_custom_build.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.285856 anastruct-1.5.0/anastruct/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.289856 anastruct-1.5.0/anastruct/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   281173 2023-10-30 11:38:54.000000 anastruct-1.5.0/anastruct/cython/basic.c
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/cython/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/cython/cbasic.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.289856 anastruct-1.5.0/anastruct/fem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.289856 anastruct-1.5.0/anastruct/fem/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/cython/celements.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   296617 2023-10-30 11:38:54.000000 anastruct-1.5.0/anastruct/fem/cython/elements.c
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/cython/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/fem/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_10_dead_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_11.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_12.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_13.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_15.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_16.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_17_gnl.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_18_discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_19_num_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_1_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_20_insert_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_21_rotate_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_22_loadcombination_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_23_sectionbase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_24_envelope_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_25_high_midspan_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_26_deflection.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_6_fixed_hinge.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_7_rotational_spring.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_8_non_linear_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/examples/ex_9_vertical_spring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/fem/plotter/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/plotter/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    50084 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/plotter/mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/plotter/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/plotter/values.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    82709 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/fem/system_components/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/system_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/system_components/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/system_components/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/system_components/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/fem/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/fem/util/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/material/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/material/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/material/units.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.293856 anastruct-1.5.0/anastruct/sectionbase/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-30 11:38:46.000000 anastruct-1.5.0/anastruct/sectionbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-10-30 11:38:47.000000 anastruct-1.5.0/anastruct/sectionbase/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2023-10-30 11:38:47.000000 anastruct-1.5.0/anastruct/sectionbase/sectionbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-10-30 11:38:47.000000 anastruct-1.5.0/anastruct/sectionbase/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-30 11:38:47.000000 anastruct-1.5.0/anastruct/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2023-10-30 11:38:47.000000 anastruct-1.5.0/anastruct/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.289856 anastruct-1.5.0/anastruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2023-10-30 11:40:01.000000 anastruct-1.5.0/anastruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-10-30 11:40:01.000000 anastruct-1.5.0/anastruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 11:40:01.000000 anastruct-1.5.0/anastruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-30 11:40:01.000000 anastruct-1.5.0/anastruct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-30 11:40:01.000000 anastruct-1.5.0/anastruct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-30 11:38:47.000000 anastruct-1.5.0/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-30 11:38:47.000000 anastruct-1.5.0/plot_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-10-30 11:38:47.000000 anastruct-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-30 11:38:47.000000 anastruct-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 11:40:01.297856 anastruct-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-30 11:38:47.000000 anastruct-1.5.0/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:40:01.297856 anastruct-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39796 2023-10-30 11:38:47.000000 anastruct-1.5.0/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-10-30 11:38:47.000000 anastruct-1.5.0/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-30 11:38:47.000000 anastruct-1.5.0/tests/test_sectionbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.863482 anastruct-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35046 2024-04-01 21:01:59.000000 anastruct-1.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-01 21:01:59.000000 anastruct-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-01 21:03:03.863482 anastruct-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-04-01 21:01:59.000000 anastruct-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-01 21:01:59.000000 anastruct-1.5.1/_custom_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.851482 anastruct-1.5.1/anastruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.851482 anastruct-1.5.1/anastruct/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283215 2024-04-01 21:02:06.000000 anastruct-1.5.1/anastruct/cython/basic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/cython/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/cython/cbasic.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.851482 anastruct-1.5.1/anastruct/fem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.855482 anastruct-1.5.1/anastruct/fem/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/cython/celements.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   298328 2024-04-01 21:02:06.000000 anastruct-1.5.1/anastruct/fem/cython/elements.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/cython/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.859482 anastruct-1.5.1/anastruct/fem/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_10_dead_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_17_gnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_18_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_19_num_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_20_insert_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_21_rotate_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_22_loadcombination_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_23_sectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_24_envelope_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_25_high_midspan_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_26_deflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_6_fixed_hinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_7_rotational_spring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_8_non_linear_portal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/examples/ex_9_vertical_spring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.859482 anastruct-1.5.1/anastruct/fem/plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/plotter/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54341 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/plotter/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/plotter/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/plotter/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11752 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83321 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.859482 anastruct-1.5.1/anastruct/fem/system_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/system_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/system_components/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/system_components/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/system_components/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.859482 anastruct-1.5.1/anastruct/fem/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/fem/util/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.859482 anastruct-1.5.1/anastruct/material/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/material/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/material/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.863482 anastruct-1.5.1/anastruct/sectionbase/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/sectionbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/sectionbase/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/sectionbase/sectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/sectionbase/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-01 21:01:59.000000 anastruct-1.5.1/anastruct/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.863482 anastruct-1.5.1/anastruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-01 21:03:03.000000 anastruct-1.5.1/anastruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-01 21:03:03.000000 anastruct-1.5.1/anastruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:03:03.000000 anastruct-1.5.1/anastruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 21:03:03.000000 anastruct-1.5.1/anastruct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 21:03:03.000000 anastruct-1.5.1/anastruct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 21:01:59.000000 anastruct-1.5.1/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 21:01:59.000000 anastruct-1.5.1/plot_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-01 21:01:59.000000 anastruct-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 21:01:59.000000 anastruct-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 21:03:03.863482 anastruct-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 21:01:59.000000 anastruct-1.5.1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:03:03.863482 anastruct-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39796 2024-04-01 21:01:59.000000 anastruct-1.5.1/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-01 21:01:59.000000 anastruct-1.5.1/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-01 21:01:59.000000 anastruct-1.5.1/tests/test_sectionbase.py
```

### Comparing `anastruct-1.5.0/LICENSE.txt` & `anastruct-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/PKG-INFO` & `anastruct-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastruct
-Version: 1.5.0
+Version: 1.5.1
 Summary: Finite element analysis of 2D structures
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Maintainer-email: Brooks Smith <smith120bh@gmail.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/ritchie46/anaStruct
 Project-URL: documentation, http://anastruct.readthedocs.io
 Project-URL: author, https://ritchievink.com
@@ -20,25 +20,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.15
 Requires-Dist: scipy>=1.1.0
 Provides-Extra: plot
 Requires-Dist: matplotlib>=3.0; extra == "plot"
 Provides-Extra: test
-Requires-Dist: black[jupyter]==23.10.1; extra == "test"
-Requires-Dist: mypy==1.6.1; extra == "test"
-Requires-Dist: pylint==3.0.2; extra == "test"
-Requires-Dist: pytest==7.4.3; extra == "test"
-Requires-Dist: pytest-describe==2.1.0; extra == "test"
+Requires-Dist: black[jupyter]==24.3.0; extra == "test"
+Requires-Dist: mypy==1.9.0; extra == "test"
+Requires-Dist: pylint==3.1.0; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-describe==2.2.0; extra == "test"
 Requires-Dist: pytest-pspec==0.0.4; extra == "test"
 Requires-Dist: pytest-raises==0.11; extra == "test"
 Provides-Extra: dev
-Requires-Dist: matplotlib==3.8.0; extra == "dev"
-Requires-Dist: numpy==1.26.1; extra == "dev"
-Requires-Dist: scipy==1.11.3; extra == "dev"
+Requires-Dist: matplotlib==3.8.3; extra == "dev"
+Requires-Dist: numpy==1.26.4; extra == "dev"
+Requires-Dist: scipy==1.12.0; extra == "dev"
 
 # anaStruct 2D Frames and Trusses
 [![Python tests](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml/badge.svg)](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.org/projects/anastruct/badge/?version=latest)](http://anastruct.readthedocs.io/en/latest/?badge=latest)
 
 Analyse 2D Frames and trusses for slender structures. Determine the bending moments, shear forces, axial forces and displacements.
```

### Comparing `anastruct-1.5.0/README.md` & `anastruct-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/_custom_build.py` & `anastruct-1.5.1/_custom_build.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/basic.py` & `anastruct-1.5.1/anastruct/basic.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/cython/basic.c` & `anastruct-1.5.1/anastruct/cython/basic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.4 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "anastruct.cython.basic",
         "sources": [
             "anastruct/cython/basic.py"
@@ -32,18 +32,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_4" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030004F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -127,14 +127,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -188,14 +190,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -249,60 +253,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -385,14 +412,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -577,26 +607,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -609,15 +640,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -642,15 +672,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -728,16 +758,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -804,14 +839,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -879,27 +916,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -935,15 +972,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1079,14 +1116,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1157,15 +1203,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1260,32 +1306,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1327,15 +1356,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1568,29 +1597,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1890,15 +1924,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3181,30 +3215,28 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("basic", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to basic pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "basic" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
@@ -3599,21 +3631,39 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
+}
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
 }
 #endif
+#endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
@@ -3698,15 +3748,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -3717,15 +3767,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -3749,15 +3799,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -3920,33 +3970,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -3990,15 +4047,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -4069,17 +4126,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -4148,16 +4211,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -4168,16 +4236,21 @@
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
     self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -4234,15 +4307,15 @@
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
     if (kwargs == NULL) {
         #if CYTHON_VECTORCALL
-        #if Py_VERSION_HEX < 0x03090000
+        #if PY_VERSION_HEX < 0x03090000
         vectorcallfunc f = _PyVectorcall_Function(func);
         #else
         vectorcallfunc f = PyVectorcall_Function(func);
         #endif
         if (f) {
             return f(func, args, (size_t)nargs, NULL);
         }
@@ -4667,18 +4740,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -5654,15 +5724,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -5993,16 +6063,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -6014,14 +6084,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -6111,15 +6183,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -6209,38 +6281,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
@@ -6430,15 +6504,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -6703,15 +6777,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -6923,15 +6997,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-static unsigned long __Pyx_get_runtime_version() {
+static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
     unsigned long factor = 0x01000000UL;
     unsigned int digit = 0;
```

### Comparing `anastruct-1.5.0/anastruct/cython/basic.py` & `anastruct-1.5.1/anastruct/cython/basic.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/cython/cbasic.pyx` & `anastruct-1.5.1/anastruct/cython/cbasic.pyx`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/cython/celements.pyx` & `anastruct-1.5.1/anastruct/fem/cython/celements.pyx`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/cython/elements.c` & `anastruct-1.5.1/anastruct/fem/cython/elements.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.4 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "anastruct.fem.cython.elements",
         "sources": [
             "anastruct/fem/cython/elements.py"
@@ -32,18 +32,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_4" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030004F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -127,14 +127,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -188,14 +190,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -249,60 +253,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -385,14 +412,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -577,26 +607,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -609,15 +640,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -642,15 +672,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -728,16 +758,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -804,14 +839,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -879,27 +916,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -935,15 +972,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1079,14 +1116,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1157,15 +1203,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1260,32 +1306,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1327,15 +1356,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1568,29 +1597,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+  #endif
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -1835,15 +1869,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2533,96 +2567,88 @@
  */
   __Pyx_XDECREF(__pyx_r);
 
   /* "anastruct/fem/cython/elements.py":22
  *         -(L**3)
  *         * kl
  *         * (14 * EI * q + 16 * EI * qi + 2 * L * kr * q + 3 * L * kr * qi)             # <<<<<<<<<<<<<<
- *         / (
- *             60
- */
-  __pyx_t_1 = (((-pow(__pyx_v_L, 3.0)) * __pyx_v_kl) * (((((14.0 * __pyx_v_EI) * __pyx_v_q) + ((16.0 * __pyx_v_EI) * __pyx_v_qi)) + (((2.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_q)) + (((3.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_qi)));
-
-  /* "anastruct/fem/cython/elements.py":26
- *             60
- *             * EI
- *             * (12 * EI**2 + 4 * EI * L * kl + 4 * EI * L * kr + L**2 * kl * kr)             # <<<<<<<<<<<<<<
- *         )
+ *         / (60 * EI * (12 * EI**2 + 4 * EI * L * kl + 4 * EI * L * kr + L**2 * kl * kr))
  *         - L
  */
-  __pyx_t_2 = ((60.0 * __pyx_v_EI) * ((((12.0 * pow(__pyx_v_EI, 2.0)) + (((4.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kl)) + (((4.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kr)) + ((pow(__pyx_v_L, 2.0) * __pyx_v_kl) * __pyx_v_kr)));
+  __pyx_t_1 = (((-pow(__pyx_v_L, 3.0)) * __pyx_v_kl) * (((((14.0 * __pyx_v_EI) * __pyx_v_q) + ((16.0 * __pyx_v_EI) * __pyx_v_qi)) + (((2.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_q)) + (((3.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_qi)));
 
   /* "anastruct/fem/cython/elements.py":23
  *         * kl
  *         * (14 * EI * q + 16 * EI * qi + 2 * L * kr * q + 3 * L * kr * qi)
- *         / (             # <<<<<<<<<<<<<<
- *             60
- *             * EI
+ *         / (60 * EI * (12 * EI**2 + 4 * EI * L * kl + 4 * EI * L * kr + L**2 * kl * kr))             # <<<<<<<<<<<<<<
+ *         - L
+ *         * x
  */
+  __pyx_t_2 = ((60.0 * __pyx_v_EI) * ((((12.0 * pow(__pyx_v_EI, 2.0)) + (((4.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kl)) + (((4.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kr)) + ((pow(__pyx_v_L, 2.0) * __pyx_v_kl) * __pyx_v_kr)));
   if (unlikely(__pyx_t_2 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
     __PYX_ERR(0, 23, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":30
+  /* "anastruct/fem/cython/elements.py":26
  *         - L
  *         * x
  *         * (             # <<<<<<<<<<<<<<
  *             -2 * L * (q + 4 * qi) * (EI * kr + kl * (EI + L * kr))
  *             + 5
  */
   __pyx_t_3 = ((__pyx_v_L * __pyx_v_x) * ((((-2.0 * __pyx_v_L) * (__pyx_v_q + (4.0 * __pyx_v_qi))) * ((__pyx_v_EI * __pyx_v_kr) + (__pyx_v_kl * (__pyx_v_EI + (__pyx_v_L * __pyx_v_kr))))) + ((5.0 * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kl))) * (((((4.0 * __pyx_v_EI) * __pyx_v_q) + ((8.0 * __pyx_v_EI) * __pyx_v_qi)) + ((__pyx_v_L * __pyx_v_kr) * __pyx_v_q)) + (((3.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_qi)))));
 
-  /* "anastruct/fem/cython/elements.py":39
+  /* "anastruct/fem/cython/elements.py":35
  *             20
  *             * EI
  *             * (             # <<<<<<<<<<<<<<
  *                 2 * EI * L * kr
  *                 - 6 * EI * (2 * EI + L * kr)
  */
   __pyx_t_4 = ((20.0 * __pyx_v_EI) * ((((((2.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kr) - ((6.0 * __pyx_v_EI) * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kr)))) + (((2.0 * __pyx_v_L) * __pyx_v_kl) * (__pyx_v_EI + (__pyx_v_L * __pyx_v_kr)))) - (((3.0 * __pyx_v_L) * __pyx_v_kl) * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kr)))));
 
-  /* "anastruct/fem/cython/elements.py":36
+  /* "anastruct/fem/cython/elements.py":32
  *             * (4 * EI * q + 8 * EI * qi + L * kr * q + 3 * L * kr * qi)
  *         )
  *         / (             # <<<<<<<<<<<<<<
  *             20
  *             * EI
  */
   if (unlikely(__pyx_t_4 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 36, __pyx_L1_error)
+    __PYX_ERR(0, 32, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":46
+  /* "anastruct/fem/cython/elements.py":42
  *             )
  *         )
  *         - qi * x**2 / (2 * EI)             # <<<<<<<<<<<<<<
  *         - x**3 * (q - qi) / (6 * EI * L)
  *     )
  */
   __pyx_t_5 = (__pyx_v_qi * pow(__pyx_v_x, 2.0));
   __pyx_t_6 = (2.0 * __pyx_v_EI);
   if (unlikely(__pyx_t_6 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 46, __pyx_L1_error)
+    __PYX_ERR(0, 42, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":47
+  /* "anastruct/fem/cython/elements.py":43
  *         )
  *         - qi * x**2 / (2 * EI)
  *         - x**3 * (q - qi) / (6 * EI * L)             # <<<<<<<<<<<<<<
  *     )
  * 
  */
   __pyx_t_7 = (pow(__pyx_v_x, 3.0) * (__pyx_v_q - __pyx_v_qi));
   __pyx_t_8 = ((6.0 * __pyx_v_EI) * __pyx_v_L);
   if (unlikely(__pyx_t_8 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 47, __pyx_L1_error)
+    __PYX_ERR(0, 43, __pyx_L1_error)
   }
 
   /* "anastruct/fem/cython/elements.py":19
  *     :return: (flt)
  *     """
  *     return EI * (             # <<<<<<<<<<<<<<
  *         -(L**3)
@@ -2649,15 +2675,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "anastruct/fem/cython/elements.py":51
+/* "anastruct/fem/cython/elements.py":47
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_shear(
  *     kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
  */
 
@@ -2729,103 +2755,103 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kl)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kr)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 1); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 1); __PYX_ERR(0, 47, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_qi)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 2); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 2); __PYX_ERR(0, 47, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_q)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 3); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 3); __PYX_ERR(0, 47, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 4); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 4); __PYX_ERR(0, 47, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_EI)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 5); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 5); __PYX_ERR(0, 47, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_L)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 6); __PYX_ERR(0, 51, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, 6); __PYX_ERR(0, 47, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "det_shear") < 0)) __PYX_ERR(0, 51, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "det_shear") < 0)) __PYX_ERR(0, 47, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 7)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
       values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
       values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
     }
-    __pyx_v_kl = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_kl == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_kr = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_kr == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_qi = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_qi == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_q = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_x = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_EI = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_EI == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
-    __pyx_v_L = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_L == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L3_error)
+    __pyx_v_kl = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_kl == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_kr = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_kr == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_qi = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_qi == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_q = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_q == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_x = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_EI = __pyx_PyFloat_AsDouble(values[5]); if (unlikely((__pyx_v_EI == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_L = __pyx_PyFloat_AsDouble(values[6]); if (unlikely((__pyx_v_L == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, __pyx_nargs); __PYX_ERR(0, 51, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("det_shear", 1, 7, 7, __pyx_nargs); __PYX_ERR(0, 47, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -2858,94 +2884,94 @@
   double __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("det_shear", 1);
 
-  /* "anastruct/fem/cython/elements.py":66
+  /* "anastruct/fem/cython/elements.py":62
  *     :return: (flt)
  *     """
  *     return EI * (             # <<<<<<<<<<<<<<
  *         -L
  *         * (
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "anastruct/fem/cython/elements.py":68
+  /* "anastruct/fem/cython/elements.py":64
  *     return EI * (
  *         -L
  *         * (             # <<<<<<<<<<<<<<
  *             -2 * L * (q + 4 * qi) * (EI * kr + kl * (EI + L * kr))
  *             + 5
  */
   __pyx_t_1 = ((-__pyx_v_L) * ((((-2.0 * __pyx_v_L) * (__pyx_v_q + (4.0 * __pyx_v_qi))) * ((__pyx_v_EI * __pyx_v_kr) + (__pyx_v_kl * (__pyx_v_EI + (__pyx_v_L * __pyx_v_kr))))) + ((5.0 * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kl))) * (((((4.0 * __pyx_v_EI) * __pyx_v_q) + ((8.0 * __pyx_v_EI) * __pyx_v_qi)) + ((__pyx_v_L * __pyx_v_kr) * __pyx_v_q)) + (((3.0 * __pyx_v_L) * __pyx_v_kr) * __pyx_v_qi)))));
 
-  /* "anastruct/fem/cython/elements.py":77
+  /* "anastruct/fem/cython/elements.py":73
  *             20
  *             * EI
  *             * (             # <<<<<<<<<<<<<<
  *                 2 * EI * L * kr
  *                 - 6 * EI * (2 * EI + L * kr)
  */
   __pyx_t_2 = ((20.0 * __pyx_v_EI) * ((((((2.0 * __pyx_v_EI) * __pyx_v_L) * __pyx_v_kr) - ((6.0 * __pyx_v_EI) * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kr)))) + (((2.0 * __pyx_v_L) * __pyx_v_kl) * (__pyx_v_EI + (__pyx_v_L * __pyx_v_kr)))) - (((3.0 * __pyx_v_L) * __pyx_v_kl) * ((2.0 * __pyx_v_EI) + (__pyx_v_L * __pyx_v_kr)))));
 
-  /* "anastruct/fem/cython/elements.py":74
+  /* "anastruct/fem/cython/elements.py":70
  *             * (4 * EI * q + 8 * EI * qi + L * kr * q + 3 * L * kr * qi)
  *         )
  *         / (             # <<<<<<<<<<<<<<
  *             20
  *             * EI
  */
   if (unlikely(__pyx_t_2 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 74, __pyx_L1_error)
+    __PYX_ERR(0, 70, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":84
+  /* "anastruct/fem/cython/elements.py":80
  *             )
  *         )
  *         - qi * x / EI             # <<<<<<<<<<<<<<
  *         - x**2 * (q - qi) / (2 * EI * L)
  *     )
  */
   __pyx_t_3 = (__pyx_v_qi * __pyx_v_x);
   if (unlikely(__pyx_v_EI == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 84, __pyx_L1_error)
+    __PYX_ERR(0, 80, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":85
+  /* "anastruct/fem/cython/elements.py":81
  *         )
  *         - qi * x / EI
  *         - x**2 * (q - qi) / (2 * EI * L)             # <<<<<<<<<<<<<<
  *     )
  * 
  */
   __pyx_t_4 = (pow(__pyx_v_x, 2.0) * (__pyx_v_q - __pyx_v_qi));
   __pyx_t_5 = ((2.0 * __pyx_v_EI) * __pyx_v_L);
   if (unlikely(__pyx_t_5 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 85, __pyx_L1_error)
+    __PYX_ERR(0, 81, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":66
+  /* "anastruct/fem/cython/elements.py":62
  *     :return: (flt)
  *     """
  *     return EI * (             # <<<<<<<<<<<<<<
  *         -L
  *         * (
  */
-  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_EI * (((__pyx_t_1 / __pyx_t_2) - (__pyx_t_3 / __pyx_v_EI)) - (__pyx_t_4 / __pyx_t_5)))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble((__pyx_v_EI * (((__pyx_t_1 / __pyx_t_2) - (__pyx_t_3 / __pyx_v_EI)) - (__pyx_t_4 / __pyx_t_5)))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "anastruct/fem/cython/elements.py":51
+  /* "anastruct/fem/cython/elements.py":47
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_shear(
  *     kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
  */
 
@@ -2956,15 +2982,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "anastruct/fem/cython/elements.py":89
+/* "anastruct/fem/cython/elements.py":85
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_axial(qi: float, q: float, x: float, EA: float, L: float) -> float:
  *     """
  */
 
@@ -3030,79 +3056,79 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_qi)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_q)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 1); __PYX_ERR(0, 89, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 1); __PYX_ERR(0, 85, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 2); __PYX_ERR(0, 89, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 2); __PYX_ERR(0, 85, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_EA)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 3); __PYX_ERR(0, 89, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 3); __PYX_ERR(0, 85, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_L)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 85, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 4); __PYX_ERR(0, 89, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, 4); __PYX_ERR(0, 85, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "det_axial") < 0)) __PYX_ERR(0, 89, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "det_axial") < 0)) __PYX_ERR(0, 85, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 5)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
     }
-    __pyx_v_qi = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_qi == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_q = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_q == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_x = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_EA = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_EA == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
-    __pyx_v_L = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_L == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
+    __pyx_v_qi = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_qi == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_q = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_q == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_x = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_EA = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_EA == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
+    __pyx_v_L = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_L == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 89, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("det_axial", 1, 5, 5, __pyx_nargs); __PYX_ERR(0, 85, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -3134,72 +3160,64 @@
   double __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("det_axial", 1);
 
-  /* "anastruct/fem/cython/elements.py":100
+  /* "anastruct/fem/cython/elements.py":96
  *     :return: (flt)
  *     """
  *     return EA * (             # <<<<<<<<<<<<<<
  *         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)
- *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)
+ *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6) / (EA * L)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "anastruct/fem/cython/elements.py":101
+  /* "anastruct/fem/cython/elements.py":97
  *     """
  *     return EA * (
  *         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)             # <<<<<<<<<<<<<<
- *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)
- *         / (EA * L)
+ *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6) / (EA * L)
+ *     )
  */
   __pyx_t_1 = (__pyx_v_x * ((((-__pyx_v_L) * __pyx_v_qi) / 2.0) + ((__pyx_v_x * ((-__pyx_v_q) + __pyx_v_qi)) / 3.0)));
   __pyx_t_2 = (__pyx_v_EA * __pyx_v_L);
   if (unlikely(__pyx_t_2 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 101, __pyx_L1_error)
+    __PYX_ERR(0, 97, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":102
+  /* "anastruct/fem/cython/elements.py":98
  *     return EA * (
  *         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)
- *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)             # <<<<<<<<<<<<<<
- *         / (EA * L)
+ *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6) / (EA * L)             # <<<<<<<<<<<<<<
  *     )
  */
   __pyx_t_3 = ((((pow(__pyx_v_L, 2.0) * (__pyx_v_q + (2.0 * __pyx_v_qi))) / 6.0) - (((__pyx_v_L * __pyx_v_qi) * __pyx_v_x) / 2.0)) + ((pow(__pyx_v_x, 2.0) * ((-__pyx_v_q) + __pyx_v_qi)) / 6.0));
-
-  /* "anastruct/fem/cython/elements.py":103
- *         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)
- *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)
- *         / (EA * L)             # <<<<<<<<<<<<<<
- *     )
- */
   __pyx_t_4 = (__pyx_v_EA * __pyx_v_L);
   if (unlikely(__pyx_t_4 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 103, __pyx_L1_error)
+    __PYX_ERR(0, 98, __pyx_L1_error)
   }
 
-  /* "anastruct/fem/cython/elements.py":100
+  /* "anastruct/fem/cython/elements.py":96
  *     :return: (flt)
  *     """
  *     return EA * (             # <<<<<<<<<<<<<<
  *         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)
- *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)
+ *         + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6) / (EA * L)
  */
-  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_EA * ((__pyx_t_1 / __pyx_t_2) + (__pyx_t_3 / __pyx_t_4)))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble((__pyx_v_EA * ((__pyx_t_1 / __pyx_t_2) + (__pyx_t_3 / __pyx_t_4)))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "anastruct/fem/cython/elements.py":89
+  /* "anastruct/fem/cython/elements.py":85
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_axial(qi: float, q: float, x: float, EA: float, L: float) -> float:
  *     """
  */
 
@@ -3281,34 +3299,34 @@
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
   __pyx_tuple__3 = PyTuple_Pack(7, __pyx_n_s_kl, __pyx_n_s_kr, __pyx_n_s_qi, __pyx_n_s_q, __pyx_n_s_x, __pyx_n_s_EI, __pyx_n_s_L); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
   __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_anastruct_fem_cython_elements_py, __pyx_n_s_det_moment, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 4, __pyx_L1_error)
 
-  /* "anastruct/fem/cython/elements.py":51
+  /* "anastruct/fem/cython/elements.py":47
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_shear(
  *     kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
  */
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_anastruct_fem_cython_elements_py, __pyx_n_s_det_shear, 51, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_anastruct_fem_cython_elements_py, __pyx_n_s_det_shear, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 47, __pyx_L1_error)
 
-  /* "anastruct/fem/cython/elements.py":89
+  /* "anastruct/fem/cython/elements.py":85
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_axial(qi: float, q: float, x: float, EA: float, L: float) -> float:
  *     """
  */
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_qi, __pyx_n_s_q, __pyx_n_s_x, __pyx_n_s_EA, __pyx_n_s_L); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_qi, __pyx_n_s_q, __pyx_n_s_x, __pyx_n_s_EA, __pyx_n_s_L); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_anastruct_fem_cython_elements_py, __pyx_n_s_det_axial, 89, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_anastruct_fem_cython_elements_py, __pyx_n_s_det_axial, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -3577,30 +3595,28 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("elements", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to elements pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "elements" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
@@ -3721,76 +3737,76 @@
   __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_det_moment, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "anastruct/fem/cython/elements.py":51
+  /* "anastruct/fem/cython/elements.py":47
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_shear(
  *     kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_lru_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_lru_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kl, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kr, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_qi, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_q, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_EI, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_L, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9anastruct_3fem_6cython_8elements_3det_shear, 0, __pyx_n_s_det_shear, NULL, __pyx_n_s_anastruct_fem_cython_elements, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kl, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kr, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_qi, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_q, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_EI, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_L, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9anastruct_3fem_6cython_8elements_3det_shear, 0, __pyx_n_s_det_shear, NULL, __pyx_n_s_anastruct_fem_cython_elements, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_det_shear, __pyx_t_3) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_det_shear, __pyx_t_3) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "anastruct/fem/cython/elements.py":89
+  /* "anastruct/fem/cython/elements.py":85
  * 
  * 
  * @lru_cache(32000)             # <<<<<<<<<<<<<<
  * def det_axial(qi: float, q: float, x: float, EA: float, L: float) -> float:
  *     """
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_lru_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_lru_cache); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_qi, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_q, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_EA, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_L, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9anastruct_3fem_6cython_8elements_5det_axial, 0, __pyx_n_s_det_axial, NULL, __pyx_n_s_anastruct_fem_cython_elements, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_qi, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_q, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_x, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_EA, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_L, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_9anastruct_3fem_6cython_8elements_5det_axial, 0, __pyx_n_s_det_axial, NULL, __pyx_n_s_anastruct_fem_cython_elements, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_det_axial, __pyx_t_3) < 0) __PYX_ERR(0, 89, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_det_axial, __pyx_t_3) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "anastruct/fem/cython/elements.py":1
  * from functools import lru_cache             # <<<<<<<<<<<<<<
  * 
  * 
  */
@@ -4064,20 +4080,38 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
+}
+#endif
 #endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
@@ -4163,15 +4197,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -4182,15 +4216,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -4214,15 +4248,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -4486,33 +4520,40 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 #endif
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -4556,15 +4597,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -4597,16 +4638,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -4685,18 +4731,15 @@
 #endif
     return 0;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -5672,15 +5715,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -5908,17 +5951,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -5987,16 +6036,21 @@
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
     self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -6053,15 +6107,15 @@
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
     if (kwargs == NULL) {
         #if CYTHON_VECTORCALL
-        #if Py_VERSION_HEX < 0x03090000
+        #if PY_VERSION_HEX < 0x03090000
         vectorcallfunc f = _PyVectorcall_Function(func);
         #else
         vectorcallfunc f = PyVectorcall_Function(func);
         #endif
         if (f) {
             return f(func, args, (size_t)nargs, NULL);
         }
@@ -6232,16 +6286,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -6253,14 +6307,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -6350,15 +6406,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -6448,38 +6504,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
@@ -6669,15 +6727,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -6942,15 +7000,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -7162,15 +7220,15 @@
         return __Pyx_inner_PyErr_GivenExceptionMatches2(err, exc_type1, exc_type2);
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
-static unsigned long __Pyx_get_runtime_version() {
+static unsigned long __Pyx_get_runtime_version(void) {
 #if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
     return Py_Version & ~0xFFUL;
 #else
     const char* rt_version = Py_GetVersion();
     unsigned long version = 0;
     unsigned long factor = 0x01000000UL;
     unsigned int digit = 0;
```

### Comparing `anastruct-1.5.0/anastruct/fem/cython/elements.py` & `anastruct-1.5.1/anastruct/fem/cython/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,15 @@
     :param L: (flt) Length of the beam
     :return: (flt)
     """
     return EI * (
         -(L**3)
         * kl
         * (14 * EI * q + 16 * EI * qi + 2 * L * kr * q + 3 * L * kr * qi)
-        / (
-            60
-            * EI
-            * (12 * EI**2 + 4 * EI * L * kl + 4 * EI * L * kr + L**2 * kl * kr)
-        )
+        / (60 * EI * (12 * EI**2 + 4 * EI * L * kl + 4 * EI * L * kr + L**2 * kl * kr))
         - L
         * x
         * (
             -2 * L * (q + 4 * qi) * (EI * kr + kl * (EI + L * kr))
             + 5
             * (2 * EI + L * kl)
             * (4 * EI * q + 8 * EI * qi + L * kr * q + 3 * L * kr * qi)
@@ -95,10 +91,9 @@
     :param x: (flt) Location of the axial force
     :param EA: (flt)
     :param L: (flt) Length of the beam
     :return: (flt)
     """
     return EA * (
         x * (-L * qi / 2 + x * (-q + qi) / 3) / (EA * L)
-        + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6)
-        / (EA * L)
+        + (L**2 * (q + 2 * qi) / 6 - L * qi * x / 2 + x**2 * (-q + qi) / 6) / (EA * L)
     )
```

### Comparing `anastruct-1.5.0/anastruct/fem/elements.py` & `anastruct-1.5.1/anastruct/fem/elements.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/examples/ex_1_2.py` & `anastruct-1.5.1/anastruct/fem/examples/ex_1_2.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/examples/ex_2.py` & `anastruct-1.5.1/anastruct/fem/examples/ex_2.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/examples/ex_22_loadcombination_doc.py` & `anastruct-1.5.1/anastruct/fem/examples/ex_22_loadcombination_doc.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/examples/ex_3.py` & `anastruct-1.5.1/anastruct/fem/examples/ex_3.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/examples/ex_8_non_linear_portal.py` & `anastruct-1.5.1/anastruct/fem/examples/ex_8_non_linear_portal.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/node.py` & `anastruct-1.5.1/anastruct/fem/node.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/plotter/element.py` & `anastruct-1.5.1/anastruct/fem/plotter/element.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/plotter/mpl.py` & `anastruct-1.5.1/anastruct/fem/plotter/mpl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
-from typing import TYPE_CHECKING, List, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple
 
+import matplotlib.colors
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 
 from anastruct.basic import find_nearest, rotate_xy
 from anastruct.fem.plotter.values import (
     PlottingValues,
@@ -40,14 +41,58 @@
         self.system: "SystemElements" = system
         self.axes: List["Axes"] = []
         self.one_fig: Optional["Axes"] = None
         self.max_q: float = 0
         self.max_qn: float = 0
         self.max_system_point_load: float = 0
         self.fig: Optional["Figure"] = None
+        self.plot_colors: Dict[str, str] = {
+            "support": "r",
+            "element": "k",
+            "node_number": "k",
+            "element_number": "k",
+            "displaced_elem": "C0",
+            "point_load_fill": "orange",
+            "point_load_edge": "b",
+            "point_load_text": "k",
+            "q_load": "g",
+            "q_load_arrow_face": "k",
+            "q_load_arrow_edge": "k",
+            "q_load_text": "b",
+            "moment_load": "orange",
+            "moment_load_text": "k",
+            "reaction_force_arrow_edge": "orange",
+            "reaction_force_arrow_fill": "b",
+            "reaction_force_text": "b",
+            "axial_force_neg": "C0",
+            "axial_force_pos": "C1",
+            "axial_force_sign": "b",
+            "bending_moment": "C0",
+            "shear_force": "C0",
+            "annotation": "b",
+        }
+
+    def change_plot_colors(self, colors: Dict) -> None:
+        """Changes the plotting color for various components of the plot.
+
+        Args:
+            colors (Dict): A dictionary containing plot components and colors
+            as key-value pairs.
+        """
+        for item, color in colors.items():
+            if not isinstance(color, str) or not isinstance(item, str):
+                print("Plot components and colors must be passed in as strings")
+            elif self.plot_colors.get(item) is None:
+                print(
+                    str(item) + " is not a valid plot component to change the color of"
+                )
+            elif not matplotlib.colors.is_color_like(color):
+                print(str(color + "is not a valid matplotlib color"))
+            else:
+                self.plot_colors[item] = color
 
     @property
     def max_val_structure(self) -> float:
         """Returns the maximum value of the structure.
 
         Returns:
             float: Maximum value of the structure
@@ -80,15 +125,15 @@
         """
         width = height = PATCH_SIZE * max_val
         for node in self.system.supports_fixed:
             support_patch = mpatches.Rectangle(
                 (node.vertex.x - width * 0.5, node.vertex.y - width * 0.5),
                 width,
                 height,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=9,
             )
             self.axes[axes_i].add_patch(support_patch)
 
     def __hinged_support_patch(self, max_val: float, axes_i: int = 0) -> None:
         """Plots the hinged supports.
 
@@ -98,15 +143,15 @@
         """
         radius = PATCH_SIZE * max_val
         for node in self.system.supports_hinged:
             support_patch = mpatches.RegularPolygon(
                 (node.vertex.x, node.vertex.y - radius),
                 numVertices=3,
                 radius=radius,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=9,
             )
             self.axes[axes_i].add_patch(support_patch)
 
     def __rotational_support_patch(self, max_val: float, axes_i: int = 0) -> None:
         """Plots the rotational supports.
 
@@ -116,15 +161,15 @@
         """
         width = height = PATCH_SIZE * max_val
         for node in self.system.supports_rotational:
             support_patch = mpatches.Rectangle(
                 (node.vertex.x - width * 0.5, node.vertex.y - width * 0.5),
                 width,
                 height,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=9,
                 fill=False,
             )
             self.axes[axes_i].add_patch(support_patch)
 
     def __roll_support_patch(self, max_val: float, axes_i: int = 0) -> None:
         """Plots the roller supports.
@@ -150,74 +195,80 @@
             z3 = np.sin(np.radians(270)) * radius + node.vertex.y  # vertex.y - radius
 
             triangle = np.array([[x1, z1], [x2, z2], [x3, z3]])
 
             if node.id in self.system.inclined_roll:
                 angle = self.system.inclined_roll[node.id]
                 triangle = rotate_xy(triangle, angle + np.pi * 0.5)
-                support_patch_poly = mpatches.Polygon(triangle, color="r", zorder=9)
+                support_patch_poly = mpatches.Polygon(
+                    triangle, color=self.plot_colors["support"], zorder=9
+                )
                 self.axes[axes_i].add_patch(support_patch_poly)
                 self.axes[axes_i].plot(
                     triangle[1:, 0] - 0.5 * radius * np.sin(angle),
                     triangle[1:, 1] - 0.5 * radius * np.cos(angle),
-                    color="r",
+                    color=self.plot_colors["support"],
                 )
                 if not rotate:
                     rect_patch_regpoly = mpatches.RegularPolygon(
                         (node.vertex.x, radius - node.vertex.y),
                         numVertices=4,
                         radius=radius,
                         orientation=angle,
-                        color="r",
+                        color=self.plot_colors["support"],
                         zorder=9,
                         fill=False,
                     )
                     self.axes[axes_i].add_patch(rect_patch_regpoly)
 
             elif direction == 2:  # horizontal roll
                 support_patch_regpoly = mpatches.RegularPolygon(
                     (node.vertex.x, node.vertex.y - radius),
                     numVertices=3,
                     radius=radius,
-                    color="r",
+                    color=self.plot_colors["support"],
                     zorder=9,
                 )
                 self.axes[axes_i].add_patch(support_patch_regpoly)
                 y = node.vertex.y - 2 * radius
                 self.axes[axes_i].plot(
-                    [node.vertex.x - radius, node.vertex.x + radius], [y, y], color="r"
+                    [node.vertex.x - radius, node.vertex.x + radius],
+                    [y, y],
+                    color=self.plot_colors["support"],
                 )
                 if not rotate:
                     rect_patch_rect = mpatches.Rectangle(
                         (node.vertex.x - radius / 2, node.vertex.y - radius / 2),
                         radius,
                         radius,
-                        color="r",
+                        color=self.plot_colors["support"],
                         zorder=9,
                         fill=False,
                     )
                     self.axes[axes_i].add_patch(rect_patch_rect)
             elif direction == 1:  # vertical roll
                 # translate the support to the node
 
-                support_patch_poly = mpatches.Polygon(triangle, color="r", zorder=9)
+                support_patch_poly = mpatches.Polygon(
+                    triangle, color=self.plot_colors["support"], zorder=9
+                )
                 self.axes[axes_i].add_patch(support_patch_poly)
 
                 y = node.vertex.y - radius
                 self.axes[axes_i].plot(
                     [node.vertex.x + radius * 1.5, node.vertex.x + radius * 1.5],
                     [y, y + 2 * radius],
-                    color="r",
+                    color=self.plot_colors["support"],
                 )
                 if not rotate:
                     rect_patch_rect = mpatches.Rectangle(
                         (node.vertex.x - radius / 2, node.vertex.y - radius / 2),
                         radius,
                         radius,
-                        color="r",
+                        color=self.plot_colors["support"],
                         zorder=9,
                         fill=False,
                     )
                     self.axes[axes_i].add_patch(rect_patch_rect)
             count += 1
 
     def __rotating_spring_support_patch(self, max_val: float, axes_i: int = 0) -> None:
@@ -230,22 +281,22 @@
         radius = PATCH_SIZE * max_val
 
         for node, _ in self.system.supports_spring_z:
             r = np.arange(0, radius, 0.001)
             theta = 25 * np.pi * r / (0.2 * max_val)
             x = np.cos(theta) * r + node.vertex.x
             y = np.sin(theta) * r - radius + node.vertex.y
-            self.axes[axes_i].plot(x, y, color="r", zorder=9)
+            self.axes[axes_i].plot(x, y, color=self.plot_colors["support"], zorder=9)
 
             # Triangle
             support_patch = mpatches.RegularPolygon(
                 (node.vertex.x, node.vertex.y - radius * 3),
                 numVertices=3,
                 radius=radius * 0.9,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=9,
             )
             self.axes[axes_i].add_patch(support_patch)
 
     def __spring_support_patch(self, max_val: float, axes_i: int = 0) -> None:
         """Plots the linear spring supports.
 
@@ -260,40 +311,44 @@
 
         for node, _ in self.system.supports_spring_y:
             yval = np.arange(0, -9, -1) * dh + node.vertex.y
             xval = (
                 np.array([0, 0, left, right, left, right, left, 0, 0]) + node.vertex.x
             )
 
-            self.axes[axes_i].plot(xval, yval, color="r", zorder=10)
+            self.axes[axes_i].plot(
+                xval, yval, color=self.plot_colors["support"], zorder=10
+            )
 
             # Triangle
             support_patch = mpatches.RegularPolygon(
                 (node.vertex.x, node.vertex.y - h * 2.6),
                 numVertices=3,
                 radius=h * 0.9,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=10,
             )
             self.axes[axes_i].add_patch(support_patch)
 
         for node, _ in self.system.supports_spring_x:
             xval = np.arange(0, 9, 1) * dh + node.vertex.x
             yval = (
                 np.array([0, 0, left, right, left, right, left, 0, 0]) + node.vertex.y
             )
 
-            self.axes[axes_i].plot(xval, yval, color="r", zorder=10)
+            self.axes[axes_i].plot(
+                xval, yval, color=self.plot_colors["support"], zorder=10
+            )
 
             # Triangle
             support_patch = mpatches.RegularPolygon(
                 (node.vertex.x + h * 1.7, node.vertex.y - h),
                 numVertices=3,
                 radius=h * 0.9,
-                color="r",
+                color=self.plot_colors["support"],
                 zorder=10,
             )
             self.axes[axes_i].add_patch(support_patch)
 
     def __q_load_patch(self, max_val: float, verbosity: int, axes_i: int = 0) -> None:
         """Plots the distributed loads.
 
@@ -338,16 +393,18 @@
             """
             # - value, because the positive y of the system is opposite of positive y of the plotter
             xn1 = x1 + np.sin(ai) * h1 * direction
             yn1 = y1 + np.cos(ai) * h1 * direction
             xn2 = x2 + np.sin(ai) * h2 * direction
             yn2 = y2 + np.cos(ai) * h2 * direction
             coordinates = ([x1, xn1, xn2, x2], [y1, yn1, yn2, y2])
-            self.axes[axes_i].plot(*coordinates, color="g")
-            rec = mpatches.Polygon(np.vstack(coordinates).T, color="g", alpha=0.3)
+            self.axes[axes_i].plot(*coordinates, color=self.plot_colors["q_load"])
+            rec = mpatches.Polygon(
+                np.vstack(coordinates).T, color=self.plot_colors["q_load"], alpha=0.3
+            )
             self.axes[axes_i].add_patch(rec)
 
             if verbosity == 0:
                 # arrow
                 # pos = np.sqrt(((y1 - y2) ** 2) + ((x1 - x2) ** 2))
                 # cg = ((pos / 3) * (qi + 2 * q)) / (qi + q)
                 # height = math.sin(el_angle) * cg
@@ -360,18 +417,28 @@
                 step_x = np.linspace(xn1, xn2, 11)
                 step_y = np.linspace(yn1, yn2, 11)
                 step_len_x = np.linspace(len_x1, len_x2, 11)
                 step_len_y = np.linspace(len_y1, len_y2, 11)
                 average_h = (h1 + h2) / 2
                 # fc = face color, ec = edge color
                 self.axes[axes_i].text(
-                    xn1, yn1, f"q={qi}", color="b", fontsize=9, zorder=10
+                    xn1,
+                    yn1,
+                    f"q={qi}",
+                    color=self.plot_colors["q_load_text"],
+                    fontsize=9,
+                    zorder=10,
                 )
                 self.axes[axes_i].text(
-                    xn2, yn2, f"q={q}", color="b", fontsize=9, zorder=10
+                    xn2,
+                    yn2,
+                    f"q={q}",
+                    color=self.plot_colors["q_load_text"],
+                    fontsize=9,
+                    zorder=10,
                 )
 
                 # add multiple arrows to fill load
                 for counter, step_xi in enumerate(step_x):
                     if q + qi >= 0:
                         if counter == 0:
                             shape = "right"
@@ -391,16 +458,16 @@
                         step_xi,
                         step_y[counter],
                         step_len_x[counter],
                         step_len_y[counter],
                         head_width=average_h * 0.25,
                         head_length=0.4
                         * np.sqrt(step_len_y[counter] ** 2 + step_len_x[counter] ** 2),
-                        ec="k",
-                        fc="k",
+                        ec=self.plot_colors["q_load_arrow_edge"],
+                        fc=self.plot_colors["q_load_arrow_face"],
                         shape=shape,
                     )
 
         for q_id in self.system.loads_q.keys():
             el = self.system.element_map[q_id]
             qi = el.q_load[0]
             q = el.q_load[1]
@@ -489,20 +556,27 @@
             self.axes[axes_i].arrow(
                 x,
                 y,
                 len_x,
                 len_y,
                 head_width=h * 0.15,
                 head_length=0.2 * h,
-                ec="b",
-                fc="orange",
+                ec=self.plot_colors["point_load_edge"],
+                fc=self.plot_colors["point_load_fill"],
                 zorder=11,
             )
             if verbosity == 0:
-                self.axes[axes_i].text(x, y, f"F={F}", color="k", fontsize=9, zorder=10)
+                self.axes[axes_i].text(
+                    x,
+                    y,
+                    f"F={F}",
+                    color=self.plot_colors["point_load_text"],
+                    fontsize=9,
+                    zorder=10,
+                )
 
     def __moment_load_patch(self, max_val: float, axes_i: int = 0) -> None:
         """Plots the moment loads.
 
         Args:
             max_val (float): Max scale of the plot
             axes_i (int, optional): Which set of axes to plot on (for multi-plot windows). Defaults to 0.
@@ -512,29 +586,29 @@
             node = self.system.node_map[k]
             if v > 0:
                 self.axes[axes_i].plot(
                     node.vertex.x,
                     node.vertex.y,
                     marker=r"$\circlearrowleft$",
                     ms=25,
-                    color="orange",
+                    color=self.plot_colors["moment_load"],
                 )
             else:
                 self.axes[axes_i].plot(
                     node.vertex.x,
                     node.vertex.y,
                     marker=r"$\circlearrowright$",
                     ms=25,
-                    color="orange",
+                    color=self.plot_colors["moment_load"],
                 )
             self.axes[axes_i].text(
                 node.vertex.x + h * 0.2,
                 node.vertex.y + h * 0.2,
                 f"T={v}",
-                color="k",
+                color=self.plot_colors["moment_load_text"],
                 fontsize=9,
                 zorder=10,
             )
 
     def plot_structure(
         self,
         figsize: Optional[Tuple[float, float]],
@@ -586,55 +660,62 @@
         minxrange = center_x - ax_range
         minyrange = center_y - ax_range * figsize[1] / figsize[0]
 
         self.axes[axes_i].axis((minxrange, plusxrange, minyrange, plusyrange))
 
         for el in self.system.element_map.values():
             x_val, y_val = plot_values_element(el)
-            self.axes[axes_i].plot(x_val, y_val, color="black", marker="s")
+            self.axes[axes_i].plot(
+                x_val, y_val, color=self.plot_colors["element"], marker="s"
+            )
 
             if verbosity == 0:
                 # add node ID to plot
                 ax_range = max_plot_range * 0.015
                 self.axes[axes_i].text(
                     x_val[0] + ax_range,
                     y_val[0] + ax_range,
                     f"{el.node_id1}",
-                    color="g",
+                    color=self.plot_colors["node_number"],
                     fontsize=9,
                     zorder=10,
                 )
                 self.axes[axes_i].text(
                     x_val[-1] + ax_range,
                     y_val[-1] + ax_range,
                     f"{el.node_id2}",
-                    color="g",
+                    color=self.plot_colors["node_number"],
                     fontsize=9,
                     zorder=10,
                 )
 
                 # add element ID to plot
                 factor = 0.02 * self.max_val_structure
                 x_scalar = (x_val[0] + x_val[-1]) / 2 - np.sin(el.angle) * factor
                 y_scalar = (y_val[0] + y_val[-1]) / 2 + np.cos(el.angle) * factor
 
                 self.axes[axes_i].text(
-                    x_scalar, y_scalar, str(el.id), color="r", fontsize=9, zorder=10
+                    x_scalar,
+                    y_scalar,
+                    str(el.id),
+                    color=self.plot_colors["element_number"],
+                    fontsize=9,
+                    zorder=10,
                 )
 
                 # add element annotation to plot
                 # TO DO: check how this holds with multiple structure scales.
                 if annotations:
                     x_scalar += +np.sin(el.angle) * factor * 2.3
                     y_scalar += -np.cos(el.angle) * factor * 2.3
                     self.axes[axes_i].text(
                         x_scalar,
                         y_scalar,
                         el.section_name,
-                        color="b",
+                        color=self.plot_colors["annotation"],
                         fontsize=9,
                         zorder=10,
                     )
 
         # add supports
         if supports:
             self.__fixed_support_patch(max_plot_range * scale)
@@ -726,15 +807,15 @@
         self,
         axis_values: Sequence,
         force_1: Optional[float] = None,
         force_2: Optional[float] = None,
         digits: int = 2,
         node_results: bool = True,
         fill_polygon: bool = True,
-        color: int = 0,
+        color: str = "b",
         axes_i: int = 0,
     ) -> None:
         """Plots a single result on the structure.
 
         Args:
             axis_values (Sequence): X and Y values
             force_1 (Optional[float], optional): First force to plot. Defaults to None.
@@ -742,30 +823,28 @@
             digits (int, optional): Number of digits to round to. Defaults to 2.
             node_results (bool, optional): Whether or not to plot nodal results. Defaults to True.
             fill_polygon (bool, optional): Whether or not to fill a polygon for the result. Defaults to True.
             color (int, optional): Color index with which to draw. Defaults to 0.
             axes_i (int, optional): Which set of axes to plot on (for multi-plot windows). Defaults to 0.
         """
         if fill_polygon:
-            rec = mpatches.Polygon(
-                np.vstack(axis_values).T, color=f"C{color}", alpha=0.3
-            )
+            rec = mpatches.Polygon(np.vstack(axis_values).T, color=color, alpha=0.3)
             self.axes[axes_i].add_patch(rec)
         # plot force
         x_val = axis_values[0]
         y_val = axis_values[1]
 
-        self.axes[axes_i].plot(x_val, y_val, color=f"C{color}")
+        self.axes[axes_i].plot(x_val, y_val, color=color)
 
         if node_results and force_1 and force_2:
             self._add_node_values(x_val, y_val, force_1, force_2, digits)
 
     def plot(self) -> None:
         """Plots the figure."""
-        plt.show()  # type: ignore
+        plt.show()
 
     def axial_force(
         self,
         factor: Optional[float] = None,
         figsize: Optional[Tuple[float, float]] = None,
         verbosity: int = 0,
         scale: float = 1,
@@ -815,15 +894,19 @@
                 math.isclose(el.N_1, 0, rel_tol=1e-5, abs_tol=1e-9)
                 and math.isclose(el.N_2, 0, rel_tol=1e-5, abs_tol=1e-9)
                 and math.isclose(el.all_qn_load[0], 0, rel_tol=1e-5, abs_tol=1e-9)
                 and math.isclose(el.all_qn_load[1], 0, rel_tol=1e-5, abs_tol=1e-9)
             ):
                 continue
             axis_values = plot_values_axial_force(el, factor, con)
-            color = 1 if el.N_1 < 0 else 0
+            color = (
+                self.plot_colors["axial_force_neg"]
+                if el.N_1 < 0
+                else self.plot_colors["axial_force_pos"]
+            )
             self.plot_result(
                 axis_values,
                 el.N_1,
                 el.N_2,
                 node_results=not bool(verbosity),
                 color=color,
                 axes_i=axes_i,
@@ -841,15 +924,15 @@
                     self.axes[axes_i].text(
                         point.x,
                         point.y,
                         "-",
                         ha="center",
                         va="center",
                         fontsize=20,
-                        color="b",
+                        color=self.plot_colors["axial_force_sign"],
                     )
             if el.N_1 > 0:
                 point.displace_polar(
                     alpha=el.angle + 0.5 * np.pi,
                     radius=0.5 * el.N_1 * factor,
                     inverse_y_axis=True,
                 )
@@ -858,15 +941,15 @@
                     self.axes[axes_i].text(
                         point.x,
                         point.y,
                         "+",
                         ha="center",
                         va="center",
                         fontsize=14,
-                        color="b",
+                        color=self.plot_colors["axial_force_sign"],
                     )
 
         if show:
             self.plot()
             return None
         return self.fig
 
@@ -901,21 +984,25 @@
         )
         assert self.system.element_map[1].bending_moment is not None
         con = len(self.system.element_map[1].bending_moment)
         if factor is None:
             # maximum moment determined by comparing the node's moments and the sagging moments.
             max_moment = max(
                 map(
-                    lambda el: max(
-                        abs(el.node_1.Tz),
-                        abs(el.node_2.Tz),
-                        abs(((el.all_qp_load[0] + el.all_qp_load[1]) / 16) * el.l**2),
-                    )
-                    if el.type == "general"
-                    else 0,
+                    lambda el: (
+                        max(
+                            abs(el.node_1.Tz),
+                            abs(el.node_2.Tz),
+                            abs(
+                                ((el.all_qp_load[0] + el.all_qp_load[1]) / 16) * el.l**2
+                            ),
+                        )
+                        if el.type == "general"
+                        else 0
+                    ),
                     self.system.element_map.values(),
                 )
             )
             factor = det_scaling_factor(max_moment, self.max_val_structure)
 
         # determine the axis values
         for el in self.system.element_map.values():
@@ -930,14 +1017,15 @@
             axis_values = plot_values_bending_moment(el, factor, con)
             node_results = verbosity == 0
             self.plot_result(
                 axis_values,
                 abs(el.node_1.Tz),
                 abs(el.node_2.Tz),
                 node_results=node_results,
+                color=self.plot_colors["bending_moment"],
                 axes_i=axes_i,
             )
 
             if el.all_qp_load:
                 assert el.bending_moment is not None
                 m_sag = min(el.bending_moment)
                 index = find_nearest(el.bending_moment, m_sag)[1]
@@ -983,17 +1071,19 @@
         if include_structure:
             self.plot_structure(
                 figsize, 1, scale=scale, offset=offset, gridplot=gridplot, axes_i=axes_i
             )
         if factor is None:
             max_force = max(
                 map(
-                    lambda el: np.max(np.abs(el.shear_force))
-                    if el.shear_force is not None
-                    else 0.0,
+                    lambda el: (
+                        np.max(np.abs(el.shear_force))
+                        if el.shear_force is not None
+                        else 0.0
+                    ),
                     self.system.element_map.values(),
                 )
             )
             factor = det_scaling_factor(max_force, self.max_val_structure)
 
         for el in self.system.element_map.values():
             if (
@@ -1011,14 +1101,15 @@
             shear_2 = el.shear_force[-1]
 
             self.plot_result(
                 axis_values,
                 shear_1,
                 shear_2,
                 node_results=not bool(verbosity),
+                color=self.plot_colors["shear_force"],
                 axes_i=axes_i,
             )
         if show:
             self.plot()
             return None
         return self.fig
 
@@ -1077,25 +1168,25 @@
                 self.axes[axes_i].arrow(
                     x,
                     y,
                     len_x,
                     len_y,
                     head_width=h * 0.15,
                     head_length=0.2 * scale,
-                    ec="b",
-                    fc="orange",
+                    ec=self.plot_colors["reaction_force_arrow_edge"],
+                    fc=self.plot_colors["reaction_force_arrow_fill"],
                     zorder=11,
                 )
 
                 if verbosity == 0:
                     self.axes[axes_i].text(
                         x,
                         y,
                         f"R={round(node.Fx, 2)}",
-                        color="k",
+                        color=self.plot_colors["reaction_force_text"],
                         fontsize=9,
                         zorder=10,
                     )
 
             if not math.isclose(node.Fy, 0, rel_tol=1e-5, abs_tol=1e-9):
                 # y direction
                 scale = abs(node.Fy) / max_force * h
@@ -1108,54 +1199,54 @@
                 self.axes[axes_i].arrow(
                     x,
                     y,
                     len_x,
                     len_y,
                     head_width=h * 0.15,
                     head_length=0.2 * scale,
-                    ec="b",
-                    fc="orange",
+                    ec=self.plot_colors["reaction_force_arrow_edge"],
+                    fc=self.plot_colors["reaction_force_arrow_fill"],
                     zorder=11,
                 )
 
                 if verbosity == 0:
                     self.axes[axes_i].text(
                         x,
                         y,
                         f"R={round(node.Fy, 2)}",
-                        color="k",
+                        color=self.plot_colors["reaction_force_text"],
                         fontsize=9,
                         zorder=10,
                     )
 
             if not math.isclose(node.Tz, 0, rel_tol=1e-5, abs_tol=1e-9):
                 # '$...$': render the strings using mathtext
                 if node.Tz > 0:
                     self.axes[axes_i].plot(
                         node.vertex.x,
                         node.vertex.y,
                         marker=r"$\circlearrowleft$",
                         ms=25,
-                        color="orange",
+                        color=self.plot_colors["reaction_force_arrow_fill"],
                     )
                 if node.Tz < 0:
                     self.axes[axes_i].plot(
                         node.vertex.x,
                         node.vertex.y,
                         marker=r"$\circlearrowright$",
                         ms=25,
-                        color="orange",
+                        color=self.plot_colors["reaction_force_arrow_fill"],
                     )
 
                 if verbosity == 0:
                     self.axes[axes_i].text(
                         node.vertex.x + h * 0.2,
                         node.vertex.y + h * 0.2,
                         f"T={round(node.Tz, 2)}",
-                        color="k",
+                        color=self.plot_colors["reaction_force_text"],
                         fontsize=9,
                         zorder=10,
                     )
         if show:
             self.plot()
             return None
         return self.fig
@@ -1191,32 +1282,35 @@
         self.plot_structure(
             figsize, 1, scale=scale, offset=offset, gridplot=gridplot, axes_i=axes_i
         )
         if factor is None:
             # needed to determine the scaling factor
             max_displacement = max(
                 map(
-                    lambda el: max(
-                        abs(el.node_1.ux),
-                        abs(el.node_1.uy),
-                        el.max_deflection or 0,
-                    )
-                    if el.type == "general"
-                    else 0,
+                    lambda el: (
+                        max(
+                            abs(el.node_1.ux),
+                            abs(el.node_1.uy),
+                            el.max_deflection or 0,
+                        )
+                        if el.type == "general"
+                        else 0
+                    ),
                     self.system.element_map.values(),
                 )
             )
             factor = det_scaling_factor(max_displacement, self.max_val_structure)
 
         for el in self.system.element_map.values():
             axis_values = plot_values_deflection(el, factor, linear)
             self.plot_result(
                 axis_values,
                 node_results=False,
                 fill_polygon=False,
+                color=self.plot_colors["displaced_elem"],
                 axes_i=axes_i,
             )
 
             if el.type == "general":
                 assert el.deflection is not None
                 # index of the max deflection
                 x = np.linspace(el.vertex_1.x, el.vertex_2.x, el.deflection.size)
```

### Comparing `anastruct-1.5.0/anastruct/fem/plotter/null.py` & `anastruct-1.5.1/anastruct/fem/plotter/null.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/plotter/values.py` & `anastruct-1.5.1/anastruct/fem/plotter/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,19 +75,21 @@
         Returns:
             Tuple[np.ndarray, np.ndarray]: x and y values
         """
         if factor is None:
             # needed to determine the scaling factor
             max_displacement = max(
                 map(
-                    lambda el: max(
-                        abs(el.node_1.ux), abs(el.node_1.uy), el.max_deflection or 0
-                    )
-                    if el.type == "general"
-                    else 0,
+                    lambda el: (
+                        max(
+                            abs(el.node_1.ux), abs(el.node_1.uy), el.max_deflection or 0
+                        )
+                        if el.type == "general"
+                        else 0
+                    ),
                     self.system.element_map.values(),
                 )
             )
             factor = det_scaling_factor(max_displacement, self.max_val_structure)
         xy = np.hstack(
             [
                 plot_values_deflection(el, factor, linear)
```

### Comparing `anastruct-1.5.0/anastruct/fem/postprocess.py` & `anastruct-1.5.1/anastruct/fem/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,32 +113,38 @@
         # Global coordinates system
         element.node_map[element.node_id1] = Node(
             id=element.node_id1,
             Fx=element.element_force_vector[0]
             + element.element_primary_force_vector[0],
             Fy=element.element_force_vector[1]
             + element.element_primary_force_vector[1],
-            Tz=element.element_force_vector[2] + element.element_primary_force_vector[2]
-            if not hinge1
-            else 0,
+            Tz=(
+                element.element_force_vector[2]
+                + element.element_primary_force_vector[2]
+                if not hinge1
+                else 0
+            ),
             ux=element.element_displacement_vector[0],
             uy=element.element_displacement_vector[1],
             phi_z=element.element_displacement_vector[2] if not hinge1 else 0,
             hinge=hinge1,
         )
 
         element.node_map[element.node_id2] = Node(
             id=element.node_id2,
             Fx=element.element_force_vector[3]
             + element.element_primary_force_vector[3],
             Fy=element.element_force_vector[4]
             + element.element_primary_force_vector[4],
-            Tz=element.element_force_vector[5] + element.element_primary_force_vector[5]
-            if not hinge2
-            else 0,
+            Tz=(
+                element.element_force_vector[5]
+                + element.element_primary_force_vector[5]
+                if not hinge2
+                else 0
+            ),
             ux=element.element_displacement_vector[3],
             uy=element.element_displacement_vector[4],
             phi_z=element.element_displacement_vector[5] if not hinge2 else 0,
             hinge=hinge2,
         )
 
         # Local coordinate system. With inclined supports
```

### Comparing `anastruct-1.5.0/anastruct/fem/system.py` & `anastruct-1.5.1/anastruct/fem/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,23 @@
         self.EA = EA
         self.EI = EI
         self.figsize = figsize
         # whether to invert the y-direction of the loads
         self.orientation_cs = -1 if invert_y_loads else 1
 
         # structure system
-        self.element_map: Dict[
-            int, Element
-        ] = {}  # maps element ids to the Element objects.
-        self.node_map: Dict[
-            int, Node  # pylint: disable=used-before-assignment
-        ] = {}  # maps node ids to the Node objects.
-        self.node_element_map: Dict[
-            int, List[Element]
-        ] = {}  # maps node ids to Element objects
+        self.element_map: Dict[int, Element] = (
+            {}
+        )  # maps element ids to the Element objects.
+        self.node_map: Dict[int, Node] = (  # pylint: disable=used-before-assignment
+            {}
+        )  # maps node ids to the Node objects.
+        self.node_element_map: Dict[int, List[Element]] = (
+            {}
+        )  # maps node ids to Element objects
         # keys matrix index (for both row and columns), values K, are processed
         # assemble_system_matrix
         self.system_spring_map: Dict[int, float] = {}
 
         # list of indexes that remain after conditions are applied
         self._remainder_indexes: List[int] = []
 
@@ -128,56 +128,54 @@
         self.supports_rotational: List[Node] = []
         self.internal_hinges: List[Node] = []
         self.supports_roll: List[Node] = []
         self.supports_spring_x: List[Tuple[Node, bool]] = []
         self.supports_spring_y: List[Tuple[Node, bool]] = []
         self.supports_spring_z: List[Tuple[Node, bool]] = []
         self.supports_roll_direction: List[Literal[1, 2]] = []
-        self.inclined_roll: Dict[
-            int, float
-        ] = {}  # map node ids to inclination angle relative to global x-axis.
+        self.inclined_roll: Dict[int, float] = (
+            {}
+        )  # map node ids to inclination angle relative to global x-axis.
         self.supports_roll_rotate: List[bool] = []
 
         # save tuples of the arguments for copying purposes.
         self.supports_spring_args: List[tuple] = []
 
         # keep track of the loads
-        self.loads_point: Dict[
-            int, Tuple[float, float]
-        ] = {}  # node ids with a point loads {node_id: (x, y)}
-        self.loads_q: Dict[
-            int, List[Tuple[float, float]]
-        ] = {}  # element ids with a q-loadad
+        self.loads_point: Dict[int, Tuple[float, float]] = (
+            {}
+        )  # node ids with a point loads {node_id: (x, y)}
+        self.loads_q: Dict[int, List[Tuple[float, float]]] = (
+            {}
+        )  # element ids with a q-loadad
         self.loads_moment: Dict[int, float] = {}
-        self.loads_dead_load: Set[
-            int
-        ] = set()  # element ids with q-load due to dead load
+        self.loads_dead_load: Set[int] = (
+            set()
+        )  # element ids with q-load due to dead load
 
         # results
         self.reaction_forces: Dict[int, Node] = {}  # node objects
         self.non_linear = False
-        self.non_linear_elements: Dict[
-            int, Dict[Literal[1, 2], float]
-        ] = (
+        self.non_linear_elements: Dict[int, Dict[Literal[1, 2], float]] = (
             {}
         )  # keys are element ids, values are dicts: {node_index: max moment capacity}
         self.buckling_factor: Optional[float] = None
 
         # previous point of element
         self._previous_point = Vertex(0, 0)
         self.load_factor = load_factor
 
         # Objects state
         self.count = 0
         self.system_matrix: Optional[np.ndarray] = None
         self.system_force_vector: Optional[np.ndarray] = None
         self.system_displacement_vector: Optional[np.ndarray] = None
-        self.shape_system_matrix: Optional[
-            int
-        ] = None  # actually is the size of the square system matrix
+        self.shape_system_matrix: Optional[int] = (
+            None  # actually is the size of the square system matrix
+        )
         self.reduced_force_vector: Optional[np.ndarray] = None
         self.reduced_system_matrix: Optional[np.ndarray] = None
         self._vertices: Dict[Vertex, int] = {}  # maps vertices to node ids
 
     @property
     def id_last_element(self) -> int:
         """ID of the last element added to the structure
@@ -1376,14 +1374,24 @@
         figsize = self.figsize if figsize is None else figsize
         if values_only:
             return self.plot_values.structure()
         return self.plotter.plot_structure(
             figsize, verbosity, show, supports, scale, offset, annotations=annotations
         )
 
+    def change_plot_colors(self, plot_colors: Dict) -> None:
+        """
+        Calls the change_plot_colors method of the plotter object
+
+        Args:
+            colors (Dict): A dictionary containing plot components and colors
+            as key-value pairs.
+        """
+        self.plotter.change_plot_colors(plot_colors)
+
     def show_bending_moment(
         self,
         factor: Optional[float] = None,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
@@ -1852,23 +1860,31 @@
             dimension (str): "both", 'x' or 'y'
 
         Returns:
             List[Union[float, Tuple[float, float], None]]: List with coordinates x or y
         """
         return list(
             map(
-                lambda x: x.vertex.x
-                if dimension == "x"
-                else x.vertex.y
-                if dimension == "y"
-                else x.vertex.y_neg
-                if dimension == "y_neg"
-                else (x.vertex.x, x.vertex.y)
-                if dimension == "both"
-                else None,
+                lambda x: (
+                    x.vertex.x
+                    if dimension == "x"
+                    else (
+                        x.vertex.y
+                        if dimension == "y"
+                        else (
+                            x.vertex.y_neg
+                            if dimension == "y_neg"
+                            else (
+                                (x.vertex.x, x.vertex.y)
+                                if dimension == "both"
+                                else None
+                            )
+                        )
+                    )
+                ),
                 self.node_map.values(),
             )
         )
 
     def nearest_node(
         self, dimension: "Dimension", val: Union[float, Sequence[float]]
     ) -> Union[int, None]:
```

### Comparing `anastruct-1.5.0/anastruct/fem/system_components/assembly.py` & `anastruct-1.5.1/anastruct/fem/system_components/assembly.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/system_components/solver.py` & `anastruct-1.5.1/anastruct/fem/system_components/solver.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/fem/system_components/util.py` & `anastruct-1.5.1/anastruct/fem/system_components/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,23 @@
 def force_elements_orientation(
     point_1: Vertex,
     point_2: Vertex,
     node_id1: int,
     node_id2: int,
     spring: Optional["Spring"],
     mp: Optional["MpType"],
-) -> Tuple[Vertex, Vertex, int, int, Optional["Spring"], Optional["MpType"], float,]:
+) -> Tuple[
+    Vertex,
+    Vertex,
+    int,
+    int,
+    Optional["Spring"],
+    Optional["MpType"],
+    float,
+]:
     """Force the elements to be in the first and the last quadrant of the unity circle.
     Meaning the first node is always left and the last node is always right. Or they
     are both on one vertical line.
 
     The angle of the element will thus always be between -90 till +90 degrees.
 
     Args:
```

### Comparing `anastruct-1.5.0/anastruct/fem/util/load.py` & `anastruct-1.5.1/anastruct/fem/util/load.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/material/profile.py` & `anastruct-1.5.1/anastruct/material/profile.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/sectionbase/properties.py` & `anastruct-1.5.1/anastruct/sectionbase/properties.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/sectionbase/sectionbase.py` & `anastruct-1.5.1/anastruct/sectionbase/sectionbase.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/types.py` & `anastruct-1.5.1/anastruct/types.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct/vertex.py` & `anastruct-1.5.1/anastruct/vertex.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/anastruct.egg-info/PKG-INFO` & `anastruct-1.5.1/anastruct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastruct
-Version: 1.5.0
+Version: 1.5.1
 Summary: Finite element analysis of 2D structures
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Maintainer-email: Brooks Smith <smith120bh@gmail.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/ritchie46/anaStruct
 Project-URL: documentation, http://anastruct.readthedocs.io
 Project-URL: author, https://ritchievink.com
@@ -20,25 +20,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.15
 Requires-Dist: scipy>=1.1.0
 Provides-Extra: plot
 Requires-Dist: matplotlib>=3.0; extra == "plot"
 Provides-Extra: test
-Requires-Dist: black[jupyter]==23.10.1; extra == "test"
-Requires-Dist: mypy==1.6.1; extra == "test"
-Requires-Dist: pylint==3.0.2; extra == "test"
-Requires-Dist: pytest==7.4.3; extra == "test"
-Requires-Dist: pytest-describe==2.1.0; extra == "test"
+Requires-Dist: black[jupyter]==24.3.0; extra == "test"
+Requires-Dist: mypy==1.9.0; extra == "test"
+Requires-Dist: pylint==3.1.0; extra == "test"
+Requires-Dist: pytest==8.1.1; extra == "test"
+Requires-Dist: pytest-describe==2.2.0; extra == "test"
 Requires-Dist: pytest-pspec==0.0.4; extra == "test"
 Requires-Dist: pytest-raises==0.11; extra == "test"
 Provides-Extra: dev
-Requires-Dist: matplotlib==3.8.0; extra == "dev"
-Requires-Dist: numpy==1.26.1; extra == "dev"
-Requires-Dist: scipy==1.11.3; extra == "dev"
+Requires-Dist: matplotlib==3.8.3; extra == "dev"
+Requires-Dist: numpy==1.26.4; extra == "dev"
+Requires-Dist: scipy==1.12.0; extra == "dev"
 
 # anaStruct 2D Frames and Trusses
 [![Python tests](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml/badge.svg)](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.org/projects/anastruct/badge/?version=latest)](http://anastruct.readthedocs.io/en/latest/?badge=latest)
 
 Analyse 2D Frames and trusses for slender structures. Determine the bending moments, shear forces, axial forces and displacements.
```

### Comparing `anastruct-1.5.0/anastruct.egg-info/SOURCES.txt` & `anastruct-1.5.1/anastruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/pyproject.toml` & `anastruct-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/tests/test_e2e.py` & `anastruct-1.5.1/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.5.0/tests/test_sectionbase.py` & `anastruct-1.5.1/tests/test_sectionbase.py`

 * *Files identical despite different names*

