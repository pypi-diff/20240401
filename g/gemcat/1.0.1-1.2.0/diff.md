# Comparing `tmp/gemcat-1.0.1.tar.gz` & `tmp/gemcat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemcat-1.0.1.tar", last modified: Wed Jan 17 19:00:13 2024, max compression
+gzip compressed data, was "gemcat-1.2.0.tar", last modified: Mon Apr  1 13:47:44 2024, max compression
```

## Comparing `gemcat-1.0.1.tar` & `gemcat-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.487889 gemcat-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.475889 gemcat-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.479889 gemcat-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-17 19:00:00.000000 gemcat-1.0.1/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-01-17 19:00:00.000000 gemcat-1.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-17 19:00:00.000000 gemcat-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-17 19:00:00.000000 gemcat-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-17 19:00:13.487889 gemcat-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-01-17 19:00:00.000000 gemcat-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-17 19:00:00.000000 gemcat-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 19:00:13.487889 gemcat-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.475889 gemcat-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.479889 gemcat-1.0.1/src/gemcat/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/adjacency_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-01-17 19:00:00.000000 gemcat-1.0.1/src/gemcat/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.487889 gemcat-1.0.1/src/gemcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-17 19:00:13.000000 gemcat-1.0.1/src/gemcat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.483889 gemcat-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_adjacency_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.483889 gemcat-1.0.1/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/create_test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/highly_connected.json
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/highly_connected.xml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini.json
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_complex_gpr.json
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_complex_gpr.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_complex_gpr_gid_version.json
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_complex_gpr_gid_version.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_redox.json
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_redox.xml
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_reversible.json
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/mini_reversible.xml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/seeds_test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_models/stoichiometry_trp.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_pagerank.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_sanity_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_seeds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 19:00:13.483889 gemcat-1.0.1/tests/test_seq/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_seq/expression_mini.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23585 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-17 19:00:00.000000 gemcat-1.0.1/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.789237 gemcat-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 13:47:33.000000 gemcat-1.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.777237 gemcat-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.781237 gemcat-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-01 13:47:33.000000 gemcat-1.2.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-01 13:47:33.000000 gemcat-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-01 13:47:33.000000 gemcat-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 13:47:33.000000 gemcat-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 13:47:44.789237 gemcat-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-01 13:47:33.000000 gemcat-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-01 13:47:33.000000 gemcat-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:47:44.789237 gemcat-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.777237 gemcat-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.781237 gemcat-1.2.0/src/gemcat/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/adjacency_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-01 13:47:33.000000 gemcat-1.2.0/src/gemcat/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.789237 gemcat-1.2.0/src/gemcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 13:47:44.000000 gemcat-1.2.0/src/gemcat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.785237 gemcat-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_adjacency_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.789237 gemcat-1.2.0/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 13:47:33.000000 gemcat-1.2.0/tests/test_models/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/Recon3D.json
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/Recon3D_301.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/Recon3D_301.mat
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/Recon3D_301.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/create_test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/highly_connected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/highly_connected.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_complex_gpr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_complex_gpr.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_complex_gpr_gid_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_complex_gpr_gid_version.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_redox.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_redox.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_reversible.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/mini_reversible.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/seeds_test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_models/stoichiometry_trp.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_pagerank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.789237 gemcat-1.2.0/tests/test_results/
+-rw-r--r--   0 runner    (1001) docker     (127)   250864 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_results/uc.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_sanity_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 13:47:44.789237 gemcat-1.2.0/tests/test_seq/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seq/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seq/expression_mini.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seq/hek293_rnaseq.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seq/prot_uc_vs_healthy.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_seq/prot_uc_vs_healthy_gid.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23585 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-01 13:47:34.000000 gemcat-1.2.0/tests/test_workflows.py
```

### Comparing `gemcat-1.0.1/.github/workflows/package.yml` & `gemcat-1.2.0/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/.github/workflows/test.yml` & `gemcat-1.2.0/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         os: [
           ubuntu-latest,
           windows-latest,
           ]
 
     steps:
     - uses: actions/checkout@v3
