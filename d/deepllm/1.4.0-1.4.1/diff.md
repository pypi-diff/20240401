# Comparing `tmp/deepllm-1.4.0.tar.gz` & `tmp/deepllm-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-1.4.0.tar", last modified: Mon Mar 25 01:05:01 2024, max compression
+gzip compressed data, was "deepllm-1.4.1.tar", last modified: Mon Apr  1 18:28:33 2024, max compression
```

## Comparing `deepllm-1.4.0.tar` & `deepllm-1.4.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.454167 deepllm-1.4.0/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.4.0/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-03-25 01:05:01.453859 deepllm-1.4.0/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.4.0/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.441506 deepllm-1.4.0/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-03-25 01:03:41.000000 deepllm-1.4.0/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.4.0/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.445513 deepllm-1.4.0/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.4.0/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.4.0/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.4.0/deepllm/apps/app.sh
--rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.0/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)    11175 2024-03-25 01:01:26.000000 deepllm-1.4.0/deepllm/apps/rel_graph.html
--rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.4.0/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.4.0/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.447318 deepllm-1.4.0/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.4.0/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.0/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.4.0/deepllm/demos/demo.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.4.0/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.4.0/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.4.0/deepllm/demos/viz.py
--rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.4.0/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)    10875 2024-03-04 01:12:04.000000 deepllm-1.4.0/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.449691 deepllm-1.4.0/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.4.0/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.0/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.0/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.4.0/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.4.0/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.4.0/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.4.0/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3708 2024-03-24 18:59:54.000000 deepllm-1.4.0/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     9634 2024-03-25 00:11:40.000000 deepllm-1.4.0/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.4.0/deepllm/questmaker.py
--rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.4.0/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     6667 2024-03-24 21:51:28.000000 deepllm-1.4.0/deepllm/refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.4.0/deepllm/requirements.txt
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.453282 deepllm-1.4.0/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.4.0/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.4.0/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.4.0/deepllm/tests/test_all.py
--rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.4.0/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.4.0/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.4.0/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.4.0/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.4.0/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.4.0/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.4.0/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.4.0/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.4.0/deepllm/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.4.0/deepllm/vis.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-25 01:05:01.443388 deepllm-1.4.0/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1319 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-03-25 01:05:01.000000 deepllm-1.4.0/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-03-25 01:05:01.454288 deepllm-1.4.0/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.4.0/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.285439 deepllm-1.4.1/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.4.1/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-01 18:28:33.285085 deepllm-1.4.1/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.4.1/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.265611 deepllm-1.4.1/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-01 18:27:10.000000 deepllm-1.4.1/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.4.1/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.271068 deepllm-1.4.1/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.4.1/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.4.1/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.4.1/deepllm/apps/app.sh
+-rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.1/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)    11175 2024-03-25 01:01:26.000000 deepllm-1.4.1/deepllm/apps/rel_graph.html
+-rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.4.1/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.4.1/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.273817 deepllm-1.4.1/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.4.1/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.1/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.4.1/deepllm/demos/demo.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.4.1/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.4.1/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.4.1/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.4.1/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10875 2024-03-04 01:12:04.000000 deepllm-1.4.1/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.277524 deepllm-1.4.1/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.4.1/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.1/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.1/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.4.1/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.4.1/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.4.1/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.4.1/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3708 2024-03-24 18:59:54.000000 deepllm-1.4.1/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     9634 2024-03-25 00:11:40.000000 deepllm-1.4.1/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.4.1/deepllm/questmaker.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.4.1/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6667 2024-03-24 21:51:28.000000 deepllm-1.4.1/deepllm/refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.4.1/deepllm/requirements.txt
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.284238 deepllm-1.4.1/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.4.1/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.4.1/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.4.1/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.4.1/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.4.1/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.4.1/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.4.1/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.4.1/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.4.1/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.4.1/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.4.1/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.4.1/deepllm/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.4.1/deepllm/vis.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-01 18:28:33.267671 deepllm-1.4.1/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1319 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-01 18:28:33.000000 deepllm-1.4.1/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-01 18:28:33.285565 deepllm-1.4.1/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.4.1/setup.py
```

### Comparing `deepllm-1.4.0/LICENSE` & `deepllm-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/PKG-INFO` & `deepllm-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.0/README.md` & `deepllm-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/api.py` & `deepllm-1.4.1/deepllm/api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/apps/app.py` & `deepllm-1.4.1/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/apps/rel_graph.html` & `deepllm-1.4.1/deepllm/apps/rel_graph.html`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/configurator.py` & `deepllm-1.4.1/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/demos/demo.py` & `deepllm-1.4.1/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/demos/viz.py` & `deepllm-1.4.1/deepllm/demos/viz.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/horn_prover.py` & `deepllm-1.4.1/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/interactors.py` & `deepllm-1.4.1/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/local_llms/local_runs.py` & `deepllm-1.4.1/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/local_llms/test_vicuna.py` & `deepllm-1.4.1/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/params.py` & `deepllm-1.4.1/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/prompters.py` & `deepllm-1.4.1/deepllm/prompters.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/questmaker.py` & `deepllm-1.4.1/deepllm/questmaker.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/recursors.py` & `deepllm-1.4.1/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/refiners.py` & `deepllm-1.4.1/deepllm/refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tests/test_all.py` & `deepllm-1.4.1/deepllm/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tests/test_api.py` & `deepllm-1.4.1/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tests/test_embedders.py` & `deepllm-1.4.1/deepllm/tests/test_embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tests/test_recursors.py` & `deepllm-1.4.1/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tests/test_refiners.py` & `deepllm-1.4.1/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/tools.py` & `deepllm-1.4.1/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm/vis.py` & `deepllm-1.4.1/deepllm/vis.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/deepllm.egg-info/PKG-INFO` & `deepllm-1.4.1/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.0
+Version: 1.4.1
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.0/deepllm.egg-info/SOURCES.txt` & `deepllm-1.4.1/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.0/setup.py` & `deepllm-1.4.1/setup.py`

 * *Files identical despite different names*

