# Comparing `tmp/RL_OM-0.7.8.tar.gz` & `tmp/RL_OM-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.7.8.tar", last modified: Wed Mar  6 05:47:27 2024, max compression
+gzip compressed data, was "RL_OM-0.7.9.tar", last modified: Wed Mar  6 06:13:50 2024, max compression
```

## Comparing `RL_OM-0.7.8.tar` & `RL_OM-0.7.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.548374 RL_OM-0.7.8/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.8/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.8/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 05:47:27.548201 RL_OM-0.7.8/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.8/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.537707 RL_OM-0.7.8/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   210138 2024-02-28 03:50:17.000000 RL_OM-0.7.8/RL_OM/_modidx 2.py
--rw-r--r--   0 magnus     (501) staff       (20)   226125 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.539555 RL_OM-0.7.8/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.542199 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/PPO_SB3.py
--rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/PPO_TEMP.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/cbs.py
--rw-r--r--   0 magnus     (501) staff       (20)     6387 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/eoq.py
--rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents.py
--rw-r--r--   0 magnus     (501) staff       (20)    51867 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     9861 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
--rw-r--r--   0 magnus     (501) staff       (20)    23262 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/qr.py
--rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/saa.py
--rw-r--r--   0 magnus     (501) staff       (20)    13804 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/benchmark_agents/ss.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.542766 RL_OM-0.7.8/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6544 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     9696 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.543182 RL_OM-0.7.8/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1141 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     6362 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.544241 RL_OM-0.7.8/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.545249 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.546840 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     3134 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)    12069 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
--rw-r--r--   0 magnus     (501) staff       (20)     4895 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)     4775 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.547614 RL_OM-0.7.8/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    13064 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    16762 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.547923 RL_OM-0.7.8/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    31373 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/experiment_functions/run_experiment.py
--rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-06 05:47:11.000000 RL_OM-0.7.8/RL_OM/utils.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 05:47:27.539368 RL_OM-0.7.8/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     2467 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.8/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2024-03-06 05:47:27.000000 RL_OM-0.7.8/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2024-03-06 05:47:19.000000 RL_OM-0.7.8/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2024-03-06 05:47:27.548429 RL_OM-0.7.8/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.8/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.762518 RL_OM-0.7.9/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.9/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.9/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 06:13:50.762386 RL_OM-0.7.9/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.9/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.752945 RL_OM-0.7.9/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   210138 2024-02-28 03:50:17.000000 RL_OM-0.7.9/RL_OM/_modidx 2.py
+-rw-r--r--   0 magnus     (501) staff       (20)   226125 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.754226 RL_OM-0.7.9/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.755989 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_SB3.py
+-rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_TEMP.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/cbs.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6387 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents.py
+-rw-r--r--   0 magnus     (501) staff       (20)    51907 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9861 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
+-rw-r--r--   0 magnus     (501) staff       (20)    23262 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/qr.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/saa.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13804 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/ss.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.756617 RL_OM-0.7.9/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6544 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9696 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.757022 RL_OM-0.7.9/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1141 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6362 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.758095 RL_OM-0.7.9/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.759225 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.760915 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     3134 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12069 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4895 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4775 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.761772 RL_OM-0.7.9/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13064 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16762 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.762149 RL_OM-0.7.9/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    31373 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/experiment_functions/run_experiment.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/utils.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.754093 RL_OM-0.7.9/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     2467 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.9/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2024-03-06 06:13:38.000000 RL_OM-0.7.9/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2024-03-06 06:13:50.762561 RL_OM-0.7.9/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.9/setup.py
```

### Comparing `RL_OM-0.7.8/LICENSE` & `RL_OM-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/PKG-INFO` & `RL_OM-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.7.8
+Version: 0.7.9
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.8/RL_OM/_modidx 2.py` & `RL_OM-0.7.9/RL_OM/_modidx 2.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/_modidx.py` & `RL_OM-0.7.9/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/PPO_SB3.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_SB3.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/cbs.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/cbs.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/mp_agents_ERM.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/mp_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents_ERM.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_ERM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1384,36 +1384,39 @@
 
     def draw_action(self, X):
         return self.predict(X)
     
     def predict(self, X):
         self.model.eval()
         self.model.to(self.device)
+
+        if len(X.shape) == 1:
+            X = np.expand_dims(X, axis=0)
+
+        # Initialize a list to hold the X_i batches
+        X_batches = []
+
+        # Create batches
         for i in range(self.feature_map.shape[1]):
-            if len(X.shape)==1:
-                X = np.expand_dims(X, axis=0)
-            X_i = X[:,self.feature_map[:,i].astype(bool)]
-            with torch.no_grad():
-                X_i=torch.from_numpy(X_i)
-                X_i=X_i.float()
-                X_i=X_i.to(self.device)
-
-                output=self.model(X_i)
-                output=output.cpu().numpy()
-            
-            if i == 0:
-                outputs = output
-            else:
-                outputs = np.hstack((outputs, output))
+            X_i = X[:, self.feature_map[:, i].astype(bool)]
+            X_batches.append(X_i)
 
+        X_batch = np.concatenate([x for x in X_batches], axis=0)
+        X_batch = torch.from_numpy(X_batch)
+        X_batch = X_batch.float().to(self.device)
+
+        with torch.no_grad():
+            output = self.model(X_batch)
+            output = output.cpu().numpy()
+        
         # print(outputs)
 
         # check if outputs need to got to cpu or handled by mushroomrl
 
-        return outputs
+        return output
 
     @staticmethod
     def pinball_loss(cu, co, demand, order_quantity, mask):
 
 
         if len(demand.shape)==1:
             demand = demand.unsqueeze(1)
```

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/nv_agents_SAA.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_SAA.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/qr.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/qr.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/saa.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/saa.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/benchmark_agents/ss.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/ss.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/networks/actors.py` & `RL_OM-0.7.9/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/networks/base.py` & `RL_OM-0.7.9/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/networks/critics.py` & `RL_OM-0.7.9/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.7.9/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/processors/processors.py` & `RL_OM-0.7.9/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/environments/calculation_functions.py` & `RL_OM-0.7.9/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/environments/data_generators.py` & `RL_OM-0.7.9/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/environments/feature_converters.py` & `RL_OM-0.7.9/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.7.9/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.7.9/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM/utils.py` & `RL_OM-0.7.9/RL_OM/utils.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.7.9/RL_OM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.7.8
+Version: 0.7.9
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.8/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.7.9/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.8/settings.ini` & `RL_OM-0.7.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.7.8
+version = 0.7.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.7.8/setup.py` & `RL_OM-0.7.9/setup.py`

 * *Files identical despite different names*