+      with:
+          lfs: 'true'
+    - name: Checkout LFS objects
+      run: git lfs checkout
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `gemcat-1.0.1/.gitignore` & `gemcat-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/LICENSE` & `gemcat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/PKG-INFO` & `gemcat-1.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemcat
-Version: 1.0.1
+Version: 1.2.0
 Summary: A toolbox for gene expression-based prediction of metabolic alterations
 Author-email: Roland Sauter <roland.sauter@uit.no>
 Keywords: python,bioinformatics,modeling,metabolites,omics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.2
@@ -15,16 +15,19 @@
 Requires-Dist: sympy>=1.12
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: pylint>=2.17.7; extra == "dev"
 Requires-Dist: ruff>=0.0.292; extra == "dev"
+Requires-Dist: requests>=2.31.0; extra == "dev"
 
-# GEMCAT: Gene Expression based Metabolite Centrality Analyses Tool
+# GEMCAT: Gene Expression-based Metabolite Centrality Analyses Tool
+A computational toolbox associated with the manuscript entitled "GEMCAT - A new algorithm for gene expression-based prediction of metabolic alterations". 
+Cite using: https://www.biorxiv.org/content/10.1101/2024.01.15.575710v1
 
 ## Compatibility
 The package is tested for compatibility with Python >= 3.10 on Ubuntu and Windows.
 
 ## Installation
 Install from pip:
 
@@ -35,26 +38,55 @@
 ```pip install .```
 
 
 ## Usage
 
 ### Standard workflow from the Command-Line Interface (CLI)
 
-``` gemcat ./expression_file.csv ./model_file.xml -e column_name -a pure -g 1.0 -o result_file.csv```
+Use a single file containing per-gene fold-changes to calculate the resulting differential centralities:
+``` gemcat ./expression_file.csv ./model_file.xml -e column_name -o <result_file.csv>```
+Make sure the .csv file is either comma- or tab-delimited.
+`column_name` is the name of the column in the file containing the fold-change.
+
+Alternatively, use two files (or one file) with expression values for condition and baseline:
+``` gemcat <./condition_file.csv> <./model_file.xml> -e <condition_column_name> -b <./baseline_file> -c <baseline_column_name> -o <result_file.csv>```
+
+Currently only models in XML/SBML format are supported in the CLI.
+Further models can be used from the Python library.
+Support will come to the CLI soon.
+
+Important points to remember:
+Your gene or protein identifiers should be the first column of the expression file.
+Make sure the gene or protein identifiers in your expression data file exactly match those in the model.
+A results list of all 1.0 is a sure sign of no identifier matching.
+
+positional arguments:
+- expression file path
+- model file path
+
+All parameters:
+`-e --expressioncolumn` name of column containing condition expression data
+`-b BASELINE, --baseline` file containing baseline expression data
+`-c BASELINECOLUMN, --baselinecolumn` name of column containing baseline expression data
+`-v VERBOSE, --verbose` enables verbose output
+`-o OUTFILE, --outfile` write output to this file
+`-l LOGFILE, --logfile` write logs to this file
+
 
 ### Standard workflow in Python using a CobraPy model
 ```
 import gemcat as gc
-results = gc.workflows.workflow_standard(cobra_model: cobra.Model,
-                                        mapped_genes_baseline: pd.Series,
-                                        mapped_genes_comparison: pd.Series,
-                                        adjacency = gc.adjacency_transformation.ATPureAdjacency,
-                                        ranking = gc.ranking.PagerankNX,
-                                        gene_fill = 1.0
-                                        )
+results = gc.workflows.workflow_standard(
+  cobra_model: cobra.Model,
+  mapped_genes_baseline: pd.Series,
+  mapped_genes_comparison: pd.Series,
+  adjacency = gc.adjacency_transformation.ATPureAdjacency,
+  ranking = gc.ranking.PagerankNX,
+  gene_fill = 1.0
+)
 ```
 This will return the changes in centrality relative to the baseline in a Pandas Series.
 When using fold-changes as the mapped expression, use a vector of all ones as a comparison.
 
 ## Modularity and Configuration
 GEMCAT is designed to be modular, and its central components can easily be swapped out or appended by other components 
 adhering to the specifications laid out in the module base classes (primarily adjacency transformation, expression integration, and ranking components).
@@ -76,7 +108,18 @@
 To customize the workflow to your needs simply copy the provided functions and switch out the desired steps.
 ### io
 Input and output functions that create GEMCAT models from different sources.
 ## utils
 Contains common utility functions used throughout the package.
 ## verification
 Functions to verify data integrity.
+
+
+## Development
+You can run all local tests with `pytest .`. Default behavior is to also run integration tests, which takes time.
+You can exclude slow running tests by using `pytest . -m "not slow"`.
+These slow running tests are integration tests with "real world data" and will take 10-30s each according to your hardware.
+
+To run tests, make sure you have [git lfs](https://git-lfs.com/) installed and all the Tests are running.
+Make sure to run `isort` and `black` to have properly formatted code.
+
+The CI pipeline in Github will check with isort, black, and pytest.
```

### Comparing `gemcat-1.0.1/README.md` & `gemcat-1.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# GEMCAT: Gene Expression based Metabolite Centrality Analyses Tool
+# GEMCAT: Gene Expression-based Metabolite Centrality Analyses Tool
+A computational toolbox associated with the manuscript entitled "GEMCAT - A new algorithm for gene expression-based prediction of metabolic alterations". 
+Cite using: https://www.biorxiv.org/content/10.1101/2024.01.15.575710v1
 
 ## Compatibility
 The package is tested for compatibility with Python >= 3.10 on Ubuntu and Windows.
 
 ## Installation
 Install from pip:
 
@@ -13,26 +15,55 @@
 ```pip install .```
 
 
 ## Usage
 
 ### Standard workflow from the Command-Line Interface (CLI)
 
-``` gemcat ./expression_file.csv ./model_file.xml -e column_name -a pure -g 1.0 -o result_file.csv```
+Use a single file containing per-gene fold-changes to calculate the resulting differential centralities:
+``` gemcat ./expression_file.csv ./model_file.xml -e column_name -o <result_file.csv>```
+Make sure the .csv file is either comma- or tab-delimited.
+`column_name` is the name of the column in the file containing the fold-change.
+
+Alternatively, use two files (or one file) with expression values for condition and baseline:
+``` gemcat <./condition_file.csv> <./model_file.xml> -e <condition_column_name> -b <./baseline_file> -c <baseline_column_name> -o <result_file.csv>```
+
+Currently only models in XML/SBML format are supported in the CLI.
+Further models can be used from the Python library.
+Support will come to the CLI soon.
+
+Important points to remember:
+Your gene or protein identifiers should be the first column of the expression file.
+Make sure the gene or protein identifiers in your expression data file exactly match those in the model.
+A results list of all 1.0 is a sure sign of no identifier matching.
+
+positional arguments:
+- expression file path
+- model file path
+
+All parameters:
+`-e --expressioncolumn` name of column containing condition expression data
+`-b BASELINE, --baseline` file containing baseline expression data
+`-c BASELINECOLUMN, --baselinecolumn` name of column containing baseline expression data
+`-v VERBOSE, --verbose` enables verbose output
+`-o OUTFILE, --outfile` write output to this file
+`-l LOGFILE, --logfile` write logs to this file
+
 
 ### Standard workflow in Python using a CobraPy model
 ```
 import gemcat as gc
-results = gc.workflows.workflow_standard(cobra_model: cobra.Model,
-                                        mapped_genes_baseline: pd.Series,
-                                        mapped_genes_comparison: pd.Series,
-                                        adjacency = gc.adjacency_transformation.ATPureAdjacency,
-                                        ranking = gc.ranking.PagerankNX,
-                                        gene_fill = 1.0
-                                        )
+results = gc.workflows.workflow_standard(
+  cobra_model: cobra.Model,
+  mapped_genes_baseline: pd.Series,
+  mapped_genes_comparison: pd.Series,
+  adjacency = gc.adjacency_transformation.ATPureAdjacency,
+  ranking = gc.ranking.PagerankNX,
+  gene_fill = 1.0
+)
 ```
 This will return the changes in centrality relative to the baseline in a Pandas Series.
 When using fold-changes as the mapped expression, use a vector of all ones as a comparison.
 
 ## Modularity and Configuration
 GEMCAT is designed to be modular, and its central components can easily be swapped out or appended by other components 
 adhering to the specifications laid out in the module base classes (primarily adjacency transformation, expression integration, and ranking components).
@@ -54,7 +85,18 @@
 To customize the workflow to your needs simply copy the provided functions and switch out the desired steps.
 ### io
 Input and output functions that create GEMCAT models from different sources.
 ## utils
 Contains common utility functions used throughout the package.
 ## verification
 Functions to verify data integrity.
+
+
+## Development
+You can run all local tests with `pytest .`. Default behavior is to also run integration tests, which takes time.
+You can exclude slow running tests by using `pytest . -m "not slow"`.
+These slow running tests are integration tests with "real world data" and will take 10-30s each according to your hardware.
+
+To run tests, make sure you have [git lfs](https://git-lfs.com/) installed and all the Tests are running.
+Make sure to run `isort` and `black` to have properly formatted code.
+
+The CI pipeline in Github will check with isort, black, and pytest.
```

### Comparing `gemcat-1.0.1/pyproject.toml` & `gemcat-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemcat"
-version = "1.0.1"
+version = "1.2.0"
 
 description = "A toolbox for gene expression-based prediction of metabolic alterations"
 keywords = ["python", "bioinformatics", "modeling", "metabolites", "omics"]
 authors = [
     {name = "Roland Sauter", email = "roland.sauter@uit.no"}
 ]
 readme = "README.md"
@@ -26,14 +26,15 @@
 [project.optional-dependencies]
 dev = [
   "pytest>=7.4.0",
   "black>=23.7.0",
   "isort>=5.12.0",
   "pylint>=2.17.7",
   "ruff>=0.0.292",
+  "requests>=2.31.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project.scripts]
 gemcat = "gemcat.cli:main"
@@ -79,7 +80,13 @@
 ]
 per-file-ignores = {}
 # Same as Black.
 line-length = 88
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 target-version = "py312"
+
+[tool.pytest.ini_options]
+markers = [
+    "slow: Slow running (usually integration) tests. Run only fast tests with '-m \"not slow\"')",
+    "serial",
+]
```

### Comparing `gemcat-1.0.1/src/gemcat/adjacency_transformation.py` & `gemcat-1.2.0/src/gemcat/adjacency_transformation.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/cli.py` & `gemcat-1.2.0/src/gemcat/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,75 @@
 #!/usr/bin/python
 
 """
 Command line interface functionality
 """
 
 import argparse
+import csv
 import logging
+from copy import deepcopy
 from pathlib import Path
 from typing import Any, Optional
 
 import cobra
 from pandas import DataFrame, Series, read_csv
 
-from .adjacency_transformation import AdjacencyTransformation, ATPureAdjacency
-from .expression import (
-    ExpressionIntegration,
-    ExpressionMapSingleAverage,
-    GeometricAndAverageMeans,
-    read_gpr_strings_from_cobra,
-)
-from .io import convert_cobra_model, load_sbml_cobra
-from .ranking import PagerankNX, Ranking
-
-ADJACENCIES = {
-    "pure": ATPureAdjacency,
-}
-ALLOWED_ADJ = ", ".join(ADJACENCIES.keys())
-
-RANKINGS = {
-    "Pagerank": PagerankNX,
-}
-
-EXPRESSION_INTEGRATIONS = {
-    "means": GeometricAndAverageMeans,
-    "average": ExpressionMapSingleAverage,
-}
-
-ALLOWED_RANKINGS = ", ".join(RANKINGS.keys())
+from .io import load_json_cobra, load_mat_cobra, load_sbml_cobra
+from .workflows import workflow_standard
 
 
 def not_implemented(whatever: Any):
     """
     Standard function raising a NotImplementedError on demand
     :param whatever: Any input
     :type whatever: Any
     :raises NotImplementedError: Always raises
     """
     raise NotImplementedError()
 
 
 MODELS = {
-    ".sbml": load_sbml_cobra,
-    ".xml": load_sbml_cobra,
-    ".json": not_implemented,
-    ".csv": not_implemented,
-    ".mat": not_implemented,
+    "sbml": load_sbml_cobra,
+    "xml": load_sbml_cobra,
+    "json": load_json_cobra,
+    "csv": not_implemented,
+    "mat": load_mat_cobra,
 }
 
 
-def parse_cobra_model(model_path: str) -> cobra.Model:
+def wrong_filetype(any: Any):
+    raise NotImplementedError(f"Not implemented for {any}")
+
+
+def parse_model(model_path: str) -> cobra.Model:
+    model_path = Path(model_path)
+    throw_for_missing_model(model_path)
+    parsing_fn = MODELS[model_path.suffix[1:]]
+    return parsing_fn(model_path)
+
+
+def get_delimiter(file_path, bytes=4096):
+    sniffer = csv.Sniffer()
+    data = open(file_path, "r").read(bytes)
+    delimiter = sniffer.sniff(data).delimiter
+    return delimiter
+
+
+def throw_for_missing_model(model_path: Path):
     """
-    Parse selected cobra model
-    :param model_path: Path to model file
+    Throw FileNotFoundError in case there is no model at the given path.
+    :param model_path: _description_
     :type model_path: str
-    :raises FileNotFoundError: If model file does not exist at path
-    :return: Loaded cobra model
-    :rtype: cobra.Model
+    :raises FileNotFoundError: _description_
     """
-    model_path = Path(model_path)
-    if not model_path.exists():
+    if not model_path.is_file():
         error_str = f"The model file at {model_path} cannot be found."
         logging.error(error_str)
         raise FileNotFoundError(error_str)
-    return cobra.io.read_sbml_model(model_path.as_posix())
 
 
 def read_expression(expression_file: str) -> DataFrame:
     """
     Parsing the expression file into a DataFrame
     :param expression_file: Path to expression file
     :type expression_file: str
@@ -86,22 +79,25 @@
     :rtype: DataFrame
     """
     file_path = Path(expression_file)
     if not file_path.exists():
         error_str = f"File {expression_file} could not be found"
         logging.error(error_str)
         raise FileNotFoundError(error_str)
-    if file_path.suffix == ".csv":
-        content = read_csv(file_path, sep=",", index_col=0)
-    elif file_path.suffix == ".tsv":
-        content = read_csv(file_path, sep="\t", index_col=0)
+    if file_path.suffix == ".csv" or file_path.suffix == "tsv":
+        delimiter = get_delimiter(file_path)
+        content = read_csv(file_path, sep=delimiter, index_col=0)
     else:
-        error_str = f"Unknown file format {file_path.suffix} in file {expression_file}"
+        error_str = (
+            f"Unsupported file format {file_path.suffix} in file {expression_file}"
+        )
         logging.error(error_str)
         raise ValueError(error_str)
+    if isinstance(content, Series):
+        return DataFrame(content)
     return content
 
 
 def parse_expression(expression_file: str, col_name: Optional[str]) -> Series:
     """
     Parse file containing expression data into pandas Series
     :param expression_file: Path to expression file
@@ -109,103 +105,36 @@
     :param col_name: ID of the column containing the expression data
     :type col_name: Optional[str]
     :raises ValueError: If expression file cannot be parsed into a series
     :return: _description_
     :rtype: Series
     """
     content = read_expression(expression_file)
-    if not content.shape[1] or (content.shape[1] == 1):
-        content = content.squeeze()
-    else:
-        content = content.loc[:, col_name]
-    if not isinstance(content, Series):
-        error_str = """
-        Expression file must be in the format of a pandas Series, 
-        mapping a gene column to a value column.
-        """
-        logging.error(error_str)
-        raise ValueError(error_str)
-    return content
-
-
-def parse_integration(integration: str) -> ExpressionIntegration:
-    """
-    Choice function for expression integration algorithms
-    :param integration: Name for expression integration algorithm
-    :type integration: str
-    :raises ValueError: In case of invalid name
-    :return: Selected expression integration algorithm
-    :rtype: ExpressionIntegration
-    """
-    if integration is None:
-        return GeometricAndAverageMeans
-    try:
-        return EXPRESSION_INTEGRATIONS[integration]
-    except KeyError as original_err:
-        error_str = f"""
-        Expression integration method {integration} does not exist. 
-        Allowed methods: {EXPRESSION_INTEGRATIONS}
-        """
-        logging.error(error_str)
-        raise ValueError(error_str) from original_err
-
-
-def parse_adjacency(adjacency: Optional[str]) -> AdjacencyTransformation:
-    """
-    Choice function for adjacency calculation algorithms
-    :param adjacency: Name for adjacency calculation algorithm
-    :type adjacency: Optional[str]
-    :raises ValueError: In case of invalid name
-    :return: Selected adjacency transformation algorithm
-    :rtype: AdjacencyTransformation
-    """
-    if adjacency is None:
-        return ATPureAdjacency
-    try:
-        return ADJACENCIES[adjacency]
-    except KeyError as original_err:
-        error_str = f"""
-        Adjacency model {adjacency} does not exist. 
-        Allowed models: {ALLOWED_ADJ}
-        """
-        logging.error(error_str)
-        raise ValueError(error_str) from original_err
-
-
-def parse_ranking(ranking: Optional[str]) -> Ranking:
-    """
-    Choice function for ranking algorithms
-    :param ranking: Name of the ranking algorithm to use
-    :type ranking: Optional[str]
-    :raises ValueError: In case of unknown ranking algorithm name
-    :return: Ranking algorithm
-    :rtype: Ranking
-    """
-    if ranking is None:
-        return PagerankNX
-    try:
-        return RANKINGS[ranking]
-    except KeyError as original_err:
-        error_str = f"""
-        {ranking} is not a valid ranking method. 
-        Available methods are: {ALLOWED_RANKINGS}
-        """
-        logging.error(error_str)
-        raise ValueError(error_str) from original_err
+    if col_name is None and len(content.columns) > 1:
+        raise ValueError(
+            """
+            If your expression file contains more than 1 column, 
+            please provide the name of the column with the expression data
+            to the -e flag of the command.
+            """
+        )
+    if col_name is None:
+        return content.iloc[:, 0]
+    return content.loc[:, col_name]
 
 
 def get_all_ones(expression: Series) -> Series:
     """
     Return a copy of a pandas series with all entries set to one
     :param expression: Gene expression values
     :type expression: pd.Series
     :return: Identical expression series with all entries set to one
     :rtype: pd.Series
     """
-    return Series(index=expression.index, data=1.0)
+    return Series(index=deepcopy(expression.index), data=1.0)
 
 
 def parse_outfile(outfile: Optional[str]) -> Path:
     """
     Parse input for output file
     :param outfile: Output file to write to, default to ./results.csv
     :type outfile: Optional[str]
@@ -228,27 +157,46 @@
     :return: _description_
     :rtype: argparse.ArgumentParser
     """
     parser = argparse.ArgumentParser(
         prog="gemcat",
         description="GEMCAT tool for metabolomics predictions",
     )
-    parser.add_argument("expressionfile")
-    parser.add_argument("modelfile")
 
-    parser.add_argument("-i", "--integration")
-    parser.add_argument("-e", "--expressioncolumn")
-    parser.add_argument("-r", "--ranking")
-    parser.add_argument("-b", "--baseline")
-    parser.add_argument("-c", "--baselinecolumn")
-    parser.add_argument("-a", "--adjacency")
-    parser.add_argument("-g", "--genefill")
-    parser.add_argument("-v", "--verbose")
-    parser.add_argument("-o", "--outfile")
-    parser.add_argument("-l", "--logfile")
+    parser.add_argument(
+        "modelfile", help="Path to model file to use (XML/SBML, JSON format)"
+    )
+    parser.add_argument(
+        "expressionfile", help="Path to file containing the condition expression data"
+    )
+
+    parser.add_argument(
+        "-e",
+        "--expressioncolumn",
+        help="Name of the column containing the condition expression data",
+    )
+    parser.add_argument(
+        "-b", "--baseline", help="File containing expression data for the baseline"
+    )
+    parser.add_argument(
+        "-c",
+        "--baselinecolumn",
+        help="Name of the column contianing the baseline expression data",
+    )
+    parser.add_argument(
+        "-g",
+        "--genefill",
+        type=float,
+        help="Value to fill in for missing expression values",
+    )
+    parser.add_argument(
+        "-v", "--verbose", action="store_true", help="Use for more verbose output"
+    )
+    parser.add_argument("-o", "--outfile", help="Write outputs to the specified file")
+    parser.add_argument("-l", "--logfile", help="Write logs to the specified file")
 
     return parser
 
 
 def save_to_file(outfile: Path, results: Series) -> None:
     """
     Write results to file
@@ -274,38 +222,27 @@
 
 def cli_standard(args: argparse.Namespace):
     """ "
     CLI interface for the standard workflow
     """
     expression = parse_expression(args.expressionfile, args.expressioncolumn)
     if args.baseline:
-        baseline = parse_expression(args.baseline, args.baseline_column)
+        baseline = parse_expression(args.baseline, args.baselinecolumn)
     else:
         print("Empty baseline expression. Defaulting to all ones.")
         baseline = get_all_ones(expression)
     try:
         gene_fill = float(args.genefill)
     except (TypeError, ValueError):
-        print("Empty or invalid gene-fill value. Defaulting to 1.0 .")
+        logging.info("Empty or invalid gene-fill value. Defaulting to 1.0 .")
         gene_fill = 1.0
-
-    cobra_model = parse_cobra_model(args.modelfile)
-    model = convert_cobra_model(cobra_model)
-    model.adjacency_transformation = parse_adjacency(args.adjacency)
-    model.ranking = parse_ranking(args.ranking)
-    gpr, rxn_gene_mapping = read_gpr_strings_from_cobra(cobra_model)
-    integration = parse_integration(args.integration)
-    expression_obj = integration(gpr, rxn_gene_mapping, expression, gene_fill=gene_fill)
-    baseline_obj = integration(gpr, rxn_gene_mapping, baseline, gene_fill=gene_fill)
-    model.load_expression(expression_obj)
-    results = model.calculate()
-    model.load_expression(baseline_obj)
-    results_baseline = model.calculate()
-
-    return results / results_baseline, parse_outfile(args.outfile)
+    cobra_model = parse_model(args.modelfile)
+    return workflow_standard(
+        cobra_model, baseline, expression, gene_fill
+    ), parse_outfile(args.outfile)
 
 
 def main():
     """
     CLI entrypoint and central function
     """
     parser = build_parser()
```

### Comparing `gemcat-1.0.1/src/gemcat/expression.py` & `gemcat-1.2.0/src/gemcat/expression.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/io.py` & `gemcat-1.2.0/src/gemcat/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,42 +29,48 @@
         raise TypeError(err)
     stoich_matrix = utils.get_stoich_matrix_from_cobra(cobra_model)
     rev = utils.get_reversibilities(cobra_model)
     metabolites = utils.get_metabolite_ids(cobra_model)
     return Model(stoich_matrix, metabolites, rev)
 
 
-def load_json_cobra(json_file: Union[str, Path]) -> Model:
+def load_json_cobra(json_file: Union[str, Path]) -> cobra.Model:
     """
     Loads a Pagerank-based Model from a COBRA json file.
     :param json_file: Path to json model file
     :type json_file: Union[str, Path]
     :return: Model object created from the COBRA model
     :rtype: Model
     """
-    if isinstance(json_file, Path):
-        json_file = json_file.as_posix()
-    cobra_model = cobra.io.load_json_model(json_file)
+    cobra_model = cobra.io.load_json_model(str(json_file))
+    return cobra_model
 
-    return convert_cobra_model(cobra_model)
 
-
-def load_sbml_cobra(sbml_file: Union[str, Path]):
+def load_sbml_cobra(sbml_file: Union[str, Path]) -> cobra.Model:
     """
     Loads a Pagerank-based Model from a COBRA SBML file.
     :param sbml_file: Path to json SBML file
     :type sbml_file: Union[str, Path]
     :return: Model object created from the COBRA model
     :rtype: Model
     """
-    if isinstance(sbml_file, Path):
-        sbml_file = sbml_file.as_posix()
-    cobra_model = cobra.io.read_sbml_model(sbml_file)
+    cobra_model = cobra.io.read_sbml_model(str(sbml_file))
+    return cobra_model
+
 
-    return convert_cobra_model(cobra_model)
+def load_mat_cobra(mat_file: Union[str, Path]) -> cobra.Model:
+    """
+    Loads a Pagerank-based Model from a COBRA SBML file.
+    :param mat_file: Path to json SBML file
+    :type mat_file: Union[str, Path]
+    :return: COBRA model object
+    :rtype: Model
+    """
+    cobra_model = cobra.io.load_matlab_model(str(mat_file))
+    return cobra_model
 
 
 def load_csv(
     csv_file: Union[Path, str], sep=",", reversibilities: Optional[list[bool]] = None
 ):
     """
     Load models from CSV file (uses Pandas).
```

### Comparing `gemcat-1.0.1/src/gemcat/model.py` & `gemcat-1.2.0/src/gemcat/model.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/ranking.py` & `gemcat-1.2.0/src/gemcat/ranking.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/utils.py` & `gemcat-1.2.0/src/gemcat/utils.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/verification.py` & `gemcat-1.2.0/src/gemcat/verification.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/src/gemcat/workflows.py` & `gemcat-1.2.0/src/gemcat/workflows.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,44 @@
 
 from . import adjacency_transformation as at
 from . import expression as ex
 from . import io
 from . import ranking as pr
 
 
+def workflow_single(
+    cobra_model: cobra.Model, mapped_genes: pd.Series, gene_fill: float
+) -> pd.Series:
+    """
+    Workflow using Expression data integration via simple averaging,
+    provides only the output from a single expression data set.
+    :param cobra_model: cobra Model used as a base for modeling
+    :type cobra_model: cobra.Model
+    :param mapped_genes: Levels of gene/protein expression values
+    :type mapped_genes: pd.Series
+    :param gene_fill: Value to fill empty genes with
+    :type gene_fill: float
+    :return: Normalized metabolite scores
+    :rtype: pd.Series
+    """
+    model = io.convert_cobra_model(cobra_model)
+    gpr, rxn_gene_mapping = ex.read_gpr_strings_from_cobra(cobra_model)
+    model.adjacency_transformation = at.ATPureAdjacency()
+    model.ranking = pr.PagerankNX()
+    ex_comparison = ex.GeometricAndAverageMeans(
+        gpr=gpr,
+        reaction_gene_mapping=rxn_gene_mapping,
+        data=mapped_genes,
+        gene_fill=gene_fill,
+    )
+    model.load_expression(ex_comparison)
+    results = model.calculate()
+    return results
+
+
 def workflow_avg_single(
     cobra_model: cobra.Model,
     mapped_genes: pd.Series,
 ) -> pd.Series:
     """
     Workflow using Expression data integration via simple averaging,
     provides only the output from a single expression data set.
```

### Comparing `gemcat-1.0.1/src/gemcat.egg-info/PKG-INFO` & `gemcat-1.2.0/src/gemcat.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemcat
-Version: 1.0.1
+Version: 1.2.0
 Summary: A toolbox for gene expression-based prediction of metabolic alterations
 Author-email: Roland Sauter <roland.sauter@uit.no>
 Keywords: python,bioinformatics,modeling,metabolites,omics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.2
@@ -15,16 +15,19 @@
 Requires-Dist: sympy>=1.12
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: black>=23.7.0; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: pylint>=2.17.7; extra == "dev"
 Requires-Dist: ruff>=0.0.292; extra == "dev"
+Requires-Dist: requests>=2.31.0; extra == "dev"
 
-# GEMCAT: Gene Expression based Metabolite Centrality Analyses Tool
+# GEMCAT: Gene Expression-based Metabolite Centrality Analyses Tool
+A computational toolbox associated with the manuscript entitled "GEMCAT - A new algorithm for gene expression-based prediction of metabolic alterations". 
+Cite using: https://www.biorxiv.org/content/10.1101/2024.01.15.575710v1
 
 ## Compatibility
 The package is tested for compatibility with Python >= 3.10 on Ubuntu and Windows.
 
 ## Installation
 Install from pip:
 
@@ -35,26 +38,55 @@
 ```pip install .```
 
 
 ## Usage
 
 ### Standard workflow from the Command-Line Interface (CLI)
 
-``` gemcat ./expression_file.csv ./model_file.xml -e column_name -a pure -g 1.0 -o result_file.csv```
+Use a single file containing per-gene fold-changes to calculate the resulting differential centralities:
+``` gemcat ./expression_file.csv ./model_file.xml -e column_name -o <result_file.csv>```
+Make sure the .csv file is either comma- or tab-delimited.
+`column_name` is the name of the column in the file containing the fold-change.
+
+Alternatively, use two files (or one file) with expression values for condition and baseline:
+``` gemcat <./condition_file.csv> <./model_file.xml> -e <condition_column_name> -b <./baseline_file> -c <baseline_column_name> -o <result_file.csv>```
+
+Currently only models in XML/SBML format are supported in the CLI.
+Further models can be used from the Python library.
+Support will come to the CLI soon.
+
+Important points to remember:
+Your gene or protein identifiers should be the first column of the expression file.
+Make sure the gene or protein identifiers in your expression data file exactly match those in the model.
+A results list of all 1.0 is a sure sign of no identifier matching.
+
+positional arguments:
+- expression file path
+- model file path
+
+All parameters:
+`-e --expressioncolumn` name of column containing condition expression data
+`-b BASELINE, --baseline` file containing baseline expression data
+`-c BASELINECOLUMN, --baselinecolumn` name of column containing baseline expression data
+`-v VERBOSE, --verbose` enables verbose output
+`-o OUTFILE, --outfile` write output to this file
+`-l LOGFILE, --logfile` write logs to this file
+
 
 ### Standard workflow in Python using a CobraPy model
 ```
 import gemcat as gc
-results = gc.workflows.workflow_standard(cobra_model: cobra.Model,
-                                        mapped_genes_baseline: pd.Series,
-                                        mapped_genes_comparison: pd.Series,
-                                        adjacency = gc.adjacency_transformation.ATPureAdjacency,
-                                        ranking = gc.ranking.PagerankNX,
-                                        gene_fill = 1.0
-                                        )
+results = gc.workflows.workflow_standard(
+  cobra_model: cobra.Model,
+  mapped_genes_baseline: pd.Series,
+  mapped_genes_comparison: pd.Series,
+  adjacency = gc.adjacency_transformation.ATPureAdjacency,
+  ranking = gc.ranking.PagerankNX,
+  gene_fill = 1.0
+)
 ```
 This will return the changes in centrality relative to the baseline in a Pandas Series.
 When using fold-changes as the mapped expression, use a vector of all ones as a comparison.
 
 ## Modularity and Configuration
 GEMCAT is designed to be modular, and its central components can easily be swapped out or appended by other components 
 adhering to the specifications laid out in the module base classes (primarily adjacency transformation, expression integration, and ranking components).
@@ -76,7 +108,18 @@
 To customize the workflow to your needs simply copy the provided functions and switch out the desired steps.
 ### io
 Input and output functions that create GEMCAT models from different sources.
 ## utils
 Contains common utility functions used throughout the package.
 ## verification
 Functions to verify data integrity.
+
+
+## Development
+You can run all local tests with `pytest .`. Default behavior is to also run integration tests, which takes time.
+You can exclude slow running tests by using `pytest . -m "not slow"`.
+These slow running tests are integration tests with "real world data" and will take 10-30s each according to your hardware.
+
+To run tests, make sure you have [git lfs](https://git-lfs.com/) installed and all the Tests are running.
+Make sure to run `isort` and `black` to have properly formatted code.
+
+The CI pipeline in Github will check with isort, black, and pytest.
```

### Comparing `gemcat-1.0.1/src/gemcat.egg-info/SOURCES.txt` & `gemcat-1.2.0/src/gemcat.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/package.yml
 .github/workflows/test.yml
 src/gemcat/__init__.py
@@ -17,25 +18,31 @@
 src/gemcat.egg-info/PKG-INFO
 src/gemcat.egg-info/SOURCES.txt
 src/gemcat.egg-info/dependency_links.txt
 src/gemcat.egg-info/entry_points.txt
 src/gemcat.egg-info/requires.txt
 src/gemcat.egg-info/top_level.txt
 tests/fixtures.py
+tests/test.ipynb
 tests/test_adjacency_calculation.py
 tests/test_cli.py
 tests/test_expression.py
 tests/test_io.py
 tests/test_model.py
 tests/test_pagerank.py
 tests/test_sanity_checks.py
 tests/test_seeds.py
 tests/test_utils.py
 tests/test_verification.py
 tests/test_workflows.py
+tests/test_models/.gitattributes
+tests/test_models/Recon3D.json
+tests/test_models/Recon3D_301.json
+tests/test_models/Recon3D_301.mat
+tests/test_models/Recon3D_301.xml
 tests/test_models/create_test_models.py
 tests/test_models/highly_connected.json
 tests/test_models/highly_connected.xml
 tests/test_models/mini.json
 tests/test_models/mini.xml
 tests/test_models/mini_complex_gpr.json
 tests/test_models/mini_complex_gpr.xml
@@ -43,8 +50,13 @@
 tests/test_models/mini_complex_gpr_gid_version.xml
 tests/test_models/mini_redox.json
 tests/test_models/mini_redox.xml
 tests/test_models/mini_reversible.json
 tests/test_models/mini_reversible.xml
 tests/test_models/seeds_test.csv
 tests/test_models/stoichiometry_trp.csv
-tests/test_seq/expression_mini.csv
+tests/test_results/uc.csv
+tests/test_seq/.gitattributes
+tests/test_seq/expression_mini.csv
+tests/test_seq/hek293_rnaseq.csv
+tests/test_seq/prot_uc_vs_healthy.csv
+tests/test_seq/prot_uc_vs_healthy_gid.csv
```

### Comparing `gemcat-1.0.1/tests/fixtures.py` & `gemcat-1.2.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_adjacency_calculation.py` & `gemcat-1.2.0/tests/test_adjacency_calculation.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_expression.py` & `gemcat-1.2.0/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_io.py` & `gemcat-1.2.0/tests/test_io.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,22 @@
     cobra_model = models["mini"]
     model = io.convert_cobra_model(cobra_model)
     assert np.allclose(model.stoichiometric_matrix, S_models["mini"])
 
 
 def test_json_io(model_files_json, S_models):
     model_file = model_files_json["mini"]
-    model = io.load_json_cobra(model_file)
+    model = io.convert_cobra_model(io.load_json_cobra(model_file))
     assert np.allclose(model.stoichiometric_matrix, S_models["mini"])
 
 
 def test_sbml_io(model_files_sbml, S_models):
     model_file = model_files_sbml["mini"]
-    model = io.load_sbml_cobra(model_file)
+    cobra_model = io.load_sbml_cobra(model_file)
+    model = io.convert_cobra_model(cobra_model)
     assert np.allclose(model.stoichiometric_matrix, S_models["mini"])
 
 
 def test_load_csv():
     filepath = Path("./tests/test_models/stoichiometry_trp.csv")
     model = io.load_csv(filepath, sep="\t")
     mets = [
```

### Comparing `gemcat-1.0.1/tests/test_model.py` & `gemcat-1.2.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/create_test_models.py` & `gemcat-1.2.0/tests/test_models/create_test_models.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/highly_connected.json` & `gemcat-1.2.0/tests/test_models/highly_connected.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/highly_connected.xml` & `gemcat-1.2.0/tests/test_models/highly_connected.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini.json` & `gemcat-1.2.0/tests/test_models/mini.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini.xml` & `gemcat-1.2.0/tests/test_models/mini.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_complex_gpr.json` & `gemcat-1.2.0/tests/test_models/mini_complex_gpr.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_complex_gpr.xml` & `gemcat-1.2.0/tests/test_models/mini_complex_gpr.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_complex_gpr_gid_version.json` & `gemcat-1.2.0/tests/test_models/mini_complex_gpr_gid_version.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_complex_gpr_gid_version.xml` & `gemcat-1.2.0/tests/test_models/mini_complex_gpr_gid_version.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_redox.json` & `gemcat-1.2.0/tests/test_models/mini_redox.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_redox.xml` & `gemcat-1.2.0/tests/test_models/mini_redox.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_reversible.json` & `gemcat-1.2.0/tests/test_models/mini_reversible.json`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/mini_reversible.xml` & `gemcat-1.2.0/tests/test_models/mini_reversible.xml`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_models/stoichiometry_trp.csv` & `gemcat-1.2.0/tests/test_models/stoichiometry_trp.csv`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_pagerank.py` & `gemcat-1.2.0/tests/test_pagerank.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_sanity_checks.py` & `gemcat-1.2.0/tests/test_sanity_checks.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_seeds.py` & `gemcat-1.2.0/tests/test_seeds.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 model_seeds = model_path / "seeds_test.csv"
 
 eps = 10**-5
 
 
 def test_seed_load():
     seeds = [1.0, 2.0, 3.0, 4.0]
-    model = pr.io.load_sbml_cobra(mini_path)
+    model = pr.io.convert_cobra_model(pr.io.load_sbml_cobra(mini_path))
     model.load_metabolite_seeds(seeds)
     assert model.seeds == seeds
 
 
 def test_wrong_seed_load():
     seeds = [1.0, 2.0, 3.0, 4.0, 5.0]
-    model = pr.io.load_sbml_cobra(mini_path)
+    model = pr.io.convert_cobra_model(pr.io.load_sbml_cobra(mini_path))
     with pytest.raises(ValueError):
         model.load_metabolite_seeds(seeds)
 
 
 # found here: https://www.briggsby.com/personalized-Pagerank
 def test_seed_integration():
     expected = Series(
```

### Comparing `gemcat-1.0.1/tests/test_utils.py` & `gemcat-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_verification.py` & `gemcat-1.2.0/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `gemcat-1.0.1/tests/test_workflows.py` & `gemcat-1.2.0/tests/test_workflows.py`

 * *Files identical despite different names*

