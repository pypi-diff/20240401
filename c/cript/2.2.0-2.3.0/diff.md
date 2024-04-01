# Comparing `tmp/cript-2.2.0.tar.gz` & `tmp/cript-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cript-2.2.0.tar", last modified: Fri Nov 17 20:40:09 2023, max compression
+gzip compressed data, was "cript-2.3.0.tar", last modified: Mon Apr  1 18:48:28 2024, max compression
```

## Comparing `cript-2.2.0.tar` & `cript-2.3.0.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.172474 cript-2.2.0/
--rw-rw-rw-   0        0        0     1122 2023-10-06 19:50:54.000000 cript-2.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     5762 2023-11-17 20:40:09.172474 cript-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5094 2023-11-17 19:59:37.000000 cript-2.2.0/README.md
--rw-rw-rw-   0        0        0      346 2023-10-06 19:50:55.000000 cript-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      799 2023-11-17 20:40:09.172474 cript-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-10-06 19:50:55.000000 cript-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.062167 cript-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.077823 cript-2.2.0/src/cript/
--rw-rw-rw-   0        0        0      889 2023-11-02 19:44:31.000000 cript-2.2.0/src/cript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.110608 cript-2.2.0/src/cript/api/
--rw-rw-rw-   0        0        0      179 2023-11-02 19:44:31.000000 cript-2.2.0/src/cript/api/__init__.py
--rw-rw-rw-   0        0        0    53233 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/api.py
--rw-rw-rw-   0        0        0      312 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/api_config.py
--rw-rw-rw-   0        0        0    10752 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/exceptions.py
--rw-rw-rw-   0        0        0     8183 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/paginator.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.115197 cript-2.2.0/src/cript/api/utils/
--rw-rw-rw-   0        0        0      137 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/utils/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/utils/aws_s3_utils.py
--rw-rw-rw-   0        0        0     1990 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/utils/get_host_token.py
--rw-rw-rw-   0        0        0     1297 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/utils/helper_functions.py
--rw-rw-rw-   0        0        0     8399 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/utils/save_helper.py
--rw-rw-rw-   0        0        0     2806 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/api/utils/web_file_downloader.py
--rw-rw-rw-   0        0        0     1086 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/valid_search_modes.py
--rw-rw-rw-   0        0        0     3097 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/api/vocabulary_categories.py
--rw-rw-rw-   0        0        0      218 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.125290 cript-2.2.0/src/cript/nodes/
--rw-rw-rw-   0        0        0      615 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/nodes/__init__.py
--rw-rw-rw-   0        0        0    27542 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/core.py
--rw-rw-rw-   0        0        0    14596 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.141700 cript-2.2.0/src/cript/nodes/primary_nodes/
--rw-rw-rw-   0        0        0      617 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/nodes/primary_nodes/__init__.py
--rw-rw-rw-   0        0        0     9802 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/collection.py
--rw-rw-rw-   0        0        0    15260 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/computation.py
--rw-rw-rw-   0        0        0    19577 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/computation_process.py
--rw-rw-rw-   0        0        0    21096 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/data.py
--rw-rw-rw-   0        0        0    14279 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/experiment.py
--rw-rw-rw-   0        0        0     4863 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/inventory.py
--rw-rw-rw-   0        0        0    15326 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/material.py
--rw-rw-rw-   0        0        0     3010 2023-10-19 18:28:20.000000 cript-2.2.0/src/cript/nodes/primary_nodes/primary_base_node.py
--rw-rw-rw-   0        0        0    21532 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/process.py
--rw-rw-rw-   0        0        0     8529 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/project.py
--rw-rw-rw-   0        0        0    20446 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/primary_nodes/reference.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.157375 cript-2.2.0/src/cript/nodes/subobjects/
--rw-rw-rw-   0        0        0      683 2023-10-06 19:50:55.000000 cript-2.2.0/src/cript/nodes/subobjects/__init__.py
--rw-rw-rw-   0        0        0     9327 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/algorithm.py
--rw-rw-rw-   0        0        0     8216 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/citation.py
--rw-rw-rw-   0        0        0    17454 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/computational_forcefield.py
--rw-rw-rw-   0        0        0    16708 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/condition.py
--rw-rw-rw-   0        0        0    10380 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/equipment.py
--rw-rw-rw-   0        0        0     7703 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/ingredient.py
--rw-rw-rw-   0        0        0     6202 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/parameter.py
--rw-rw-rw-   0        0        0    24625 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/property.py
--rw-rw-rw-   0        0        0     8053 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/quantity.py
--rw-rw-rw-   0        0        0     5298 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/software.py
--rw-rw-rw-   0        0        0     9519 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/subobjects/software_configuration.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.157375 cript-2.2.0/src/cript/nodes/supporting_nodes/
--rw-rw-rw-   0        0        0      132 2023-10-06 19:50:56.000000 cript-2.2.0/src/cript/nodes/supporting_nodes/__init__.py
--rw-rw-rw-   0        0        0    16826 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/supporting_nodes/file.py
--rw-rw-rw-   0        0        0     4409 2023-10-06 19:50:56.000000 cript-2.2.0/src/cript/nodes/supporting_nodes/user.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.157375 cript-2.2.0/src/cript/nodes/util/
--rw-rw-rw-   0        0        0    21136 2023-11-17 19:59:37.000000 cript-2.2.0/src/cript/nodes/util/__init__.py
--rw-rw-rw-   0        0        0     2339 2023-10-06 19:50:56.000000 cript-2.2.0/src/cript/nodes/util/material_deserialization.py
--rw-rw-rw-   0        0        0     2083 2023-11-06 23:33:25.000000 cript-2.2.0/src/cript/nodes/uuid_base.py
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.093725 cript-2.2.0/src/cript.egg-info/
--rw-rw-rw-   0        0        0     5762 2023-11-17 20:40:09.000000 cript-2.2.0/src/cript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2068 2023-11-17 20:40:09.000000 cript-2.2.0/src/cript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 20:40:09.000000 cript-2.2.0/src/cript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-11-17 20:40:09.000000 cript-2.2.0/src/cript.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-11-17 20:40:09.000000 cript-2.2.0/src/cript.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-17 20:40:09.157375 cript-2.2.0/tests/
--rw-rw-rw-   0        0        0    14184 2023-11-17 19:59:37.000000 cript-2.2.0/tests/test_node_util.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.763323 cript-2.3.0/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1122 2023-08-30 00:21:45.000000 cript-2.3.0/LICENSE.md
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5659 2024-04-01 18:48:28.763323 cript-2.3.0/PKG-INFO
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5012 2024-02-21 00:00:01.000000 cript-2.3.0/README.md
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      346 2023-08-30 00:21:45.000000 cript-2.3.0/pyproject.toml
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      762 2024-04-01 18:48:28.763323 cript-2.3.0/setup.cfg
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)       69 2023-08-30 00:21:45.000000 cript-2.3.0/setup.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.755323 cript-2.3.0/src/
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.755323 cript-2.3.0/src/cript/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      849 2024-03-25 21:02:04.000000 cript-2.3.0/src/cript/__init__.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/api/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      219 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    40944 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/api/api.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      316 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/api_config.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9155 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/data_schema.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10793 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/exceptions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9520 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/paginator.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/api/utils/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      137 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/api/utils/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1310 2024-02-21 00:00:01.000000 cript-2.3.0/src/cript/api/utils/aws_s3_utils.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1990 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/api/utils/get_host_token.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1302 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/utils/helper_functions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8399 2024-02-21 21:14:12.000000 cript-2.3.0/src/cript/api/utils/save_helper.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2806 2023-09-11 22:06:53.000000 cript-2.3.0/src/cript/api/utils/web_file_downloader.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     1035 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/valid_search_modes.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3006 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/api/vocabulary_categories.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      218 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/exceptions.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      615 2024-03-25 21:02:04.000000 cript-2.3.0/src/cript/nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    27915 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/core.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14386 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/exceptions.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2296 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/node_iterator.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/primary_nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      617 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/primary_nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9735 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/collection.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    15136 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/computation.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19308 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/computation_process.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    20789 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/data.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14052 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/experiment.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4825 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/inventory.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21826 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/primary_nodes/material.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2891 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/primary_nodes/primary_base_node.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    21207 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/process.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8528 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/primary_nodes/project.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    19736 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/primary_nodes/reference.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/subobjects/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      683 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/subobjects/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9286 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/algorithm.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     8103 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/citation.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    17261 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/computational_forcefield.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16294 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/condition.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    10346 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/equipment.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7580 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/ingredient.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     6017 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/parameter.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    24342 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/property.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     7819 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/quantity.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5126 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/software.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     9502 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/subobjects/software_configuration.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/supporting_nodes/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      132 2023-08-30 00:21:45.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    16377 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/file.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     4439 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/supporting_nodes/user.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript/nodes/util/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)      234 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/util/__init__.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     3398 2024-04-01 18:45:13.000000 cript-2.3.0/src/cript/nodes/util/core.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    18567 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/util/json.py
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2886 2024-04-01 16:46:26.000000 cript-2.3.0/src/cript/nodes/uuid_base.py
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/src/cript.egg-info/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     5659 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/PKG-INFO
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)     2139 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)        1 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)       68 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/requires.txt
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)        6 2024-04-01 18:48:28.000000 cript-2.3.0/src/cript.egg-info/top_level.txt
+drwxr-xr-x   0 ludwig    (1000) ludwig    (1000)        0 2024-04-01 18:48:28.759323 cript-2.3.0/tests/
+-rw-r--r--   0 ludwig    (1000) ludwig    (1000)    14716 2024-04-01 18:45:13.000000 cript-2.3.0/tests/test_node_util.py
```

### Comparing `cript-2.2.0/LICENSE.md` & `cript-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/PKG-INFO` & `cript-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-Metadata-Version: 2.1
-Name: cript
-Version: 2.2.0
-Summary: CRIPT Python SDK
-Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
-Author: CRIPT Development Team
-License: MIT
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests==2.31.0
-Requires-Dist: jsonschema>=4.17.3
-Requires-Dist: beartype==0.14.1
-Requires-Dist: boto3==1.28.39
-
-# CRIPT Python SDK
-
-[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-
-[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
-[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
-[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
-[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
-[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
-[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
-[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
-
-[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
-[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
-[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
-
-<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
-
-<!-- just shows pass/fail instead of percentage
-[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
--->
-
-## CRIPT Availability
-
-Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
-
----
-
-## What is it?
-
-The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
-
----
-
-## Installation
-
-CRIPT Python SDK requires Python 3.8+
-
-The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
-
-```bash
-pip install cript
-```
-
----
-
-## Documentation
-
-To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
-
-To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
-
----
-
-## Release Notes
-
-Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
-
----
-
-## We Invite Contribution
-
-To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
-a detailed guide on how to contribute to our repository and become a part of our community.
-
-Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
-
-For development documentation to better understand the Python SDK code please visit the
-[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
-If you encounter any issues please let us know via
-[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
-[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
-
-To learn more about our great community and all the open source plugins made by our fantastic community available
-for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
-[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
-
-We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
-
-Happy coding!
+Metadata-Version: 2.1
+Name: cript
+Version: 2.3.0
+Summary: CRIPT Python SDK
+Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
+Author: CRIPT Development Team
+License: MIT
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: requests==2.31.0
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: beartype==0.14.1
+Requires-Dist: boto3==1.28.39
+
+# CRIPT Python SDK
+
+[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+
+[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
+[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
+[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
+[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
+[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
+[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
+
+[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
+[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
+[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
+
+<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
+
+<!-- just shows pass/fail instead of percentage
+[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
+-->
+
+## CRIPT Availability
+
+Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
+
+---
+
+## What is it?
+
+The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
+
+---
+
+## Installation
+
+CRIPT Python SDK requires Python 3.8+
+
+The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
+
+```bash
+pip install cript
+```
+
+---
+
+## Documentation
+
+To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
+
+To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
+
+---
+
+## Release Notes
+
+Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
+
+---
+
+## We Invite Contribution
+
+To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
+a detailed guide on how to contribute to our repository and become a part of our community.
+
+Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
+
+For development documentation to better understand the Python SDK code please visit the
+[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
+If you encounter any issues please let us know via
+[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
+[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
+
+To learn more about our great community and all the open source plugins made by our fantastic community available
+for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
+[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
+
+We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
+
+Happy coding!
```

### Comparing `cript-2.2.0/README.md` & `cript-2.3.0/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-# CRIPT Python SDK
-
-[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-
-[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
-[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
-[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
-[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
-[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
-[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
-[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
-
-[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
-[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
-[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
-
-<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
-
-<!-- just shows pass/fail instead of percentage
-[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
--->
-
-## CRIPT Availability
-
-Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
-
----
-
-## What is it?
-
-The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
-
----
-
-## Installation
-
-CRIPT Python SDK requires Python 3.8+
-
-The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
-
-```bash
-pip install cript
-```
-
----
-
-## Documentation
-
-To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
-
-To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
-
----
-
-## Release Notes
-
-Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
-
----
-
-## We Invite Contribution
-
-To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
-a detailed guide on how to contribute to our repository and become a part of our community.
-
-Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
-
-For development documentation to better understand the Python SDK code please visit the
-[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
-If you encounter any issues please let us know via
-[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
-[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
-
-To learn more about our great community and all the open source plugins made by our fantastic community available
-for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
-[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
-
-We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
-
-Happy coding!
+# CRIPT Python SDK
+
+[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+
+[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
+[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
+[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
+[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
+[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
+[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
+
+[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
+[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
+[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
+
+<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
+
+<!-- just shows pass/fail instead of percentage
+[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
+-->
+
+## CRIPT Availability
+
+Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
+
+---
+
+## What is it?
+
+The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
+
+---
+
+## Installation
+
+CRIPT Python SDK requires Python 3.8+
+
+The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
+
+```bash
+pip install cript
+```
+
+---
+
+## Documentation
+
+To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
+
+To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
+
+---
+
+## Release Notes
+
+Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
+
+---
+
+## We Invite Contribution
+
+To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
+a detailed guide on how to contribute to our repository and become a part of our community.
+
+Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
+
+For development documentation to better understand the Python SDK code please visit the
+[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
+If you encounter any issues please let us know via
+[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
+[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
+
+To learn more about our great community and all the open source plugins made by our fantastic community available
+for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
+[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
+
+We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
+
+Happy coding!
```

### Comparing `cript-2.2.0/src/cript/api/api.py` & `cript-2.3.0/src/cript/api/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1301 +1,1002 @@
-import copy
-import json
-import logging
-import os
-import uuid
-import warnings
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
-
-import boto3
-import jsonschema
-import requests
-from beartype import beartype
-
-from cript.api.api_config import _API_TIMEOUT
-from cript.api.exceptions import (
-    APIError,
-    CRIPTAPIRequiredError,
-    CRIPTAPISaveError,
-    CRIPTConnectionError,
-    CRIPTDuplicateNameError,
-    InvalidHostError,
-    InvalidVocabulary,
-)
-from cript.api.paginator import Paginator
-from cript.api.utils.aws_s3_utils import get_s3_client
-from cript.api.utils.get_host_token import resolve_host_and_token
-from cript.api.utils.helper_functions import _get_node_type_from_json
-from cript.api.utils.save_helper import (
-    _fix_node_save,
-    _get_uuid_from_error_message,
-    _identify_suppress_attributes,
-    _InternalSaveValues,
-)
-from cript.api.utils.web_file_downloader import download_file_from_url
-from cript.api.valid_search_modes import SearchModes
-from cript.api.vocabulary_categories import VocabCategories
-from cript.nodes.exceptions import CRIPTNodeSchemaError
-from cript.nodes.primary_nodes.project import Project
-
-# Do not use this directly! That includes devs.
-# Use the `_get_global_cached_api for access.
-_global_cached_api = None
-
-
-def _get_global_cached_api():
-    """
-    Read-Only access to the globally cached API object.
-    Raises an exception if no global API object is cached yet.
-    """
-    if _global_cached_api is None:
-        raise CRIPTAPIRequiredError()
-    return _global_cached_api
-
-
-class API:
-    """
-    ## Definition
-    API Client class to communicate with the CRIPT API
-    """
-
-    # dictates whether the user wants to see terminal log statements or not
-    _verbose: bool = True
-    logger: logging.Logger = None  # type: ignore
-
-    _host: str = ""
-    _api_token: str = ""
-    _storage_token: str = ""
-    _http_headers: dict = {}
-    _vocabulary: dict = {}
-    _db_schema: dict = {}
-    _api_prefix: str = "api"
-    _api_version: str = "v1"
-
-    # trunk-ignore-begin(cspell)
-    # AWS S3 constants
-    _REGION_NAME: str = "us-east-1"
-    _IDENTITY_POOL_ID: str = "us-east-1:9426df38-994a-4191-86ce-3cb0ce8ac84d"
-    _COGNITO_LOGIN_PROVIDER: str = "cognito-idp.us-east-1.amazonaws.com/us-east-1_SZGBXPl2j"
-    _BUCKET_NAME: str = "cript-user-data"
-    _BUCKET_DIRECTORY_NAME: str = "python_sdk_files"
-    _internal_s3_client: Any = None  # type: ignore
-    # trunk-ignore-end(cspell)
-
-    # Advanced User Tip: Disabling Node Validation
-    # For experienced users, deactivating node validation during creation can be a time-saver.
-    # Note that the complete node graph will still undergo validation before being saved to the back end.
-    # Caution: It's advisable to keep validation active while debugging scripts, as disabling it can delay error notifications and complicate the debugging process.
-    skip_validation: bool = False
-
-    @beartype
-    def __init__(self, host: Union[str, None] = None, api_token: Union[str, None] = None, storage_token: Union[str, None] = None, config_file_path: Union[str, Path] = ""):
-        """
-        Initialize CRIPT API client with host and token.
-        Additionally, you can  use a config.json file and specify the file path.
-
-        !!! note "api client context manager"
-            It is necessary to use a `with` context manager for the API
-
-        Examples
-        --------
-        ### Create API client with host and token
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...    # node creation, api.save(), etc.
-        ...    pass
-
-
-        ---
-
-        ### Creating API Client
-        !!! Warning "Token Security"
-            It is **highly** recommended that you store your API tokens in a safe location and read it into your code
-            Hard-coding API tokens directly into the code can pose security risks,
-            as the token might be exposed if the code is shared or stored in a version control system.
-            Anyone that has access to your tokens can impersonate you on the CRIPT platform
-
-        ### Create API Client with Environment Variables
-
-        Another great way to keep sensitive information secure is by using
-        [environment variables](https://www.freecodecamp.org/news/python-env-vars-how-to-get-an-environment-variable-in-python/).
-        Sensitive information can be securely stored in environment variables and loaded into the code using
-        [os.getenv()](https://docs.python.org/3/library/os.html#os.getenv).
-
-        Examples
-        --------
-        >>> import cript
-        >>> import os
-        >>> # securely load sensitive data into the script
-        >>> cript_host = os.getenv("cript_host")
-        >>> cript_api_token = os.getenv("cript_api_token")
-        >>> cript_storage_token = os.getenv("cript_storage_token")
-        >>> with cript.API(
-        ...     host=cript_host, api_token=cript_api_token, storage_token=cript_storage_token
-        ... ) as api:
-        ...     pass
-
-        ### Create API Client with None
-        Alternatively you can configure your system to have an environment variable of
-        `CRIPT_TOKEN` for the API token and `CRIPT_STORAGE_TOKEN` for the storage token, then
-        initialize `cript.API` `api_token` and `storage_token` with `None`.
-
-        The CRIPT Python SDK will try to read the API Token and Storage token from your system's environment variables.
-
-        ```python
-        with cript.API(host=cript_host, api_token=None, storage_token=None) as api:
-            # write your script
-            pass
-        ```
-
-        ### Create API client with config.json
-        `config.json`
-        ```json
-        {
-            "host": "https://api.criptapp.org/",
-            "api_token": "I am API token",
-            "storage_token": "I am storage token"
-        }
-        ```
-
-        Examples
-        --------
-        `my_script.py`
-        >>> from pathlib import Path
-        >>> import cript
-        >>> # create a file path object of where the config file is
-        >>> config_file_path = Path(__file__) / Path('./config.json')
-        >>> with cript.API(config_file_path=config_file_path) as api:   # doctest: +SKIP
-        ...     # node creation, api.save(), etc.
-        ...     pass
-
-        Parameters
-        ----------
-        host : str, None
-            CRIPT host for the Python SDK to connect to such as https://api.criptapp.org/`
-            This host address is the same address used to login to cript website.
-            If `None` is specified, the host is inferred from the environment variable `CRIPT_HOST`.
-        api_token : str, None
-            CRIPT API Token used to connect to CRIPT and upload all data with the exception to file upload that needs
-            a different token.
-            You can find your personal token on the cript website at User > Security Settings.
-            The user icon is in the top right.
-            If `None` is specified, the token is inferred from the environment variable `CRIPT_TOKEN`.
-        storage_token: str
-            This token is used to upload local files to CRIPT cloud storage when needed
-        config_file_path: str
-            the file path to the config.json file where the token and host can be found
-
-
-        Notes
-        -----
-        * if `host=None` and `token=None`
-            then the Python SDK will grab the host from the users environment variable of `"CRIPT_HOST"`
-            and `"CRIPT_TOKEN"`
-
-        Warns
-        -----
-        UserWarning
-            If `host` is using "http" it gives the user a warning that HTTP is insecure and the user should use HTTPS
-
-        Raises
-        ------
-        CRIPTConnectionError
-            If it cannot connect to CRIPT with the provided host and token a CRIPTConnectionError is thrown.
-
-        Returns
-        -------
-        None
-            Instantiate a new CRIPT API object
-        """
-
-        # if there is a config.json file or any of the parameters are None, then get the variables from file or env vars
-        if config_file_path or (host is None or api_token is None or storage_token is None):
-            authentication_dict: Dict[str, str] = resolve_host_and_token(host, api_token=api_token, storage_token=storage_token, config_file_path=config_file_path)
-
-            host = authentication_dict["host"]
-            api_token = authentication_dict["api_token"]
-            storage_token = authentication_dict["storage_token"]
-
-        self._host = self._prepare_host(host=host)  # type: ignore
-        self._api_token = api_token  # type: ignore
-        self._storage_token = storage_token  # type: ignore
-
-        # add Bearer to token for HTTP requests
-        self._http_headers = {"Authorization": f"Bearer {self._api_token}", "Content-Type": "application/json"}
-
-        # check that api can connect to CRIPT with host and token
-        self._check_initial_host_connection()
-
-        self._get_db_schema()
-
-        # set a logger instance to use for the class logs
-        self._set_logger()
-
-    def __str__(self) -> str:
-        """
-        States the host of the CRIPT API client
-
-        Examples
-        --------
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...     print(api)
-        CRIPT API Client - Host URL: 'https://api.criptapp.org/api/v1'
-
-        Returns
-        -------
-        str
-        """
-        return f"CRIPT API Client - Host URL: '{self.host}'"
-
-    def _set_logger(self, verbose: bool = True) -> None:
-        """
-        Prepare and configure the logger for the API class.
-
-        This function creates and configures a logger instance associated with the current module (class).
-
-        Parameters
-        ----------
-        verbose: bool default True
-            set if you want `cript.API` to give logs to console or not
-
-        Returns
-        -------
-        logging.Logger
-            The configured logger instance.
-        """
-        # Create a logger instance associated with the current module
-        logger = logging.getLogger(__name__)
-
-        # Set the logger's level based on the verbose flag
-        if verbose:
-            logger.setLevel(logging.INFO)  # Display INFO logs
-        else:
-            logger.setLevel(logging.CRITICAL)  # Display no logs
-
-        # Create a console handler
-        console_handler = logging.StreamHandler()
-
-        # Create a formatter for log messages (customize the format as desired)
-        formatter = logging.Formatter("%(levelname)s: %(message)s")
-
-        # Associate the formatter with the console handler
-        console_handler.setFormatter(formatter)
-
-        # Add the console handler to the logger
-        logger.addHandler(console_handler)
-
-        # set logger for the class
-        self.logger = logger
-
-    @property
-    def verbose(self) -> bool:
-        """
-        A boolean flag that controls whether verbose logging is enabled or not.
-
-        When `verbose` is set to `True`, the class will provide additional detailed logging
-        to the terminal. This can be useful for debugging and understanding the internal
-        workings of the class.
-
-        ```bash
-        INFO: Validating Project graph...
-        ```
-
-        When `verbose` is set to `False`, the class will only provide essential logging information,
-        making the terminal output less cluttered and more user-friendly.
-
-        Examples
-        --------
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...     # turn off the terminal logs
-        ...     api.verbose = False
-
-        Returns
-        -------
-        bool
-            verbose boolean value
-        """
-        return self._verbose
-
-    @verbose.setter
-    def verbose(self, new_verbose_value: bool) -> None:
-        """
-        sets the verbose value and then sets a new logger for the class
-
-        Parameters
-        ----------
-        new_verbose_value: bool
-            new verbose value to turn the logging ON or OFF
-
-        Returns
-        -------
-        None
-        """
-        self._verbose = new_verbose_value
-        self._set_logger(verbose=new_verbose_value)
-
-    @beartype
-    def _prepare_host(self, host: str) -> str:
-        """
-        Takes the host URL provided by the user during API object construction (e.g., `https://api.criptapp.org`)
-        and standardizes it for internal use. Performs any required string manipulation to ensure uniformity.
-
-        Parameters
-        ----------
-        host: str
-            The host URL specified during API initialization, typically in the form `https://api.criptapp.org`.
-
-        Warnings
-        --------
-        If the specified host uses the unsafe "http://" protocol, a warning will be raised to consider using HTTPS.
-
-        Raises
-        ------
-        InvalidHostError
-            If the host string does not start with either "http" or "https", an InvalidHostError will be raised.
-            Only HTTP protocol is acceptable at this time.
-
-        Returns
-        -------
-        str
-            A standardized host string formatted for internal use.
-
-        """
-        # strip ending slash to make host always uniform
-        host = host.rstrip("/")
-        host = f"{host}/{self._api_prefix}/{self._api_version}"
-
-        # if host is using unsafe "http://" then give a warning
-        if host.startswith("http://"):
-            warnings.warn("HTTP is an unsafe protocol please consider using HTTPS.")
-
-        if not host.startswith("http"):
-            raise InvalidHostError()
-
-        return host
-
-    # Use a property to ensure delayed init of s3_client
-    @property
-    def _s3_client(self) -> boto3.client:  # type: ignore
-        """
-        Property to use when wanting to interact with AWS S3.
-
-        Gets a fully authenticated AWS S3 client if it was never created and stash it,
-        if the AWS S3 client has been created before, then returns the client that it has
-
-        Returns
-        -------
-        s3_client: boto3.client
-            fully prepared and authenticated s3 client ready to be used throughout the script
-        """
-        if self._internal_s3_client is None:
-            self._internal_s3_client = get_s3_client(region_name=self._REGION_NAME, identity_pool_id=self._IDENTITY_POOL_ID, cognito_login_provider=self._COGNITO_LOGIN_PROVIDER, storage_token=self._storage_token)
-
-        return self._internal_s3_client
-
-    def __enter__(self):
-        self.connect()
-        return self
-
-    @beartype
-    def __exit__(self, type, value, traceback):
-        self.disconnect()
-
-    def connect(self):
-        """
-        Connect this API globally as the current active access point.
-        It is not necessary to call this function manually if a context manager is used.
-        A context manager is preferred where possible.
-        Jupyter notebooks are a use case where this connection can be handled manually.
-        If this function is called manually, the `API.disconnect` function has to be called later.
-
-        For manual connection: nested API object are discouraged.
-        """
-        # Store the last active global API (might be None)
-        global _global_cached_api
-        self._previous_global_cached_api = copy.copy(_global_cached_api)
-        _global_cached_api = self
-        return self
-
-    def disconnect(self):
-        """
-        Disconnect this API from the active access point.
-        It is not necessary to call this function manually if a context manager is used.
-        A context manager is preferred where possible.
-        Jupyter notebooks are a use case where this connection can be handled manually.
-        This function has to be called manually if  the `API.connect` function has to be called before.
-
-        For manual connection: nested API object are discouraged.
-        """
-        # Restore the previously active global API (might be None)
-        global _global_cached_api
-        _global_cached_api = self._previous_global_cached_api
-
-    @property
-    def schema(self):
-        """
-        Access the CRIPT Database Schema that is associated with this API connection.
-        The CRIPT Database Schema is used  to validate a node's JSON so that it is compatible with the CRIPT API.
-        """
-        return self._db_schema
-
-    @property
-    def host(self):
-        """
-        Read only access to the currently connected host.
-
-        The term "host" designates the specific CRIPT instance to which you intend to upload your data.
-
-        For most users, the host will be `https://api.criptapp.org`
-
-        ```yaml
-        host: https://api.criptapp.org
-        ```
-
-        Examples
-        --------
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...    print(api.host)
-        https://api.criptapp.org/api/v1
-        """
-        return self._host
-
-    def _check_initial_host_connection(self) -> None:
-        """
-        tries to create a connection with host and if the host does not respond or is invalid it raises an error
-
-        Raises
-        -------
-        CRIPTConnectionError
-            raised when the host does not give the expected response
-
-        Returns
-        -------
-        None
-        """
-        try:
-            pass
-        except Exception as exc:
-            raise CRIPTConnectionError(self.host, self._api_token) from exc
-
-    def _get_vocab(self) -> dict:
-        """
-        gets the entire CRIPT controlled vocabulary and stores it in _vocabulary
-
-        1. loops through all controlled vocabulary categories
-            1. if the category already exists in the controlled vocabulary then skip that category and continue
-            1. if the category does not exist in the `_vocabulary` dict,
-            then request it from the API and append it to the `_vocabulary` dict
-        1. at the end the `_vocabulary` should have all the controlled vocabulary and that will be returned
-
-           Examples
-           --------
-           The vocabulary looks like this
-           ```json
-           {'algorithm_key':
-                [
-                    {
-                    'description': "Velocity-Verlet integration algorithm. Parameters: 'integration_timestep'.",
-                    'name': 'velocity_verlet'
-                    },
-            }
-           ```
-        """
-
-        # loop through all vocabulary categories and make a request to each vocabulary category
-        # and put them all inside of self._vocab with the keys being the vocab category name
-        for category in VocabCategories:
-            if category in self._vocabulary:
-                continue
-
-            self._vocabulary[category.value] = self.get_vocab_by_category(category)
-
-        return self._vocabulary
-
-    @beartype
-    def get_vocab_by_category(self, category: VocabCategories) -> List[dict]:
-        """
-        get the CRIPT controlled vocabulary by category
-
-        Examples
-        --------
-        >>> import os
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...     api.get_vocab_by_category(cript.VocabCategories.MATERIAL_IDENTIFIER_KEY)  # doctest: +SKIP
-
-        Parameters
-        ----------
-        category: str
-            category of
-
-        Returns
-        -------
-        List[dict]
-            list of JSON containing the controlled vocabulary
-        """
-
-        # check if the vocabulary category is already cached
-        if category.value in self._vocabulary:
-            return self._vocabulary[category.value]
-
-        vocabulary_category_url: str = f"{self.host}/cv/{category.value}/"
-
-        # if vocabulary category is not in cache, then get it from API and cache it
-        response: Dict = requests.get(url=vocabulary_category_url, timeout=_API_TIMEOUT).json()
-
-        if response["code"] != 200:
-            raise APIError(api_error=str(response), http_method="GET", api_url=vocabulary_category_url)
-
-        # add to cache
-        self._vocabulary[category.value] = response["data"]
-
-        return self._vocabulary[category.value]
-
-    @beartype
-    def _is_vocab_valid(self, vocab_category: VocabCategories, vocab_word: str) -> bool:
-        """
-        checks if the vocabulary is valid within the CRIPT controlled vocabulary.
-        Either returns True or InvalidVocabulary Exception
-
-        1. if the vocabulary is custom (starts with "+")
-            then it is automatically valid
-        2. if vocabulary is not custom, then it is checked against its category
-            if the word cannot be found in the category then it returns False
-
-        Parameters
-        ----------
-        vocab_category: VocabCategories
-            ControlledVocabularyCategories enums
-        vocab_word: str
-            the vocabulary word e.g. "CAS", "SMILES", "BigSmiles", "+my_custom_key"
-
-        Returns
-        -------
-        a boolean of if the vocabulary is valid
-
-        Raises
-        ------
-        InvalidVocabulary
-            If the vocabulary is invalid then the error gets raised
-        """
-
-        # check if vocab is custom
-        # This is deactivated currently, no custom vocab allowed.
-        if vocab_word.startswith("+"):
-            return True
-
-        # get the entire vocabulary
-        controlled_vocabulary = self._get_vocab()
-        # get just the category needed
-        controlled_vocabulary = controlled_vocabulary[vocab_category.value]
-
-        # TODO this can be faster with a dict of dicts that can do o(1) look up
-        #  looping through an unsorted list is an O(n) look up which is slow
-        # loop through the list
-        for vocab_dict in controlled_vocabulary:
-            # check the name exists within the dict
-            if vocab_dict.get("name") == vocab_word:
-                return True
-
-        raise InvalidVocabulary(vocab=vocab_word, possible_vocab=list(controlled_vocabulary))
-
-    def _get_db_schema(self) -> dict:
-        """
-        Sends a GET request to CRIPT to get the database schema and returns it.
-        The database schema can be used for validating the JSON request
-        before submitting it to CRIPT.
-
-        1. checks if the db schema is already set
-            * if already exists then it skips fetching it from the API and just returns what it already has
-        2. if db schema has not been set yet, then it fetches it from the API
-            * after getting it from the API it saves it in the `_schema` class variable,
-            so it can be easily and efficiently gotten next time
-        """
-
-        # check if db schema is already saved
-        if bool(self._db_schema):
-            return self._db_schema
-
-        # fetch db_schema from API
-        else:
-            # fetch db schema from API
-            response: requests.Response = requests.get(url=f"{self.host}/schema/", timeout=_API_TIMEOUT)
-
-            # raise error if not HTTP 200
-            response.raise_for_status()
-
-            # if no error, take the JSON from the API response
-            response_dict: Dict = response.json()
-
-            # get the data from the API JSON response
-            self._db_schema = response_dict["data"]
-            return self._db_schema
-
-    @beartype
-    def _is_node_schema_valid(self, node_json: str, is_patch: bool = False, force_validation: bool = False) -> Union[bool, None]:
-        """
-        checks a node JSON schema against the db schema to return if it is valid or not.
-
-        1. get db schema
-        1. convert node_json str to dict
-        1. take out the node type from the dict
-            1. "node": ["material"]
-        1. use the node type from dict to tell the db schema which node schema to validate against
-            1. Manipulates the string to be title case to work with db schema
-
-        Parameters
-        ----------
-        node_json: str
-            a node in JSON form string
-        is_patch: bool
-            a boolean flag checking if it needs to validate against `NodePost` or `NodePatch`
-
-        Notes
-        -----
-        This function does not take into consideration vocabulary validation.
-            For vocabulary validation please check `is_vocab_valid`
-
-        Raises
-        ------
-        CRIPTNodeSchemaError
-            in case a node is invalid
-
-        Returns
-        -------
-        bool
-            whether the node JSON is valid or not
-        """
-
-        # Fast exit without validation
-        if self.skip_validation and not force_validation:
-            return None
-
-        db_schema = self._get_db_schema()
-
-        node_type: str = _get_node_type_from_json(node_json=node_json)
-
-        node_dict = json.loads(node_json)
-
-        # logging out info to the terminal for the user feedback
-        # (improve UX because the program is currently slow)
-        log_message = f"Validating {node_type} graph..."
-        if force_validation:
-            log_message = "Forced: " + log_message + " if error occur, try setting `cript.API.skip_validation = False` for debugging."
-        else:
-            log_message += " (Can be disabled by setting `cript.API.skip_validation = True`.)"
-
-        self.logger.info(log_message)
-
-        # set the schema to test against http POST or PATCH of DB Schema
-        schema_http_method: str
-
-        if is_patch:
-            schema_http_method = "Patch"
-        else:
-            schema_http_method = "Post"
-
-        # set which node you are using schema validation for
-        db_schema["$ref"] = f"#/$defs/{node_type}{schema_http_method}"
-
-        try:
-            jsonschema.validate(instance=node_dict, schema=db_schema)
-        except jsonschema.exceptions.ValidationError as error:
-            raise CRIPTNodeSchemaError(node_type=node_dict["node"], json_schema_validation_error=str(error)) from error
-
-        # if validation goes through without any problems return True
-        return True
-
-    def save(self, project: Project) -> None:
-        """
-        This method takes a project node, serializes the class into JSON
-        and then sends the JSON to be saved to the API.
-        It takes Project node because everything is connected to the Project node,
-        and it can be used to send either a POST or PATCH request to API
-
-        Parameters
-        ----------
-        project: Project
-            the Project Node that the user wants to save
-
-        Raises
-        ------
-        CRIPTAPISaveError
-            If the API responds with anything other than an HTTP of `200`, the API error is displayed to the user
-
-        Returns
-        -------
-        A set of extra saved node UUIDs.
-            Just sends a `POST` or `Patch` request to the API
-        """
-        try:
-            self._internal_save(project)
-        except CRIPTAPISaveError as exc:
-            if exc.pre_saved_nodes:
-                for node_uuid in exc.pre_saved_nodes:
-                    # TODO remove all pre-saved nodes by their uuid.
-                    pass
-            raise exc from exc
-
-    def _internal_save(self, node, save_values: Optional[_InternalSaveValues] = None) -> _InternalSaveValues:
-        """
-        Internal helper function that handles the saving of different nodes (not just project).
-
-        If a "Bad UUID" error happens, we find that node with the UUID and save it first.
-        Then we recursively call the _internal_save again.
-        Because it is recursive, this repeats until no "Bad UUID" error happen anymore.
-        This works, because we keep track of "Bad UUID" handled nodes, and represent them in the JSON only as the UUID.
-        """
-
-        if save_values is None:
-            save_values = _InternalSaveValues()
-
-        # saves all the local files to cloud storage right before saving the Project node
-        # Ensure that all file nodes have uploaded there payload before actual save.
-        for file_node in node.find_children({"node": ["File"]}):
-            file_node.ensure_uploaded(api=self)
-
-        node.validate(force_validation=True)
-
-        # Dummy response to have a virtual do-while loop, instead of while loop.
-        response = {"code": -1}
-        # TODO remove once get works properly
-        force_patch = False
-
-        while response["code"] != 200:
-            # Keep a record of how the state was before the loop
-            old_save_values = copy.deepcopy(save_values)
-            # We assemble the JSON to be saved to back end.
-            # Note how we exclude pre-saved uuid nodes.
-            json_data = node.get_json(known_uuid=save_values.saved_uuid, suppress_attributes=save_values.suppress_attributes).json
-
-            # This checks if the current node exists on the back end.
-            # if it does exist we use `patch` if it doesn't `post`.
-            test_get_response: Dict = requests.get(url=f"{self._host}/{node.node_type_snake_case}/{str(node.uuid)}/", headers=self._http_headers, timeout=_API_TIMEOUT).json()
-            patch_request = test_get_response["code"] == 200
-
-            # TODO remove once get works properly
-            if not patch_request and force_patch:
-                patch_request = True
-                force_patch = False
-            # TODO activate patch validation
-            # node.validate(is_patch=patch_request)
-
-            # If all that is left is a UUID, we don't need to save it, we can just exit the loop.
-            if patch_request and len(json.loads(json_data)) == 1:
-                response = {"code": 200}
-                break
-
-            if patch_request:
-                response: Dict = requests.patch(url=f"{self._host}/{node.node_type_snake_case}/{str(node.uuid)}/", headers=self._http_headers, data=json_data, timeout=_API_TIMEOUT).json()  # type: ignore
-            else:
-                response: Dict = requests.post(url=f"{self._host}/{node.node_type_snake_case}/", headers=self._http_headers, data=json_data, timeout=_API_TIMEOUT).json()  # type: ignore
-
-            # If we get an error we may be able to fix, we to handle this extra and save the bad node first.
-            # Errors with this code, may be fixable
-            if response["code"] in (400, 409):
-                try:
-                    returned_save_values = _fix_node_save(self, node, response, save_values)
-                except CRIPTAPISaveError as exc:
-                    # If the previous error was a duplicated name issue
-                    if "duplicate item [{'name':" in str(response["error"]):
-                        # And (second condition) the request failed bc of the now suppressed name
-                        if "'name' is a required property" in exc.api_response:
-                            # Raise a save error, with the nice name related error message
-                            raise CRIPTDuplicateNameError(response, json_data, exc) from exc
-                    # Else just raise the exception as normal.
-                    raise exc
-
-                save_values += returned_save_values
-
-            # Handle errors from patching with too many attributes
-            if patch_request and response["code"] in (400,):
-                suppress_attributes = _identify_suppress_attributes(node, response)
-                new_save_values = _InternalSaveValues(save_values.saved_uuid, suppress_attributes)
-                save_values += new_save_values
-
-            # It is only worthwhile repeating the attempted save loop if our state has improved.
-            # Aka we did something to fix the occurring error
-            if not save_values > old_save_values:
-                # TODO remove once get works properly
-                if not patch_request and response["code"] == 409 and response["error"].strip().startswith("Duplicate uuid:"):  # type: ignore
-                    duplicate_uuid = _get_uuid_from_error_message(response["error"])  # type: ignore
-                    if str(node.uuid) == duplicate_uuid:
-                        force_patch = True
-                        continue
-
-                break
-
-        if response["code"] != 200:
-            raise CRIPTAPISaveError(api_host_domain=self._host, http_code=response["code"], api_response=response["error"], patch_request=patch_request, pre_saved_nodes=save_values.saved_uuid, json_data=json_data)  # type: ignore
-
-        save_values.saved_uuid.add(str(node.uuid))
-        return save_values
-
-    def upload_file(self, file_path: Union[Path, str]) -> str:
-        # trunk-ignore-begin(cspell)
-        """
-        uploads a file to AWS S3 bucket and returns a URL of the uploaded file in AWS S3
-        The URL is has no expiration time limit and is available forever
-
-        1. take a file path of type path or str to the file on local storage
-            * see Example for more details
-        1. convert the file path to pathlib object, so it is versatile and
-            always uniform regardless if the user passes in a str or path object
-        1. get the file
-        1. rename the file to avoid clash or overwriting of previously uploaded files
-            * change file name to `original_name_uuid4.extension`
-                *  `document_42926a201a624fdba0fd6271defc9e88.txt`
-        1. upload file to AWS S3
-        1. get the link of the uploaded file and return it
-
-
-        Parameters
-        ----------
-        file_path: Union[str, Path]
-            file path as str or Path object. Path Object is recommended
-
-        Examples
-        --------
-        >>> from pathlib import Path
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...     # programmatically create the absolute path of your file, so the program always works correctly
-        ...     my_file_path = (Path(__file__) / Path('../upload_files/my_file.txt')).resolve()
-        ...     my_file_cloud_storage_source = api.upload_file(file_path=my_file_path)  # doctest: +SKIP
-
-        Notes
-        -----
-        We recommend using a [Path](https://docs.python.org/3/library/pathlib.html) object for specifying a file path.
-        Using the Python [pathlib library](https://docs.python.org/3/library/pathlib.html) provides platform-agnostic approach
-        for filesystem operations, ensuring seamless functionality across different operating systems.
-        Additionally, [Path](https://docs.python.org/3/library/pathlib.html) objects offer various built-in methods
-        for more sophisticated and secure file handling and has a easy to use interface that can make working with it a breeze
-        and can help reduce errors.
-
-        Other options include using a raw string for relative/absolute file path,
-        or using the [os.path module](https://docs.python.org/3/library/os.path.html).
-
-
-        Raises
-        ------
-        FileNotFoundError
-            In case the CRIPT Python SDK cannot find the file on your computer because the file does not exist
-            or the path to it is incorrect it raises
-            [FileNotFoundError](https://docs.python.org/3/library/exceptions.html#FileNotFoundError)
-
-        Returns
-        -------
-        object_name: str
-            object_name of the AWS S3 uploaded file to be put into the File node source attribute
-        """
-        # trunk-ignore-end(cspell)
-
-        # TODO consider using a new variable when converting `file_path` from parameter
-        #  to a Path object with a new type
-        # convert file path from whatever the user passed in to a pathlib object
-        file_path = Path(file_path).resolve()
-
-        # get file_name and file_extension from absolute file path
-        # file_extension includes the dot, e.g. ".txt"
-        file_name, file_extension = os.path.splitext(os.path.basename(file_path))
-
-        # generate a UUID4 string without dashes, making a cleaner file name
-        uuid_str: str = str(uuid.uuid4().hex)
-
-        new_file_name: str = f"{file_name}_{uuid_str}{file_extension}"
-
-        # e.g. "directory/file_name_uuid.extension"
-        object_name: str = f"{self._BUCKET_DIRECTORY_NAME}/{new_file_name}"
-
-        # upload file to AWS S3
-        self._s3_client.upload_file(Filename=file_path, Bucket=self._BUCKET_NAME, Key=object_name)  # type: ignore
-
-        self.logger.info(f"Uploaded File: '{file_path}' to CRIPT storage")
-
-        # return the object_name within AWS S3 for easy retrieval
-        return object_name
-
-    @beartype
-    def download_file(self, file_source: str, destination_path: str = ".") -> None:
-        """
-        Download a file from CRIPT Cloud Storage (AWS S3) and save it to the specified path.
-
-        ??? Info "Cloud Storage vs Web URL File Download"
-
-            If the `object_name` does not starts with `http` then the program assumes the file is in AWS S3 storage,
-            and attempts to retrieve it via
-            [boto3 client](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html).
-
-            If the `object_name` starts with `http` then the program knows that
-            it is a file stored on the web. The program makes a simple
-            [GET](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET) request to get the file,
-            then writes the contents of it to the specified destination.
-
-            > Note: The current version of the program is designed to download files from the web in a straightforward
-            manner. However, please be aware that the program may encounter limitations when dealing with URLs that
-            require JavaScript or a session to be enabled. In such cases, the download method may fail.
-
-            > We acknowledge these limitations and plan to enhance the method in future versions to ensure compatibility
-            with a wider range of web file URLs. Our goal is to develop a robust solution capable of handling any and
-            all web file URLs.
-
-        Parameters
-        ----------
-        file_source: str
-            `object_name`: file downloaded via object_name from cloud storage and saved to local storage
-            object_name e.g. `"Data/{file_name}"`
-            ---
-            `URL file source`: If the file source starts with `http` then it is downloaded via `GET` request and
-            saved to local storage
-           URL file source e.g. `https://criptscripts.org/cript_graph_json/JSON/cao_protein.json`
-        destination_path: str
-            please provide a path with file name of where you would like the file to be saved
-            on local storage.
-            > If no path is specified, then by default it will download the file
-            to the current working directory.
-
-            > The destination path must include a file name and file extension
-                e.g.: `~/Desktop/my_example_file_name.extension`
-
-        Examples
-        --------
-        >>> from pathlib import Path
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...     desktop_path = (Path(__file__).parent / "cript_downloads" / "my_downloaded_file.txt").resolve()
-        ...     my_file = cript.File(
-        ...         name="my file node name",
-        ...         source="https://criptapp.org",
-        ...         type="calibration",
-        ...         extension=".csv",
-        ...     )
-        ...     api.download_file(file_source=my_file.source, destination_path=str(desktop_path)) # doctest: +SKIP
-
-        Raises
-        ------
-        FileNotFoundError
-            In case the file could not be found because the file does not exist or the path given is incorrect
-
-        Returns
-        -------
-        None
-            Simply downloads the file
-        """
-
-        # if the file source is a URL
-        if file_source.startswith("http"):
-            download_file_from_url(url=file_source, destination_path=Path(destination_path).resolve())
-            return
-
-        # the file is stored in cloud storage and must be retrieved via object_name
-        self._s3_client.download_file(Bucket=self._BUCKET_NAME, Key=file_source, Filename=destination_path)  # type: ignore
-
-    @beartype
-    def search(
-        self,
-        node_type: Any,
-        search_mode: SearchModes,
-        value_to_search: Optional[str],
-    ) -> Paginator:
-        """
-        This method is used to perform search on the CRIPT platform.
-
-        Essentially creates needed resources and passes it to paginator to get results from API
-        and display them.
-
-        Examples
-        --------
-        ???+ Example "Search by Node Type"
-            ```python
-            materials_paginator = cript_api.search(
-                node_type=cript.Material,
-                search_mode=cript.SearchModes.NODE_TYPE,
-                value_to_search=None
-            )
-            ```
-
-        ??? Example "Search by Contains name"
-            ```python
-            contains_name_paginator = cript_api.search(
-                node_type=cript.Process,
-                search_mode=cript.SearchModes.CONTAINS_NAME,
-                value_to_search="poly"
-            )
-            ```
-
-        ??? Example "Search by Exact Name"
-            ```python
-            exact_name_paginator = cript_api.search(
-                node_type=cript.Project,
-                search_mode=cript.SearchModes.EXACT_NAME,
-                value_to_search="Sodium polystyrene sulfonate"
-            )
-            ```
-
-        ??? Example "Search by UUID"
-            ```python
-            uuid_paginator = cript_api.search(
-                node_type=cript.Collection,
-                search_mode=cript.SearchModes.UUID,
-                value_to_search="75fd3ee5-48c2-4fc7-8d0b-842f4fc812b7"
-            )
-            ```
-
-        ??? Example "Search by BigSmiles"
-            ```python
-            paginator = cript_api.search(
-                node_type=cript.Material,
-                search_mode=cript.SearchModes.BIGSMILES,
-                value_to_search="{[][$]CC(C)(C(=O)OCCCC)[$][]}"
-            )
-            ```
-
-        Parameters
-        ----------
-        node_type : UUIDBaseNode
-            Type of node that you are searching for.
-        search_mode : SearchModes
-            Type of search you want to do. You can search by name, `UUID`, `EXACT_NAME`, etc.
-            Refer to [valid search modes](../search_modes)
-        value_to_search : Optional[str]
-            What you are searching for can be either a value, and if you are only searching for
-            a `NODE_TYPE`, then this value can be empty or `None`
-
-        Returns
-        -------
-        Paginator
-            paginator object for the user to use to flip through pages of search results
-
-        Notes
-        -----
-        To learn more about working with pagination, please refer to our
-        [paginator object documentation](../paginator).
-
-        Additionally, you can utilize the utility function
-        [`load_nodes_from_json(node_json)`](../../utility_functions/#cript.nodes.util.load_nodes_from_json)
-        to convert API JSON responses into Python SDK nodes.
-
-        ???+ Example "Convert API JSON Response to Python SDK Nodes"
-            ```python
-            # Get updated project from API
-            my_paginator = api.search(
-                node_type=cript.Project,
-                search_mode=cript.SearchModes.EXACT_NAME,
-                value_to_search="my project name",
-            )
-
-            # Take specific Project you want from paginator
-            my_project_from_api_dict: dict = my_paginator.current_page_results[0]
-
-            # Deserialize your Project dict into a Project node
-            my_project_node_from_api = cript.load_nodes_from_json(
-                nodes_json=json.dumps(my_project_from_api_dict)
-            )
-            ```
-        """
-
-        # get node typ from class
-        node_type = node_type.node_type_snake_case
-
-        # always putting a page parameter of 0 for all search URLs
-        page_number = 0
-
-        api_endpoint: str = ""
-
-        # requesting a page of some primary node
-        if search_mode == SearchModes.NODE_TYPE:
-            api_endpoint = f"{self._host}/{node_type}"
-
-        elif search_mode == SearchModes.CONTAINS_NAME:
-            api_endpoint = f"{self._host}/search/{node_type}"
-
-        elif search_mode == SearchModes.EXACT_NAME:
-            api_endpoint = f"{self._host}/search/exact/{node_type}"
-
-        elif search_mode == SearchModes.UUID:
-            api_endpoint = f"{self._host}/{node_type}/{value_to_search}"
-            # putting the value_to_search in the URL instead of a query
-            value_to_search = None
-
-        elif search_mode == SearchModes.BIGSMILES:
-            api_endpoint = f"{self._host}/search/bigsmiles/"
-
-        # error handling if none of the API endpoints got hit
-        else:
-            raise RuntimeError("Internal Error: Failed to recognize any search modes. Please report this bug on https://github.com/C-Accel-CRIPT/Python-SDK/issues.")
-
-        return Paginator(http_headers=self._http_headers, api_endpoint=api_endpoint, query=value_to_search, current_page_number=page_number)
-
-    def delete(self, node) -> None:
-        """
-        Simply deletes the desired node from the CRIPT API and writes a log in the terminal that the node has been
-        successfully deleted.
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_material_node = cript.Material(
-        ...     name="my component material 1",
-        ...     identifier=[{"amino_acid": "component 1 alternative name"}],
-        ... )
-        >>> api.delete(node=my_material_node) # doctest: +SKIP
-
-        Notes
-        -----
-        After the node has been successfully deleted, a log is written to the terminal if `cript.API.verbose = True`
-
-        ```bash
-        INFO: Deleted 'Material' with UUID of '80bfc642-157e-4692-a547-97c470725397' from CRIPT API.
-        ```
-
-        ??? info "Implementation Details"
-            Under the hood, this method actually calls
-            [delete_node_by_uuid](./#cript.api.api.API.delete_node_by_uuid)
-            with the node_type and node UUID
-
-        Warnings
-        --------
-        After successfully deleting a node from the API, keep in mind that your local Project node in your script
-        may still contain outdated data as it has not been synced with the API.
-
-        To ensure you have the latest data, follow these steps:
-
-        1. Fetch the newest Project node from the API using the [`cript.API.search()`](./#cript.api.api.API.search) provided by the SDK.
-        1. Deserialize the retrieved data into a new Project node using the [`load_nodes_from_json`](../../utility_functions/#cript.nodes.util.load_nodes_from_json) utility function.
-        1. Replace your old Project node with the new one in your script for accurate and up-to-date information.
-
-        Parameters
-        ----------
-        node: UUIDBaseNode
-            The node that you want to delete
-
-        Raises
-        ------
-        APIError
-            If the API responds with anything other than HTTP status 200, then the CRIPT Python SDK raises `APIError`
-            `APIError` is raised in case the API cannot delete the specified node.
-            Such cases can happen if you do not have permission to delete the node
-            or if the node is actively being used elsewhere in CRIPT platform and the API cannot delete it.
-
-        Returns
-        -------
-        None
-        """
-        self.delete_node_by_uuid(node_type=node.node_type_snake_case, node_uuid=str(node.uuid))
-
-    @beartype
-    def delete_node_by_uuid(self, node_type: str, node_uuid: str) -> None:
-        """
-        Simply deletes the desired node from the CRIPT API and writes a log in the terminal that the node has been
-        successfully deleted.
-
-        Examples
-        --------
-        >>> import cript
-        >>> with cript.API(
-        ...     host="https://api.criptapp.org/",
-        ...     api_token=os.getenv("CRIPT_TOKEN"),
-        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
-        ... ) as api:
-        ...      api.delete_node_by_uuid(
-        ...         node_type="computation_process",
-        ...         node_uuid="2fd3d500-304d-4a06-8628-a79b59344b2f"
-        ...     ) # doctest: +SKIP
-
-        ??? "How to get `node_type in snake case`"
-               You can get the `node type in snake case` of a node via:
-               ```python
-                import cript
-                print(cript.ComputationProcess.node_type_snake_case)
-               computation_process
-               ```
-
-               You can also call `api.delete_node_by_uuid()` with
-               ```python
-               api.delete(
-                   node_type=cript.ComputationProcess.node_type_snake_case,
-                   node_uuid="2fd3d500-304d-4a06-8628-a79b59344b2f",
-               )
-               ```
-
-        Notes
-        -----
-        After the node has been successfully deleted, a log is written to the terminal if `cript.API.verbose = True`
-
-        ```bash
-        INFO: Deleted 'Material' with UUID of '80bfc642-157e-4692-a547-97c470725397' from CRIPT API.
-        ```
-
-        Warnings
-        --------
-        After successfully deleting a node from the API, keep in mind that your local Project node in your script
-        may still contain outdated data as it has not been synced with the API.
-
-        To ensure you have the latest data, follow these steps:
-
-        1. Fetch the newest Project node from the API using the
-        [`cript.API.search()`](./#cript.api.api.API.search) provided by the SDK.
-        1. Deserialize the retrieved data into a new Project node using the
-        [`load_nodes_from_json`](../../utility_functions/#cript.nodes.util.load_nodes_from_json) utility function.
-        1. Replace your old Project node with the new one in your script for accurate and up-to-date information.
-
-        Parameters
-        ----------
-        node_type: str
-           the type of node that you want to delete in snake case
-        node_uuid: str
-           the UUID of the primary node, supporting node, or sub-object
-           that you want to delete from the API
-
-        Raises
-        ------
-        APIError
-            If the API responds with anything other than HTTP status 200, then the CRIPT Python SDK raises `APIError`
-            `APIError` is raised in case the API cannot delete the specified node.
-            Such cases can happen if you do not have permission to delete the node
-            or if the node is actively being used elsewhere in CRIPT platform and the API cannot delete it.
-
-        Returns
-        -------
-        None
-        """
-        delete_node_api_url: str = f"{self._host}/{node_type.lower()}/{node_uuid}/"
-
-        response: Dict = requests.delete(headers=self._http_headers, url=delete_node_api_url, timeout=_API_TIMEOUT).json()
-
-        if response["code"] != 200:
-            raise APIError(api_error=str(response), http_method="DELETE", api_url=delete_node_api_url)
-
-        self.logger.info(f"Deleted '{node_type.title()}' with UUID of '{node_uuid}' from CRIPT API.")
+import copy
+import json
+import logging
+import os
+import traceback
+import uuid
+from pathlib import Path
+from typing import Any, Dict, Optional, Union
+
+import boto3
+import requests
+from beartype import beartype
+
+from cript.api.api_config import _API_TIMEOUT
+from cript.api.data_schema import DataSchema
+from cript.api.exceptions import (
+    APIError,
+    CRIPTAPIRequiredError,
+    CRIPTAPISaveError,
+    CRIPTConnectionError,
+    CRIPTDuplicateNameError,
+)
+from cript.api.paginator import Paginator
+from cript.api.utils.aws_s3_utils import get_s3_client
+from cript.api.utils.get_host_token import resolve_host_and_token
+from cript.api.utils.save_helper import (
+    _fix_node_save,
+    _identify_suppress_attributes,
+    _InternalSaveValues,
+)
+from cript.api.utils.web_file_downloader import download_file_from_url
+from cript.api.valid_search_modes import SearchModes
+from cript.nodes.primary_nodes.project import Project
+
+# Do not use this directly! That includes devs.
+# Use the `_get_global_cached_api for access.
+_global_cached_api = None
+
+
+def _get_global_cached_api():
+    """
+    Read-Only access to the globally cached API object.
+    Raises an exception if no global API object is cached yet.
+    """
+    if _global_cached_api is None:
+        raise CRIPTAPIRequiredError()
+    return _global_cached_api
+
+
+class API:
+    """
+    ## Definition
+    API Client class to communicate with the CRIPT API
+    """
+
+    # dictates whether the user wants to see terminal log statements or not
+    _logger: logging.Logger = None  # type: ignore
+
+    _host: str = ""
+    _api_token: str = ""
+    _storage_token: str = ""
+    _db_schema: Optional[DataSchema] = None
+    _api_prefix: str = "api"
+    _api_version: str = "v1"
+    _api_request_session: Union[None, requests.Session] = None
+
+    # trunk-ignore-begin(cspell)
+    # AWS S3 constants
+    _REGION_NAME: str = "us-east-1"
+    _IDENTITY_POOL_ID: str = "us-east-1:9426df38-994a-4191-86ce-3cb0ce8ac84d"
+    _COGNITO_LOGIN_PROVIDER: str = "cognito-idp.us-east-1.amazonaws.com/us-east-1_SZGBXPl2j"
+    _BUCKET_NAME: str = "cript-user-data"
+    _BUCKET_DIRECTORY_NAME: str = "python_sdk_files"
+    _internal_s3_client: Any = None  # type: ignore
+    # trunk-ignore-end(cspell)
+
+    extra_api_log_debug_info: bool = False
+
+    @beartype
+    def __init__(self, host: Union[str, None] = None, api_token: Union[str, None] = None, storage_token: Union[str, None] = None, config_file_path: Union[str, Path] = "", default_log_level=logging.INFO):
+        """
+        Initialize CRIPT API client with host and token.
+        Additionally, you can  use a config.json file and specify the file path.
+
+        !!! note "api client context manager"
+            It is necessary to use a `with` context manager for the API
+
+        Examples
+        --------
+        ### Create API client with host and token
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...    # node creation, api.save(), etc.
+        ...    pass
+
+
+        ---
+
+        ### Creating API Client
+        !!! Warning "Token Security"
+            It is **highly** recommended that you store your API tokens in a safe location and read it into your code
+            Hard-coding API tokens directly into the code can pose security risks,
+            as the token might be exposed if the code is shared or stored in a version control system.
+            Anyone that has access to your tokens can impersonate you on the CRIPT platform
+
+        ### Create API Client with Environment Variables
+
+        Another great way to keep sensitive information secure is by using
+        [environment variables](https://www.freecodecamp.org/news/python-env-vars-how-to-get-an-environment-variable-in-python/).
+        Sensitive information can be securely stored in environment variables and loaded into the code using
+        [os.getenv()](https://docs.python.org/3/library/os.html#os.getenv).
+
+        Examples
+        --------
+        >>> import cript
+        >>> import os
+        >>> # securely load sensitive data into the script
+        >>> cript_host = os.getenv("cript_host")
+        >>> cript_api_token = os.getenv("cript_api_token")
+        >>> cript_storage_token = os.getenv("cript_storage_token")
+        >>> with cript.API(
+        ...     host=cript_host, api_token=cript_api_token, storage_token=cript_storage_token
+        ... ) as api:
+        ...     pass
+
+        ### Create API Client with None
+        Alternatively you can configure your system to have an environment variable of
+        `CRIPT_TOKEN` for the API token and `CRIPT_STORAGE_TOKEN` for the storage token, then
+        initialize `cript.API` `api_token` and `storage_token` with `None`.
+
+        The CRIPT Python SDK will try to read the API Token and Storage token from your system's environment variables.
+
+        ```python
+        with cript.API(host=cript_host, api_token=None, storage_token=None) as api:
+            # write your script
+            pass
+        ```
+
+        ### Create API client with config.json
+        `config.json`
+        ```json
+        {
+            "host": "https://api.criptapp.org/",
+            "api_token": "I am API token",
+            "storage_token": "I am storage token"
+        }
+        ```
+
+        Examples
+        --------
+        `my_script.py`
+        >>> from pathlib import Path
+        >>> import cript
+        >>> # create a file path object of where the config file is
+        >>> config_file_path = Path(__file__) / Path('./config.json')
+        >>> with cript.API(config_file_path=config_file_path) as api:   # doctest: +SKIP
+        ...     # node creation, api.save(), etc.
+        ...     pass
+
+        Parameters
+        ----------
+        host : str, None
+            CRIPT host for the Python SDK to connect to such as https://api.criptapp.org/`
+            This host address is the same address used to login to cript website.
+            If `None` is specified, the host is inferred from the environment variable `CRIPT_HOST`.
+        api_token : str, None
+            CRIPT API Token used to connect to CRIPT and upload all data with the exception to file upload that needs
+            a different token.
+            You can find your personal token on the cript website at User > Security Settings.
+            The user icon is in the top right.
+            If `None` is specified, the token is inferred from the environment variable `CRIPT_TOKEN`.
+        storage_token: str
+            This token is used to upload local files to CRIPT cloud storage when needed
+        config_file_path: str
+            the file path to the config.json file where the token and host can be found
+
+
+        Notes
+        -----
+        * if `host=None` and `token=None`
+            then the Python SDK will grab the host from the users environment variable of `"CRIPT_HOST"`
+            and `"CRIPT_TOKEN"`
+
+        Warns
+        -----
+        UserWarning
+            If `host` is using "http" it gives the user a warning that HTTP is insecure and the user should use HTTPS
+
+        Raises
+        ------
+        CRIPTConnectionError
+            If it cannot connect to CRIPT with the provided host and token a CRIPTConnectionError is thrown.
+
+        Returns
+        -------
+        None
+            Instantiate a new CRIPT API object
+        """
+
+        # if there is a config.json file or any of the parameters are None, then get the variables from file or env vars
+        if config_file_path or (host is None or api_token is None or storage_token is None):
+            authentication_dict: Dict[str, str] = resolve_host_and_token(host, api_token=api_token, storage_token=storage_token, config_file_path=config_file_path)
+
+            host = authentication_dict["host"]
+            api_token = authentication_dict["api_token"]
+            storage_token = authentication_dict["storage_token"]
+
+        self._host: str = host.rstrip("/")
+        self._api_token = api_token  # type: ignore
+        self._storage_token = storage_token  # type: ignore
+
+        # set a logger instance to use for the class logs
+        self._init_logger(default_log_level)
+
+    def __str__(self) -> str:
+        """
+        States the host of the CRIPT API client
+
+        Examples
+        --------
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...     print(api)
+        CRIPT API Client - Host URL: 'https://api.criptapp.org'
+
+        Returns
+        -------
+        str
+        """
+        return f"CRIPT API Client - Host URL: '{self.host}'"
+
+    def _init_logger(self, log_level=logging.INFO) -> None:
+        """
+        Prepare and configure the logger for the API class.
+
+        This function creates and configures a logger instance associated with the current module (class).
+
+        Parameters
+        ----------
+        log_level: logging.LEVEL default logging.INFO
+            set if you want `cript.API` to give logs to console or not
+
+        Returns
+        -------
+        logging.Logger
+            The configured logger instance.
+        """
+        # Create a logger instance associated with the current module
+        logger = logging.getLogger(__name__)
+
+        logger.setLevel(log_level)
+
+        # Create a console handler
+        console_handler = logging.StreamHandler()
+
+        # Create a formatter for log messages (customize the format as desired)
+        formatter = logging.Formatter("%(levelname)s: %(message)s")
+
+        # Associate the formatter with the console handler
+        console_handler.setFormatter(formatter)
+
+        # Add the console handler to the logger
+        logger.addHandler(console_handler)
+
+        # set logger for the class
+        self._logger = logger
+
+    @property
+    def logger(self):
+        return self._logger
+
+    # Use a property to ensure delayed init of s3_client
+    @property
+    def _s3_client(self) -> boto3.client:  # type: ignore
+        """
+        Property to use when wanting to interact with AWS S3.
+
+        Gets a fully authenticated AWS S3 client if it was never created and stash it,
+        if the AWS S3 client has been created before, then returns the client that it has
+
+        Returns
+        -------
+        s3_client: boto3.client
+            fully prepared and authenticated s3 client ready to be used throughout the script
+        """
+        if self._internal_s3_client is None:
+            self._internal_s3_client = get_s3_client(region_name=self._REGION_NAME, identity_pool_id=self._IDENTITY_POOL_ID, cognito_login_provider=self._COGNITO_LOGIN_PROVIDER, storage_token=self._storage_token)
+
+        return self._internal_s3_client
+
+    def __enter__(self):
+        self.connect()
+        return self
+
+    @beartype
+    def __exit__(self, type, value, traceback):
+        self.disconnect()
+
+    def connect(self):
+        """
+        Connect this API globally as the current active access point.
+        It is not necessary to call this function manually if a context manager is used.
+        A context manager is preferred where possible.
+        Jupyter notebooks are a use case where this connection can be handled manually.
+        If this function is called manually, the `API.disconnect` function has to be called later.
+
+        For manual connection: nested API object are discouraged.
+
+        Raises
+        -------
+        CRIPTConnectionError
+            raised when the host does not give the expected response
+        """
+
+        # Establish a requests session object
+        if self._api_request_session:
+            self.disconnect()
+        self._api_request_session = requests.Session()
+        # add Bearer to token for HTTP requests
+        self._api_request_session.headers = {"Authorization": f"Bearer {self._api_token}", "Content-Type": "application/json"}
+
+        # As a form to check our connection, we pull and establish the data schema
+        try:
+            self._db_schema = DataSchema(self)
+        except APIError as exc:
+            raise CRIPTConnectionError(self.host, self._api_token) from exc
+
+        # Store the last active global API (might be None)
+        global _global_cached_api
+        self._previous_global_cached_api = copy.copy(_global_cached_api)
+        _global_cached_api = self
+        return self
+
+    def disconnect(self):
+        """
+        Disconnect this API from the active access point.
+        It is not necessary to call this function manually if a context manager is used.
+        A context manager is preferred where possible.
+        Jupyter notebooks are a use case where this connection can be handled manually.
+        This function has to be called manually if  the `API.connect` function has to be called before.
+
+        For manual connection: nested API object are discouraged.
+        """
+        # Disconnect request session
+        if self._api_request_session:
+            self._api_request_session.close()
+
+        # Restore the previously active global API (might be None)
+        global _global_cached_api
+        _global_cached_api = self._previous_global_cached_api
+
+    @property
+    def schema(self):
+        """
+        Access the CRIPT Database Schema that is associated with this API connection.
+        The CRIPT Database Schema is used  to validate a node's JSON so that it is compatible with the CRIPT API.
+        """
+        return self._db_schema
+
+    @property
+    def host(self):
+        """
+        Read only access to the currently connected host.
+
+        The term "host" designates the specific CRIPT instance to which you intend to upload your data.
+
+        For most users, the host will be `https://api.criptapp.org`
+
+        ```yaml
+        host: https://api.criptapp.org
+        ```
+
+        Examples
+        --------
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...    print(api.host)
+        https://api.criptapp.org
+        """
+        return self._host
+
+    @property
+    def api_prefix(self):
+        return self._api_prefix
+
+    @property
+    def api_version(self):
+        return self._api_version
+
+    def save(self, project: Project) -> None:
+        """
+        This method takes a project node, serializes the class into JSON
+        and then sends the JSON to be saved to the API.
+        It takes Project node because everything is connected to the Project node,
+        and it can be used to send either a POST or PATCH request to API
+
+        Parameters
+        ----------
+        project: Project
+            the Project Node that the user wants to save
+
+        Raises
+        ------
+        CRIPTAPISaveError
+            If the API responds with anything other than an HTTP of `200`, the API error is displayed to the user
+
+        Returns
+        -------
+        A set of extra saved node UUIDs.
+            Just sends a `POST` or `Patch` request to the API
+        """
+        try:
+            self._internal_save(project)
+        except CRIPTAPISaveError as exc:
+            if exc.pre_saved_nodes:
+                for node_uuid in exc.pre_saved_nodes:
+                    # TODO remove all pre-saved nodes by their uuid.
+                    pass
+            raise exc from exc
+
+    def _internal_save(self, node, save_values: Optional[_InternalSaveValues] = None) -> _InternalSaveValues:
+        """
+        Internal helper function that handles the saving of different nodes (not just project).
+
+        If a "Bad UUID" error happens, we find that node with the UUID and save it first.
+        Then we recursively call the _internal_save again.
+        Because it is recursive, this repeats until no "Bad UUID" error happen anymore.
+        This works, because we keep track of "Bad UUID" handled nodes, and represent them in the JSON only as the UUID.
+        """
+
+        if save_values is None:
+            save_values = _InternalSaveValues()
+
+        # saves all the local files to cloud storage right before saving the Project node
+        # Ensure that all file nodes have uploaded there payload before actual save.
+        for file_node in node.find_children({"node": ["File"]}):
+            file_node.ensure_uploaded(api=self)
+
+        node.validate(force_validation=True)
+
+        # Dummy response to have a virtual do-while loop, instead of while loop.
+        response = {"code": -1}
+        # TODO remove once get works properly
+        force_patch = False
+
+        while response["code"] != 200:
+            # Keep a record of how the state was before the loop
+            old_save_values = copy.deepcopy(save_values)
+            # We assemble the JSON to be saved to back end.
+            # Note how we exclude pre-saved uuid nodes.
+            json_data = node.get_json(known_uuid=save_values.saved_uuid, suppress_attributes=save_values.suppress_attributes).json
+
+            # This checks if the current node exists on the back end.
+            # if it does exist we use `patch` if it doesn't `post`.
+            test_get_response: Dict = self._capsule_request(url_path=f"/{node.node_type_snake_case}/{str(node.uuid)}/", method="GET").json()
+            patch_request = test_get_response["code"] == 200
+
+            # TODO remove once get works properly
+            if not patch_request and force_patch:
+                patch_request = True
+                force_patch = False
+            # TODO activate patch validation
+            # node.validate(is_patch=patch_request)
+
+            # If all that is left is a UUID, we don't need to save it, we can just exit the loop.
+            if patch_request and len(json.loads(json_data)) == 1:
+                response = {"code": 200}
+                break
+
+            method = "POST"
+            url_path = f"/{node.node_type_snake_case}/"
+            if patch_request:
+                method = "PATCH"
+                url_path += f"{str(node.uuid)}/"
+
+            response: Dict = self._capsule_request(url_path=url_path, method=method, data=json_data).json()  # type: ignore
+
+            # if node.node_type != "Project":
+            #     test_success: Dict = requests.get(url=f"{self._host}/{node.node_type_snake_case}/{str(node.uuid)}/", headers=self._http_headers, timeout=_API_TIMEOUT).json()
+            #     print("XYZ", json_data, save_values, response, test_success)
+
+            # print(json_data, patch_request, response, save_values)
+            # If we get an error we may be able to fix, we to handle this extra and save the bad node first.
+            # Errors with this code, may be fixable
+            if response["code"] in (400, 409):
+                try:
+                    returned_save_values = _fix_node_save(self, node, response, save_values)
+                except CRIPTAPISaveError as exc:
+                    # If the previous error was a duplicated name issue
+                    if "duplicate item [{'name':" in str(response["error"]):
+                        # And (second condition) the request failed bc of the now suppressed name
+                        if "'name' is a required property" in exc.api_response:
+                            # Raise a save error, with the nice name related error message
+                            raise CRIPTDuplicateNameError(response, json_data, exc) from exc
+                    # Else just raise the exception as normal.
+                    raise exc
+                save_values += returned_save_values
+
+            # Handle errors from patching with too many attributes
+            if patch_request and response["code"] in (400,):
+                suppress_attributes = _identify_suppress_attributes(node, response)
+                new_save_values = _InternalSaveValues(save_values.saved_uuid, suppress_attributes)
+                save_values += new_save_values
+
+            # It is only worthwhile repeating the attempted save loop if our state has improved.
+            # Aka we did something to fix the occurring error
+            if not save_values > old_save_values:
+                # TODO remove once get works properly
+                if not patch_request:
+                    # and response["code"] == 409 and response["error"].strip().startswith("Duplicate uuid:"):  # type: ignore
+                    # duplicate_uuid = _get_uuid_from_error_message(response["error"])  # type: ignore
+                    # if str(node.uuid) == duplicate_uuid:
+                    force_patch = True
+                    continue
+                break
+
+        if response["code"] != 200:
+            raise CRIPTAPISaveError(api_host_domain=self._host, http_code=response["code"], api_response=response["error"], patch_request=patch_request, pre_saved_nodes=save_values.saved_uuid, json_data=json_data)  # type: ignore
+
+        save_values.saved_uuid.add(str(node.uuid))
+        return save_values
+
+    def upload_file(self, file_path: Union[Path, str]) -> str:
+        # trunk-ignore-begin(cspell)
+        """
+        uploads a file to AWS S3 bucket and returns a URL of the uploaded file in AWS S3
+        The URL is has no expiration time limit and is available forever
+
+        1. take a file path of type path or str to the file on local storage
+            * see Example for more details
+        1. convert the file path to pathlib object, so it is versatile and
+            always uniform regardless if the user passes in a str or path object
+        1. get the file
+        1. rename the file to avoid clash or overwriting of previously uploaded files
+            * change file name to `original_name_uuid4.extension`
+                *  `document_42926a201a624fdba0fd6271defc9e88.txt`
+        1. upload file to AWS S3
+        1. get the link of the uploaded file and return it
+
+
+        Parameters
+        ----------
+        file_path: Union[str, Path]
+            file path as str or Path object. Path Object is recommended
+
+        Examples
+        --------
+        >>> from pathlib import Path
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...     # programmatically create the absolute path of your file, so the program always works correctly
+        ...     my_file_path = (Path(__file__) / Path('../upload_files/my_file.txt')).resolve()
+        ...     my_file_cloud_storage_source = api.upload_file(file_path=my_file_path)  # doctest: +SKIP
+
+        Notes
+        -----
+        We recommend using a [Path](https://docs.python.org/3/library/pathlib.html) object for specifying a file path.
+        Using the Python [pathlib library](https://docs.python.org/3/library/pathlib.html) provides platform-agnostic approach
+        for filesystem operations, ensuring seamless functionality across different operating systems.
+        Additionally, [Path](https://docs.python.org/3/library/pathlib.html) objects offer various built-in methods
+        for more sophisticated and secure file handling and has a easy to use interface that can make working with it a breeze
+        and can help reduce errors.
+
+        Other options include using a raw string for relative/absolute file path,
+        or using the [os.path module](https://docs.python.org/3/library/os.path.html).
+
+
+        Raises
+        ------
+        FileNotFoundError
+            In case the CRIPT Python SDK cannot find the file on your computer because the file does not exist
+            or the path to it is incorrect it raises
+            [FileNotFoundError](https://docs.python.org/3/library/exceptions.html#FileNotFoundError)
+
+        Returns
+        -------
+        object_name: str
+            object_name of the AWS S3 uploaded file to be put into the File node source attribute
+        """
+        # trunk-ignore-end(cspell)
+
+        # TODO consider using a new variable when converting `file_path` from parameter
+        #  to a Path object with a new type
+        # convert file path from whatever the user passed in to a pathlib object
+        file_path = Path(file_path).resolve()
+
+        # get file_name and file_extension from absolute file path
+        # file_extension includes the dot, e.g. ".txt"
+        file_name, file_extension = os.path.splitext(os.path.basename(file_path))
+
+        # generate a UUID4 string without dashes, making a cleaner file name
+        uuid_str: str = str(uuid.uuid4().hex)
+
+        new_file_name: str = f"{file_name}_{uuid_str}{file_extension}"
+
+        # e.g. "directory/file_name_uuid.extension"
+        object_name: str = f"{self._BUCKET_DIRECTORY_NAME}/{new_file_name}"
+
+        # upload file to AWS S3
+        self._s3_client.upload_file(Filename=file_path, Bucket=self._BUCKET_NAME, Key=object_name)  # type: ignore
+
+        self.logger.info(f"Uploaded File: '{file_path}' to CRIPT storage")
+
+        # return the object_name within AWS S3 for easy retrieval
+        return object_name
+
+    @beartype
+    def download_file(self, file_source: str, destination_path: str = ".") -> None:
+        """
+        Download a file from CRIPT Cloud Storage (AWS S3) and save it to the specified path.
+
+        ??? Info "Cloud Storage vs Web URL File Download"
+
+            If the `object_name` does not starts with `http` then the program assumes the file is in AWS S3 storage,
+            and attempts to retrieve it via
+            [boto3 client](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html).
+
+            If the `object_name` starts with `http` then the program knows that
+            it is a file stored on the web. The program makes a simple
+            [GET](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET) request to get the file,
+            then writes the contents of it to the specified destination.
+
+            > Note: The current version of the program is designed to download files from the web in a straightforward
+            manner. However, please be aware that the program may encounter limitations when dealing with URLs that
+            require JavaScript or a session to be enabled. In such cases, the download method may fail.
+
+            > We acknowledge these limitations and plan to enhance the method in future versions to ensure compatibility
+            with a wider range of web file URLs. Our goal is to develop a robust solution capable of handling any and
+            all web file URLs.
+
+        Parameters
+        ----------
+        file_source: str
+            `object_name`: file downloaded via object_name from cloud storage and saved to local storage
+            object_name e.g. `"Data/{file_name}"`
+            ---
+            `URL file source`: If the file source starts with `http` then it is downloaded via `GET` request and
+            saved to local storage
+           URL file source e.g. `https://criptscripts.org/cript_graph_json/JSON/cao_protein.json`
+        destination_path: str
+            please provide a path with file name of where you would like the file to be saved
+            on local storage.
+            > If no path is specified, then by default it will download the file
+            to the current working directory.
+
+            > The destination path must include a file name and file extension
+                e.g.: `~/Desktop/my_example_file_name.extension`
+
+        Examples
+        --------
+        >>> from pathlib import Path
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...     desktop_path = (Path(__file__).parent / "cript_downloads" / "my_downloaded_file.txt").resolve()
+        ...     my_file = cript.File(
+        ...         name="my file node name",
+        ...         source="https://criptapp.org",
+        ...         type="calibration",
+        ...         extension=".csv",
+        ...     )
+        ...     api.download_file(file_source=my_file.source, destination_path=str(desktop_path)) # doctest: +SKIP
+
+        Raises
+        ------
+        FileNotFoundError
+            In case the file could not be found because the file does not exist or the path given is incorrect
+
+        Returns
+        -------
+        None
+            Simply downloads the file
+        """
+
+        # if the file source is a URL
+        if file_source.startswith("http"):
+            download_file_from_url(url=file_source, destination_path=Path(destination_path).resolve())
+            return
+
+        # the file is stored in cloud storage and must be retrieved via object_name
+        self._s3_client.download_file(Bucket=self._BUCKET_NAME, Key=file_source, Filename=destination_path)  # type: ignore
+
+    @beartype
+    def search(
+        self,
+        node_type: Any,
+        search_mode: SearchModes,
+        value_to_search: str = "",
+    ) -> Paginator:
+        """
+        This method is used to perform search on the CRIPT platform.
+
+        Essentially creates needed resources and passes it to paginator to get results from API
+        and display them.
+
+        Examples
+        --------
+        ???+ Example "Search by Node Type"
+            ```python
+            materials_iterator = cript_api.search(
+                node_type=cript.Material,
+                search_mode=cript.SearchModes.NODE_TYPE,
+            )
+            ```
+
+        ??? Example "Search by Contains name"
+            ```python
+            contains_name_iterator = cript_api.search(
+                node_type=cript.Process,
+                search_mode=cript.SearchModes.CONTAINS_NAME,
+                value_to_search="poly"
+            )
+            ```
+
+        ??? Example "Search by Exact Name"
+            ```python
+            exact_name_iterator = cript_api.search(
+                node_type=cript.Project,
+                search_mode=cript.SearchModes.EXACT_NAME,
+                value_to_search="Sodium polystyrene sulfonate"
+            )
+            ```
+
+        ??? Example "Search by UUID"
+            ```python
+            uuid_iterator = cript_api.search(
+                node_type=cript.Collection,
+                search_mode=cript.SearchModes.UUID,
+                value_to_search="75fd3ee5-48c2-4fc7-8d0b-842f4fc812b7"
+            )
+            ```
+
+        ??? Example "Search by BigSmiles"
+            ```python
+            iterator = cript_api.search(
+                node_type=cript.Material,
+                search_mode=cript.SearchModes.BIGSMILES,
+                value_to_search="{[][$]CC(C)(C(=O)OCCCC)[$][]}"
+            )
+            ```
+
+        Parameters
+        ----------
+        node_type : UUIDBaseNode
+            Type of node that you are searching for.
+        search_mode : SearchModes
+            Type of search you want to do. You can search by name, `UUID`, `EXACT_NAME`, etc.
+            Refer to [valid search modes](../search_modes)
+        value_to_search : str
+            What you are searching for can be either a value, and if you are only searching for
+            a `NODE_TYPE`, then this value can be empty or `None`
+
+        Returns
+        -------
+        Paginator
+            An iterator that will present and fetch the results to the user seamlessly
+
+        Notes
+        -----
+        To learn more about working with pagination, please refer to our
+        [paginator object documentation](../paginator).
+        """
+
+        # get node typ from class
+        node_type = node_type.node_type_snake_case
+
+        api_endpoint: str = ""
+        page_number: Union[int, None] = None
+
+        if search_mode == SearchModes.NODE_TYPE:
+            api_endpoint = f"/search/{node_type}"
+            page_number = 0
+
+        elif search_mode == SearchModes.CONTAINS_NAME:
+            api_endpoint = f"/search/{node_type}"
+            page_number = 0
+
+        elif search_mode == SearchModes.EXACT_NAME:
+            api_endpoint = f"/search/exact/{node_type}"
+            page_number = None
+
+        elif search_mode == SearchModes.UUID:
+            api_endpoint = f"/{node_type}/{value_to_search}"
+            # putting the value_to_search in the URL instead of a query
+            value_to_search = ""
+            page_number = None
+
+        elif search_mode == SearchModes.BIGSMILES:
+            api_endpoint = "/search/bigsmiles/"
+            page_number = 0
+
+        # error handling if none of the API endpoints got hit
+        else:
+            raise RuntimeError("Internal Error: Failed to recognize any search modes. Please report this bug on https://github.com/C-Accel-CRIPT/Python-SDK/issues.")
+
+        return Paginator(api=self, url_path=api_endpoint, page_number=page_number, query=value_to_search)
+
+    def delete(self, node) -> None:
+        """
+        Simply deletes the desired node from the CRIPT API and writes a log in the terminal that the node has been
+        successfully deleted.
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_material_node = cript.Material(
+        ...     name="my component material 1",
+        ...     names = ["component 1 alternative name"],
+        ... )
+        >>> api.delete(node=my_material_node) # doctest: +SKIP
+
+        Notes
+        -----
+        After the node has been successfully deleted, a log is written to the terminal
+
+        ```bash
+        INFO: Deleted 'Material' with UUID of '80bfc642-157e-4692-a547-97c470725397' from CRIPT API.
+        ```
+
+        ??? info "Implementation Details"
+            Under the hood, this method actually calls
+            [delete_node_by_uuid](./#cript.api.api.API.delete_node_by_uuid)
+            with the node_type and node UUID
+
+        Warnings
+        --------
+        After successfully deleting a node from the API, keep in mind that your local Project node in your script
+        may still contain outdated data as it has not been synced with the API.
+
+        To ensure you have the latest data, follow these steps:
+
+        1. Fetch the newest Project node from the API using the [`cript.API.search()`](./#cript.api.api.API.search) provided by the SDK.
+        1. Deserialize the retrieved data into a new Project node using the [`load_nodes_from_json`](../../utility_functions/#cript.nodes.util.load_nodes_from_json) utility function.
+        1. Replace your old Project node with the new one in your script for accurate and up-to-date information.
+
+        Parameters
+        ----------
+        node: UUIDBaseNode
+            The node that you want to delete
+
+        Raises
+        ------
+        APIError
+            If the API responds with anything other than HTTP status 200, then the CRIPT Python SDK raises `APIError`
+            `APIError` is raised in case the API cannot delete the specified node.
+            Such cases can happen if you do not have permission to delete the node
+            or if the node is actively being used elsewhere in CRIPT platform and the API cannot delete it.
+
+        Returns
+        -------
+        None
+        """
+        self.delete_node_by_uuid(node_type=node.node_type_snake_case, node_uuid=str(node.uuid))
+
+    @beartype
+    def delete_node_by_uuid(self, node_type: str, node_uuid: str) -> None:
+        """
+        Simply deletes the desired node from the CRIPT API and writes a log in the terminal that the node has been
+        successfully deleted.
+
+        Examples
+        --------
+        >>> import cript
+        >>> with cript.API(
+        ...     host="https://api.criptapp.org/",
+        ...     api_token=os.getenv("CRIPT_TOKEN"),
+        ...     storage_token=os.getenv("CRIPT_STORAGE_TOKEN")
+        ... ) as api:
+        ...      api.delete_node_by_uuid(
+        ...         node_type="computation_process",
+        ...         node_uuid="2fd3d500-304d-4a06-8628-a79b59344b2f"
+        ...     ) # doctest: +SKIP
+
+        ??? "How to get `node_type in snake case`"
+               You can get the `node type in snake case` of a node via:
+               ```python
+                import cript
+                print(cript.ComputationProcess.node_type_snake_case)
+               computation_process
+               ```
+
+               You can also call `api.delete_node_by_uuid()` with
+               ```python
+               api.delete(
+                   node_type=cript.ComputationProcess.node_type_snake_case,
+                   node_uuid="2fd3d500-304d-4a06-8628-a79b59344b2f",
+               )
+               ```
+
+        Notes
+        -----
+        After the node has been successfully deleted, a log is written
+
+        ```bash
+        INFO: Deleted 'Material' with UUID of '80bfc642-157e-4692-a547-97c470725397' from CRIPT API.
+        ```
+
+        Warnings
+        --------
+        After successfully deleting a node from the API, keep in mind that your local Project node in your script
+        may still contain outdated data as it has not been synced with the API.
+
+        To ensure you have the latest data, follow these steps:
+
+        1. Fetch the newest Project node from the API using the
+        [`cript.API.search()`](./#cript.api.api.API.search) provided by the SDK.
+        1. Deserialize the retrieved data into a new Project node using the
+        [`load_nodes_from_json`](../../utility_functions/#cript.nodes.util.load_nodes_from_json) utility function.
+        1. Replace your old Project node with the new one in your script for accurate and up-to-date information.
+
+        Parameters
+        ----------
+        node_type: str
+           the type of node that you want to delete in snake case
+        node_uuid: str
+           the UUID of the primary node, supporting node, or sub-object
+           that you want to delete from the API
+
+        Raises
+        ------
+        APIError
+            If the API responds with anything other than HTTP status 200, then the CRIPT Python SDK raises `APIError`
+            `APIError` is raised in case the API cannot delete the specified node.
+            Such cases can happen if you do not have permission to delete the node
+            or if the node is actively being used elsewhere in CRIPT platform and the API cannot delete it.
+
+        Returns
+        -------
+        None
+        """
+
+        response: Dict = self._capsule_request(url_path=f"/{node_type.lower()}/{node_uuid}/", method="DELETE").json()
+
+        if response["code"] != 200:
+            raise APIError(api_error=str(response), http_method="DELETE", api_url=f"/{node_type.lower()}/{node_uuid}/")
+
+        self.logger.info(f"Deleted '{node_type.title()}' with UUID of '{node_uuid}' from CRIPT API.")
+
+    def _capsule_request(self, url_path: str, method: str, api_request: bool = True, timeout: int = _API_TIMEOUT, **kwargs) -> requests.Response:
+        """Helper function that capsules every request call we make against the backend.
+
+        Please *always* use this methods instead of `requests` directly.
+        We can log all request calls this way, which can help debugging immensely.
+
+        Parameters
+        ----------
+        url_path:str
+          URL path that we want to request from. So every thing that follows api.host. You can omit the api prefix and api version if you use api_request=True they are automatically added.
+
+        method: str
+          One of `GET`, `OPTIONS`, `HEAD`, `POST`, `PUT, `PATCH`, or `DELETE` as this will directly passed to `requests.request(...)`. See https://docs.python-requests.org/en/latest/api/ for details.
+
+        headers: Dict
+          HTTPS headers to use for the request.
+          If None (default) use the once associated with this API object for authentication.
+
+        timeout:int
+          Time out to be used for the request call.
+
+        kwargs
+          additional keyword arguments that are passed to `request.request`
+        """
+
+        url: str = self.host
+        if api_request:
+            url += f"/{self.api_prefix}/{self.api_version}"
+        url += url_path
+
+        pre_log_message: str = f"Requesting {method} from {url}"
+        if self.extra_api_log_debug_info:
+            pre_log_message += f" from {traceback.format_stack(limit=4)} kwargs {kwargs}"
+        pre_log_message += "..."
+        self.logger.debug(pre_log_message)
+
+        if self._api_request_session is None:
+            raise CRIPTAPIRequiredError
+        response: requests.Response = self._api_request_session.request(url=url, method=method, timeout=timeout, **kwargs)
+        post_log_message: str = f"Request return with {response.status_code}"
+        if self.extra_api_log_debug_info:
+            post_log_message += f" {response.text}"
+        self.logger.debug(post_log_message)
+
+        return response
```

### Comparing `cript-2.2.0/src/cript/api/exceptions.py` & `cript-2.3.0/src/cript/api/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,277 +1,286 @@
-import json
-from typing import List, Set
-
-from beartype import beartype
-
-from cript.exceptions import CRIPTException
-
-
-class CRIPTConnectionError(CRIPTException):
-    """
-    ## Definition
-    Raised when the cript.API object cannot connect to CRIPT with the given host and token
-
-    ## Troubleshooting
-    The best way to fix this error is to check that your host and token are written and used correctly within
-    the cript.API object. This error could also be shown if the API is unresponsive and the cript.API object
-    just cannot successfully connect to it.
-    """
-
-    def __init__(self, host, token):
-        self.host = host
-        # Do not store full token in stack trace for security reasons
-        uncovered_chars = len(token) // 4
-        self.token = token[:uncovered_chars]
-        self.token += "*" * (len(token) - 2 * uncovered_chars)
-        self.token += token[-uncovered_chars:]
-
-    def __str__(self) -> str:
-        error_message = f"Could not connect to CRIPT with the given host ({self.host}) and token ({self.token}). " f"Please be sure both host and token are entered correctly."
-
-        return error_message
-
-
-class InvalidVocabulary(CRIPTException):
-    """
-    Raised when the CRIPT controlled vocabulary is invalid
-    """
-
-    vocab: str = ""
-    possible_vocab: List[str] = []
-
-    def __init__(self, vocab: str, possible_vocab: List[str]) -> None:
-        self.vocab = vocab
-        self.possible_vocab = possible_vocab
-
-    def __str__(self) -> str:
-        error_message = f"The vocabulary '{self.vocab}' entered does not exist within the CRIPT controlled vocabulary." f" Please pick a valid CRIPT vocabulary from {self.possible_vocab}"
-        return error_message
-
-
-class InvalidVocabularyCategory(CRIPTException):
-    """
-    Raised when the CRIPT controlled vocabulary category is unknown
-    and gives the user a list of all valid vocabulary categories
-    """
-
-    def __init__(self, vocab_category: str, valid_vocab_category: List[str]):
-        self.vocab_category = vocab_category
-        self.valid_vocab_category = valid_vocab_category
-
-    def __str__(self) -> str:
-        error_message = f"The vocabulary category {self.vocab_category} does not exist within the CRIPT controlled vocabulary. " f"Please pick a valid CRIPT vocabulary category from {self.valid_vocab_category}."
-
-        return error_message
-
-
-class CRIPTAPIRequiredError(CRIPTException):
-    """
-    ## Definition
-    Exception to be raised when the API object is requested, but no cript.API object exists yet.
-
-    The CRIPT Python SDK relies on a cript.API object for creation, validation, and modification of nodes.
-    The cript.API object may be explicitly called by the user to perform operations to the API, or
-    implicitly called by the Python SDK under the hood to perform some sort of validation.
-
-    ## Troubleshooting
-    To fix this error please instantiate an api object
-
-    ```python
-    import cript
-
-    my_host = "https://api.criptapp.org/"
-    my_token = "123456" # To use your token securely, please consider using environment variables
-
-    my_api = cript.API(host=my_host, token=my_token)
-    ```
-    """
-
-    def __init__(self):
-        pass
-
-    def __str__(self) -> str:
-        error_message = "cript.API object is required for an operation, but it does not exist." "Please instantiate a cript.API object to continue." "See the documentation for more details."
-
-        return error_message
-
-
-class CRIPTAPISaveError(CRIPTException):
-    """
-    ## Definition
-    CRIPTAPISaveError is raised when the API responds with a http status code that is anything other than 200.
-    The status code and API response is shown to the user to help them debug the issue.
-
-    ## Troubleshooting
-    This error is more of a case by case basis, but the best way to approach it to understand that the
-    CRIPT Python SDK sent an HTTP POST request with a giant JSON in the request body
-    to the CRIPT API. The API then read that request, and it responded with some sort of error either
-    to the that JSON or how the request was sent.
-    """
-
-    api_host_domain: str
-    http_code: str
-    api_response: str
-
-    def __init__(self, api_host_domain: str, http_code: str, api_response: str, patch_request: bool, pre_saved_nodes: Set[str], json_data: str):
-        self.api_host_domain = api_host_domain
-        self.http_code = http_code
-        self.api_response = api_response
-        self.patch_request = patch_request
-        self.pre_saved_nodes = pre_saved_nodes
-        self.json_data = json_data
-
-    def __str__(self) -> str:
-        type = "POST"
-        if self.patch_request:
-            type = "PATCH"
-        error_message = f"API responded to {type} with 'http:{self.http_code} {self.api_response}'"
-        if self.json_data:
-            error_message += f" data: {self.json_data}"
-
-        return error_message
-
-
-class CRIPTDuplicateNameError(CRIPTAPISaveError):
-    """
-    Exception raised when attempting to save a node with a name that already exists in CRIPT.
-
-    This exception class extends `CRIPTAPISaveError` and is used to handle errors
-    that occur when a node's name duplicates an existing node's name in the CRIPT database.
-
-    Parameters
-    ----------
-    api_response : dict
-        The response returned from the API that contains the error details.
-    json_data : str
-        The JSON data of the node that caused the duplication error.
-    parent_cript_save_error : CRIPTAPISaveError
-        The original `CRIPTAPISaveError` instance containing additional context of the error.
-
-    ## Troubleshooting
-    #### Duplicate Name Errors
-    Make sure that the name you are using to save a node is unique and does not already exist in the database.
-    If you encounter a `CRIPTDuplicateNameError`, check the name of your node and try a different name.
-    """
-
-    def __init__(self, api_response, json_data: str, parent_cript_save_error: CRIPTAPISaveError):
-        super().__init__(
-            parent_cript_save_error.api_host_domain, api_response["code"], api_response=api_response["error"], patch_request=parent_cript_save_error.patch_request, pre_saved_nodes=parent_cript_save_error.pre_saved_nodes, json_data=json_data
-        )
-
-        # We don't care if the data is invalid JSON
-        # So let's catch a couple of common exceptions and ensure still meaning error messages
-        # (and debug info in case it does happen.)
-        try:
-            json_dict = json.loads(self.json_data)
-        except (TypeError, json.JSONDecodeError):
-            self.name = "unknown_name"
-            self.node = "UnknownType"
-        try:
-            self.name = json_dict["name"]
-        except KeyError:
-            self.name = "unknown_name_key"
-        try:
-            self.node = json_dict["node"][0]
-        except KeyError:
-            self.node = "UnknownTypeKey"
-        except IndexError:
-            self.node = "UnknownTypeIdx"
-
-    def __str__(self) -> str:
-        return f"The name '{self.name}' for your {self.node} node is already present in CRIPT. Please use a unique name"
-
-
-class InvalidHostError(CRIPTException):
-    """
-    ## Definition
-    Exception is raised when the host given to the API is invalid
-
-    ## Troubleshooting
-    This is a simple error to fix, simply put `http://` or preferably `https://` in front of your domain
-    when passing in the host to the cript.API class such as `https://api.criptapp.org/`
-
-    Currently, the only web protocol that is supported with the CRIPT Python SDK is `HTTP`.
-
-    ### Example
-    ```python
-    import cript
-
-    my_valid_host = "https://api.criptapp.org/"
-    my_token = "123456" # To use your token securely, please consider using environment variables
-
-    my_api = cript.API(host=my_valid_host, token=my_token)
-    ```
-
-    Warnings
-    --------
-    Please consider always using [HTTPS](https://developer.mozilla.org/en-US/docs/Glossary/HTTPS)
-    as that is a secure protocol and avoid using `HTTP` as it is insecure.
-    The CRIPT Python SDK will give a warning in the terminal when it detects a host with `HTTP`
-
-
-    """
-
-    def __init__(self) -> None:
-        pass
-
-    def __str__(self) -> str:
-        return "The host must start with http or https"
-
-
-class APIError(CRIPTException):
-    """
-    ## Definition
-    This is a generic error made to display API errors to the user to troubleshoot.
-
-    ## Troubleshooting
-    Please keep in mind that the CRIPT Python SDK turns the [Project](../../nodes/primary_nodes/project)
-    node into a giant JSON and sends that to the API to be processed. If there are any errors while processing
-    the giant JSON generated by the CRIPT Python SDK, then the API will return an error about the http request
-    and the JSON sent to it.
-
-    The best way to trouble shoot this is to figure out what the API error means and figure out where
-    in the Python SDK this error occurred and what could be the reason under the hood.
-
-    ### Steps to try:
-    1. What does the API error mean?
-        1. Is the error something you can easily fix by maybe renaming a node?
-        1. Does the `http_method` look reasonable?
-        1. Does the `URL` that the data was sent to look reasonable?
-    1. Is there a problem within the JSON?
-    1. Is the problem within how the SDK is converting nodes from and to JSON (serialization and deserialization)?
-    """
-
-    api_error: str = ""
-
-    # having the URL that the API gave an error for helps in debugging
-    api_url: str = ""
-    http_method: str = ""
-
-    @beartype
-    def __init__(self, api_error: str, http_method: str, api_url: str) -> None:
-        self.api_error = api_error
-
-        self.api_url = api_url
-
-        # TODO consider having an enum for all the HTTP methods so they are easily entered and disallows anything
-        #   that would be not make sense
-        self.http_method = http_method
-
-    def __str__(self) -> str:
-        return f"CRIPT Python SDK sent HTTP `{self.http_method.upper()}` request to URL: `{self.api_url}` and API responded with {self.api_error}"
-
-
-class FileDownloadError(CRIPTException):
-    """
-    ## Definition
-    This error is raised when the API wants to download a file from an AWS S3 URL
-    via the `cript.API.download_file()` method, but the status is something other than 200.
-    """
-
-    error_message: str = ""
-
-    def __init__(self, error_message: str) -> None:
-        self.error_message = error_message
-
-    def __str__(self) -> str:
-        return self.error_message
+import json
+from typing import List, Set
+
+from beartype import beartype
+
+from cript.exceptions import CRIPTException
+
+
+class CRIPTConnectionError(CRIPTException):
+    """
+    ## Definition
+    Raised when the cript.API object cannot connect to CRIPT with the given host and token
+
+    ## Troubleshooting
+    The best way to fix this error is to check that your host and token are written and used correctly within
+    the cript.API object. This error could also be shown if the API is unresponsive and the cript.API object
+    just cannot successfully connect to it.
+    """
+
+    def __init__(self, host, token):
+        self.host = host
+        # Do not store full token in stack trace for security reasons
+        uncovered_chars = len(token) // 4
+        self.token = token[:uncovered_chars]
+        self.token += "*" * (len(token) - 2 * uncovered_chars)
+        self.token += token[-uncovered_chars:]
+
+    def __str__(self) -> str:
+        error_message = f"Could not connect to CRIPT with the given host ({self.host}) and token ({self.token}). " f"Please be sure both host and token are entered correctly."
+
+        return error_message
+
+
+class InvalidVocabulary(CRIPTException):
+    """
+    Raised when the CRIPT controlled vocabulary is invalid
+    """
+
+    vocab: str = ""
+    possible_vocab: List[str] = []
+
+    def __init__(self, vocab: str, possible_vocab: List[str]) -> None:
+        self.vocab = vocab
+        self.possible_vocab = possible_vocab
+
+    def __str__(self) -> str:
+        error_message = f"The vocabulary '{self.vocab}' entered does not exist within the CRIPT controlled vocabulary." f" Please pick a valid CRIPT vocabulary from {self.possible_vocab}"
+        return error_message
+
+
+class InvalidVocabularyCategory(CRIPTException):
+    """
+    Raised when the CRIPT controlled vocabulary category is unknown
+    and gives the user a list of all valid vocabulary categories
+    """
+
+    def __init__(self, vocab_category: str, valid_vocab_category: List[str]):
+        self.vocab_category = vocab_category
+        self.valid_vocab_category = valid_vocab_category
+
+    def __str__(self) -> str:
+        error_message = f"The vocabulary category {self.vocab_category} does not exist within the CRIPT controlled vocabulary. " f"Please pick a valid CRIPT vocabulary category from {self.valid_vocab_category}."
+
+        return error_message
+
+
+class CRIPTAPIRequiredError(CRIPTException):
+    """
+    ## Definition
+    Exception to be raised when the API object is requested, but no cript.API object exists yet.
+    Also make sure to use it in a context manager `with cript.API as api:` or  manually call
+    `connect` and `disconnect`.
+
+    The CRIPT Python SDK relies on a cript.API object for creation, validation, and modification of nodes.
+    The cript.API object may be explicitly called by the user to perform operations to the API, or
+    implicitly called by the Python SDK under the hood to perform some sort of validation.
+
+    ## Troubleshooting
+    To fix this error please instantiate an api object
+
+    ```python
+    import cript
+
+    my_host = "https://api.criptapp.org/"
+    my_token = "123456" # To use your token securely, please consider using environment variables
+
+    my_api = cript.API(host=my_host, token=my_token)
+    my_api.connect()
+    # Your code
+    my_api.disconnect()
+    ```
+    """
+
+    def __init__(self):
+        pass
+
+    def __str__(self) -> str:
+        error_message = (
+            "cript.API object is required for an operation, but it does not exist."
+            "Please instantiate a cript.API object and connect it to API for example with a context manager `with cript.API() as api:` to continue."
+            "See the documentation for more details."
+        )
+
+        return error_message
+
+
+class CRIPTAPISaveError(CRIPTException):
+    """
+    ## Definition
+    CRIPTAPISaveError is raised when the API responds with a http status code that is anything other than 200.
+    The status code and API response is shown to the user to help them debug the issue.
+
+    ## Troubleshooting
+    This error is more of a case by case basis, but the best way to approach it to understand that the
+    CRIPT Python SDK sent an HTTP POST request with a giant JSON in the request body
+    to the CRIPT API. The API then read that request, and it responded with some sort of error either
+    to the that JSON or how the request was sent.
+    """
+
+    api_host_domain: str
+    http_code: str
+    api_response: str
+
+    def __init__(self, api_host_domain: str, http_code: str, api_response: str, patch_request: bool, pre_saved_nodes: Set[str], json_data: str):
+        self.api_host_domain = api_host_domain
+        self.http_code = http_code
+        self.api_response = api_response
+        self.patch_request = patch_request
+        self.pre_saved_nodes = pre_saved_nodes
+        self.json_data = json_data
+
+    def __str__(self) -> str:
+        type = "POST"
+        if self.patch_request:
+            type = "PATCH"
+        error_message = f"API responded to {type} with 'http:{self.http_code} {self.api_response}'"
+        if self.json_data:
+            error_message += f" data: {self.json_data}"
+
+        return error_message
+
+
+class CRIPTDuplicateNameError(CRIPTAPISaveError):
+    """
+    Exception raised when attempting to save a node with a name that already exists in CRIPT.
+
+    This exception class extends `CRIPTAPISaveError` and is used to handle errors
+    that occur when a node's name duplicates an existing node's name in the CRIPT database.
+
+    Parameters
+    ----------
+    api_response : dict
+        The response returned from the API that contains the error details.
+    json_data : str
+        The JSON data of the node that caused the duplication error.
+    parent_cript_save_error : CRIPTAPISaveError
+        The original `CRIPTAPISaveError` instance containing additional context of the error.
+
+    ## Troubleshooting
+    #### Duplicate Name Errors
+    Make sure that the name you are using to save a node is unique and does not already exist in the database.
+    If you encounter a `CRIPTDuplicateNameError`, check the name of your node and try a different name.
+    """
+
+    def __init__(self, api_response, json_data: str, parent_cript_save_error: CRIPTAPISaveError):
+        super().__init__(
+            parent_cript_save_error.api_host_domain, api_response["code"], api_response=api_response["error"], patch_request=parent_cript_save_error.patch_request, pre_saved_nodes=parent_cript_save_error.pre_saved_nodes, json_data=json_data
+        )
+
+        # We don't care if the data is invalid JSON
+        # So let's catch a couple of common exceptions and ensure still meaning error messages
+        # (and debug info in case it does happen.)
+        try:
+            json_dict = json.loads(self.json_data)
+        except (TypeError, json.JSONDecodeError):
+            self.name = "unknown_name"
+            self.node = "UnknownType"
+        try:
+            self.name = json_dict["name"]
+        except KeyError:
+            self.name = "unknown_name_key"
+        try:
+            self.node = json_dict["node"][0]
+        except KeyError:
+            self.node = "UnknownTypeKey"
+        except IndexError:
+            self.node = "UnknownTypeIdx"
+
+    def __str__(self) -> str:
+        return f"The name '{self.name}' for your {self.node} node is already present in CRIPT. Please use a unique name"
+
+
+class InvalidHostError(CRIPTException):
+    """
+    ## Definition
+    Exception is raised when the host given to the API is invalid
+
+    ## Troubleshooting
+    This is a simple error to fix, simply put `http://` or preferably `https://` in front of your domain
+    when passing in the host to the cript.API class such as `https://api.criptapp.org/`
+
+    Currently, the only web protocol that is supported with the CRIPT Python SDK is `HTTP`.
+
+    ### Example
+    ```python
+    import cript
+
+    my_valid_host = "https://api.criptapp.org/"
+    my_token = "123456" # To use your token securely, please consider using environment variables
+
+    my_api = cript.API(host=my_valid_host, token=my_token)
+    ```
+
+    Warnings
+    --------
+    Please consider always using [HTTPS](https://developer.mozilla.org/en-US/docs/Glossary/HTTPS)
+    as that is a secure protocol and avoid using `HTTP` as it is insecure.
+    The CRIPT Python SDK will give a warning in the terminal when it detects a host with `HTTP`
+
+
+    """
+
+    def __init__(self) -> None:
+        pass
+
+    def __str__(self) -> str:
+        return "The host must start with http or https"
+
+
+class APIError(CRIPTException):
+    """
+    ## Definition
+    This is a generic error made to display API errors to the user to troubleshoot.
+
+    ## Troubleshooting
+    Please keep in mind that the CRIPT Python SDK turns the [Project](../../nodes/primary_nodes/project)
+    node into a giant JSON and sends that to the API to be processed. If there are any errors while processing
+    the giant JSON generated by the CRIPT Python SDK, then the API will return an error about the http request
+    and the JSON sent to it.
+
+    The best way to trouble shoot this is to figure out what the API error means and figure out where
+    in the Python SDK this error occurred and what could be the reason under the hood.
+
+    ### Steps to try:
+    1. What does the API error mean?
+        1. Is the error something you can easily fix by maybe renaming a node?
+        1. Does the `http_method` look reasonable?
+        1. Does the `URL` that the data was sent to look reasonable?
+    1. Is there a problem within the JSON?
+    1. Is the problem within how the SDK is converting nodes from and to JSON (serialization and deserialization)?
+    """
+
+    api_error: str = ""
+
+    # having the URL that the API gave an error for helps in debugging
+    api_url: str = ""
+    http_method: str = ""
+
+    @beartype
+    def __init__(self, api_error: str, http_method: str, api_url: str) -> None:
+        self.api_error = api_error
+
+        self.api_url = api_url
+
+        # TODO consider having an enum for all the HTTP methods so they are easily entered and disallows anything
+        #   that would be not make sense
+        self.http_method = http_method
+
+    def __str__(self) -> str:
+        return f"CRIPT Python SDK sent HTTP `{self.http_method.upper()}` request to URL: `{self.api_url}` and API responded with {self.api_error}"
+
+
+class FileDownloadError(CRIPTException):
+    """
+    ## Definition
+    This error is raised when the API wants to download a file from an AWS S3 URL
+    via the `cript.API.download_file()` method, but the status is something other than 200.
+    """
+
+    error_message: str = ""
+
+    def __init__(self, error_message: str) -> None:
+        self.error_message = error_message
+
+    def __str__(self) -> str:
+        return self.error_message
```

### Comparing `cript-2.2.0/src/cript/api/utils/get_host_token.py` & `cript-2.3.0/src/cript/api/utils/get_host_token.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/api/utils/helper_functions.py` & `cript-2.3.0/src/cript/api/utils/helper_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import Dict, List, Union
 
 from cript.nodes.exceptions import CRIPTJsonNodeError
-from cript.nodes.util import _is_node_field_valid
+from cript.nodes.util.json import _is_node_field_valid
 
 
 def _get_node_type_from_json(node_json: Union[Dict, str]) -> str:
     """
     takes a node JSON and output the node_type `Project`, `Material`, etc.
 
     1. convert node JSON dict or str to dict
```

### Comparing `cript-2.2.0/src/cript/api/utils/save_helper.py` & `cript-2.3.0/src/cript/api/utils/save_helper.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/api/utils/web_file_downloader.py` & `cript-2.3.0/src/cript/api/utils/web_file_downloader.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/api/valid_search_modes.py` & `cript-2.3.0/src/cript/api/valid_search_modes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from enum import Enum
-
-
-class SearchModes(Enum):
-    """
-    Available search modes to use with the CRIPT API search
-
-    Attributes
-    ----------
-    NODE_TYPE : str
-        Search by node type.
-    EXACT_NAME : str
-        Search by exact node name.
-    CONTAINS_NAME : str
-        Search by node name containing a given string.
-    UUID : str
-        Search by node UUID.
-    BIGSMILES: str
-        search materials by bigsmiles identifier.
-
-    Examples
-    -------
-    >>> import cript
-    >>> # search by node type
-    >>> materials_paginator = api.search(
-    ...     node_type=cript.Material,
-    ...     search_mode=cript.SearchModes.NODE_TYPE,
-    ...     value_to_search=None,
-    ... )   # doctest: +SKIP
-
-    For more details and code examples,
-    please check the [cript.API.search( ) method](../api/#cript.api.api.API.search)
-    """
-
-    NODE_TYPE: str = ""
-    EXACT_NAME: str = "exact_name"
-    CONTAINS_NAME: str = "contains_name"
-    UUID: str = "uuid"
-    # UUID_CHILDREN = "uuid_children"
-    BIGSMILES: str = "bigsmiles"
+from enum import Enum
+
+
+class SearchModes(Enum):
+    """
+    Available search modes to use with the CRIPT API search
+
+    Attributes
+    ----------
+    NODE_TYPE : str
+        Search by node type.
+    EXACT_NAME : str
+        Search by exact node name.
+    CONTAINS_NAME : str
+        Search by node name containing a given string.
+    UUID : str
+        Search by node UUID.
+    BIGSMILES: str
+        search materials by bigsmiles.
+
+    Examples
+    -------
+    >>> import cript
+    >>> # search by node type
+    >>> materials_paginator = api.search(
+    ...     node_type=cript.Material,
+    ...     search_mode=cript.SearchModes.NODE_TYPE,
+    ...     value_to_search=None,
+    ... )   # doctest: +SKIP
+
+    For more details and code examples,
+    please check the [cript.API.search( ) method](../api/#cript.api.api.API.search)
+    """
+
+    NODE_TYPE: str = ""
+    EXACT_NAME: str = "exact_name"
+    CONTAINS_NAME: str = "contains_name"
+    UUID: str = "uuid"
+    # UUID_CHILDREN = "uuid_children"
+    BIGSMILES: str = "bigsmiles"
```

### Comparing `cript-2.2.0/src/cript/nodes/__init__.py` & `cript-2.3.0/src/cript/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/nodes/core.py` & `cript-2.3.0/src/cript/nodes/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,622 +1,658 @@
-import copy
-import dataclasses
-import json
-import re
-import uuid
-from abc import ABC
-from dataclasses import asdict, dataclass, replace
-from typing import Dict, List, Optional, Set
-
-from cript.nodes.exceptions import (
-    CRIPTAttributeModificationError,
-    CRIPTExtraJsonAttributes,
-    CRIPTJsonSerializationError,
-)
-
-tolerated_extra_json = []
-
-
-def add_tolerated_extra_json(additional_tolerated_json: str):
-    """
-    In case a node should be loaded from JSON (such as `getting` them from the API),
-    but the API sends additional JSON attributes, these can be set to tolerated temporarily with this routine.
-    """
-    tolerated_extra_json.append(additional_tolerated_json)
-
-
-def get_new_uid():
-    return "_:" + str(uuid.uuid4())
-
-
-class classproperty(object):
-    def __init__(self, f):
-        self.f = f
-
-    def __get__(self, obj, owner):
-        if obj is None:
-            return self.f(owner)
-        return self.f(obj)
-
-
-class BaseNode(ABC):
-    """
-    This abstract class is the base of all CRIPT nodes.
-    It offers access to a json attribute class,
-    which reflects the data model JSON attributes.
-    Also, some basic shared functionality is provided by this base class.
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes:
-        node: List[str] = dataclasses.field(default_factory=list)
-        uid: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @classproperty
-    def node_type(self):
-        name = type(self).__name__
-        if name == "ABCMeta":
-            name = self.__name__
-        return name
-
-    @classproperty
-    def node_type_snake_case(self):
-        camel_case = self.node_type
-        # Regex to convert camel case to snake case.
-        snake_case = re.sub(r"(?<!^)(?=[A-Z])", "_", camel_case).lower()
-        return snake_case
-
-    # Prevent new attributes being set.
-    # This might just be temporary, but for now, I don't want to accidentally add new attributes, when I mean to modify one.
-    def __setattr__(self, key, value):
-        if not hasattr(self, key):
-            raise CRIPTAttributeModificationError(self.node_type, key, value)
-        super().__setattr__(key, value)
-
-    def __init__(self, **kwargs):
-        for kwarg in kwargs:
-            if kwarg not in tolerated_extra_json:
-                if kwarg.endswith("_count"):
-                    try:
-                        possible_array = getattr(self._json_attrs.kwarg[: -len("_count")])
-                        if not isinstance(possible_array, list):
-                            raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
-                    except AttributeError:
-                        raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
-                else:
-                    try:
-                        getattr(self._json_attrs, kwarg)
-                    except AttributeError:
-                        raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
-
-        uid = get_new_uid()
-        self._json_attrs = replace(self._json_attrs, node=[self.node_type], uid=uid)
-
-    def __str__(self) -> str:
-        """
-        Return a string representation of a node data model attributes.
-
-        Returns
-        -------
-        str
-            A string representation of the node.
-        """
-        return str(asdict(self._json_attrs))
-
-    @property
-    def uid(self):
-        return self._json_attrs.uid
-
-    @property
-    def node(self):
-        return self._json_attrs.node
-
-    def _update_json_attrs_if_valid(self, new_json_attr: JsonAttributes) -> None:
-        """
-        tries to update the node if valid and then checks if it is valid or not
-
-        1. updates the node with the new information
-        1. run db schema validation on it
-            1. if db schema validation succeeds then update and continue
-            1. else: raise an error and tell the user what went wrong
-
-        Parameters
-        ----------
-        new_json_attr
-
-        Raises
-        ------
-        Exception
-
-        Returns
-        -------
-        None
-        """
-        old_json_attrs = self._json_attrs
-        self._json_attrs = new_json_attr
-
-        try:
-            self.validate()
-        except Exception as exc:
-            self._json_attrs = old_json_attrs
-            raise exc
-
-    def validate(self, api=None, is_patch: bool = False, force_validation: bool = False) -> None:
-        """
-        Validate this node (and all its children) against the schema provided by the data bank.
-
-        Raises:
-        -------
-        Exception with more error information.
-        """
-        from cript.api.api import _get_global_cached_api
-
-        if api is None:
-            api = _get_global_cached_api()
-        api._is_node_schema_valid(self.get_json(is_patch=is_patch).json, is_patch=is_patch, force_validation=force_validation)
-
-    @classmethod
-    def _from_json(cls, json_dict: dict):
-        # TODO find a way to handle uuid nodes only
-
-        # Child nodes can inherit and overwrite this.
-        # They should call super()._from_json first, and modified the returned object after if necessary
-        # We create manually a dict that contains all elements from the send dict.
-        # That eliminates additional fields and doesn't require asdict.
-        arguments = {}
-        default_dataclass = cls.JsonAttributes()
-        for field in json_dict:
-            try:
-                getattr(default_dataclass, field)
-            except AttributeError:
-                pass
-            else:
-                arguments[field] = json_dict[field]
-
-        # add omitted fields from default (necessary if they are required)
-        for field_name in [field.name for field in dataclasses.fields(default_dataclass)]:
-            if field_name not in arguments:
-                arguments[field_name] = getattr(default_dataclass, field_name)
-
-        # If a node with this UUID already exists, we don't create a new node.
-        # Instead we use the existing node from the cache and just update it.
-        from cript.nodes.uuid_base import UUIDBaseNode
-
-        if "uuid" in json_dict and json_dict["uuid"] in UUIDBaseNode._uuid_cache:
-            node = UUIDBaseNode._uuid_cache[json_dict["uuid"]]
-        else:  # Create a new node
-            try:
-                node = cls(**arguments)
-            # TODO we should not catch all exceptions if we are handling them, and instead let it fail
-            #  to create a good error message that points to the correct place that it failed to make debugging easier
-            except Exception as exc:
-                print(cls, arguments)
-                raise exc
-
-        attrs = cls.JsonAttributes(**arguments)
-
-        # Handle default attributes manually.
-        for field in attrs.__dict__:
-            # Conserve newly assigned uid if uid is default (empty)
-            if getattr(attrs, field) == getattr(default_dataclass, field):
-                attrs = replace(attrs, **{str(field): getattr(node, field)})
-
-        try:  # TODO remove this temporary solution
-            if not attrs.uid.startswith("_:"):
-                attrs = replace(attrs, uid="_:" + attrs.uid)
-        except AttributeError:
-            pass
-        # But here we force even usually unwritable fields to be set.
-        node._update_json_attrs_if_valid(attrs)
-
-        return node
-
-    def __deepcopy__(self, memo):
-        # Ideally I would call `asdict`, but that is not allowed inside a deepcopy chain.
-        # Making a manual transform into a dictionary here.
-        arguments = {}
-        for field in self.JsonAttributes().__dataclass_fields__:
-            arguments[field] = copy.deepcopy(getattr(self._json_attrs, field), memo)
-        # TODO URL handling
-
-        # Since we excluded 'uuid' from arguments,
-        # a new uid will prompt the creation of a new matching uuid.
-        uid = get_new_uid()
-        arguments["uid"] = uid
-
-        # Create node and init constructor attributes
-        node = self.__class__(**arguments)
-        # Update none constructor writable attributes.
-        node._update_json_attrs_if_valid(self.JsonAttributes(**arguments))
-        return node
-
-    @property
-    def json(self):
-        """
-        Property to obtain a simple json string.
-        Calls `get_json` with default arguments.
-        """
-        # We cannot validate in `get_json` because we call it inside `validate`.
-        # But most uses are probably the property, so we can validate the node here.
-        json_string: str = self.get_json().json
-
-        from cript.api.api import _get_global_cached_api
-
-        api = _get_global_cached_api()
-        api._is_node_schema_valid(json_string, force_validation=True)
-
-        return json_string
-
-    def get_expanded_json(self, **kwargs) -> str:
-        """
-        Generates a long-form JSON representation of the current node and its hierarchy.
-
-        The long-form JSON includes complete details of the node, eliminating the need for
-         references to UUIDs to nodes stored in the CRIPT database. This comprehensive representation
-         is useful for offline storage of CRIPT nodes, transferring nodes between different CRIPT instances,
-         or for backup purposes.
-
-        The generated long-form JSON can be reloaded into the SDK using
-        [`cript.load_nodes_from_json()`](../../../utility_functions/#cript.nodes.util.load_nodes_from_json),
-        ensuring consistency and completeness of the node data.
-        However, it's important to note that this long-form JSON might not comply directly with the JSON schema
-        required for POST or PATCH requests to the CRIPT API.
-
-        Optional keyword arguments (`kwargs`) are supported and are passed directly to `json.dumps()`.
-        These arguments allow customization of the JSON output, such as formatting for readability
-        or pretty printing.
-
-        Parameters
-        ----------
-        **kwargs : dict, optional
-            Additional keyword arguments for `json.dumps()` to customize the JSON output, such as `indent`
-            for pretty-printing.
-
-        Returns
-        -------
-        str
-            A comprehensive JSON string representing the current node and its entire hierarchy in long-form.
-
-        Notes
-        -----
-        The `get_expanded_json()` method differs from the standard [`json`](./#cript.nodes.core.BaseNode.json)
-        property or method, which might provide a more condensed version of the node's data.
-
-        > For more information on condensed JSON and deserialization, please feel free to reference our discussion
-        > on [deserializing Python nodes to JSON](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/177)
-
-        Examples
-        --------
-        >>> import cript
-        >>> # ============= Create all needed nodes =============
-        >>> my_project = cript.Project(name=f"my_Project")
-        >>> my_collection = cript.Collection(name="my collection")
-        >>> my_material_1 = cript.Material(
-        ...     name="my material 1", identifier=[{"bigsmiles": "my material 1 bigsmiles"}]
-        ... )
-        >>> my_material_2 = cript.Material(
-        ...     name="my material 2", identifier=[{"bigsmiles": "my material 2 bigsmiles"}]
-        ... )
-        >>> my_inventory = cript.Inventory(
-        ...     name="my inventory", material=[my_material_1, my_material_2]
-        ... )
-        >>> #  ============= Assemble nodes =============
-        >>> my_project.collection = [my_collection]
-        >>> my_project.collection[0].inventory = [my_inventory]
-        >>> #  ============= Get long form JSON =============
-        >>> long_form_json = my_project.get_expanded_json(indent=4)
-
-        ???+ info "Condensed JSON VS Expanded JSON"
-            # Default Condensed JSON
-            > This is the JSON when `my_project.json` is called
-
-            ```json linenums="1"
-            {
-               "node":[
-                  "Project"
-               ],
-               "uid":"_:d0d1b3c9-d552-4d4f-afd2-76f01538b87a",
-               "uuid":"d0d1b3c9-d552-4d4f-afd2-76f01538b87a",
-               "name":"my_Project",
-               "collection":[
-                  {
-                     "node":[
-                        "Collection"
-                     ],
-                     "uid":"_:07765ac8-862a-459e-9d99-d0439d6a6a09",
-                     "uuid":"07765ac8-862a-459e-9d99-d0439d6a6a09",
-                     "name":"my collection",
-                     "inventory":[
-                        {
-                           "node":[
-                              "Inventory"
-                           ],
-                           "uid":"_:4cf2bbee-3dc0-400b-8269-709f99d89d9f",
-                           "uuid":"4cf2bbee-3dc0-400b-8269-709f99d89d9f",
-                           "name":"my inventory",
-                           "material":[
-                              {
-                                 "uuid":"0cf14572-4da2-43f2-8cb9-e8374086368e"
-                              },
-                              {
-                                 "uuid":"6302a8b0-4265-4a3a-a40f-bbcbb7293046"
-                              }
-                           ]
-                        }
-                     ]
-                  }
-               ]
-            }
-            ```
-
-            # Expanded JSON
-            > This is what is created when `my_project.get_expanded_json()`
-
-            ```json linenums="1"
-            {
-               "node":[
-                  "Project"
-               ],
-               "uid":"_:afe4bb2f-fa75-4736-b692-418a5143e6f5",
-               "uuid":"afe4bb2f-fa75-4736-b692-418a5143e6f5",
-               "name":"my_Project",
-               "collection":[
-                  {
-                     "node":[
-                        "Collection"
-                     ],
-                     "uid":"_:8b5c8125-c956-472a-9d07-8cb7b402b101",
-                     "uuid":"8b5c8125-c956-472a-9d07-8cb7b402b101",
-                     "name":"my collection",
-                     "inventory":[
-                        {
-                           "node":[
-                              "Inventory"
-                           ],
-                           "uid":"_:1bd3c966-cb35-494d-85cd-3515cde570f3",
-                           "uuid":"1bd3c966-cb35-494d-85cd-3515cde570f3",
-                           "name":"my inventory",
-                           "material":[
-                              {
-                                 "node":[
-                                    "Material"
-                                 ],
-                                 "uid":"_:07bc3e4f-757f-4ac7-ae8a-7a0c68272531",
-                                 "uuid":"07bc3e4f-757f-4ac7-ae8a-7a0c68272531",
-                                 "name":"my material 1",
-                                 "bigsmiles":"my material 1 bigsmiles"
-                              },
-                              {
-                                 "node":[
-                                    "Material"
-                                 ],
-                                 "uid":"_:64565687-5707-4d67-860f-5ee4a057a45f",
-                                 "uuid":"64565687-5707-4d67-860f-5ee4a057a45f",
-                                 "name":"my material 2",
-                                 "bigsmiles":"my material 2 bigsmiles"
-                              }
-                           ]
-                        }
-                     ]
-                  }
-               ]
-            }
-            ```
-        """
-        return self.get_json(handled_ids=None, known_uuid=None, suppress_attributes=None, is_patch=False, condense_to_uuid={}, **kwargs).json
-
-    def get_json(
-        self,
-        handled_ids: Optional[Set[str]] = None,
-        known_uuid: Optional[Set[str]] = None,
-        suppress_attributes: Optional[Dict[str, Set[str]]] = None,
-        is_patch: bool = False,
-        condense_to_uuid: Dict[str, Set[str]] = {
-            "Material": {"parent_material", "component"},
-            "Experiment": {"data"},
-            "Inventory": {"material"},
-            "Ingredient": {"material"},
-            "Property": {"component"},
-            "ComputationProcess": {"material"},
-            "Data": {"material"},
-            "Process": {"product", "waste"},
-            "Project": {"member", "admin"},
-            "Collection": {"member", "admin"},
-        },
-        **kwargs
-    ):
-        """
-        User facing access to get the JSON of a node.
-        Opposed to the also available property json this functions allows further control.
-        Additionally, this function does not call `self.validate()` but the property `json` does.
-        We also accept `kwargs`, that are passed on to the JSON decoding via `json.dumps()` this can be used for example to prettify the output.
-
-
-        Returns named tuple with json and handled ids as result.
-        """
-
-        @dataclass(frozen=True)
-        class ReturnTuple:
-            json: str
-            handled_ids: set
-
-        # Do not check for circular references, since we handle them manually
-        kwargs["check_circular"] = kwargs.get("check_circular", False)
-
-        # Delayed import to avoid circular imports
-        from cript.nodes.util import NodeEncoder
-
-        if handled_ids is None:
-            handled_ids = set()
-        previous_handled_nodes = copy.deepcopy(NodeEncoder.handled_ids)
-        NodeEncoder.handled_ids = handled_ids
-
-        # Similar to uid, we handle pre-saved known uuid such that they are UUID edges only
-        if known_uuid is None:
-            known_uuid = set()
-        previous_known_uuid = copy.deepcopy(NodeEncoder.known_uuid)
-        NodeEncoder.known_uuid = known_uuid
-        previous_suppress_attributes = copy.deepcopy(NodeEncoder.suppress_attributes)
-        NodeEncoder.suppress_attributes = suppress_attributes
-        previous_condense_to_uuid = copy.deepcopy(NodeEncoder.condense_to_uuid)
-        NodeEncoder.condense_to_uuid = condense_to_uuid
-
-        try:
-            return ReturnTuple(json.dumps(self, cls=NodeEncoder, **kwargs), NodeEncoder.handled_ids)
-        except Exception as exc:
-            # TODO this handling that doesn't tell the user what happened and how they can fix it
-            #   this just tells the user that something is wrong
-            #   this should be improved to tell the user what went wrong and where
-            raise CRIPTJsonSerializationError(str(type(self)), str(self._json_attrs)) from exc
-        finally:
-            NodeEncoder.handled_ids = previous_handled_nodes
-            NodeEncoder.known_uuid = previous_known_uuid
-            NodeEncoder.suppress_attributes = previous_suppress_attributes
-            NodeEncoder.condense_to_uuid = previous_condense_to_uuid
-
-    def find_children(self, search_attr: dict, search_depth: int = -1, handled_nodes=None) -> List:
-        """
-        Finds all the children in a given tree of nodes (specified by its root),
-        that match the criteria of search_attr.
-        If a node is present multiple times in the graph, it is only once in the search results.
-
-        search_dept: Max depth of the search into the tree. Helpful if circles are expected. -1 specifies no limit
-
-        search_attr: dict
-           Dictionary that specifies which JSON attributes have to be present in a given node.
-           If an attribute is a list, it it is sufficient if the specified attributes are in the list,
-           if others are present too, that does not exclude the child.
-
-           Example: search_attr = `{"node": ["Parameter"]}` finds all "Parameter" nodes.
-                    search_attr = `{"node": ["Algorithm"], "parameter": {"name" : "update_frequency"}}`
-                                           finds all "Algorithm" nodes, that have a parameter "update_frequency".
-                                           Since parameter is a list an alternative notation is
-                                           ``{"node": ["Algorithm"], "parameter": [{"name" : "update_frequency"}]}`
-                                           and Algorithms are not excluded they have more parameters.
-                    search_attr = `{"node": ["Algorithm"], "parameter": [{"name" : "update_frequency"},
-                                           {"name" : "cutoff_distance"}]}`
-                                           finds all algorithms that have a parameter "update_frequency" and "cutoff_distance".
-
-        """
-
-        def is_attr_present(node: BaseNode, key, value):
-            """
-            Helper function that checks if an attribute is present in a node.
-            """
-            try:
-                attr_key = getattr(node._json_attrs, key)
-            except AttributeError:
-                return False
-
-            # To save code paths, I convert non-lists into lists with one element.
-            if not isinstance(attr_key, list):
-                attr_key = [attr_key]
-            if not isinstance(value, list):
-                value = [value]
-
-            # The definition of search is, that all values in a list have to be present.
-            # To fulfill this AND condition, we count the number of occurrences of that value condition
-            number_values_found = 0
-            # Runtime contribution: O(m), where is is the number of search keys
-            for v in value:
-                # Test for simple values (not-nodes)
-                if v in attr_key:
-                    number_values_found += 1
-
-                # Test if value is present in one of the specified attributes (OR condition)
-                # Runtime contribution: O(m), where m is the number of nodes in the attribute list.
-                for attr in attr_key:
-                    # if the attribute is a node and the search value is a dictionary,
-                    # we can verify that this condition is met if it finds the node itself with `find_children`.
-                    if isinstance(attr, BaseNode) and isinstance(v, dict):
-                        # Since we only want to test the node itself and not any of its children, we set recursion to 0.
-                        # Runtime contribution: recursive call, with depth search depth of the search dictionary O(h)
-                        if len(attr.find_children(v, 0)) > 0:
-                            number_values_found += 1
-                            # Since this an OR condition, we abort early.
-                            # This also doesn't inflate the number_values_count,
-                            # since every OR condition should only add a max of 1.
-                            break
-            # Check if the AND condition of the values is met
-            return number_values_found == len(value)
-
-        if handled_nodes is None:
-            handled_nodes = []
-
-        # Protect against cycles in graph, by handling every instance of a node only once
-        if self in handled_nodes:
-            return []
-        handled_nodes += [self]
-
-        found_children = []
-
-        # In this search we include the calling node itself.
-        # We check for this node if all specified attributes are present by counting them (AND condition).
-        found_attr = 0
-        for key, value in search_attr.items():
-            if is_attr_present(self, key, value):
-                found_attr += 1
-        # If exactly all attributes are found, it matches the search criterion
-        if found_attr == len(search_attr):
-            found_children += [self]
-
-        # Recursion according to the recursion depth for all node children.
-        if search_depth != 0:
-            # Loop over all attributes, runtime contribution (none, or constant (max number of attributes of a node)
-            for field in self._json_attrs.__dataclass_fields__:
-                value = getattr(self._json_attrs, field)
-                # To save code paths, I convert non-lists into lists with one element.
-                if not isinstance(value, list):
-                    value = [value]
-                # Run time contribution: number of elements in the attribute list.
-                for v in value:
-                    try:  # Try every attribute for recursion (duck-typing)
-                        found_children += v.find_children(search_attr, search_depth - 1, handled_nodes=handled_nodes)
-                    except AttributeError:
-                        pass
-        # Total runtime, of non-recursive call: O(m*h) + O(k) where k is the number of children for this node,
-        #   h being the depth of the search dictionary, m being the number of nodes in the attribute list.
-        # Total runtime, with recursion: O(n*(k+m*h). A full graph traversal O(n) with a cost per node, that scales with the number of children per node and the search depth of the search dictionary.
-        return found_children
-
-    def remove_child(self, child) -> bool:
-        """
-        This safely removes the first found child node from the parent.
-        This requires exact node as we test with `is` instead of `==`.
-
-        returns True if child was found and deleted, False if child not found,
-        raise DB schema exception if deletion violates DB schema.
-        """
-
-        # If we delete a child, we have to replace that with a default value.
-        # The easiest way to access this default value is to get it from the the default JsonAttribute of that class
-        default_json_attrs = self.JsonAttributes()
-        new_attrs = self._json_attrs
-        for field in self._json_attrs.__dataclass_fields__:
-            value = getattr(self._json_attrs, field)
-            if value is child:
-                new_attrs = replace(new_attrs, **{field: getattr(default_json_attrs, field)})
-                # We only want to delete the first found child
-            elif not isinstance(value, str):  # Strings are iterable, but we don't want them
-                try:  # Try if we are facing a list at the moment
-                    new_attr_list = [element for element in value]
-                except TypeError:
-                    pass  # It is OK if this field is not a list
-                else:
-                    found_child = False
-                    for i, list_value in enumerate(value):
-                        if list_value is child:
-                            found_child = True
-                            del new_attr_list[i]
-                            # Only delete first child.
-                            # Important to break loop here, since value and new_attr_list are not identical any more.
-                    if found_child:
-                        new_attrs = replace(new_attrs, **{field: new_attr_list})  # type: ignore
-                        # Again only first found place is removed
-                        break
-        # Let's see if we found the child aka the new_attrs are different than the old ones
-        if new_attrs is self._json_attrs:
-            return False
-        self._update_json_attrs_if_valid(new_attrs)
-        return True
+import copy
+import dataclasses
+import json
+import re
+import uuid
+from abc import ABC
+from dataclasses import dataclass, replace
+from typing import Dict, List, Optional, Set
+
+from cript.nodes.exceptions import (
+    CRIPTAttributeModificationError,
+    CRIPTExtraJsonAttributes,
+    CRIPTJsonSerializationError,
+)
+from cript.nodes.node_iterator import NodeIterator
+
+tolerated_extra_json = []
+
+
+def add_tolerated_extra_json(additional_tolerated_json: str):
+    """
+    In case a node should be loaded from JSON (such as `getting` them from the API),
+    but the API sends additional JSON attributes, these can be set to tolerated temporarily with this routine.
+    """
+    tolerated_extra_json.append(additional_tolerated_json)
+
+
+def get_new_uid():
+    return "_:" + str(uuid.uuid4())
+
+
+class classproperty(object):
+    def __init__(self, f):
+        self.f = f
+
+    def __get__(self, obj, owner):
+        if obj is None:
+            return self.f(owner)
+        return self.f(obj)
+
+
+class BaseNode(ABC):
+    """
+    This abstract class is the base of all CRIPT nodes.
+    It offers access to a json attribute class,
+    which reflects the data model JSON attributes.
+    Also, some basic shared functionality is provided by this base class.
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes:
+        node: List[str] = dataclasses.field(default_factory=list)
+        uid: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @classproperty
+    def node_type(self):
+        name = type(self).__name__
+        if name == "ABCMeta":
+            name = self.__name__
+        return name
+
+    @classproperty
+    def node_type_snake_case(self):
+        camel_case = self.node_type
+        # Regex to convert camel case to snake case.
+        snake_case = re.sub(r"(?<!^)(?=[A-Z])", "_", camel_case).lower()
+        return snake_case
+
+    # Prevent new attributes being set.
+    # This might just be temporary, but for now, I don't want to accidentally add new attributes, when I mean to modify one.
+    def __setattr__(self, key, value):
+        if not hasattr(self, key):
+            raise CRIPTAttributeModificationError(self.node_type, key, value)
+        super().__setattr__(key, value)
+
+    def __init__(self, **kwargs):
+        for kwarg in kwargs:
+            if kwarg not in tolerated_extra_json:
+                if kwarg.endswith("_count"):
+                    try:
+                        possible_array = getattr(self._json_attrs.kwarg[: -len("_count")])
+                        if not isinstance(possible_array, list):
+                            raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
+                    except AttributeError:
+                        raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
+                else:
+                    try:
+                        getattr(self._json_attrs, kwarg)
+                    except AttributeError:
+                        raise CRIPTExtraJsonAttributes(self.node_type, kwarg)
+
+        uid = get_new_uid()
+        self._json_attrs = replace(self._json_attrs, node=[self.node_type], uid=uid)
+
+    def __str__(self) -> str:
+        """
+        Return a string representation of a node data model attributes.
+
+        Returns
+        -------
+        str
+            A string representation of the node.
+        """
+        return str(self._json_attrs)
+
+    @property
+    def uid(self):
+        return self._json_attrs.uid
+
+    @property
+    def node(self):
+        return self._json_attrs.node
+
+    def _update_json_attrs_if_valid(self, new_json_attr: JsonAttributes) -> None:
+        """
+        tries to update the node if valid and then checks if it is valid or not
+
+        1. updates the node with the new information
+        1. run db schema validation on it
+            1. if db schema validation succeeds then update and continue
+            1. else: raise an error and tell the user what went wrong
+
+        Parameters
+        ----------
+        new_json_attr
+
+        Raises
+        ------
+        Exception
+
+        Returns
+        -------
+        None
+        """
+        old_json_attrs = self._json_attrs
+        self._json_attrs = new_json_attr
+
+        try:
+            self.validate()
+        except Exception as exc:
+            self._json_attrs = old_json_attrs
+            raise exc
+
+    def validate(self, api=None, is_patch: bool = False, force_validation: bool = False) -> None:
+        """
+        Validate this node (and all its children) against the schema provided by the data bank.
+
+        Raises:
+        -------
+        Exception with more error information.
+        """
+        from cript.api.api import _get_global_cached_api
+
+        if api is None:
+            api = _get_global_cached_api()
+        api.schema.is_node_schema_valid(self.get_json(is_patch=is_patch).json, is_patch=is_patch, force_validation=force_validation)
+
+    @classmethod
+    def _from_json(cls, json_dict: dict):
+        # TODO find a way to handle uuid nodes only
+
+        # Child nodes can inherit and overwrite this.
+        # They should call super()._from_json first, and modified the returned object after if necessary
+        # We create manually a dict that contains all elements from the send dict.
+        # That eliminates additional fields and doesn't require asdict.
+        arguments = {}
+        default_dataclass = cls.JsonAttributes()
+        for field in json_dict:
+            try:
+                getattr(default_dataclass, field)
+            except AttributeError:
+                pass
+            else:
+                arguments[field] = json_dict[field]
+
+        # add omitted fields from default (necessary if they are required)
+        for field_name in [field.name for field in dataclasses.fields(default_dataclass)]:
+            if field_name not in arguments:
+                arguments[field_name] = getattr(default_dataclass, field_name)
+
+        try:
+            node = cls(**arguments)
+        # TODO we should not catch all exceptions if we are handling them, and instead let it fail
+        #  to create a good error message that points to the correct place that it failed to make debugging easier
+        except Exception as exc:
+            print(cls, arguments)
+            raise exc
+
+        attrs = cls.JsonAttributes(**arguments)
+
+        # Handle default attributes manually.
+        for field in attrs.__dict__:
+            # Conserve newly assigned uid if uid is default (empty)
+            if getattr(attrs, field) == getattr(default_dataclass, field):
+                attrs = replace(attrs, **{str(field): getattr(node, field)})
+
+        try:  # TODO remove this temporary solution
+            if not attrs.uid.startswith("_:"):
+                attrs = replace(attrs, uid="_:" + attrs.uid)
+        except AttributeError:
+            pass
+
+        # But here we force even usually unwritable fields to be set.
+        node._update_json_attrs_if_valid(attrs)
+
+        return node
+
+    def __deepcopy__(self, memo):
+        from cript.nodes.util.core import get_uuid_from_uid
+
+        # Ideally I would call `asdict`, but that is not allowed inside a deepcopy chain.
+        # Making a manual transform into a dictionary here.
+        arguments = {}
+        for field in self.JsonAttributes().__dataclass_fields__:
+            arguments[field] = copy.deepcopy(getattr(self._json_attrs, field), memo)
+        # TODO URL handling
+
+        # Since we excluded 'uuid' from arguments,
+        # a new uid will prompt the creation of a new matching uuid.
+        uid = get_new_uid()
+        arguments["uid"] = uid
+        if "uuid" in arguments:
+            arguments["uuid"] = get_uuid_from_uid(uid)
+
+        # Create node and init constructor attributes
+        node = self.__class__(**arguments)
+        # Update none constructor writable attributes.
+        node._update_json_attrs_if_valid(self.JsonAttributes(**arguments))
+        return node
+
+    @property
+    def json(self):
+        """
+        Property to obtain a simple json string.
+        Calls `get_json` with default arguments.
+        """
+        # We cannot validate in `get_json` because we call it inside `validate`.
+        # But most uses are probably the property, so we can validate the node here.
+        json_string: str = self.get_json().json
+
+        from cript.api.api import _get_global_cached_api
+
+        api = _get_global_cached_api()
+        api.schema.is_node_schema_valid(json_string, force_validation=True)
+
+        return json_string
+
+    def get_expanded_json(self, **kwargs) -> str:
+        """
+        Generates a long-form JSON representation of the current node and its hierarchy.
+
+        The long-form JSON includes complete details of the node, eliminating the need for
+         references to UUIDs to nodes stored in the CRIPT database. This comprehensive representation
+         is useful for offline storage of CRIPT nodes, transferring nodes between different CRIPT instances,
+         or for backup purposes.
+
+        The generated long-form JSON can be reloaded into the SDK using
+        [`cript.load_nodes_from_json()`](../../../utility_functions/#cript.nodes.util.load_nodes_from_json),
+        ensuring consistency and completeness of the node data.
+        However, it's important to note that this long-form JSON might not comply directly with the JSON schema
+        required for POST or PATCH requests to the CRIPT API.
+
+        Optional keyword arguments (`kwargs`) are supported and are passed directly to `json.dumps()`.
+        These arguments allow customization of the JSON output, such as formatting for readability
+        or pretty printing.
+
+        Parameters
+        ----------
+        **kwargs : dict, optional
+            Additional keyword arguments for `json.dumps()` to customize the JSON output, such as `indent`
+            for pretty-printing.
+
+        Returns
+        -------
+        str
+            A comprehensive JSON string representing the current node and its entire hierarchy in long-form.
+
+        Notes
+        -----
+        The `get_expanded_json()` method differs from the standard [`json`](./#cript.nodes.core.BaseNode.json)
+        property or method, which might provide a more condensed version of the node's data.
+
+        > For more information on condensed JSON and deserialization, please feel free to reference our discussion
+        > on [deserializing Python nodes to JSON](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/177)
+
+        Examples
+        --------
+        >>> import cript
+        >>> # ============= Create all needed nodes =============
+        >>> my_project = cript.Project(name=f"my_Project")
+        >>> my_collection = cript.Collection(name="my collection")
+        >>> my_material_1 = cript.Material(
+        ...     name="my material 1", bigsmiles = "my material 1 bigsmiles"
+        ... )
+        >>> my_material_2 = cript.Material(
+        ...     name="my material 2", bigsmiles = "my material 2 bigsmiles"
+        ... )
+        >>> my_inventory = cript.Inventory(
+        ...     name="my inventory", material=[my_material_1, my_material_2]
+        ... )
+        >>> #  ============= Assemble nodes =============
+        >>> my_project.collection = [my_collection]
+        >>> my_project.collection[0].inventory = [my_inventory]
+        >>> #  ============= Get long form JSON =============
+        >>> long_form_json = my_project.get_expanded_json(indent=4)
+
+        ???+ info "Condensed JSON VS Expanded JSON"
+            # Default Condensed JSON
+            > This is the JSON when `my_project.json` is called
+
+            ```json linenums="1"
+            {
+               "node":[
+                  "Project"
+               ],
+               "uid":"_:d0d1b3c9-d552-4d4f-afd2-76f01538b87a",
+               "uuid":"d0d1b3c9-d552-4d4f-afd2-76f01538b87a",
+               "name":"my_Project",
+               "collection":[
+                  {
+                     "node":[
+                        "Collection"
+                     ],
+                     "uid":"_:07765ac8-862a-459e-9d99-d0439d6a6a09",
+                     "uuid":"07765ac8-862a-459e-9d99-d0439d6a6a09",
+                     "name":"my collection",
+                     "inventory":[
+                        {
+                           "node":[
+                              "Inventory"
+                           ],
+                           "uid":"_:4cf2bbee-3dc0-400b-8269-709f99d89d9f",
+                           "uuid":"4cf2bbee-3dc0-400b-8269-709f99d89d9f",
+                           "name":"my inventory",
+                           "material":[
+                              {
+                                 "uuid":"0cf14572-4da2-43f2-8cb9-e8374086368e"
+                              },
+                              {
+                                 "uuid":"6302a8b0-4265-4a3a-a40f-bbcbb7293046"
+                              }
+                           ]
+                        }
+                     ]
+                  }
+               ]
+            }
+            ```
+
+            # Expanded JSON
+            > This is what is created when `my_project.get_expanded_json()`
+
+            ```json linenums="1"
+            {
+               "node":[
+                  "Project"
+               ],
+               "uid":"_:afe4bb2f-fa75-4736-b692-418a5143e6f5",
+               "uuid":"afe4bb2f-fa75-4736-b692-418a5143e6f5",
+               "name":"my_Project",
+               "collection":[
+                  {
+                     "node":[
+                        "Collection"
+                     ],
+                     "uid":"_:8b5c8125-c956-472a-9d07-8cb7b402b101",
+                     "uuid":"8b5c8125-c956-472a-9d07-8cb7b402b101",
+                     "name":"my collection",
+                     "inventory":[
+                        {
+                           "node":[
+                              "Inventory"
+                           ],
+                           "uid":"_:1bd3c966-cb35-494d-85cd-3515cde570f3",
+                           "uuid":"1bd3c966-cb35-494d-85cd-3515cde570f3",
+                           "name":"my inventory",
+                           "material":[
+                              {
+                                 "node":[
+                                    "Material"
+                                 ],
+                                 "uid":"_:07bc3e4f-757f-4ac7-ae8a-7a0c68272531",
+                                 "uuid":"07bc3e4f-757f-4ac7-ae8a-7a0c68272531",
+                                 "name":"my material 1",
+                                 "bigsmiles":"my material 1 bigsmiles"
+                              },
+                              {
+                                 "node":[
+                                    "Material"
+                                 ],
+                                 "uid":"_:64565687-5707-4d67-860f-5ee4a057a45f",
+                                 "uuid":"64565687-5707-4d67-860f-5ee4a057a45f",
+                                 "name":"my material 2",
+                                 "bigsmiles":"my material 2 bigsmiles"
+                              }
+                           ]
+                        }
+                     ]
+                  }
+               ]
+            }
+            ```
+        """
+        return self.get_json(handled_ids=None, known_uuid=None, suppress_attributes=None, is_patch=False, condense_to_uuid={}, **kwargs).json
+
+    def get_json(
+        self,
+        handled_ids: Optional[Set[str]] = None,
+        known_uuid: Optional[Set[str]] = None,
+        suppress_attributes: Optional[Dict[str, Set[str]]] = None,
+        is_patch: bool = False,
+        condense_to_uuid: Dict[str, Set[str]] = {
+            "Material": {"parent_material", "component"},
+            "Experiment": {"data"},
+            "Inventory": {"material"},
+            "Ingredient": {"material"},
+            "Property": {"component"},
+            "ComputationProcess": {"material"},
+            "Data": {"material"},
+            "Process": {"product", "waste"},
+            "Project": {"member", "admin"},
+            "Collection": {"member", "admin"},
+        },
+        **kwargs
+    ):
+        """
+        User facing access to get the JSON of a node.
+        Opposed to the also available property json this functions allows further control.
+        Additionally, this function does not call `self.validate()` but the property `json` does.
+        We also accept `kwargs`, that are passed on to the JSON decoding via `json.dumps()` this can be used for example to prettify the output.
+
+
+        Returns named tuple with json and handled ids as result.
+        """
+
+        @dataclass(frozen=True)
+        class ReturnTuple:
+            json: str
+            json_dict: dict
+            handled_ids: set
+
+        # Do not check for circular references, since we handle them manually
+        kwargs["check_circular"] = kwargs.get("check_circular", False)
+
+        # Delayed import to avoid circular imports
+        from cript.nodes.util import NodeEncoder
+
+        if handled_ids is None:
+            handled_ids = set()
+        previous_handled_nodes = copy.deepcopy(NodeEncoder.handled_ids)
+        NodeEncoder.handled_ids = handled_ids
+
+        # Similar to uid, we handle pre-saved known uuid such that they are UUID edges only
+        if known_uuid is None:
+            known_uuid = set()
+        previous_known_uuid = copy.deepcopy(NodeEncoder.known_uuid)
+        NodeEncoder.known_uuid = known_uuid
+        previous_suppress_attributes = copy.deepcopy(NodeEncoder.suppress_attributes)
+        NodeEncoder.suppress_attributes = suppress_attributes
+        previous_condense_to_uuid = copy.deepcopy(NodeEncoder.condense_to_uuid)
+        NodeEncoder.condense_to_uuid = condense_to_uuid
+
+        try:
+            tmp_json = json.dumps(self, cls=NodeEncoder, **kwargs)
+            tmp_dict = json.loads(tmp_json)
+            if is_patch:
+                del tmp_dict["uuid"]  # patches do not allow UUID is the parent most node
+
+            return ReturnTuple(json.dumps(tmp_dict, **kwargs), tmp_dict, NodeEncoder.handled_ids)
+        except Exception as exc:
+            # TODO this handling that doesn't tell the user what happened and how they can fix it
+            #   this just tells the user that something is wrong
+            #   this should be improved to tell the user what went wrong and where
+            raise CRIPTJsonSerializationError(str(type(self)), str(self._json_attrs)) from exc
+        finally:
+            NodeEncoder.handled_ids = previous_handled_nodes
+            NodeEncoder.known_uuid = previous_known_uuid
+            NodeEncoder.suppress_attributes = previous_suppress_attributes
+            NodeEncoder.condense_to_uuid = previous_condense_to_uuid
+
+    def find_children(self, search_attr: dict, search_depth: int = -1, handled_nodes: Optional[List] = None) -> List:
+        """
+        Finds all the children in a given tree of nodes (specified by its root),
+        that match the criteria of search_attr.
+        If a node is present multiple times in the graph, it is only once in the search results.
+
+        Parameters
+        ----------
+        search_attr: dict
+            What you are searching for within the JSON.
+            Dictionary that specifies which JSON attributes have to be present in a given node.
+            If an attribute is a list, it is sufficient if the specified attributes are in the list,
+            if others are present too, that does not exclude the child.
+        search_depth: int default -1
+            Max depth of the search into the tree. Helpful if circles are expected. -1 specifies no limit
+        handled_nodes: Optional[List] default None
+            A list used to track nodes that have already been processed during the search.
+            This parameter is primarily used internally to prevent infinite loops in cases
+            where the node graph contains cycles. When a node is processed, it is added to this list.
+            If a node is encountered that is already in this list, it is skipped to avoid redundant processing.
+            By default, this parameter is `None`, which means that the search starts with an empty list of handled nodes.
+            In most use cases, users do not need to provide this parameter, as it is managed internally by the
+            method.
+
+        Returns
+        -------
+        List
+            list of all nodes that match the criteria found within the graph
+
+        Examples
+        --------
+        >>> import cript
+        >>> # ============= Create nodes =============
+        >>> my_project = cript.Project(name=f"my_Project")
+        >>> my_collection = cript.Collection(name="my collection")
+        >>> my_material_1 = cript.Material(
+        ...     name="my material 1", bigsmiles = "my material 1 bigsmiles"
+        ... )
+        >>> my_material_2 = cript.Material(
+        ...     name="my material 2", bigsmiles = "my material 2 bigsmiles"
+        ... )
+        >>> my_inventory = cript.Inventory(
+        ...     name="my inventory", material=[my_material_1, my_material_2]
+        ... )
+        >>> #  ============= Assemble nodes =============
+        >>> my_project.collection = [my_collection]
+        >>> my_project.collection[0].inventory = [my_inventory]
+        >>> #  ============= Get list of all material nodes in project =============
+        >>> all_materials_in_project: list = my_project.find_children({"node": ["Material"]})
+
+        Notes
+        -----
+        The `find_children` method is versatile and can be used to search for nodes based on various criteria.
+        Here are some examples to illustrate its usage:
+
+        * Searching for Specific Node Types:
+          `search_attr = {"node": ["Parameter"]}` will find all nodes of type "Parameter".
+        * Searching with Additional Attributes:
+          `search_attr = {"node": ["Algorithm"], "parameter": {"name" : "update_frequency"}}`
+          will locate "Algorithm" nodes containing a parameter named "update_frequency".
+          Note: For list attributes, a match occurs if the specified attribute is part of the list.
+            * Alternate notation: `{"node": ["Algorithm"], "parameter": [{"name" : "update_frequency"}]}`.
+          In this case, nodes with additional parameters are also included.
+        * Combining Multiple Search Criteria:
+          ```python
+          search_attr = {
+              "node": ["Algorithm"],
+              "parameter": [{"name": "update_frequency"}, {"name": "cutoff_distance"}]
+          }
+          ```
+          This finds all "Algorithm" nodes with both "update_frequency" and "cutoff_distance" parameters.
+
+        The `search_depth` parameter controls how deep the search goes into the node tree.
+        A value of `-1` indicates no depth limit.
+        The method effectively handles cycles in the graph by ensuring each node is processed only once.
+        This makes the function suitable for complex node structures.
+        """
+
+        def is_attr_present(node: BaseNode, key, value):
+            """
+            Helper function that checks if an attribute is present in a node.
+            """
+            try:
+                attr_key = getattr(node._json_attrs, key)
+            except AttributeError:
+                return False
+
+            # To save code paths, I convert non-lists into lists with one element.
+            if not isinstance(attr_key, list):
+                attr_key = [attr_key]
+            if not isinstance(value, list):
+                value = [value]
+
+            # The definition of search is, that all values in a list have to be present.
+            # To fulfill this AND condition, we count the number of occurrences of that value condition
+            number_values_found = 0
+            # Runtime contribution: O(m), where is is the number of search keys
+            for v in value:
+                # Test for simple values (not-nodes)
+                if v in attr_key:
+                    number_values_found += 1
+
+                # Test if value is present in one of the specified attributes (OR condition)
+                # Runtime contribution: O(m), where m is the number of nodes in the attribute list.
+                for attr in attr_key:
+                    # if the attribute is a node and the search value is a dictionary,
+                    # we can verify that this condition is met if it finds the node itself with `find_children`.
+                    if isinstance(attr, BaseNode) and isinstance(v, dict):
+                        # Since we only want to test the node itself and not any of its children, we set recursion to 0.
+                        # Runtime contribution: recursive call, with depth search depth of the search dictionary O(h)
+                        if len(attr.find_children(v, 0)) > 0:
+                            number_values_found += 1
+                            # Since this an OR condition, we abort early.
+                            # This also doesn't inflate the number_values_count,
+                            # since every OR condition should only add a max of 1.
+                            break
+            # Check if the AND condition of the values is met
+            return number_values_found == len(value)
+
+        if handled_nodes is None:
+            handled_nodes = []
+
+        found_children = []
+
+        node_iterator = NodeIterator(self, search_depth)
+        for node in node_iterator:
+            found_attr = 0
+            for key, value in search_attr.items():
+                if is_attr_present(node, key, value):
+                    found_attr += 1
+            # If exactly all attributes are found, it matches the search criterion
+            if found_attr == len(search_attr):
+                found_children += [node]
+
+        return found_children
+
+    def remove_child(self, child) -> bool:
+        """
+        This safely removes the first found child node from the parent.
+        This requires exact node as we test with `is` instead of `==`.
+
+        returns True if child was found and deleted, False if child not found,
+        raise DB schema exception if deletion violates DB schema.
+        """
+
+        # If we delete a child, we have to replace that with a default value.
+        # The easiest way to access this default value is to get it from the the default JsonAttribute of that class
+        default_json_attrs = self.JsonAttributes()
+        new_attrs = self._json_attrs
+        for field in self._json_attrs.__dataclass_fields__:
+            value = getattr(self._json_attrs, field)
+            if value is child:
+                new_attrs = replace(new_attrs, **{field: getattr(default_json_attrs, field)})
+                # We only want to delete the first found child
+            elif not isinstance(value, str):  # Strings are iterable, but we don't want them
+                try:  # Try if we are facing a list at the moment
+                    new_attr_list = [element for element in value]
+                except TypeError:
+                    pass  # It is OK if this field is not a list
+                else:
+                    found_child = False
+                    for i, list_value in enumerate(value):
+                        if list_value is child:
+                            found_child = True
+                            del new_attr_list[i]
+                            # Only delete first child.
+                            # Important to break loop here, since value and new_attr_list are not identical any more.
+                    if found_child:
+                        new_attrs = replace(new_attrs, **{field: new_attr_list})  # type: ignore
+                        # Again only first found place is removed
+                        break
+        # Let's see if we found the child aka the new_attrs are different than the old ones
+        if new_attrs is self._json_attrs:
+            return False
+        self._update_json_attrs_if_valid(new_attrs)
+        return True
```

### Comparing `cript-2.2.0/src/cript/nodes/exceptions.py` & `cript-2.3.0/src/cript/nodes/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,401 +1,406 @@
-from abc import ABC, abstractmethod
-from typing import List
-
-from cript.exceptions import CRIPTException
-
-
-class CRIPTNodeSchemaError(CRIPTException):
-    """
-    ## Definition
-    This error is raised when the CRIPT [json database schema](https://json-schema.org/)
-    validation fails for a node.
-
-    Please keep in mind that the CRIPT Python SDK converts all the Python nodes inside the
-    [Project](../../nodes/primary_nodes/project) into a giant JSON
-    and sends an HTTP `POST` or `PATCH` request to the API to be processed.
-
-    However, before a request is sent to the API, the JSON is validated against API database schema
-    via the [JSON Schema library](https://python-jsonschema.readthedocs.io/en/stable/),
-    and if the database schema validation fails for whatever reason this error is shown.
-
-    ### Possible Reasons
-
-    1. There was a mistake in nesting of the nodes
-    1. There was a mistake in creating the nodes
-    1. Nodes are missing
-    1. Nodes have invalid vocabulary
-        * The database schema wants something a different controlled vocabulary than what is provided
-    1. There was an error with the way the JSON was created within the Python SDK
-        * The format of the JSON the CRIPT Python SDK created was invalid
-    1. There is something wrong with the database schema
-
-    ## Troubleshooting
-    The easiest way to troubleshoot this is to examine the JSON that the SDK created via printing out the
-    [Project](../../nodes/primary_nodes/project) node's JSON and checking the place that the schema validation
-    says failed
-
-    ### Example
-    ```python
-    print(my_project.json)
-    ```
-    """
-
-    node_type: str = ""
-    json_schema_validation_error: str = ""
-
-    def __init__(self, node_type: str, json_schema_validation_error: str) -> None:
-        self.json_schema_validation_error: str = json_schema_validation_error
-        self.node_type = node_type
-
-    def __str__(self) -> str:
-        error_message: str = f"JSON database schema validation for node {self.node_type} failed."
-        error_message += f"Error: {self.json_schema_validation_error}"
-
-        return error_message
-
-
-class CRIPTJsonDeserializationError(CRIPTException):
-    """
-    ## Definition
-    This exception is raised when converting a node from JSON to Python class fails.
-    This process fails when the attributes within the JSON does not match the node's class
-    attributes within the `JsonAttributes` of that specific node
-
-    ### Error Example
-    Invalid JSON that cannot be deserialized to a CRIPT Python SDK Node
-
-    ```json
-    ```
-
-
-    ### Valid Example
-    Valid JSON that can be deserialized to a CRIPT Python SDK Node
-
-    ```json
-    ```
-
-    ## Troubleshooting
-    """
-
-    def __init__(self, node_type: str, json_str: str) -> None:
-        self.node_type = node_type
-        self.json_str = json_str
-
-    def __str__(self) -> str:
-        return f"JSON deserialization failed for node type {self.node_type} with JSON str: {self.json_str}"
-
-
-class CRIPTDeserializationUIDError(CRIPTException):
-    """
-    ## Definition
-    This exception is raised when converting a node from JSON to Python class fails,
-    because a node is specified with its UID only, but not part of the data graph elsewhere.
-
-    ### Error Example
-    Invalid JSON that cannot be deserialized to a CRIPT Python SDK Node
-
-    ```json
-    {
-    "node": ["Algorithm"],
-    "key": "mc_barostat",
-    "type": "barostat",
-    "parameter": {"node": ["Parameter"], "uid": "uid-string"}
-    }
-    ```
-    Here the algorithm has a parameter attribute, but the parameter is specified as uid only.
-
-    ### Valid Example
-    Valid JSON that can be deserialized to a CRIPT Python SDK Node
-
-    ```json
-    {
-       "node":["Algorithm"],
-       "key":"mc_barostat",
-       "type":"barostat",
-       "parameter":{
-          "node":["Parameter"],
-          "uid":"uid-string",
-          "key":"update_frequency",
-          "value":1,
-          "unit":"1/second"
-       }
-    }
-    ```
-    Now the node is fully specified.
-
-    ## Troubleshooting
-    Specify the full node instead. This error might appear if you try to partially load previously generated JSON.
-    """
-
-    def __init__(self, node_type: str, uid: str) -> None:
-        self.node_type = node_type
-        self.uid = uid
-
-    def __str__(self) -> str:
-        return f"JSON deserialization failed for node type {self.node_type} with unknown UID: {self.uid}"
-
-
-class CRIPTJsonNodeError(CRIPTJsonDeserializationError):
-    """
-    ## Definition
-    This exception is raised if a `node` attribute is present in JSON,
-    but the list has more or less than exactly one type of node type.
-
-    > Note: It is expected that there is only a single node type per JSON object.
-
-    ### Example
-    !!! Example "Valid JSON representation of a Material node"
-        ```json
-        {
-          "node": [
-            "Material"
-          ],
-          "name": "Whey protein isolate",
-          "uid": "_:Whey protein isolate"
-        },
-        ```
-
-    ??? Example "Invalid JSON representation of a Material node"
-
-        ```json
-        {
-          "node": [
-            "Material",
-            "Property"
-          ],
-          "name": "Whey protein isolate",
-          "uid": "_:Whey protein isolate"
-        },
-        ```
-
-        ---
-
-        ```json
-        {
-          "node": [],
-          "name": "Whey protein isolate",
-          "uid": "_:Whey protein isolate"
-        },
-        ```
-
-
-    ## Troubleshooting
-    Debugging skills are most helpful here as there is no one-size-fits-all approach.
-
-    It is best to identify whether the invalid JSON was created in the Python SDK
-    or if the invalid JSON was given from the API.
-
-    If the Python SDK created invalid JSON during serialization, then it is helpful to track down and
-    identify the point where the invalid JSON was started.
-
-    You may consider, inspecting the python objects to see if the node type are written incorrectly in python
-    and the issue is only being caught during serialization or if the Python node is written correctly
-    and the issue is created during serialization.
-
-    If the problem is with the Python SDK or API, it is best to leave an issue or create a discussion within the
-    [Python SDK GitHub repository](https://github.com/C-Accel-CRIPT/Python-SDK) for one of the members of the
-    CRIPT team to look into any issues that there could have been.
-    """
-
-    def __init__(self, node_list: List, json_str: str) -> None:
-        self.node_list = node_list
-        self.json_str = json_str
-
-    def __str__(self) -> str:
-        error_message: str = f"The 'node' attribute in the JSON string must be a single element list with the node name " f" such as `'node: ['Material']`. The `node` attribute provided was: `{self.node_list}`" f"The full JSON was: {self.json_str}."
-
-        return error_message
-
-
-class CRIPTJsonSerializationError(CRIPTException):
-    """
-    ## Definition
-    This Exception is raised if serialization of node from JSON to Python Object fails.
-
-    ## Troubleshooting
-    """
-
-    def __init__(self, node_type: str, json_dict: str) -> None:
-        self.node_type = node_type
-        self.json_str = str(json_dict)
-
-    def __str__(self) -> str:
-        return f"JSON Serialization failed for node type {self.node_type} with JSON dict: {self.json_str}"
-
-
-class CRIPTAttributeModificationError(CRIPTException):
-    """
-    Exception that is thrown when a node attribute is modified, that wasn't intended to be modified.
-    """
-
-    def __init__(self, name, key, value):
-        self.name = name
-        self.key = key
-        self.value = value
-
-    def __str__(self):
-        return (
-            f"Attempt to modify an attribute of a node ({self.name}) that wasn't intended to be modified.\n"
-            f"Here the non-existing attribute {self.key} of {self.name} was attempted to be modified.\n"
-            "Most likely this is due to a typo in the attribute that was intended to be modified i.e. `project.materials` instead of `project.material`.\n"
-            "To ensure compatibility with the underlying CRIPT data model we do not allow custom attributes.\n"
-        )
-
-
-class CRIPTExtraJsonAttributes(CRIPTException):
-    def __init__(self, name_type: str, extra_attribute: str):
-        self.name_type = name_type
-        self.extra_attribute = extra_attribute
-
-    def __str__(self):
-        return (
-            f"During the construction of a node {self.name_type} an additional attribute {self.extra_attribute} was detected.\n"
-            "This might be a typo or an extra delivered argument from the back end.\n"
-            f"In the latter case, you can disable this error temporarily by calling `cript.add_tolerated_extra_json('{self.extra_attribute}')`.\n"
-        )
-
-
-class CRIPTOrphanedNodesError(CRIPTException, ABC):
-    """
-    ## Definition
-    This error is raised when a child node is not attached to the
-    appropriate parent node. For example, all material nodes used
-    within a project must belong to the project inventory or are explicitly listed as material of that project.
-    If there is a material node that is used within a project but not a part of the
-    inventory and the validation code finds it then it raises an `CRIPTOrphanedNodeError`
-
-    ## Troubleshooting
-    Fixing this is simple and easy, just take the node that CRIPT Python SDK
-    found a problem with and associate it with the appropriate parent via
-
-    ```
-    my_project.material += my_orphaned_material_node
-    ```
-    """
-
-    def __init__(self, orphaned_node):
-        self.orphaned_node = orphaned_node
-
-    @abstractmethod
-    def __str__(self):
-        pass
-
-
-class CRIPTOrphanedMaterialError(CRIPTOrphanedNodesError):
-    """
-    ## Definition
-    CRIPTOrphanedNodesError, but specific for orphaned materials.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned materials into the parent project or its inventories.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
-
-    def __str__(self):
-        ret_string = "While validating a project graph, an orphaned material node was found. "
-        ret_string += "This material is present in the graph, but not listed in the project. "
-        ret_string += "Please add the node like: `my_project.material += [orphaned_material]`. "
-        ret_string += f"The orphaned material was {self.orphaned_node}."
-        return ret_string
-
-
-class CRIPTOrphanedExperimentError(CRIPTOrphanedNodesError):
-    """
-    ## Definition
-    CRIPTOrphanedNodesError, but specific for orphaned nodes that should be listed in one of the experiments.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned node into one the parent project's experiments.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
-
-    def __str__(self) -> str:
-        node_name = self.orphaned_node.node_type.lower()
-        ret_string = f"While validating a project graph, an orphaned {node_name} node was found. "
-        ret_string += f"This {node_name} node is present in the graph, but not listed in any of the experiments of the  project. "
-        ret_string += f"Please add the node like: `your_experiment.{node_name} += [orphaned_{node_name}]`. "
-        ret_string += f"The orphaned {node_name} was {self.orphaned_node}."
-        return ret_string
-
-
-def get_orphaned_experiment_exception(orphaned_node):
-    """
-    Return the correct specific Exception based in the orphaned node type for nodes not correctly listed in experiment.
-    """
-    from cript.nodes.primary_nodes.computation import Computation
-    from cript.nodes.primary_nodes.computation_process import ComputationProcess
-    from cript.nodes.primary_nodes.data import Data
-    from cript.nodes.primary_nodes.process import Process
-
-    if isinstance(orphaned_node, Data):
-        return CRIPTOrphanedDataError(orphaned_node)
-    if isinstance(orphaned_node, Process):
-        return CRIPTOrphanedProcessError(orphaned_node)
-    if isinstance(orphaned_node, Computation):
-        return CRIPTOrphanedComputationError(orphaned_node)
-    if isinstance(orphaned_node, ComputationProcess):
-        return CRIPTOrphanedComputationalProcessError(orphaned_node)
-    # Base case raise the parent exception. TODO add bug warning.
-    return CRIPTOrphanedExperimentError(orphaned_node)
-
-
-class CRIPTOrphanedDataError(CRIPTOrphanedExperimentError):
-    """
-    ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Data node that should be listed in one of the experiments.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned node into one the parent project's experiments `data` attribute.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
-
-
-class CRIPTOrphanedProcessError(CRIPTOrphanedExperimentError):
-    """
-    ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Process node that should be
-    listed in one of the experiments.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned node into one the parent project's experiments
-    `process` attribute.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
-
-
-class CRIPTOrphanedComputationError(CRIPTOrphanedExperimentError):
-    """
-    ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned Computation node that should be
-    listed in one of the experiments.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned node into one the parent project's experiments
-    `Computation` attribute.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
-
-
-class CRIPTOrphanedComputationalProcessError(CRIPTOrphanedExperimentError):
-    """
-    ## Definition
-    CRIPTOrphanedExperimentError, but specific for orphaned ComputationalProcess
-    node that should be listed in one of the experiments.
-
-    ## Troubleshooting
-    Handle this error by adding the orphaned node into one the parent project's experiments
-    `ComputationalProcess` attribute.
-    """
-
-    def __init__(self, orphaned_node):
-        super().__init__(orphaned_node)
+from abc import ABC, abstractmethod
+from typing import List
+
+from cript.exceptions import CRIPTException
+
+
+class CRIPTUUIDException(CRIPTException):
+    def __init__(self, uuid: str, old_type: str, new_type: str):
+        self.uuid = uuid
+        self.old_type = old_type
+        self.new_type = new_type
+
+    def __str__(self) -> str:
+        return_msg = f"UUID collision error. A new node with UUID {self.uuid} is created of type {self.new_type},"
+        return_msg += f" but a node with the same UUID exists already as type {self.old_type}."
+        return_msg += " Please report the error on https://github.com/C-Accel-CRIPT/Python-SDK/issues , thank you."
+        return return_msg
+
+
+class CRIPTNodeSchemaError(CRIPTException):
+    """
+    ## Definition
+    This error is raised when the CRIPT [json database schema](https://json-schema.org/)
+    validation fails for a node.
+
+    Please keep in mind that the CRIPT Python SDK converts all the Python nodes inside the
+    [Project](../../nodes/primary_nodes/project) into a giant JSON
+    and sends an HTTP `POST` or `PATCH` request to the API to be processed.
+
+    However, before a request is sent to the API, the JSON is validated against API database schema
+    via the [JSON Schema library](https://python-jsonschema.readthedocs.io/en/stable/),
+    and if the database schema validation fails for whatever reason this error is shown.
+
+    ### Possible Reasons
+
+    1. There was a mistake in nesting of the nodes
+    1. There was a mistake in creating the nodes
+    1. Nodes are missing
+    1. Nodes have invalid vocabulary
+        * The database schema wants something a different controlled vocabulary than what is provided
+    1. There was an error with the way the JSON was created within the Python SDK
+        * The format of the JSON the CRIPT Python SDK created was invalid
+    1. There is something wrong with the database schema
+
+    ## Troubleshooting
+    The easiest way to troubleshoot this is to examine the JSON that the SDK created via printing out the
+    [Project](../../nodes/primary_nodes/project) node's JSON and checking the place that the schema validation
+    says failed
+
+    ### Example
+    ```python
+    print(my_project.json)
+    ```
+    """
+
+    node_type: str = ""
+    json_schema_validation_error: str = ""
+
+    def __init__(self, node_type: str, json_schema_validation_error: str) -> None:
+        self.json_schema_validation_error: str = json_schema_validation_error
+        self.node_type = node_type
+
+    def __str__(self) -> str:
+        error_message: str = f"JSON database schema validation for node {self.node_type} failed."
+        error_message += f"Error: {self.json_schema_validation_error}"
+
+        return error_message
+
+
+class CRIPTMaterialIdentifierError(CRIPTException):
+    """Every material node needs to have at least one identifier set."""
+
+    def __init__(self, material_node):
+        self.material_node = material_node
+
+    def __str__(self) -> str:
+        error_message = "Every Material node needs at least one identifier from "
+        error_message += " [ 'amino_acid', 'bigsmiles', 'chem_formula', 'chem_repeat', 'chemical_id', 'inchi', 'lot_number', 'names', 'pubchem_cid', 'smiles','vendor'] set."
+        error_message += f" This node {self.material_node} has none set."
+        return error_message
+
+
+class CRIPTJsonDeserializationError(CRIPTException):
+    """
+    ## Definition
+    This exception is raised when converting a node from JSON to Python class fails.
+    This process fails when the attributes within the JSON does not match the node's class
+    attributes within the `JsonAttributes` of that specific node
+
+    ### Error Example
+    Invalid JSON that cannot be deserialized to a CRIPT Python SDK Node
+
+    ```json
+    ```
+
+
+    ### Valid Example
+    Valid JSON that can be deserialized to a CRIPT Python SDK Node
+
+    ```json
+    ```
+
+    ## Troubleshooting
+    """
+
+    def __init__(self, node_type: str, json_str: str) -> None:
+        self.node_type = node_type
+        self.json_str = json_str
+
+    def __str__(self) -> str:
+        return f"JSON deserialization failed for node type {self.node_type} with JSON str: {self.json_str}"
+
+
+class CRIPTDeserializationUIDError(CRIPTException):
+    """
+    ## Definition
+    This exception is raised when converting a node from JSON to Python class fails,
+    because a node is specified with its UID only, but not part of the data graph elsewhere.
+
+    ### Error Example
+    Invalid JSON that cannot be deserialized to a CRIPT Python SDK Node
+
+    ```json
+    {
+    "node": ["Algorithm"],
+    "key": "mc_barostat",
+    "type": "barostat",
+    "parameter": {"node": ["Parameter"], "uid": "uid-string"}
+    }
+    ```
+    Here the algorithm has a parameter attribute, but the parameter is specified as uid only.
+
+    ### Valid Example
+    Valid JSON that can be deserialized to a CRIPT Python SDK Node
+
+    ```json
+    {
+       "node":["Algorithm"],
+       "key":"mc_barostat",
+       "type":"barostat",
+       "parameter":{
+          "node":["Parameter"],
+          "uid":"uid-string",
+          "key":"update_frequency",
+          "value":1,
+          "unit":"1/second"
+       }
+    }
+    ```
+    Now the node is fully specified.
+
+    ## Troubleshooting
+    Specify the full node instead. This error might appear if you try to partially load previously generated JSON.
+    """
+
+    def __init__(self, node_type: str, uid: str) -> None:
+        self.node_type = node_type
+        self.uid = uid
+
+    def __str__(self) -> str:
+        return f"JSON deserialization failed for node type {self.node_type} with unknown UID: {self.uid}"
+
+
+class CRIPTJsonNodeError(CRIPTJsonDeserializationError):
+    """
+    ## Definition
+    This exception is raised if a `node` attribute is present in JSON,
+    but the list has more or less than exactly one type of node type.
+
+    > Note: It is expected that there is only a single node type per JSON object.
+
+    ### Example
+    !!! Example "Valid JSON representation of a Material node"
+        ```json
+        {
+          "node": [
+            "Material"
+          ],
+          "name": "Whey protein isolate",
+          "uid": "_:Whey protein isolate"
+        },
+        ```
+
+    ??? Example "Invalid JSON representation of a Material node"
+
+        ```json
+        {
+          "node": [
+            "Material",
+            "Property"
+          ],
+          "name": "Whey protein isolate",
+          "uid": "_:Whey protein isolate"
+        },
+        ```
+
+        ---
+
+        ```json
+        {
+          "node": [],
+          "name": "Whey protein isolate",
+          "uid": "_:Whey protein isolate"
+        },
+        ```
+
+
+    ## Troubleshooting
+    Debugging skills are most helpful here as there is no one-size-fits-all approach.
+
+    It is best to identify whether the invalid JSON was created in the Python SDK
+    or if the invalid JSON was given from the API.
+
+    If the Python SDK created invalid JSON during serialization, then it is helpful to track down and
+    identify the point where the invalid JSON was started.
+
+    You may consider, inspecting the python objects to see if the node type are written incorrectly in python
+    and the issue is only being caught during serialization or if the Python node is written correctly
+    and the issue is created during serialization.
+
+    If the problem is with the Python SDK or API, it is best to leave an issue or create a discussion within the
+    [Python SDK GitHub repository](https://github.com/C-Accel-CRIPT/Python-SDK) for one of the members of the
+    CRIPT team to look into any issues that there could have been.
+    """
+
+    def __init__(self, node_list: List, json_str: str) -> None:
+        self.node_list = node_list
+        self.json_str = json_str
+
+    def __str__(self) -> str:
+        error_message: str = f"The 'node' attribute in the JSON string must be a single element list with the node name " f" such as `'node: ['Material']`. The `node` attribute provided was: `{self.node_list}`" f"The full JSON was: {self.json_str}."
+
+        return error_message
+
+
+class CRIPTJsonSerializationError(CRIPTException):
+    """
+    ## Definition
+    This Exception is raised if serialization of node from JSON to Python Object fails.
+
+    ## Troubleshooting
+    """
+
+    def __init__(self, node_type: str, json_dict: str) -> None:
+        self.node_type = node_type
+        self.json_str = str(json_dict)
+
+    def __str__(self) -> str:
+        return f"JSON Serialization failed for node type {self.node_type} with JSON dict: {self.json_str}"
+
+
+class CRIPTAttributeModificationError(CRIPTException):
+    """
+    Exception that is thrown when a node attribute is modified, that wasn't intended to be modified.
+    """
+
+    def __init__(self, name, key, value):
+        self.name = name
+        self.key = key
+        self.value = value
+
+    def __str__(self):
+        return (
+            f"Attempt to modify an attribute of a node ({self.name}) that wasn't intended to be modified.\n"
+            f"Here the non-existing attribute {self.key} of {self.name} was attempted to be modified.\n"
+            "Most likely this is due to a typo in the attribute that was intended to be modified i.e. `project.materials` instead of `project.material`.\n"
+            "To ensure compatibility with the underlying CRIPT data model we do not allow custom attributes.\n"
+        )
+
+
+class CRIPTExtraJsonAttributes(CRIPTException):
+    def __init__(self, name_type: str, extra_attribute: str):
+        self.name_type = name_type
+        self.extra_attribute = extra_attribute
+
+    def __str__(self):
+        return (
+            f"During the construction of a node {self.name_type} an additional attribute {self.extra_attribute} was detected.\n"
+            "This might be a typo or an extra delivered argument from the back end.\n"
+            f"In the latter case, you can disable this error temporarily by calling `cript.add_tolerated_extra_json('{self.extra_attribute}')`.\n"
+        )
+
+
+class CRIPTOrphanedNodesError(CRIPTException, ABC):
+    """
+    ## Definition
+    This error is raised when a child node is not attached to the
+    appropriate parent node. For example, all material nodes used
+    within a project must belong to the project inventory or are explicitly listed as material of that project.
+    If there is a material node that is used within a project but not a part of the
+    inventory and the validation code finds it then it raises an `CRIPTOrphanedNodeError`
+
+    ## Troubleshooting
+    Fixing this is simple and easy, just take the node that CRIPT Python SDK
+    found a problem with and associate it with the appropriate parent via
+
+    ```
+    my_project.material += my_orphaned_material_node
+    ```
+    """
+
+    def __init__(self, orphaned_node):
+        self.orphaned_node = orphaned_node
+
+    @abstractmethod
+    def __str__(self):
+        pass
+
+
+class CRIPTOrphanedMaterialError(CRIPTOrphanedNodesError):
+    """
+    ## Definition
+    CRIPTOrphanedNodesError, but specific for orphaned materials.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned materials into the parent project or its inventories.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
+
+    def __str__(self):
+        ret_string = "While validating a project graph, an orphaned material node was found. "
+        ret_string += "This material is present in the graph, but not listed in the project. "
+        ret_string += "Please add the node like: `my_project.material += [orphaned_material]`. "
+        ret_string += f"The orphaned material was {self.orphaned_node}."
+        return ret_string
+
+
+class CRIPTOrphanedExperimentError(CRIPTOrphanedNodesError):
+    """
+    ## Definition
+    CRIPTOrphanedNodesError, but specific for orphaned nodes that should be listed in one of the experiments.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned node into one the parent project's experiments.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
+
+    def __str__(self) -> str:
+        node_name = self.orphaned_node.node_type.lower()
+        ret_string = f"While validating a project graph, an orphaned {node_name} node was found. "
+        ret_string += f"This {node_name} node is present in the graph, but not listed in any of the experiments of the  project. "
+        ret_string += f"Please add the node like: `your_experiment.{node_name} += [orphaned_{node_name}]`. "
+        ret_string += f"The orphaned {node_name} was {self.orphaned_node}."
+        return ret_string
+
+
+class CRIPTOrphanedDataError(CRIPTOrphanedExperimentError):
+    """
+    ## Definition
+    CRIPTOrphanedExperimentError, but specific for orphaned Data node that should be listed in one of the experiments.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned node into one the parent project's experiments `data` attribute.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
+
+
+class CRIPTOrphanedProcessError(CRIPTOrphanedExperimentError):
+    """
+    ## Definition
+    CRIPTOrphanedExperimentError, but specific for orphaned Process node that should be
+    listed in one of the experiments.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned node into one the parent project's experiments
+    `process` attribute.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
+
+
+class CRIPTOrphanedComputationError(CRIPTOrphanedExperimentError):
+    """
+    ## Definition
+    CRIPTOrphanedExperimentError, but specific for orphaned Computation node that should be
+    listed in one of the experiments.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned node into one the parent project's experiments
+    `Computation` attribute.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
+
+
+class CRIPTOrphanedComputationalProcessError(CRIPTOrphanedExperimentError):
+    """
+    ## Definition
+    CRIPTOrphanedExperimentError, but specific for orphaned ComputationalProcess
+    node that should be listed in one of the experiments.
+
+    ## Troubleshooting
+    Handle this error by adding the orphaned node into one the parent project's experiments
+    `ComputationalProcess` attribute.
+    """
+
+    def __init__(self, orphaned_node):
+        super().__init__(orphaned_node)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/__init__.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/collection.py` & `cript-2.3.0/src/cript/nodes/subobjects/equipment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,299 +1,314 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-from cript.nodes.supporting_nodes import User
-
-
-class Collection(PrimaryBaseNode):
-    """
-    ## Definition
-
-    A
-    [Collection node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=8)
-    is nested inside a [Project](../project) node.
-
-    A Collection node can be thought as a folder/bucket that can hold [experiment](../experiment)
-    or [Inventories](../inventory) node.
-
-    | attribute  | type             | example             | description                                                                    |
-    |------------|------------------|---------------------|--------------------------------------------------------------------------------|
-    | experiment | list[Experiment] |                     | experiment that relate to the collection                                       |
-    | inventory  | list[Inventory]  |                     | inventory owned by the collection                                              |
-    | doi        | str              | `10.1038/1781168a0` | DOI: digital object identifier for a published collection; CRIPT generated DOI |
-    | citation   | list[Citation]   |                     | reference to a book, paper, or scholarly work                                  |
-    | notes      | str              | "my awesome notes"  | miscellaneous information, or custom data structure                            |
-
-
-    ## JSON Representation
-    ```json
-    {
-    "name": "my collection JSON",
-     "node":["Collection"],
-     "uid":"_:fccd3549-07cb-4e23-ba79-323597ec9bfd",
-     "uuid":"fccd3549-07cb-4e23-ba79-323597ec9bfd"
-
-     "experiment":[
-        {
-           "name":"my experiment name",
-           "node":["Experiment"],
-           "uid":"_:8256b75b-1f4e-4f69-9fe6-3bcb2298e470",
-           "uuid":"8256b75b-1f4e-4f69-9fe6-3bcb2298e470"
-        }
-     ],
-     "inventory":[],
-     "citation":[],
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Collection attributes
-        """
-
-        # TODO add proper typing in future, using Any for now to avoid circular import error
-        member: List[User] = field(default_factory=list)
-        admin: List[User] = field(default_factory=list)
-        experiment: List[Any] = field(default_factory=list)
-        inventory: List[Any] = field(default_factory=list)
-        doi: str = ""
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, experiment: Optional[List[Any]] = None, inventory: Optional[List[Any]] = None, doi: str = "", citation: Optional[List[Any]] = None, notes: str = "", **kwargs) -> None:
-        """
-        create a Collection with a name
-        add list of experiment, inventory, citation, doi, and notes if available.
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_collection = cript.Collection(name="my collection name")
-
-        Parameters
-        ----------
-        name: str
-            name of the Collection you want to make
-        experiment: Optional[List[Experiment]], default=None
-            list of experiment within the Collection
-        inventory: Optional[List[Inventory]], default=None
-            list of inventories within this collection
-        doi: str = "", default=""
-            cript doi
-        citation: Optional[List[Citation]], default=None
-            List of citations for this collection
-
-        Returns
-        -------
-        None
-            Instantiates a Collection node
-        """
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        if experiment is None:
-            experiment = []
-
-        if inventory is None:
-            inventory = []
-
-        if citation is None:
-            citation = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            name=name,
-            experiment=experiment,
-            inventory=inventory,
-            doi=doi,
-            citation=citation,
-        )
-
-        self.validate()
-
-    @property
-    @beartype
-    def member(self) -> List[User]:
-        return self._json_attrs.member.copy()
-
-    @property
-    @beartype
-    def admin(self) -> List[User]:
-        return self._json_attrs.admin
-
-    @property
-    @beartype
-    def experiment(self) -> List[Any]:
-        """
-        List of all [experiment](../experiment) within this Collection
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_collection = cript.Collection(name="my collection name")
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_collection.experiment = [my_experiment]
-
-        Returns
-        -------
-        List[Experiment]
-            list of all [experiment](../experiment) within this Collection
-        """
-        return self._json_attrs.experiment.copy()  # type: ignore
-
-    @experiment.setter
-    @beartype
-    def experiment(self, new_experiment: List[Any]) -> None:
-        """
-        sets the Experiment list within this collection
-
-        Parameters
-        ----------
-        new_experiment: List[Experiment]
-            list of experiment
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, experiment=new_experiment)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def inventory(self) -> List[Any]:
-        """
-        List of [inventory](../inventory) that belongs to this collection
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_collection = cript.Collection(name="my collection name")
-        >>> material_1 = cript.Material(
-        ...     name="material 1",
-        ...     identifier=[{"bigsmiles": "material 1 bigsmiles"}],
-        ... )
-        >>> material_2 = cript.Material(
-        ...     name="material 2",
-        ...     identifier=[{"bigsmiles": "material 2 bigsmiles"}],
-        ... )
-        >>> my_inventory = cript.Inventory(
-        ...     name="my inventory name", material=[material_1, material_2]
-        ... )
-        >>> my_collection.inventory = [my_inventory]
-
-        Returns
-        -------
-        inventory: List[Inventory]
-            list of inventories in this collection
-        """
-        return self._json_attrs.inventory.copy()  # type: ignore
-
-    @inventory.setter
-    @beartype
-    def inventory(self, new_inventory: List[Any]) -> None:
-        """
-        Sets the List of inventories within this collection to a new list
-
-        Parameters
-        ----------
-        new_inventory: List[Inventory]
-            new list of inventories for the collection to overwrite the current list
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, inventory=new_inventory)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def doi(self) -> str:
-        """
-        The CRIPT DOI for this collection
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_collection = cript.Collection(name="my collection name")
-        >>> my_collection.doi = "10.1038/1781168a0"
-
-        Returns
-        -------
-        doi: str
-            the CRIPT DOI e.g. `10.1038/1781168a0`
-        """
-        return self._json_attrs.doi
-
-    @doi.setter
-    @beartype
-    def doi(self, new_doi: str) -> None:
-        """
-        set the CRIPT DOI for this collection to new CRIPT DOI
-
-        Parameters
-        ----------
-        new_doi: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, doi=new_doi)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of Citations within this Collection
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_collection = cript.Collection(name="my collection name")
-        >>> my_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title="title",
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_collection.citation = [my_citation]
-
-        Returns
-        -------
-        citation: List[Citation]:
-            list of Citations within this Collection
-        """
-        return self._json_attrs.citation.copy()  # type: ignore
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation: List[Any]) -> None:
-        """
-        set the list of citations for this Collection
-
-        Parameters
-        ----------
-        new_citation: List[Citation]
-            set the list of citations for this Collection
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.subobjects.citation import Citation
+from cript.nodes.subobjects.condition import Condition
+from cript.nodes.supporting_nodes.file import File
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Equipment(UUIDBaseNode):
+    """
+    ## Definition
+    An [Equipment](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=23)
+    sub-object specifies the physical instruments, tools, glassware, etc. used in a process.
+
+    ---
+
+    ## Can Be Added To:
+    * [Process node](../../primary_nodes/process)
+
+    ## Available sub-objects:
+    * [Condition](../condition)
+    * [Citation](../citation)
+
+    ---
+
+    ## Attributes
+
+    | attribute   | type            | example                                       | description                                                                    | required | vocab |
+    |-------------|-----------------|-----------------------------------------------|--------------------------------------------------------------------------------|----------|-------|
+    | key         | str             | hot plate                                     | material                                                                       | True     | True  |
+    | description | str             | Hot plate with silicon oil bath with stir bar | additional details about the equipment                                         |          |       |
+    | condition   | list[Condition] |                                               | conditions under which the property was measured                               |          |       |
+    | files       | list[File]      |                                               | list of file nodes to link to calibration or equipment specification documents |          |       |
+    | citation    | list[Citation]  |                                               | reference to a book, paper, or scholarly work                                  |          |       |
+
+    ## JSON Representation
+    ```json
+    {
+       "node":["Equipment"],
+       "description": "my equipment description",
+       "key":"burner",
+       "uid":"_:19708284-1bd7-42e4-b8b2-da7ea0bc2ac9",
+       "uuid":"19708284-1bd7-42e4-b8b2-da7ea0bc2ac9"
+    }
+    ```
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        description: str = ""
+        condition: List[Union[Condition, UIDProxy]] = field(default_factory=list)
+        file: List[Union[File, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Citation, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, key: str, description: str = "", condition: Optional[List[Union[Condition, UIDProxy]]] = None, file: Optional[List[Union[File, UIDProxy]]] = None, citation: Optional[List[Union[Citation, UIDProxy]]] = None, **kwargs) -> None:
+        """
+        create equipment sub-object
+
+        Parameters
+        ----------
+        key : str
+            Equipment key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/equipment_key)
+        description : str, optional
+            additional details about the equipment, by default ""
+        condition : Union[List[Condition], None], optional
+            Conditions under which the property was measured, by default None
+        file : Union[List[File], None], optional
+            list of file nodes to link to calibration or equipment specification documents, by default None
+        citation : Union[List[Citation], None], optional
+            reference to a scholarly work, by default None
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+
+        Returns
+        -------
+        None
+            instantiate equipment sub-object
+        """
+        if condition is None:
+            condition = []
+        if file is None:
+            file = []
+        if citation is None:
+            citation = []
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, key=key, description=description, condition=condition, file=file, citation=citation)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        scientific instrument
+
+        Equipment key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/equipment_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> my_equipment.key = "hot_plate"
+
+        Returns
+        -------
+        Equipment: str
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    @beartype
+    def key(self, new_key: str) -> None:
+        """
+        set the equipment key
+
+        Parameters
+        ----------
+        new_key : str
+            equipment sub-object key
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def description(self) -> str:
+        """
+        description of the equipment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> my_equipment.description = "additional details about the equipment"
+
+        Returns
+        -------
+        str
+            additional description of the equipment
+        """
+        return self._json_attrs.description
+
+    @description.setter
+    @beartype
+    def description(self, new_description: str) -> None:
+        """
+        set this equipments description
+
+        Parameters
+        ----------
+        new_description : str
+            equipment description
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, description=new_description)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def condition(self) -> List[Union[Condition, UIDProxy]]:
+        """
+        conditions under which the property was measured
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_equipment.condition = [my_condition]
+
+        Returns
+        -------
+        List[Condition]
+            list of Condition sub-objects
+        """
+        return self._json_attrs.condition.copy()
+
+    @condition.setter
+    @beartype
+    def condition(self, new_condition: List[Union[Condition, UIDProxy]]) -> None:
+        """
+        set a list of Conditions for the equipment sub-object
+
+        Parameters
+        ----------
+        new_condition : List[Condition]
+            list of Condition sub-objects
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, condition=new_condition)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def file(self) -> List[Union[File, UIDProxy]]:
+        """
+        list of file nodes to link to calibration or equipment specification documents
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
+        ...     type="calibration",
+        ...     extension=".pdf",
+        ... )
+        >>> my_equipment.file = [my_file]
+
+        Returns
+        -------
+        List[File]
+            list of file nodes
+        """
+        return self._json_attrs.file.copy()
+
+    @file.setter
+    @beartype
+    def file(self, new_file: List[Union[File, UIDProxy]]) -> None:
+        """
+        set the file node for the equipment subobject
+
+        Parameters
+        ----------
+        new_file : List[File]
+            list of File nodes
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, file=new_file)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Union[Citation, UIDProxy]]:
+        """
+        reference to a book, paper, or scholarly work
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_equipment.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of Citation subobjects
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation: List[Union[Citation, UIDProxy]]) -> None:
+        """
+        set the citation subobject for this equipment subobject
+
+        Parameters
+        ----------
+        new_citation : List[Citation]
+            list of Citation subobjects
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/computation.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/computation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,442 +1,442 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class Computation(PrimaryBaseNode):
-    """
-    ## Definition
-
-    The
-    [Computation node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=14)
-    describes the transformation of data or the creation of a computational data
-    set.
-
-    **Common computations for simulations** are energy minimization, annealing, quenching, or
-    NPT/NVT (isothermal-isobaric/canonical ensemble) simulations.
-
-    **Common computations for experimental** data include fitting a reaction model to kinetic data
-    to determine rate constants, a plateau modulus from a time-temperature-superposition, or calculating radius of
-    gyration with the Debye function from small angle scattering data.
-
-
-
-    ## Attributes
-    | attribute                | type                          | example                               | description                                   | required | vocab |
-    |--------------------------|-------------------------------|---------------------------------------|-----------------------------------------------|----------|-------|
-    | type                     | str                           | general molecular dynamics simulation | category of computation                       | True     | True  |
-    | input_data               | list[Data]                    |                                       | input data nodes                              |          |       |
-    | output_data              | list[Data]                    |                                       | output data nodes                             |          |       |
-    | software_ configurations | list[Software  Configuration] |                                       | software and algorithms used                  |          |       |
-    | condition                | list[Condition]               |                                       | setup information                             |          |       |
-    | prerequisite_computation | Computation                   |                                       | prior computation method in chain             |          |       |
-    | citation                 | list[Citation]                |                                       | reference to a book, paper, or scholarly work |          |       |
-    | notes                    | str                           |                                       | additional description of the step            |          |       |
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my computation name",
-       "node":["Computation"],
-       "type":"analysis",
-       "uid":"_:69f29bec-e30a-4932-b78d-2e4585b37d74",
-       "uuid":"69f29bec-e30a-4932-b78d-2e4585b37d74"
-       "citation":[],
-    }
-    ```
-
-
-    ## Available Subobjects
-    * [Software Configuration](../../subobjects/software_configuration)
-    * [Condition](../../subobjects/condition)
-    * [Citation](../../subobjects/citation)
-
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all computation nodes attributes
-        """
-
-        type: str = ""
-        # TODO add proper typing in future, using Any for now to avoid circular import error
-        input_data: List[Any] = field(default_factory=list)
-        output_data: List[Any] = field(default_factory=list)
-        software_configuration: List[Any] = field(default_factory=list)
-        condition: List[Any] = field(default_factory=list)
-        prerequisite_computation: Optional["Computation"] = None
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        name: str,
-        type: str,
-        input_data: Optional[List[Any]] = None,
-        output_data: Optional[List[Any]] = None,
-        software_configuration: Optional[List[Any]] = None,
-        condition: Optional[List[Any]] = None,
-        prerequisite_computation: Optional["Computation"] = None,
-        citation: Optional[List[Any]] = None,
-        notes: str = "",
-        **kwargs
-    ) -> None:
-        """
-        create a computation node
-
-        Parameters
-        ----------
-        name: str
-            name of computation node
-        type: str
-            type of computation node. Computation type must come from CRIPT controlled vocabulary
-        input_data: List[Data] default=None
-            input data (data node)
-        output_data: List[Data] default=None
-            output data (data node)
-        software_configuration: List[SoftwareConfiguration] default=None
-            software configuration of computation node
-        condition: List[Condition] default=None
-            condition for the computation node
-        prerequisite_computation: Computation default=None
-            prerequisite computation
-        citation: List[Citation] default=None
-            list of citations
-        notes: str = ""
-            any notes for this computation node
-        **kwargs
-            for internal use of deserialize JSON from API to node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-
-        Returns
-        -------
-        None
-            instantiate a computation node
-
-        """
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        if input_data is None:
-            input_data = []
-
-        if output_data is None:
-            output_data = []
-
-        if software_configuration is None:
-            software_configuration = []
-
-        if condition is None:
-            condition = []
-
-        if citation is None:
-            citation = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            type=type,
-            input_data=input_data,
-            output_data=output_data,
-            software_configuration=software_configuration,
-            condition=condition,
-            prerequisite_computation=prerequisite_computation,
-            citation=citation,
-        )
-
-        self.validate()
-
-    # ------------------ Properties ------------------
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        The type of computation
-
-        The [computation type](https://app.criptapp.org/vocab/computation_type)
-        must come from CRIPT controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_computation.type = type="analysis"
-
-        Returns
-        -------
-        str
-            type of computation
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_computation_type: str) -> None:
-        """
-        set the computation type
-
-        the computation type must come from CRIPT controlled vocabulary
-
-        Parameters
-        ----------
-        new_computation_type: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_computation_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def input_data(self) -> List[Any]:
-        """
-        List of input data (data nodes) for this node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_input_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_computation.input_data = [my_input_data]
-
-        Returns
-        -------
-        List[Data]
-            list of input data for this computation
-        """
-        return self._json_attrs.input_data.copy()
-
-    @input_data.setter
-    @beartype
-    def input_data(self, new_input_data_list: List[Any]) -> None:
-        """
-        set the input data list
-
-        Parameters
-        ----------
-        new_input_data_list: List[Data]
-            list of input data (data nodes) to replace the current
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, input_data=new_input_data_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def output_data(self) -> List[Any]:
-        """
-        List of output data (data nodes)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_output_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_computation.output_data = [my_output_data]
-
-        Returns
-        -------
-        List[Data]
-            list of output data for this computation
-        """
-        return self._json_attrs.output_data.copy()
-
-    @output_data.setter
-    @beartype
-    def output_data(self, new_output_data_list: List[Any]) -> None:
-        """
-        set the list of output data (data nodes) for this node
-
-        Parameters
-        ----------
-        new_output_data_list: List[Data]
-            replace the current list of output data for this node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, output_data=new_output_data_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def software_configuration(self) -> List[Any]:
-        """
-        List of software_configuration for this computation node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_computation.software_configuration = [my_software_configuration]
-
-        Returns
-        -------
-        List[SoftwareConfiguration]
-            list of software configurations
-        """
-        return self._json_attrs.software_configuration.copy()
-
-    @software_configuration.setter
-    @beartype
-    def software_configuration(self, new_software_configuration_list: List[Any]) -> None:
-        """
-        set the list of software_configuration for this computation node
-
-        Parameters
-        ----------
-        new_software_configuration_list: List[software_configuration]
-            new_software_configuration_list to replace the current one
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, software_configuration=new_software_configuration_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def condition(self) -> List[Any]:
-        """
-        List of condition for this computation node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
-        >>> my_computation.condition = [my_condition]
-
-        Returns
-        -------
-        List[Condition]
-            list of condition for the computation node
-        """
-        return self._json_attrs.condition.copy()
-
-    @condition.setter
-    @beartype
-    def condition(self, new_condition_list: List[Any]) -> None:
-        """
-        set the list of condition for this node
-
-        Parameters
-        ----------
-        new_condition_list: List[Condition]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, condition=new_condition_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def prerequisite_computation(self) -> Optional["Computation"]:
-        """
-        prerequisite computation
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_prerequisite_computation = cript.Computation(
-        ...     name="my prerequisite computation name", type="data_fit"
-        ... )
-        >>> my_computation.prerequisite_computation = my_prerequisite_computation
-
-        Returns
-        -------
-        Computation
-            prerequisite computation
-        """
-        return self._json_attrs.prerequisite_computation
-
-    @prerequisite_computation.setter
-    @beartype
-    def prerequisite_computation(self, new_prerequisite_computation: Optional["Computation"]) -> None:
-        """
-        set new prerequisite_computation
-
-        Parameters
-        ----------
-        new_prerequisite_computation: "Computation"
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, prerequisite_computation=new_prerequisite_computation)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of citations
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_computation.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of citations for this computation node
-        """
-        return self._json_attrs.citation.copy()  # type: ignore
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation_list: List[Any]) -> None:
-        """
-        set the List of citations
-
-        Parameters
-        ----------
-        new_citation_list: List[Citation]
-            list of citations for this computation node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import Any, List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class Computation(PrimaryBaseNode):
+    """
+    ## Definition
+
+    The
+    [Computation node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=14)
+    describes the transformation of data or the creation of a computational data
+    set.
+
+    **Common computations for simulations** are energy minimization, annealing, quenching, or
+    NPT/NVT (isothermal-isobaric/canonical ensemble) simulations.
+
+    **Common computations for experimental** data include fitting a reaction model to kinetic data
+    to determine rate constants, a plateau modulus from a time-temperature-superposition, or calculating radius of
+    gyration with the Debye function from small angle scattering data.
+
+
+
+    ## Attributes
+    | attribute                | type                          | example                               | description                                   | required | vocab |
+    |--------------------------|-------------------------------|---------------------------------------|-----------------------------------------------|----------|-------|
+    | type                     | str                           | general molecular dynamics simulation | category of computation                       | True     | True  |
+    | input_data               | list[Data]                    |                                       | input data nodes                              |          |       |
+    | output_data              | list[Data]                    |                                       | output data nodes                             |          |       |
+    | software_ configurations | list[Software  Configuration] |                                       | software and algorithms used                  |          |       |
+    | condition                | list[Condition]               |                                       | setup information                             |          |       |
+    | prerequisite_computation | Computation                   |                                       | prior computation method in chain             |          |       |
+    | citation                 | list[Citation]                |                                       | reference to a book, paper, or scholarly work |          |       |
+    | notes                    | str                           |                                       | additional description of the step            |          |       |
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my computation name",
+       "node":["Computation"],
+       "type":"analysis",
+       "uid":"_:69f29bec-e30a-4932-b78d-2e4585b37d74",
+       "uuid":"69f29bec-e30a-4932-b78d-2e4585b37d74"
+       "citation":[],
+    }
+    ```
+
+
+    ## Available Subobjects
+    * [Software Configuration](../../subobjects/software_configuration)
+    * [Condition](../../subobjects/condition)
+    * [Citation](../../subobjects/citation)
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all computation nodes attributes
+        """
+
+        type: str = ""
+        # TODO add proper typing in future, using Any for now to avoid circular import error
+        input_data: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        output_data: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        software_configuration: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        condition: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        prerequisite_computation: Optional[Union["Computation", UIDProxy]] = None
+        citation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        name: str,
+        type: str,
+        input_data: Optional[List[Union[Any, UIDProxy]]] = None,
+        output_data: Optional[List[Union[Any, UIDProxy]]] = None,
+        software_configuration: Optional[List[Union[Any, UIDProxy]]] = None,
+        condition: Optional[List[Union[Any, UIDProxy]]] = None,
+        prerequisite_computation: Optional[Union["Computation", UIDProxy]] = None,
+        citation: Optional[List[Union[Any, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ) -> None:
+        """
+        create a computation node
+
+        Parameters
+        ----------
+        name: str
+            name of computation node
+        type: str
+            type of computation node. Computation type must come from CRIPT controlled vocabulary
+        input_data: List[Data] default=None
+            input data (data node)
+        output_data: List[Data] default=None
+            output data (data node)
+        software_configuration: List[SoftwareConfiguration] default=None
+            software configuration of computation node
+        condition: List[Condition] default=None
+            condition for the computation node
+        prerequisite_computation: Computation default=None
+            prerequisite computation
+        citation: List[Citation] default=None
+            list of citations
+        notes: str = ""
+            any notes for this computation node
+        **kwargs
+            for internal use of deserialize JSON from API to node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+
+        Returns
+        -------
+        None
+            instantiate a computation node
+
+        """
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        if input_data is None:
+            input_data = []
+
+        if output_data is None:
+            output_data = []
+
+        if software_configuration is None:
+            software_configuration = []
+
+        if condition is None:
+            condition = []
+
+        if citation is None:
+            citation = []
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            type=type,
+            input_data=input_data,
+            output_data=output_data,
+            software_configuration=software_configuration,
+            condition=condition,
+            prerequisite_computation=prerequisite_computation,
+            citation=citation,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    # ------------------ Properties ------------------
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        The type of computation
+
+        The [computation type](https://app.criptapp.org/vocab/computation_type)
+        must come from CRIPT controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_computation.type = type="analysis"
+
+        Returns
+        -------
+        str
+            type of computation
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_computation_type: str) -> None:
+        """
+        set the computation type
+
+        the computation type must come from CRIPT controlled vocabulary
+
+        Parameters
+        ----------
+        new_computation_type: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_computation_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def input_data(self) -> List[Any]:
+        """
+        List of input data (data nodes) for this node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_input_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_computation.input_data = [my_input_data]
+
+        Returns
+        -------
+        List[Data]
+            list of input data for this computation
+        """
+        return self._json_attrs.input_data.copy()
+
+    @input_data.setter
+    @beartype
+    def input_data(self, new_input_data_list: List[Any]) -> None:
+        """
+        set the input data list
+
+        Parameters
+        ----------
+        new_input_data_list: List[Data]
+            list of input data (data nodes) to replace the current
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, input_data=new_input_data_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def output_data(self) -> List[Any]:
+        """
+        List of output data (data nodes)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_output_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_computation.output_data = [my_output_data]
+
+        Returns
+        -------
+        List[Data]
+            list of output data for this computation
+        """
+        return self._json_attrs.output_data.copy()
+
+    @output_data.setter
+    @beartype
+    def output_data(self, new_output_data_list: List[Any]) -> None:
+        """
+        set the list of output data (data nodes) for this node
+
+        Parameters
+        ----------
+        new_output_data_list: List[Data]
+            replace the current list of output data for this node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, output_data=new_output_data_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def software_configuration(self) -> List[Any]:
+        """
+        List of software_configuration for this computation node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_computation.software_configuration = [my_software_configuration]
+
+        Returns
+        -------
+        List[SoftwareConfiguration]
+            list of software configurations
+        """
+        return self._json_attrs.software_configuration.copy()
+
+    @software_configuration.setter
+    @beartype
+    def software_configuration(self, new_software_configuration_list: List[Any]) -> None:
+        """
+        set the list of software_configuration for this computation node
+
+        Parameters
+        ----------
+        new_software_configuration_list: List[software_configuration]
+            new_software_configuration_list to replace the current one
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, software_configuration=new_software_configuration_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def condition(self) -> List[Any]:
+        """
+        List of condition for this computation node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
+        >>> my_computation.condition = [my_condition]
+
+        Returns
+        -------
+        List[Condition]
+            list of condition for the computation node
+        """
+        return self._json_attrs.condition.copy()
+
+    @condition.setter
+    @beartype
+    def condition(self, new_condition_list: List[Any]) -> None:
+        """
+        set the list of condition for this node
+
+        Parameters
+        ----------
+        new_condition_list: List[Condition]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, condition=new_condition_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def prerequisite_computation(self) -> Optional[Union["Computation", UIDProxy]]:
+        """
+        prerequisite computation
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_prerequisite_computation = cript.Computation(
+        ...     name="my prerequisite computation name", type="data_fit"
+        ... )
+        >>> my_computation.prerequisite_computation = my_prerequisite_computation
+
+        Returns
+        -------
+        Computation
+            prerequisite computation
+        """
+        return self._json_attrs.prerequisite_computation
+
+    @prerequisite_computation.setter
+    @beartype
+    def prerequisite_computation(self, new_prerequisite_computation: Optional[Union["Computation", UIDProxy]]) -> None:
+        """
+        set new prerequisite_computation
+
+        Parameters
+        ----------
+        new_prerequisite_computation: "Computation"
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, prerequisite_computation=new_prerequisite_computation)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Any]:
+        """
+        List of citations
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
+        >>> my_computation.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of citations for this computation node
+        """
+        return self._json_attrs.citation.copy()  # type: ignore
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation_list: List[Any]) -> None:
+        """
+        set the List of citations
+
+        Parameters
+        ----------
+        new_citation_list: List[Citation]
+            list of citations for this computation node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/computation_process.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/computation_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,549 +1,549 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class ComputationProcess(PrimaryBaseNode):
-    """
-    ## Definition
-
-    A
-    [Computational_Process](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=15)
-    is a simulation that processes or changes a virtual material. Examples
-    include simulations of chemical reactions, chain scission, cross-linking, strong shear, etc. A
-    computational process may also encapsulate any computation that dramatically changes the
-    materials properties, molecular topology, and physical aspects like molecular orientation, etc. The
-    computation_forcefield of a simulation is associated with a material. As a consequence, if the
-    forcefield changes or gets refined via a computational procedure (density functional theory,
-    iterative Boltzmann inversion for coarse-graining etc.) this forcefield changing step must be
-    described as a computational_process and a new material node with a different
-    computation_forcefield needs to be created.
-
-    ## Attributes
-    | attribute                | type                          | example                               | description                                   | required | vocab |
-    |--------------------------|-------------------------------|---------------------------------------|-----------------------------------------------|----------|-------|
-    | type                     | str                           | general molecular dynamics simulation | category of computation                       | True     | True  |
-    | input_data               | list[Data]                    |                                       | input data nodes                              | True     |       |
-    | output_data              | list[Data]                    |                                       | output data nodes                             |          |       |
-    | ingredient               | list[Ingredient]              |                                       | ingredients                                   | True     |       |
-    | software_ configurations | list[Software  Configuration] |                                       | software and algorithms used                  |          |       |
-    | condition                | list[Condition]               |                                       | setup information                             |          |       |
-    | property                 | list[Property]                |                                       | computation process properties                |          |       |
-    | citation                 | list[Citation]                |                                       | reference to a book, paper, or scholarly work |          |       |
-    | notes                    | str                           |                                       | additional description of the step            |          |       |
-
-
-    ## Available Subobjects
-    * [ingredient](../../subobjects/ingredient)
-    * [software_configuration](../../subobjects/software_configuration)
-    * [property](../../subobjects/property)
-    * [condition](../../subobjects/condition)
-    * [citation](../../subobjects/citation)
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my computational process node name",
-       "node":["ComputationProcess"],
-       "type":"cross_linking",
-       "uid":"_:b88ac0a5-b5c0-4197-a63d-b37e1fe8c6c6",
-       "uuid":"b88ac0a5-b5c0-4197-a63d-b37e1fe8c6c6"
-       "ingredient":[
-          {
-            "node":["Ingredient"],
-            "uid":"_:f68d6fff-9327-48b1-9249-33ce498005e8",
-             "uuid":"f68d6fff-9327-48b1-9249-33ce498005e8"
-             "keyword":["catalyst"],
-             "material":{
-                "name":"my material name",
-                "node":["Material"],
-                "uid":"_:3b12f92c-2121-4520-920e-b4c5622de34a",
-                "uuid":"3b12f92c-2121-4520-920e-b4c5622de34a",
-                "bigsmiles":"[H]{[>][<]C(C[>])c1ccccc1[]}",
-             },
-
-             "quantity":[
-                {
-                   "key":"mass",
-                   "node":["Quantity"],
-                   "uid":"_:07c4a6a9-9385-4505-a30a-ca3549cedcd8",
-                   "uuid":"07c4a6a9-9385-4505-a30a-ca3549cedcd8",
-                   "uncertainty":0.2,
-                   "uncertainty_type":"stdev",
-                   "unit":"kg",
-                   "value":11.2
-                }
-             ]
-          }
-       ],
-       "input_data":[
-          {
-            "name":"my data name",
-             "node":["Data"],
-             "type":"afm_amp",
-             "uid":"_:3c16bb05-ded1-4f52-9d02-c88c1a1de915",
-             "uuid":"3c16bb05-ded1-4f52-9d02-c88c1a1de915"
-             "file":[
-                {
-                   "name":"my file node name",
-                   "node":["File"],
-                   "source":"https://criptapp.org",
-                   "type":"calibration",
-                    "data_dictionary":"my file's data dictionary",
-                   "extension":".csv",
-                   "uid":"_:ee8153db-4108-49e4-8c5b-ffc26d4e6f71",
-                   "uuid":"ee8153db-4108-49e4-8c5b-ffc26d4e6f71"
-                }
-             ],
-          }
-       ],
-    }
-    ```
-
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all computational_process nodes attributes
-        """
-
-        type: str = ""
-        # TODO add proper typing in future, using Any for now to avoid circular import error
-        input_data: List[Any] = field(default_factory=list)
-        output_data: List[Any] = field(default_factory=list)
-        ingredient: List[Any] = field(default_factory=list)
-        software_configuration: List[Any] = field(default_factory=list)
-        condition: List[Any] = field(default_factory=list)
-        property: List[Any] = field(default_factory=list)
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        name: str,
-        type: str,
-        input_data: List[Any],
-        ingredient: List[Any],
-        output_data: Optional[List[Any]] = None,
-        software_configuration: Optional[List[Any]] = None,
-        condition: Optional[List[Any]] = None,
-        property: Optional[List[Any]] = None,
-        citation: Optional[List[Any]] = None,
-        notes: str = "",
-        **kwargs
-    ):
-        """
-        create a computational_process node
-
-        Examples
-        --------
-        >>> import cript
-        >>> data_files = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> input_data = cript.Data(name="my data name", type="afm_amp", file=[data_files])
-        >>> my_material = cript.Material(
-        ...     name="my material",
-        ...     identifier=[{"alternative_names": "my material alternative name"}]
-        ... )
-        >>> my_quantity = cript.Quantity(key="mass", value=1.23, unit="kg")
-        >>> ingredient = cript.Ingredient(
-        ...     material=my_material,
-        ...     quantity=[my_quantity],
-        ... )
-        >>> my_computation_process = cript.ComputationProcess(
-        ...     name="my computational process name",
-        ...     type="cross_linking",
-        ...     input_data=[input_data],
-        ...     ingredient=[ingredient],
-        ... )
-
-
-        Parameters
-        ----------
-        name: str
-            computational process name
-        type: str
-            type of computation process from CRIPT controlled vocabulary
-        input_data: List[Data]
-            list of input data for computational process
-        ingredient: List[Ingredient]
-            list of ingredients for this computational process node
-        output_data: List[Data] default=None
-            list of output data for this computational process node
-        software_configuration: List[SoftwareConfiguration] default=None
-            list of software configurations for this computational process node
-        condition: List[Condition] default=None
-            list of condition for this computational process node
-        property: List[Property] default=None
-            list of properties for this computational process node
-        citation: List[Citation] default=None
-            list of citation for this computational process node
-        notes: str default=""
-            optional notes for the computational process node
-
-        Returns
-        -------
-        None
-            instantiate computationalProcess node
-        """
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        if input_data is None:
-            input_data = []
-
-        if ingredient is None:
-            ingredient = []
-
-        if output_data is None:
-            output_data = []
-
-        if software_configuration is None:
-            software_configuration = []
-
-        if condition is None:
-            condition = []
-
-        if property is None:
-            property = []
-
-        if citation is None:
-            citation = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            type=type,
-            input_data=input_data,
-            ingredient=ingredient,
-            output_data=output_data,
-            software_configuration=software_configuration,
-            condition=condition,
-            property=property,
-            citation=citation,
-        )
-
-        # self.validate()
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        The [computational process type](https://app.criptapp.org/vocab/computational_process_type)
-        must come from CRIPT Controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computation_process.type = "DPD"   # doctest: +SKIP
-
-        Returns
-        -------
-        str
-            computational process type
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_type: str) -> None:
-        """
-        set the computational_process type
-
-        computational_process type must come from CRIPT controlled vocabulary
-
-        Parameters
-        ----------
-        new_type: str
-            new computational process type.
-            computational process type must come from CRIPT controlled vocabulary
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def input_data(self) -> List[Any]:
-        """
-        List of input data for the computational process node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     data_dictionary="my file's data dictionary",
-        ...     extension=".csv",
-        ... )
-        >>> my_input_data = cript.Data(name="my input data name", type="afm_amp", file=[my_file])
-        >>> my_computation_process.input_data = [my_input_data]     # doctest: +SKIP
-
-        Returns
-        -------
-        List[Data]
-            list of input data for this computational process node
-        """
-        return self._json_attrs.input_data.copy()
-
-    @input_data.setter
-    @beartype
-    def input_data(self, new_input_data_list: List[Any]) -> None:
-        """
-        set the input data for this computational process
-
-        Parameters
-        ----------
-        new_input_data_list: List[Data]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, input_data=new_input_data_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def output_data(self) -> List[Any]:
-        """
-        List of the output data for the computational_process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_output_data = cript.Data(name="my output data name", type="afm_amp", file=[my_file])
-        >>> my_computation_process.output_data = [my_output_data]    # doctest: +SKIP
-
-        Returns
-        -------
-        List[Data]
-            list of output data from this computational process node
-        """
-        return self._json_attrs.output_data.copy()
-
-    @output_data.setter
-    @beartype
-    def output_data(self, new_output_data_list: List[Any]) -> None:
-        """
-        set the output_data list for the computational_process
-
-        Parameters
-        ----------
-        new_output_data_list: List[Data]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, output_data=new_output_data_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def ingredient(self) -> List[Any]:
-        """
-        List of ingredients for the computational_process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_material = cript.Material(name="my material", identifier=[{"bigsmiles": "123456"}])
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_ingredient = cript.Ingredient(
-        ...     material=my_material, quantity=[my_quantity], keyword=["catalyst"]
-        ... )
-        >>> my_computation_process.ingredient = [my_ingredient]   # doctest: +SKIP
-
-        Returns
-        -------
-        List[Ingredient]
-            list of ingredients for this computational process
-        """
-        return self._json_attrs.ingredient.copy()
-
-    @ingredient.setter
-    @beartype
-    def ingredient(self, new_ingredient_list: List[Any]) -> None:
-        """
-        set the ingredients list for this computational process
-
-        Parameters
-        ----------
-        new_ingredient_list: List[Ingredient]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, ingredient=new_ingredient_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def software_configuration(self) -> List[Any]:
-        """
-        List of software_configuration for the computational process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_computation_process.software_configuration = [my_software_configuration]   # doctest: +SKIP
-
-        Returns
-        -------
-        List[SoftwareConfiguration]
-            List of software configurations used for this computational process node
-        """
-        return self._json_attrs.software_configuration.copy()
-
-    @software_configuration.setter
-    @beartype
-    def software_configuration(self, new_software_configuration_list: List[Any]) -> None:
-        """
-        set the list of software_configuration for the computational process
-
-        Parameters
-        ----------
-        new_software_configuration_list: List[SoftwareConfiguration]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, software_configuration=new_software_configuration_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def condition(self) -> List[Any]:
-        """
-        List of condition for the computational process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
-        >>> my_computation_process.condition = [my_condition]     # doctest: +SKIP
-
-        Returns
-        -------
-        List[Condition]
-            list of condition for this computational process node
-        """
-        return self._json_attrs.condition.copy()
-
-    @condition.setter
-    @beartype
-    def condition(self, new_condition: List[Any]) -> None:
-        """
-        set the condition for the computational process
-
-        Parameters
-        ----------
-        new_condition: List[Condition]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, condition=new_condition)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of citation for the computational process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_computation_process.citation = [my_citation]     # doctest: +SKIP
-
-        Returns
-        -------
-        List[Citation]
-            list of citation for this computational process
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation_list: List[Any]) -> None:
-        """
-        set the citation list for the computational process node
-
-        Parameters
-        ----------
-        new_citation_list: List[Citation]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def property(self) -> List[Any]:
-        """
-        List of properties
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
-        >>> my_computation_process.property = [my_property]     # doctest: +SKIP
-
-        Returns
-        -------
-        List[Property]
-            list of properties for this computational process node
-        """
-        return self._json_attrs.property.copy()
-
-    @property.setter
-    @beartype
-    def property(self, new_property_list: List[Any]) -> None:
-        """
-        set the properties list for the computational process
-
-        Parameters
-        ----------
-        new_property_list: List[Property]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, property=new_property_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import Any, List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class ComputationProcess(PrimaryBaseNode):
+    """
+    ## Definition
+
+    A
+    [Computational_Process](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=15)
+    is a simulation that processes or changes a virtual material. Examples
+    include simulations of chemical reactions, chain scission, cross-linking, strong shear, etc. A
+    computational process may also encapsulate any computation that dramatically changes the
+    materials properties, molecular topology, and physical aspects like molecular orientation, etc. The
+    computation_forcefield of a simulation is associated with a material. As a consequence, if the
+    forcefield changes or gets refined via a computational procedure (density functional theory,
+    iterative Boltzmann inversion for coarse-graining etc.) this forcefield changing step must be
+    described as a computational_process and a new material node with a different
+    computation_forcefield needs to be created.
+
+    ## Attributes
+    | attribute                | type                          | example                               | description                                   | required | vocab |
+    |--------------------------|-------------------------------|---------------------------------------|-----------------------------------------------|----------|-------|
+    | type                     | str                           | general molecular dynamics simulation | category of computation                       | True     | True  |
+    | input_data               | list[Data]                    |                                       | input data nodes                              | True     |       |
+    | output_data              | list[Data]                    |                                       | output data nodes                             |          |       |
+    | ingredient               | list[Ingredient]              |                                       | ingredients                                   | True     |       |
+    | software_ configurations | list[Software  Configuration] |                                       | software and algorithms used                  |          |       |
+    | condition                | list[Condition]               |                                       | setup information                             |          |       |
+    | property                 | list[Property]                |                                       | computation process properties                |          |       |
+    | citation                 | list[Citation]                |                                       | reference to a book, paper, or scholarly work |          |       |
+    | notes                    | str                           |                                       | additional description of the step            |          |       |
+
+
+    ## Available Subobjects
+    * [ingredient](../../subobjects/ingredient)
+    * [software_configuration](../../subobjects/software_configuration)
+    * [property](../../subobjects/property)
+    * [condition](../../subobjects/condition)
+    * [citation](../../subobjects/citation)
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my computational process node name",
+       "node":["ComputationProcess"],
+       "type":"cross_linking",
+       "uid":"_:b88ac0a5-b5c0-4197-a63d-b37e1fe8c6c6",
+       "uuid":"b88ac0a5-b5c0-4197-a63d-b37e1fe8c6c6"
+       "ingredient":[
+          {
+            "node":["Ingredient"],
+            "uid":"_:f68d6fff-9327-48b1-9249-33ce498005e8",
+             "uuid":"f68d6fff-9327-48b1-9249-33ce498005e8"
+             "keyword":["catalyst"],
+             "material":{
+                "name":"my material name",
+                "node":["Material"],
+                "uid":"_:3b12f92c-2121-4520-920e-b4c5622de34a",
+                "uuid":"3b12f92c-2121-4520-920e-b4c5622de34a",
+                "bigsmiles":"[H]{[>][<]C(C[>])c1ccccc1[]}",
+             },
+
+             "quantity":[
+                {
+                   "key":"mass",
+                   "node":["Quantity"],
+                   "uid":"_:07c4a6a9-9385-4505-a30a-ca3549cedcd8",
+                   "uuid":"07c4a6a9-9385-4505-a30a-ca3549cedcd8",
+                   "uncertainty":0.2,
+                   "uncertainty_type":"stdev",
+                   "unit":"kg",
+                   "value":11.2
+                }
+             ]
+          }
+       ],
+       "input_data":[
+          {
+            "name":"my data name",
+             "node":["Data"],
+             "type":"afm_amp",
+             "uid":"_:3c16bb05-ded1-4f52-9d02-c88c1a1de915",
+             "uuid":"3c16bb05-ded1-4f52-9d02-c88c1a1de915"
+             "file":[
+                {
+                   "name":"my file node name",
+                   "node":["File"],
+                   "source":"https://criptapp.org",
+                   "type":"calibration",
+                    "data_dictionary":"my file's data dictionary",
+                   "extension":".csv",
+                   "uid":"_:ee8153db-4108-49e4-8c5b-ffc26d4e6f71",
+                   "uuid":"ee8153db-4108-49e4-8c5b-ffc26d4e6f71"
+                }
+             ],
+          }
+       ],
+    }
+    ```
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all computational_process nodes attributes
+        """
+
+        type: str = ""
+        # TODO add proper typing in future, using Any for now to avoid circular import error
+        input_data: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        output_data: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        ingredient: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        software_configuration: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        condition: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        property: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        name: str,
+        type: str,
+        input_data: List[Union[Any, UIDProxy]],
+        ingredient: List[Union[Any, UIDProxy]],
+        output_data: Optional[List[Union[Any, UIDProxy]]] = None,
+        software_configuration: Optional[List[Union[Any, UIDProxy]]] = None,
+        condition: Optional[List[Union[Any, UIDProxy]]] = None,
+        property: Optional[List[Union[Any, UIDProxy]]] = None,
+        citation: Optional[List[Union[Any, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ):
+        """
+        create a computational_process node
+
+        Examples
+        --------
+        >>> import cript
+        >>> data_files = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> input_data = cript.Data(name="my data name", type="afm_amp", file=[data_files])
+        >>> my_material = cript.Material(
+        ...     name="my material",
+        ...     names = ["my material alternative name"]
+        ... )
+        >>> my_quantity = cript.Quantity(key="mass", value=1.23, unit="kg")
+        >>> ingredient = cript.Ingredient(
+        ...     material=my_material,
+        ...     quantity=[my_quantity],
+        ... )
+        >>> my_computation_process = cript.ComputationProcess(
+        ...     name="my computational process name",
+        ...     type="cross_linking",
+        ...     input_data=[input_data],
+        ...     ingredient=[ingredient],
+        ... )
+
+
+        Parameters
+        ----------
+        name: str
+            computational process name
+        type: str
+            type of computation process from CRIPT controlled vocabulary
+        input_data: List[Data]
+            list of input data for computational process
+        ingredient: List[Ingredient]
+            list of ingredients for this computational process node
+        output_data: List[Data] default=None
+            list of output data for this computational process node
+        software_configuration: List[SoftwareConfiguration] default=None
+            list of software configurations for this computational process node
+        condition: List[Condition] default=None
+            list of condition for this computational process node
+        property: List[Property] default=None
+            list of properties for this computational process node
+        citation: List[Citation] default=None
+            list of citation for this computational process node
+        notes: str default=""
+            optional notes for the computational process node
+
+        Returns
+        -------
+        None
+            instantiate computationalProcess node
+        """
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        if input_data is None:
+            input_data = []
+
+        if ingredient is None:
+            ingredient = []
+
+        if output_data is None:
+            output_data = []
+
+        if software_configuration is None:
+            software_configuration = []
+
+        if condition is None:
+            condition = []
+
+        if property is None:
+            property = []
+
+        if citation is None:
+            citation = []
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            type=type,
+            input_data=input_data,
+            ingredient=ingredient,
+            output_data=output_data,
+            software_configuration=software_configuration,
+            condition=condition,
+            property=property,
+            citation=citation,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        The [computational process type](https://app.criptapp.org/vocab/computational_process_type)
+        must come from CRIPT Controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computation_process.type = "DPD"   # doctest: +SKIP
+
+        Returns
+        -------
+        str
+            computational process type
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_type: str) -> None:
+        """
+        set the computational_process type
+
+        computational_process type must come from CRIPT controlled vocabulary
+
+        Parameters
+        ----------
+        new_type: str
+            new computational process type.
+            computational process type must come from CRIPT controlled vocabulary
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def input_data(self) -> List[Any]:
+        """
+        List of input data for the computational process node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     data_dictionary="my file's data dictionary",
+        ...     extension=".csv",
+        ... )
+        >>> my_input_data = cript.Data(name="my input data name", type="afm_amp", file=[my_file])
+        >>> my_computation_process.input_data = [my_input_data]     # doctest: +SKIP
+
+        Returns
+        -------
+        List[Data]
+            list of input data for this computational process node
+        """
+        return self._json_attrs.input_data.copy()
+
+    @input_data.setter
+    @beartype
+    def input_data(self, new_input_data_list: List[Any]) -> None:
+        """
+        set the input data for this computational process
+
+        Parameters
+        ----------
+        new_input_data_list: List[Data]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, input_data=new_input_data_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def output_data(self) -> List[Any]:
+        """
+        List of the output data for the computational_process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_output_data = cript.Data(name="my output data name", type="afm_amp", file=[my_file])
+        >>> my_computation_process.output_data = [my_output_data]    # doctest: +SKIP
+
+        Returns
+        -------
+        List[Data]
+            list of output data from this computational process node
+        """
+        return self._json_attrs.output_data.copy()
+
+    @output_data.setter
+    @beartype
+    def output_data(self, new_output_data_list: List[Any]) -> None:
+        """
+        set the output_data list for the computational_process
+
+        Parameters
+        ----------
+        new_output_data_list: List[Data]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, output_data=new_output_data_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def ingredient(self) -> List[Any]:
+        """
+        List of ingredients for the computational_process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_material = cript.Material(name="my material", bigsmiles = "my bigsmiles")
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_ingredient = cript.Ingredient(
+        ...     material=my_material, quantity=[my_quantity], keyword=["catalyst"]
+        ... )
+        >>> my_computation_process.ingredient = [my_ingredient]   # doctest: +SKIP
+
+        Returns
+        -------
+        List[Ingredient]
+            list of ingredients for this computational process
+        """
+        return self._json_attrs.ingredient.copy()
+
+    @ingredient.setter
+    @beartype
+    def ingredient(self, new_ingredient_list: List[Any]) -> None:
+        """
+        set the ingredients list for this computational process
+
+        Parameters
+        ----------
+        new_ingredient_list: List[Ingredient]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, ingredient=new_ingredient_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def software_configuration(self) -> List[Any]:
+        """
+        List of software_configuration for the computational process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_computation_process.software_configuration = [my_software_configuration]   # doctest: +SKIP
+
+        Returns
+        -------
+        List[SoftwareConfiguration]
+            List of software configurations used for this computational process node
+        """
+        return self._json_attrs.software_configuration.copy()
+
+    @software_configuration.setter
+    @beartype
+    def software_configuration(self, new_software_configuration_list: List[Any]) -> None:
+        """
+        set the list of software_configuration for the computational process
+
+        Parameters
+        ----------
+        new_software_configuration_list: List[SoftwareConfiguration]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, software_configuration=new_software_configuration_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def condition(self) -> List[Any]:
+        """
+        List of condition for the computational process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
+        >>> my_computation_process.condition = [my_condition]     # doctest: +SKIP
+
+        Returns
+        -------
+        List[Condition]
+            list of condition for this computational process node
+        """
+        return self._json_attrs.condition.copy()
+
+    @condition.setter
+    @beartype
+    def condition(self, new_condition: List[Any]) -> None:
+        """
+        set the condition for the computational process
+
+        Parameters
+        ----------
+        new_condition: List[Condition]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, condition=new_condition)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Any]:
+        """
+        List of citation for the computational process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
+        >>> my_computation_process.citation = [my_citation]     # doctest: +SKIP
+
+        Returns
+        -------
+        List[Citation]
+            list of citation for this computational process
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation_list: List[Any]) -> None:
+        """
+        set the citation list for the computational process node
+
+        Parameters
+        ----------
+        new_citation_list: List[Citation]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def property(self) -> List[Any]:
+        """
+        List of properties
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
+        >>> my_computation_process.property = [my_property]     # doctest: +SKIP
+
+        Returns
+        -------
+        List[Property]
+            list of properties for this computational process node
+        """
+        return self._json_attrs.property.copy()
+
+    @property.setter
+    @beartype
+    def property(self, new_property_list: List[Any]) -> None:
+        """
+        set the properties list for the computational process
+
+        Parameters
+        ----------
+        new_property_list: List[Property]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, property=new_property_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/data.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,586 +1,586 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class Data(PrimaryBaseNode):
-    """
-    ## Definition
-    A [Data node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=13)
-     node contains the meta-data to describe raw data that is beyond a single value, (i.e. n-dimensional data).
-     Each `Data` node must be linked to a single `Experiment` node.
-
-    ## Available Sub-Objects
-    * [Citation](../../subobjects/citation)
-
-    ## Attributes
-    | Attribute           | Type                                              | Example                    | Description                                                                                  | Required |
-    |---------------------|---------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------|----------|
-    | name                | str                                               | `"my_data_name"`           | Name of the data node                                                                        | True     |
-    | type                | str                                               | `"nmr_h1"`                 | Pick from [CRIPT data type controlled vocabulary](https://app.criptapp.org/vocab/data_type/) | True     |
-    | file                | List[[File](../supporting_nodes/file.md)]         | `[file_1, file_2, file_3]` | list of file nodes                                                                           | False    |
-    | sample_preparation  | [Process](process.md)                             |                            |                                                                                              | False    |
-    | computation         | List[[Computation](computation.md)]               |                            | data produced from this Computation method                                                   | False    |
-    | computation_process | [Computational Process](./computation_process.md) |                            | data was produced from this computation process                                              | False    |
-    | material            | List[[Material](./material.md)]                   |                            | materials with attributes associated with the data node                                      | False    |
-    | process             | List[[Process](./process.md)]                     |                            | processes with attributes associated with the data node                                      | False    |
-    | citation            | [Citation](../subobjects/citation.md)             |                            | reference to a book, paper, or scholarly work                                                | False    |
-    | notes               | str                                               | "my awesome notes"         | miscellaneous information, or custom data structure                                          | False    |
-
-    Examples
-    --------
-    >>> import cript
-    >>> my_file = cript.File(
-    ...    name="my file node name",
-    ...    source="https://criptapp.org",
-    ...    type="calibration",
-    ...    extension=".csv",
-    ...    data_dictionary="my file's data dictionary"
-    ... )
-    >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my data name",
-       "node":["Data"],
-       "type":"afm_amp",
-       "uid":"_:80b02470-73d0-416e-8d93-12fdf69e481a",
-       "uuid":"80b02470-73d0-416e-8d93-12fdf69e481a"
-       "file":[
-          {
-            "node":["File"],
-            "name":"my file node name",
-             "uid":"_:535779ea-0d1f-4b23-b3e8-60052f717307",
-             "uuid":"535779ea-0d1f-4b23-b3e8-60052f717307"
-             "type":"calibration",
-             "source":"https://criptapp.org",
-             "extension":".csv",
-             "data_dictionary":"my file's data dictionary",
-          }
-       ]
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Data attributes
-        """
-
-        type: str = ""
-        # TODO add proper typing in future, using Any for now to avoid circular import error
-        file: List[Any] = field(default_factory=list)
-        sample_preparation: Any = field(default_factory=list)
-        computation: List[Any] = field(default_factory=list)
-        computation_process: Any = field(default_factory=list)
-        material: List[Any] = field(default_factory=list)
-        process: List[Any] = field(default_factory=list)
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        name: str,
-        type: str,
-        file: List[Any],
-        sample_preparation: Any = None,
-        computation: Optional[List[Any]] = None,
-        computation_process: Optional[Any] = None,
-        material: Optional[List[Any]] = None,
-        process: Optional[List[Any]] = None,
-        citation: Optional[List[Any]] = None,
-        notes: str = "",
-        **kwargs
-    ) -> None:
-        """
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
-        ...      type="calibration",
-        ...      extension=".pdf",
-        ... )
-        >>> my_data = cript.Data(
-        ...     name="my data node name",
-        ...     type="afm_amp",
-        ...     file=[my_file],
-        ... )
-
-        Parameters
-        ----------
-        name: str
-            data node name
-        type: str
-            [data type](https://app.criptapp.org/vocab/data_type) must come from CRIPT controlled vocabulary
-        file: List[File], default None
-            list of CRIPT file nodes within the data node
-        sample_preparation: Process, default None
-            sample preparation
-        computation: Optional[Computation], default None
-            data was produced from this computation method
-        computation_process: Optional[ComputationalProcess], default None
-            data was produced from this computation process
-        material: Optional[List[Material]], default None
-            materials with attributes associated with the data node
-        process: Optional[List[Process]], default None
-            processes with attributes associated with the data node
-        citation: Optional[List[Citation]], default None
-            reference to a book, paper, or scholarly work
-        notes: str, default ""
-            miscellaneous information, or custom data structure
-        kwargs
-            used for deserializing JSON into Python SDK nodes
-
-        Returns
-        -------
-        None
-        """
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        if file is None:
-            file = []
-
-        if sample_preparation is None:
-            sample_preparation = []
-
-        if computation is None:
-            computation = []
-
-        if computation_process is None:
-            computation_process = []
-
-        if material is None:
-            material = []
-
-        if process is None:
-            process = []
-
-        if citation is None:
-            citation = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            type=type,
-            file=file,
-            sample_preparation=sample_preparation,
-            computation=computation,
-            computation_process=computation_process,
-            material=material,
-            process=process,
-            citation=citation,
-        )
-
-        self.validate()
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        The data type must come from [CRIPT data type vocabulary](https://app.criptapp.org/vocab/data_type)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_data.type = "nmr_h1"
-
-        Returns
-        -------
-        data type: str
-            data type for the data node must come from CRIPT controlled vocabulary
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_data_type: str) -> None:
-        """
-        set the data type.
-        The data type must come from [CRIPT data type vocabulary](https://app.criptapp.org/vocab/data_type)
-
-        Parameters
-        ----------
-        new_data_type: str
-            new data type to replace the current data type
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_data_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def file(self) -> List[Any]:
-        """
-        get the list of [files](../../supporting_nodes/file) for this data node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_new_file = cript.File(
-        ...    name="my new file node name",
-        ...    source="path/to/local/file",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data.file += [my_new_file]
-
-        Returns
-        -------
-        List[File]
-            list of files for this data node
-        """
-        return self._json_attrs.file.copy()
-
-    @file.setter
-    @beartype
-    def file(self, new_file_list: List[Any]) -> None:
-        """
-        set the list of file for this data node
-
-        Parameters
-        ----------
-        new_files_list: List[File]
-            new list of file nodes to replace the current list
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, file=new_file_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def sample_preparation(self) -> Union[Any, None]:
-        """
-        The [sample preparation](../process) for this data node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_new_files = cript.File(
-        ...     name="my file node name",
-        ...     source="https://pubs.acs.org/doi/10.1021/acscentsci.3c00011",
-        ...     type="computation_config",
-        ...     extension=".pdf",
-        ...     data_dictionary="my data dictionary",
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_new_files])
-        >>> my_sample_preparation = cript.Process(name="my sample preparation name", type="affinity_pure")
-        >>> my_data.sample_preparation = my_sample_preparation
-
-        Returns
-        -------
-        sample_preparation: Process
-            sample preparation for this data node
-        """
-        return self._json_attrs.sample_preparation
-
-    @sample_preparation.setter
-    @beartype
-    def sample_preparation(self, new_sample_preparation: Union[Any, None]) -> None:
-        """
-        set sample_preparation
-
-        Parameters
-        ----------
-        new_sample_preparation: Process
-            new_sample_preparation to replace the current one for this node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, sample_preparation=new_sample_preparation)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def computation(self) -> List[Any]:
-        """
-        list of [computation nodes](../computation/) for this material node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_data.computation = [my_computation]
-
-        Returns
-        -------
-        None
-            list of computation nodes
-        """
-        return self._json_attrs.computation.copy()
-
-    @computation.setter
-    @beartype
-    def computation(self, new_computation_list: List[Any]) -> None:
-        """
-        set list of computation  for this data node
-
-        Parameters
-        ----------
-        new_computation_list: List[Computation]
-            new computation list to replace the current one
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, computation=new_computation_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def computation_process(self) -> Union[Any, None]:
-        """
-        The [computation_process](../computation_process) for this data node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(
-        ...     name="my data name",
-        ...     type="afm_amp",
-        ...     file=[my_file]
-        ... )
-        >>> my_file_for_second_data_node = cript.File(
-        ...     name="my second file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_second_data_node = cript.Data(
-        ...     name="my data name",
-        ...     type="afm_amp",
-        ...     file=[my_file_for_second_data_node]
-        ... )
-        >>> my_material = cript.Material(
-        ...     name="my material name",
-        ...     identifier=[{"bigsmiles": "123456"}]
-        ... )
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_ingredient = cript.Ingredient(
-        ...     material=my_material,
-        ...     quantity=[my_quantity],
-        ...     keyword=["catalyst"],
-        ... )
-        >>> my_computational_process = cript.ComputationProcess(
-        ...     name="my computational process node name",
-        ...     type="cross_linking",
-        ...     input_data=[my_second_data_node],
-        ...     ingredient=[my_ingredient],
-        ... )
-
-        Returns
-        -------
-        ComputationalProcess
-            computational process node for this data node
-        """
-        return self._json_attrs.computation_process
-
-    @computation_process.setter
-    @beartype
-    def computation_process(self, new_computation_process: Union[Any, None]) -> None:
-        """
-        set the computational process
-
-        Parameters
-        ----------
-        new_computation_process: ComputationalProcess
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, computation_process=new_computation_process)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def material(self) -> List[Any]:
-        """
-        List of [materials](../material) for this node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_material = cript.Material(name="my material name", identifier=[{"bigsmiles": "123456"}])
-        >>> my_data.material = [my_material]
-
-        Returns
-        -------
-        List[Material]
-            list of material
-        """
-        return self._json_attrs.material.copy()
-
-    @material.setter
-    @beartype
-    def material(self, new_material_list: List[Any]) -> None:
-        """
-        set the list of materials for this data node
-
-        Parameters
-        ----------
-        new_material_list: List[Material]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, material=new_material_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def process(self) -> List[Any]:
-        """
-        list of [Process nodes](./process.md) for this data node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_data.process = [my_process]
-
-        Notes
-        -----
-        Please note that while the process attribute of the data node is currently set to `Any`
-        the software still expects a Process node in the data's process attribute
-        > It is currently set to `Any` to avoid the circular import error
-
-        Returns
-        -------
-        List[Process]
-            list of process for the data node
-        """
-        return self._json_attrs.process.copy()
-
-    @process.setter
-    @beartype
-    def process(self, new_process_list: List[Any]) -> None:
-        """
-        set the list of process for this data node
-
-        Parameters
-        ----------
-        new_process_list: List[Process]
-            new list of Process
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, process=new_process_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of [citation](../../subobjects/citation) within the data node
-
-        Examples
-        --------
-        >>> import cript
-        >>> import cript
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary"
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_data.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of citations for this data node
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation_list: List[Any]) -> None:
-        """
-        set the list of citation
-
-        Parameters
-        ----------
-        new_citation_list: List[Citation]
-            new list of citation to replace the current one
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import Any, List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class Data(PrimaryBaseNode):
+    """
+    ## Definition
+    A [Data node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=13)
+     node contains the meta-data to describe raw data that is beyond a single value, (i.e. n-dimensional data).
+     Each `Data` node must be linked to a single `Experiment` node.
+
+    ## Available Sub-Objects
+    * [Citation](../../subobjects/citation)
+
+    ## Attributes
+    | Attribute           | Type                                              | Example                    | Description                                                                                  | Required |
+    |---------------------|---------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------|----------|
+    | name                | str                                               | `"my_data_name"`           | Name of the data node                                                                        | True     |
+    | type                | str                                               | `"nmr_h1"`                 | Pick from [CRIPT data type controlled vocabulary](https://app.criptapp.org/vocab/data_type/) | True     |
+    | file                | List[[File](../supporting_nodes/file.md)]         | `[file_1, file_2, file_3]` | list of file nodes                                                                           | False    |
+    | sample_preparation  | [Process](process.md)                             |                            |                                                                                              | False    |
+    | computation         | List[[Computation](computation.md)]               |                            | data produced from this Computation method                                                   | False    |
+    | computation_process | [Computational Process](./computation_process.md) |                            | data was produced from this computation process                                              | False    |
+    | material            | List[[Material](./material.md)]                   |                            | materials with attributes associated with the data node                                      | False    |
+    | process             | List[[Process](./process.md)]                     |                            | processes with attributes associated with the data node                                      | False    |
+    | citation            | [Citation](../subobjects/citation.md)             |                            | reference to a book, paper, or scholarly work                                                | False    |
+    | notes               | str                                               | "my awesome notes"         | miscellaneous information, or custom data structure                                          | False    |
+
+    Examples
+    --------
+    >>> import cript
+    >>> my_file = cript.File(
+    ...    name="my file node name",
+    ...    source="https://criptapp.org",
+    ...    type="calibration",
+    ...    extension=".csv",
+    ...    data_dictionary="my file's data dictionary"
+    ... )
+    >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my data name",
+       "node":["Data"],
+       "type":"afm_amp",
+       "uid":"_:80b02470-73d0-416e-8d93-12fdf69e481a",
+       "uuid":"80b02470-73d0-416e-8d93-12fdf69e481a"
+       "file":[
+          {
+            "node":["File"],
+            "name":"my file node name",
+             "uid":"_:535779ea-0d1f-4b23-b3e8-60052f717307",
+             "uuid":"535779ea-0d1f-4b23-b3e8-60052f717307"
+             "type":"calibration",
+             "source":"https://criptapp.org",
+             "extension":".csv",
+             "data_dictionary":"my file's data dictionary",
+          }
+       ]
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all Data attributes
+        """
+
+        type: str = ""
+        # TODO add proper typing in future, using Any for now to avoid circular import error
+        file: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        sample_preparation: Union[Any, UIDProxy] = field(default_factory=list)
+        computation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        computation_process: Union[Any, UIDProxy] = field(default_factory=list)
+        material: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        process: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        name: str,
+        type: str,
+        file: List[Union[Any, UIDProxy]],
+        sample_preparation: Union[Any, UIDProxy] = None,
+        computation: Optional[List[Union[Any, UIDProxy]]] = None,
+        computation_process: Optional[Union[Any, UIDProxy]] = None,
+        material: Optional[List[Union[Any, UIDProxy]]] = None,
+        process: Optional[List[Union[Any, UIDProxy]]] = None,
+        citation: Optional[List[Union[Any, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ) -> None:
+        """
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
+        ...      type="calibration",
+        ...      extension=".pdf",
+        ... )
+        >>> my_data = cript.Data(
+        ...     name="my data node name",
+        ...     type="afm_amp",
+        ...     file=[my_file],
+        ... )
+
+        Parameters
+        ----------
+        name: str
+            data node name
+        type: str
+            [data type](https://app.criptapp.org/vocab/data_type) must come from CRIPT controlled vocabulary
+        file: List[File], default None
+            list of CRIPT file nodes within the data node
+        sample_preparation: Process, default None
+            sample preparation
+        computation: Optional[Computation], default None
+            data was produced from this computation method
+        computation_process: Optional[ComputationalProcess], default None
+            data was produced from this computation process
+        material: Optional[List[Material]], default None
+            materials with attributes associated with the data node
+        process: Optional[List[Process]], default None
+            processes with attributes associated with the data node
+        citation: Optional[List[Citation]], default None
+            reference to a book, paper, or scholarly work
+        notes: str, default ""
+            miscellaneous information, or custom data structure
+        kwargs
+            used for deserializing JSON into Python SDK nodes
+
+        Returns
+        -------
+        None
+        """
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        if file is None:
+            file = []
+
+        if sample_preparation is None:
+            sample_preparation = []
+
+        if computation is None:
+            computation = []
+
+        if computation_process is None:
+            computation_process = []
+
+        if material is None:
+            material = []
+
+        if process is None:
+            process = []
+
+        if citation is None:
+            citation = []
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            type=type,
+            file=file,
+            sample_preparation=sample_preparation,
+            computation=computation,
+            computation_process=computation_process,
+            material=material,
+            process=process,
+            citation=citation,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        The data type must come from [CRIPT data type vocabulary](https://app.criptapp.org/vocab/data_type)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_data.type = "nmr_h1"
+
+        Returns
+        -------
+        data type: str
+            data type for the data node must come from CRIPT controlled vocabulary
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_data_type: str) -> None:
+        """
+        set the data type.
+        The data type must come from [CRIPT data type vocabulary](https://app.criptapp.org/vocab/data_type)
+
+        Parameters
+        ----------
+        new_data_type: str
+            new data type to replace the current data type
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_data_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def file(self) -> List[Any]:
+        """
+        get the list of [files](../../supporting_nodes/file) for this data node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_new_file = cript.File(
+        ...    name="my new file node name",
+        ...    source="path/to/local/file",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data.file += [my_new_file]
+
+        Returns
+        -------
+        List[File]
+            list of files for this data node
+        """
+        return self._json_attrs.file.copy()
+
+    @file.setter
+    @beartype
+    def file(self, new_file_list: List[Any]) -> None:
+        """
+        set the list of file for this data node
+
+        Parameters
+        ----------
+        new_files_list: List[File]
+            new list of file nodes to replace the current list
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, file=new_file_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def sample_preparation(self) -> Union[Any, None]:
+        """
+        The [sample preparation](../process) for this data node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_new_files = cript.File(
+        ...     name="my file node name",
+        ...     source="https://pubs.acs.org/doi/10.1021/acscentsci.3c00011",
+        ...     type="computation_config",
+        ...     extension=".pdf",
+        ...     data_dictionary="my data dictionary",
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_new_files])
+        >>> my_sample_preparation = cript.Process(name="my sample preparation name", type="affinity_pure")
+        >>> my_data.sample_preparation = my_sample_preparation
+
+        Returns
+        -------
+        sample_preparation: Process
+            sample preparation for this data node
+        """
+        return self._json_attrs.sample_preparation
+
+    @sample_preparation.setter
+    @beartype
+    def sample_preparation(self, new_sample_preparation: Union[Any, None]) -> None:
+        """
+        set sample_preparation
+
+        Parameters
+        ----------
+        new_sample_preparation: Process
+            new_sample_preparation to replace the current one for this node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, sample_preparation=new_sample_preparation)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def computation(self) -> List[Any]:
+        """
+        list of [computation nodes](../computation/) for this material node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_data.computation = [my_computation]
+
+        Returns
+        -------
+        None
+            list of computation nodes
+        """
+        return self._json_attrs.computation.copy()
+
+    @computation.setter
+    @beartype
+    def computation(self, new_computation_list: List[Any]) -> None:
+        """
+        set list of computation  for this data node
+
+        Parameters
+        ----------
+        new_computation_list: List[Computation]
+            new computation list to replace the current one
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, computation=new_computation_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def computation_process(self) -> Union[Any, None]:
+        """
+        The [computation_process](../computation_process) for this data node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(
+        ...     name="my data name",
+        ...     type="afm_amp",
+        ...     file=[my_file]
+        ... )
+        >>> my_file_for_second_data_node = cript.File(
+        ...     name="my second file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_second_data_node = cript.Data(
+        ...     name="my data name",
+        ...     type="afm_amp",
+        ...     file=[my_file_for_second_data_node]
+        ... )
+        >>> my_material = cript.Material(
+        ...     name="my material name",
+        ...     bigsmiles = "123456"
+        ... )
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_ingredient = cript.Ingredient(
+        ...     material=my_material,
+        ...     quantity=[my_quantity],
+        ...     keyword=["catalyst"],
+        ... )
+        >>> my_computational_process = cript.ComputationProcess(
+        ...     name="my computational process node name",
+        ...     type="cross_linking",
+        ...     input_data=[my_second_data_node],
+        ...     ingredient=[my_ingredient],
+        ... )
+
+        Returns
+        -------
+        ComputationalProcess
+            computational process node for this data node
+        """
+        return self._json_attrs.computation_process
+
+    @computation_process.setter
+    @beartype
+    def computation_process(self, new_computation_process: Union[Any, None]) -> None:
+        """
+        set the computational process
+
+        Parameters
+        ----------
+        new_computation_process: ComputationalProcess
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, computation_process=new_computation_process)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def material(self) -> List[Any]:
+        """
+        List of [materials](../material) for this node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_material = cript.Material(name="my material name", bigsmiles = "123456")
+        >>> my_data.material = [my_material]
+
+        Returns
+        -------
+        List[Material]
+            list of material
+        """
+        return self._json_attrs.material.copy()
+
+    @material.setter
+    @beartype
+    def material(self, new_material_list: List[Any]) -> None:
+        """
+        set the list of materials for this data node
+
+        Parameters
+        ----------
+        new_material_list: List[Material]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, material=new_material_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def process(self) -> List[Any]:
+        """
+        list of [Process nodes](./process.md) for this data node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_data.process = [my_process]
+
+        Notes
+        -----
+        Please note that while the process attribute of the data node is currently set to `Any`
+        the software still expects a Process node in the data's process attribute
+        > It is currently set to `Any` to avoid the circular import error
+
+        Returns
+        -------
+        List[Process]
+            list of process for the data node
+        """
+        return self._json_attrs.process.copy()
+
+    @process.setter
+    @beartype
+    def process(self, new_process_list: List[Any]) -> None:
+        """
+        set the list of process for this data node
+
+        Parameters
+        ----------
+        new_process_list: List[Process]
+            new list of Process
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, process=new_process_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Any]:
+        """
+        List of [citation](../../subobjects/citation) within the data node
+
+        Examples
+        --------
+        >>> import cript
+        >>> import cript
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary"
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
+        >>> my_data.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of citations for this data node
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation_list: List[Any]) -> None:
+        """
+        set the list of citation
+
+        Parameters
+        ----------
+        new_citation_list: List[Citation]
+            new list of citation to replace the current one
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/experiment.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/experiment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,419 +1,419 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class Experiment(PrimaryBaseNode):
-    """
-    ## Definition
-    An
-    [Experiment node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
-    is nested inside a [Collection](../collection) node.
-
-    ## Attributes
-
-    | attribute           | type                         | description                                               | required |
-    |---------------------|------------------------------|-----------------------------------------------------------|----------|
-    | collection          | Collection                   | collection associated with the experiment                 | True     |
-    | process             | List[Process]                | process nodes associated with this experiment             | False    |
-    | computations        | List[Computation]            | computation method nodes associated with this experiment  | False    |
-    | computation_process | List[Computational  Process] | computation process nodes associated with this experiment | False    |
-    | data                | List[Data]                   | data nodes associated with this experiment                | False    |
-    | funding             | List[str]                    | funding source for experiment                             | False    |
-    | citation            | List[Citation]               | reference to a book, paper, or scholarly work             | False    |
-    | notes               | str                          | miscellaneous information, or custom data structure       | False    |
-
-
-    ## Sub-objects
-    An
-    [Experiment node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
-    can be thought as a folder/bucket that can hold:
-
-    * [Process](../process)
-    * [Computations](../computation)
-    * [Computation_Process](../computation_process)
-    * [Data](../data)
-    * [Funding](./#cript.nodes.primary_nodes.experiment.Experiment.funding)
-    * [Citation](../../subobjects/citation)
-
-
-    Warnings
-    --------
-    !!! warning "Experiment names"
-        Experiment names **MUST** be unique within a [Collection](../collection)
-
-    ---
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my experiment name",
-       "node":["Experiment"],
-       "uid":"_:886c4deb-2186-4f11-8134-a37111200b83",
-       "uuid":"886c4deb-2186-4f11-8134-a37111200b83"
-    }
-    ```
-
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Collection attributes
-        """
-
-        process: List[Any] = field(default_factory=list)
-        computation: List[Any] = field(default_factory=list)
-        computation_process: List[Any] = field(default_factory=list)
-        data: List[Any] = field(default_factory=list)
-        funding: List[str] = field(default_factory=list)
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        name: str,
-        process: Optional[List[Any]] = None,
-        computation: Optional[List[Any]] = None,
-        computation_process: Optional[List[Any]] = None,
-        data: Optional[List[Any]] = None,
-        funding: Optional[List[str]] = None,
-        citation: Optional[List[Any]] = None,
-        notes: str = "",
-        **kwargs
-    ):
-        """
-        create an Experiment node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-
-        Parameters
-        ----------
-        name: str
-            name of Experiment
-        process: List[Process]
-            list of Process nodes for this Experiment
-        computation: List[Computation]
-            list of computation nodes for this Experiment
-        computation_process: List[ComputationalProcess]
-            list of computational_process nodes for this Experiment
-        data: List[Data]
-            list of data nodes for this experiment
-        funding: List[str]
-            list of the funders names for this Experiment
-        citation: List[Citation]
-            list of Citation nodes for this experiment
-        notes: str default=""
-            notes for the experiment node
-
-        Returns
-        -------
-        None
-            Instantiate an Experiment node
-        """
-
-        if process is None:
-            process = []
-        if computation is None:
-            computation = []
-        if computation_process is None:
-            computation_process = []
-        if data is None:
-            data = []
-        if funding is None:
-            funding = []
-        if citation is None:
-            citation = []
-
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            name=name,
-            process=process,
-            computation=computation,
-            computation_process=computation_process,
-            data=data,
-            funding=funding,
-            citation=citation,
-            notes=notes,
-        )
-
-        # check if the code is still valid
-        self.validate()
-
-    @property
-    @beartype
-    def process(self) -> List[Any]:
-        """
-        List of process for experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_experiment.process = [my_process]
-
-        Returns
-        -------
-        List[Process]
-            List of process that were performed in this experiment
-        """
-        return self._json_attrs.process.copy()
-
-    @process.setter
-    @beartype
-    def process(self, new_process_list: List[Any]) -> None:
-        """
-        set the list of process for this experiment
-
-        Parameters
-        ----------
-        new_process_list: List[Process]
-            new process list to replace the current process list
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, process=new_process_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def computation(self) -> List[Any]:
-        """
-        List of the [computations](../computation) in this experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_experiment.computation = [my_computation]
-
-        Returns
-        -------
-        List[Computation]
-            List of [computations](../computation) for this experiment
-        """
-        return self._json_attrs.computation.copy()
-
-    @computation.setter
-    @beartype
-    def computation(self, new_computation_list: List[Any]) -> None:
-        """
-        set the list of computations for this experiment
-
-        Parameters
-        ----------
-        new_computation_list: List[Computation]
-            new list of computations to replace the current list of experiments
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, computation=new_computation_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def computation_process(self) -> List[Any]:
-        """
-        List of [computation_process](../computation_process) for this experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_file = cript.File(
-        ...     name="my file node",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary",
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_material = cript.Material(
-        ...     name="my material name", identifier=[{"bigsmiles": "123456"}]
-        ... )
-        >>> my_quantity = cript.Quantity(
-        ... key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_ingredient = cript.Ingredient(
-        ... material=my_material, quantity=[my_quantity], keyword=["catalyst"]
-        ... )
-        >>> my_computation_process = cript.ComputationProcess(
-        ...     name="my computational process name",
-        ...     type="cross_linking",         # must come from CRIPT Controlled Vocabulary
-        ...     input_data=[my_data],         # input data is another data node
-        ...     ingredient=[my_ingredient],  # output data is another data node
-        ... )
-        >>> my_experiment.computation_process = [my_computation_process]
-
-        Returns
-        -------
-        List[ComputationalProcess]
-            computational process that were performed in this experiment
-        """
-        return self._json_attrs.computation_process.copy()
-
-    @computation_process.setter
-    @beartype
-    def computation_process(self, new_computation_process_list: List[Any]) -> None:
-        """
-        set the list of computation_process for this experiment
-
-        Parameters
-        ----------
-        new_computation_process_list: List[ComputationalProcess]
-            new list of computations to replace the current for the experiment
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, computation_process=new_computation_process_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def data(self) -> List[Any]:
-        """
-        List of [data nodes](../data) for this experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_file = cript.File(
-        ...    name="my file node name",
-        ...    source="https://criptapp.org",
-        ...    type="calibration",
-        ...    extension=".csv",
-        ...    data_dictionary="my file's data dictionary",
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_experiment.data = [my_data]
-
-        Returns
-        -------
-        List[Data]
-            list of [data nodes](../data) that belong to this experiment
-        """
-        return self._json_attrs.data.copy()
-
-    @data.setter
-    @beartype
-    def data(self, new_data_list: List[Any]) -> None:
-        """
-        set the list of data for this experiment
-
-        Parameters
-        ----------
-        new_data_list: List[Data]
-            new list of data to replace the current list for this experiment
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, data=new_data_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def funding(self) -> List[str]:
-        """
-        List of strings of all the funders for this experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_experiment.funding = ["National Science Foundation", "IRIS", "NIST"]
-
-        Returns
-        -------
-        List[str]
-            List of funders for this experiment
-        """
-        return self._json_attrs.funding.copy()
-
-    @funding.setter
-    @beartype
-    def funding(self, new_funding_list: List[str]) -> None:
-        """
-        set the list of funders for this experiment
-
-        Parameters
-        ----------
-        new_funding_list: List[str]
-            replace the current list of funders
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, funding=new_funding_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of [citation](../../subobjects/citation) for this experiment
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_experiment = cript.Experiment(name="my experiment name")
-        >>> my_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title="title",
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_experiment.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of citations of scholarly work that was used in this experiment
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation_list: List[Any]) -> None:
-        """
-        set the list of citations for this experiment
-
-        Parameters
-        ----------
-        new_citations_list: List[Citation]
-            replace the list of citations for this experiment with a new list of citations
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import Any, List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class Experiment(PrimaryBaseNode):
+    """
+    ## Definition
+    An
+    [Experiment node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
+    is nested inside a [Collection](../collection) node.
+
+    ## Attributes
+
+    | attribute           | type                         | description                                               | required |
+    |---------------------|------------------------------|-----------------------------------------------------------|----------|
+    | collection          | Collection                   | collection associated with the experiment                 | True     |
+    | process             | List[Process]                | process nodes associated with this experiment             | False    |
+    | computations        | List[Computation]            | computation method nodes associated with this experiment  | False    |
+    | computation_process | List[Computational  Process] | computation process nodes associated with this experiment | False    |
+    | data                | List[Data]                   | data nodes associated with this experiment                | False    |
+    | funding             | List[str]                    | funding source for experiment                             | False    |
+    | citation            | List[Citation]               | reference to a book, paper, or scholarly work             | False    |
+    | notes               | str                          | miscellaneous information, or custom data structure       | False    |
+
+
+    ## Sub-objects
+    An
+    [Experiment node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
+    can be thought as a folder/bucket that can hold:
+
+    * [Process](../process)
+    * [Computations](../computation)
+    * [Computation_Process](../computation_process)
+    * [Data](../data)
+    * [Funding](./#cript.nodes.primary_nodes.experiment.Experiment.funding)
+    * [Citation](../../subobjects/citation)
+
+
+    Warnings
+    --------
+    !!! warning "Experiment names"
+        Experiment names **MUST** be unique within a [Collection](../collection)
+
+    ---
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my experiment name",
+       "node":["Experiment"],
+       "uid":"_:886c4deb-2186-4f11-8134-a37111200b83",
+       "uuid":"886c4deb-2186-4f11-8134-a37111200b83"
+    }
+    ```
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all Collection attributes
+        """
+
+        process: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        computation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        computation_process: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        data: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        funding: List[str] = field(default_factory=list)
+        citation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        name: str,
+        process: Optional[List[Union[Any, UIDProxy]]] = None,
+        computation: Optional[List[Union[Any, UIDProxy]]] = None,
+        computation_process: Optional[List[Union[Any, UIDProxy]]] = None,
+        data: Optional[List[Union[Any, UIDProxy]]] = None,
+        funding: Optional[List[str]] = None,
+        citation: Optional[List[Union[Any, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ):
+        """
+        create an Experiment node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+
+        Parameters
+        ----------
+        name: str
+            name of Experiment
+        process: List[Process]
+            list of Process nodes for this Experiment
+        computation: List[Computation]
+            list of computation nodes for this Experiment
+        computation_process: List[ComputationalProcess]
+            list of computational_process nodes for this Experiment
+        data: List[Data]
+            list of data nodes for this experiment
+        funding: List[str]
+            list of the funders names for this Experiment
+        citation: List[Citation]
+            list of Citation nodes for this experiment
+        notes: str default=""
+            notes for the experiment node
+
+        Returns
+        -------
+        None
+            Instantiate an Experiment node
+        """
+
+        if process is None:
+            process = []
+        if computation is None:
+            computation = []
+        if computation_process is None:
+            computation_process = []
+        if data is None:
+            data = []
+        if funding is None:
+            funding = []
+        if citation is None:
+            citation = []
+
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            name=name,
+            process=process,
+            computation=computation,
+            computation_process=computation_process,
+            data=data,
+            funding=funding,
+            citation=citation,
+            notes=notes,
+        )
+
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def process(self) -> List[Any]:
+        """
+        List of process for experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_experiment.process = [my_process]
+
+        Returns
+        -------
+        List[Process]
+            List of process that were performed in this experiment
+        """
+        return self._json_attrs.process.copy()
+
+    @process.setter
+    @beartype
+    def process(self, new_process_list: List[Any]) -> None:
+        """
+        set the list of process for this experiment
+
+        Parameters
+        ----------
+        new_process_list: List[Process]
+            new process list to replace the current process list
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, process=new_process_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def computation(self) -> List[Any]:
+        """
+        List of the [computations](../computation) in this experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_experiment.computation = [my_computation]
+
+        Returns
+        -------
+        List[Computation]
+            List of [computations](../computation) for this experiment
+        """
+        return self._json_attrs.computation.copy()
+
+    @computation.setter
+    @beartype
+    def computation(self, new_computation_list: List[Any]) -> None:
+        """
+        set the list of computations for this experiment
+
+        Parameters
+        ----------
+        new_computation_list: List[Computation]
+            new list of computations to replace the current list of experiments
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, computation=new_computation_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def computation_process(self) -> List[Any]:
+        """
+        List of [computation_process](../computation_process) for this experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_file = cript.File(
+        ...     name="my file node",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary",
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_material = cript.Material(
+        ...     name="my material name", bigsmiles = "123456"
+        ... )
+        >>> my_quantity = cript.Quantity(
+        ... key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_ingredient = cript.Ingredient(
+        ... material=my_material, quantity=[my_quantity], keyword=["catalyst"]
+        ... )
+        >>> my_computation_process = cript.ComputationProcess(
+        ...     name="my computational process name",
+        ...     type="cross_linking",         # must come from CRIPT Controlled Vocabulary
+        ...     input_data=[my_data],         # input data is another data node
+        ...     ingredient=[my_ingredient],  # output data is another data node
+        ... )
+        >>> my_experiment.computation_process = [my_computation_process]
+
+        Returns
+        -------
+        List[ComputationalProcess]
+            computational process that were performed in this experiment
+        """
+        return self._json_attrs.computation_process.copy()
+
+    @computation_process.setter
+    @beartype
+    def computation_process(self, new_computation_process_list: List[Any]) -> None:
+        """
+        set the list of computation_process for this experiment
+
+        Parameters
+        ----------
+        new_computation_process_list: List[ComputationalProcess]
+            new list of computations to replace the current for the experiment
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, computation_process=new_computation_process_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def data(self) -> List[Any]:
+        """
+        List of [data nodes](../data) for this experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_file = cript.File(
+        ...    name="my file node name",
+        ...    source="https://criptapp.org",
+        ...    type="calibration",
+        ...    extension=".csv",
+        ...    data_dictionary="my file's data dictionary",
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_experiment.data = [my_data]
+
+        Returns
+        -------
+        List[Data]
+            list of [data nodes](../data) that belong to this experiment
+        """
+        return self._json_attrs.data.copy()
+
+    @data.setter
+    @beartype
+    def data(self, new_data_list: List[Any]) -> None:
+        """
+        set the list of data for this experiment
+
+        Parameters
+        ----------
+        new_data_list: List[Data]
+            new list of data to replace the current list for this experiment
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, data=new_data_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def funding(self) -> List[str]:
+        """
+        List of strings of all the funders for this experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_experiment.funding = ["National Science Foundation", "IRIS", "NIST"]
+
+        Returns
+        -------
+        List[str]
+            List of funders for this experiment
+        """
+        return self._json_attrs.funding.copy()
+
+    @funding.setter
+    @beartype
+    def funding(self, new_funding_list: List[str]) -> None:
+        """
+        set the list of funders for this experiment
+
+        Parameters
+        ----------
+        new_funding_list: List[str]
+            replace the current list of funders
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, funding=new_funding_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Any]:
+        """
+        List of [citation](../../subobjects/citation) for this experiment
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_experiment = cript.Experiment(name="my experiment name")
+        >>> my_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title="title",
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
+        >>> my_experiment.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of citations of scholarly work that was used in this experiment
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation_list: List[Any]) -> None:
+        """
+        set the list of citations for this experiment
+
+        Parameters
+        ----------
+        new_citations_list: List[Citation]
+            replace the list of citations for this experiment with a new list of citations
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/inventory.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/inventory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,147 +1,149 @@
-from dataclasses import dataclass, field, replace
-from typing import List
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.material import Material
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class Inventory(PrimaryBaseNode):
-    """
-    ## Definition
-    An
-    [Inventory Node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
-    is a list of material nodes.
-    An example of an inventory can be a grouping of materials that were extracted from literature
-    and curated into a group for machine learning, or it can be a subset of chemicals that are used for a
-    certain type of synthesis.
-
-    ## Attributes
-    | Attribute | Type                            | Example            | Description                                         |
-    |-----------|---------------------------------|--------------------|-----------------------------------------------------|
-    | material  | list[[Material](./material.md)] |                    | material that you like to group together            |
-    | notes     | str                             | "my awesome notes" | miscellaneous information, or custom data structure |
-
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my inventory name",
-       "node":["Inventory"],
-       "uid":"_:90f45778-b7c9-4b77-8b83-a6ea9671a937",
-       "uuid":"90f45778-b7c9-4b77-8b83-a6ea9671a937",
-       "material":[
-          {
-             "node":["Material"],
-             "name":"my material 1",
-             "uid":"_:9679ff12-f9b4-41f4-be95-080b78fa71fd",
-             "uuid":"9679ff12-f9b4-41f4-be95-080b78fa71fd"
-             "bigsmiles":"[H]{[>][<]C(C[>])c1ccccc1[]}",
-          },
-          {
-             "node":["Material"],
-             "name":"my material 2",
-             "uid":"_:1ee41708-3531-43eb-8049-4bb91ad73df6",
-             "uuid":"1ee41708-3531-43eb-8049-4bb91ad73df6"
-             "bigsmiles":"654321",
-          }
-       ]
-    }
-    ```
-
-
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Inventory attributes
-        """
-
-        material: List[Material] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, material: List[Material], notes: str = "", **kwargs) -> None:
-        """
-        Instantiate an inventory node
-
-        Examples
-        --------
-        >>> import cript
-        >>> material_1 = cript.Material(
-        ...    name="material 1",
-        ...    identifier=[{"bigsmiles": "material 1 bigsmiles"}],
-        ... )
-        >>> material_2 = cript.Material(
-        ...    name="material 2",
-        ...    identifier=[{"bigsmiles": "material 2 bigsmiles"}],
-        ... )
-        >>> my_inventory = cript.Inventory(
-        ...    name="my inventory name", material=[material_1, material_2]
-        ... )
-
-        Parameters
-        ----------
-        material: List[Material]
-            list of materials in this inventory
-
-        Returns
-        -------
-        None
-            instantiate an inventory node
-        """
-
-        if material is None:
-            material = []
-
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        self._json_attrs = replace(self._json_attrs, material=material)
-
-    @property
-    @beartype
-    def material(self) -> List[Material]:
-        """
-        List of [material](../material) in this inventory
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_material = cript.Material(
-        ...    name="my material",
-        ...    identifier=[{"bigsmiles": "my bigsmiles"}],
-        ... )
-        >>> my_inventory = cript.Inventory(name="my inventory", material=[my_material])
-        >>> new_material = cript.Material(
-        ...    name="new material",
-        ...    identifier=[{"bigsmiles": "my bigsmiles"}],
-        ... )
-        >>> my_inventory.material = [new_material]
-
-        Returns
-        -------
-        List[Material]
-            list of material representing the inventory within the collection
-        """
-        return self._json_attrs.material.copy()
-
-    @material.setter
-    @beartype
-    def material(self, new_material_list: List[Material]):
-        """
-        set the list of material for this inventory node
-
-        Parameters
-        ----------
-        new_material_list: List[Material]
-            new list of material to replace the current list of material nodes for this inventory node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, material=new_material_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.material import Material
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class Inventory(PrimaryBaseNode):
+    """
+    ## Definition
+    An
+    [Inventory Node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=9)
+    is a list of material nodes.
+    An example of an inventory can be a grouping of materials that were extracted from literature
+    and curated into a group for machine learning, or it can be a subset of chemicals that are used for a
+    certain type of synthesis.
+
+    ## Attributes
+    | Attribute | Type                            | Example            | Description                                         |
+    |-----------|---------------------------------|--------------------|-----------------------------------------------------|
+    | material  | list[[Material](./material.md)] |                    | material that you like to group together            |
+    | notes     | str                             | "my awesome notes" | miscellaneous information, or custom data structure |
+
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my inventory name",
+       "node":["Inventory"],
+       "uid":"_:90f45778-b7c9-4b77-8b83-a6ea9671a937",
+       "uuid":"90f45778-b7c9-4b77-8b83-a6ea9671a937",
+       "material":[
+          {
+             "node":["Material"],
+             "name":"my material 1",
+             "uid":"_:9679ff12-f9b4-41f4-be95-080b78fa71fd",
+             "uuid":"9679ff12-f9b4-41f4-be95-080b78fa71fd"
+             "bigsmiles":"[H]{[>][<]C(C[>])c1ccccc1[]}",
+          },
+          {
+             "node":["Material"],
+             "name":"my material 2",
+             "uid":"_:1ee41708-3531-43eb-8049-4bb91ad73df6",
+             "uuid":"1ee41708-3531-43eb-8049-4bb91ad73df6"
+             "bigsmiles":"654321",
+          }
+       ]
+    }
+    ```
+
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all Inventory attributes
+        """
+
+        material: List[Union[Material, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, name: str, material: List[Union[Material, UIDProxy]], notes: str = "", **kwargs) -> None:
+        """
+        Instantiate an inventory node
+
+        Examples
+        --------
+        >>> import cript
+        >>> material_1 = cript.Material(
+        ...    name="material 1",
+        ...    bigsmiles = "material 1 bigsmiles",
+        ... )
+        >>> material_2 = cript.Material(
+        ...    name="material 2",
+        ...    bigsmiles = "material 2 bigsmiles",
+        ... )
+        >>> my_inventory = cript.Inventory(
+        ...    name="my inventory name", material=[material_1, material_2]
+        ... )
+
+        Parameters
+        ----------
+        material: List[Material]
+            list of materials in this inventory
+
+        Returns
+        -------
+        None
+            instantiate an inventory node
+        """
+
+        if material is None:
+            material = []
+
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        new_json_attrs = replace(self._json_attrs, material=material)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def material(self) -> List[Union[Material, UIDProxy]]:
+        """
+        List of [material](../material) in this inventory
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_material = cript.Material(
+        ...    name="my material",
+        ...    bigsmiles = "my bigsmiles",
+        ... )
+        >>> my_inventory = cript.Inventory(name="my inventory", material=[my_material])
+        >>> new_material = cript.Material(
+        ...    name="new material",
+        ...    bigsmiles = "my bigsmiles",
+        ... )
+        >>> my_inventory.material = [new_material]
+
+        Returns
+        -------
+        List[Material]
+            list of material representing the inventory within the collection
+        """
+        return self._json_attrs.material.copy()
+
+    @material.setter
+    @beartype
+    def material(self, new_material_list: List[Union[Material, UIDProxy]]):
+        """
+        set the list of material for this inventory node
+
+        Parameters
+        ----------
+        new_material_list: List[Material]
+            new list of material to replace the current list of material nodes for this inventory node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, material=new_material_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/primary_base_node.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/primary_base_node.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from abc import ABC
-from dataclasses import dataclass, replace
-
-from beartype import beartype
-
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class PrimaryBaseNode(UUIDBaseNode, ABC):
-    """
-    Abstract class that defines what it means to be a PrimaryNode,
-    and other primary nodes can inherit from.
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        """
-        All shared attributes between all Primary nodes and set to their default values
-        """
-
-        locked: bool = False
-        model_version: str = ""
-        public: bool = False
-        name: str = ""
-        notes: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, notes: str, **kwargs):
-        # initialize Base class with node
-        super().__init__(**kwargs)
-        # replace name and notes within PrimaryBase
-        self._json_attrs = replace(self._json_attrs, name=name, notes=notes)
-
-    @beartype
-    def __str__(self) -> str:
-        """
-        Return a string representation of a primary node dataclass attributes.
-        Every node that inherits from this class should overwrite it to best fit
-        their use case, but this provides a nice default value just in case
-
-        Examples
-        --------
-        {
-        'locked': False,
-        'model_version': '',
-        'public': False,
-        'notes': ''
-        }
-
-
-        Returns
-        -------
-        str
-            A string representation of the primary node common attributes.
-        """
-        return super().__str__()
-
-    @property
-    @beartype
-    def locked(self):
-        return self._json_attrs.locked
-
-    @property
-    @beartype
-    def model_version(self):
-        return self._json_attrs.model_version
-
-    @property
-    @beartype
-    def updated_by(self):
-        return self._json_attrs.updated_by
-
-    @property
-    @beartype
-    def created_by(self):
-        return self._json_attrs.created_by
-
-    @property
-    @beartype
-    def public(self):
-        return self._json_attrs.public
-
-    @property
-    @beartype
-    def name(self):
-        return self._json_attrs.name
-
-    @name.setter
-    @beartype
-    def name(self, new_name: str) -> None:
-        """
-        set the PrimaryBaseNode name
-
-        Parameters
-        ----------
-        new_name: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, name=new_name)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def notes(self):
-        return self._json_attrs.notes
-
-    @notes.setter
-    @beartype
-    def notes(self, new_notes: str) -> None:
-        """
-        allow every node that inherits base attributes to set its notes
-        """
-        new_attrs = replace(self._json_attrs, notes=new_notes)
-        self._update_json_attrs_if_valid(new_attrs)
+from abc import ABC
+from dataclasses import dataclass, replace
+
+from beartype import beartype
+
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class PrimaryBaseNode(UUIDBaseNode, ABC):
+    """
+    Abstract class that defines what it means to be a PrimaryNode,
+    and other primary nodes can inherit from.
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        """
+        All shared attributes between all Primary nodes and set to their default values
+        """
+
+        locked: bool = False
+        model_version: str = ""
+        public: bool = False
+        name: str = ""
+        notes: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, name: str, notes: str, **kwargs):
+        # initialize Base class with node
+        super().__init__(**kwargs)
+        # replace name and notes within PrimaryBase
+        self._json_attrs = replace(self._json_attrs, name=name, notes=notes)
+
+    @beartype
+    def __str__(self) -> str:
+        """
+        Return a string representation of a primary node dataclass attributes.
+        Every node that inherits from this class should overwrite it to best fit
+        their use case, but this provides a nice default value just in case
+
+        Examples
+        --------
+        {
+        'locked': False,
+        'model_version': '',
+        'public': False,
+        'notes': ''
+        }
+
+
+        Returns
+        -------
+        str
+            A string representation of the primary node common attributes.
+        """
+        return super().__str__()
+
+    @property
+    @beartype
+    def locked(self):
+        return self._json_attrs.locked
+
+    @property
+    @beartype
+    def model_version(self):
+        return self._json_attrs.model_version
+
+    @property
+    @beartype
+    def updated_by(self):
+        return self._json_attrs.updated_by
+
+    @property
+    @beartype
+    def created_by(self):
+        return self._json_attrs.created_by
+
+    @property
+    @beartype
+    def public(self):
+        return self._json_attrs.public
+
+    @property
+    @beartype
+    def name(self):
+        return self._json_attrs.name
+
+    @name.setter
+    @beartype
+    def name(self, new_name: str) -> None:
+        """
+        set the PrimaryBaseNode name
+
+        Parameters
+        ----------
+        new_name: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, name=new_name)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def notes(self):
+        return self._json_attrs.notes
+
+    @notes.setter
+    @beartype
+    def notes(self, new_notes: str) -> None:
+        """
+        allow every node that inherits base attributes to set its notes
+        """
+        new_attrs = replace(self._json_attrs, notes=new_notes)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/process.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,609 +1,609 @@
-from dataclasses import dataclass, field, replace
-from typing import Any, List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-class Process(PrimaryBaseNode):
-    """
-    ## Definition
-    The process node contains a list of [ingredients](../../subobjects/ingredient),
-    [quantities](../../subobjects/quantity), and procedure information for an experimental
-    [material](../material) transformation (chemical and physical).
-
-    ## Attributes
-
-    | attribute               | type             | example                                                                         | description                                                         | required | vocab |
-    |-------------------------|------------------|---------------------------------------------------------------------------------|---------------------------------------------------------------------|----------|-------|
-    | type                    | str              | mix                                                                             | type of process                                                     | True     | True  |
-    | ingredient              | list[Ingredient] |                                                                                 | ingredients                                                         |          |       |
-    | description             | str              | To oven-dried 20 mL glass vial, 5 mL of styrene and 10 ml of toluene was added. | explanation of the process                                          |          |       |
-    | equipment               | list[Equipment]  |                                                                                 | equipment used in the process                                       |          |       |
-    | product                 | list[Material]   |                                                                                 | desired material produced from the process                          |          |       |
-    | waste                   | list[Material]   |                                                                                 | material sent to waste                                              |          |       |
-    | prerequisite_ processes | list[Process]    |                                                                                 | processes that must be completed prior to the start of this process |          |       |
-    | condition               | list[Condition]  |                                                                                 | global process condition                                            |          |       |
-    | property                | list[Property]   |                                                                                 | process properties                                                  |          |       |
-    | keyword                 | list[str]        |                                                                                 | words that classify the process                                     |          | True  |
-    | citation                | list[Citation]   |                                                                                 | reference to a book, paper, or scholarly work                       |          |       |
-    | notes                   | str              |                                                                                 | miscellaneous information, or custom data structure                 |          |       |
-
-    ## Can be added to
-    * [Experiment](../experiment)
-
-    ## Available Subobjects
-    * [Ingredient](../../subobjects/ingredient)
-    * [Equipment](../../subobjects/equipment)
-    * [Property](../../subobjects/property)
-    * [Condition](../../subobjects/condition)
-    * [Citation](../../subobjects/citation)
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my minimal process name",
-       "node":["Process"],
-       "type":"affinity_pure",
-       "keyword":[],
-       "uid":"_:f8ef33f3-677a-40f3-b24e-65ab2c99d796",
-       "uuid":"f8ef33f3-677a-40f3-b24e-65ab2c99d796"
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Process attributes
-        """
-
-        type: str = ""
-        # TODO add proper typing in future, using Any for now to avoid circular import error
-        ingredient: List[Any] = field(default_factory=list)
-        description: str = ""
-        equipment: List[Any] = field(default_factory=list)
-        product: List[Any] = field(default_factory=list)
-        waste: List[Any] = field(default_factory=list)
-        prerequisite_process: List["Process"] = field(default_factory=list)
-        condition: List[Any] = field(default_factory=list)
-        property: List[Any] = field(default_factory=list)
-        keyword: List[str] = field(default_factory=list)
-        citation: List[Any] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        name: str,
-        type: str,
-        ingredient: Optional[List[Any]] = None,
-        description: str = "",
-        equipment: Optional[List[Any]] = None,
-        product: Optional[List[Any]] = None,
-        waste: Optional[List[Any]] = None,
-        prerequisite_process: Optional[List[Any]] = None,
-        condition: Optional[List[Any]] = None,
-        property: Optional[List[Any]] = None,
-        keyword: Optional[List[str]] = None,
-        citation: Optional[List[Any]] = None,
-        notes: str = "",
-        **kwargs
-    ) -> None:
-        """
-        create a process node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-
-        Parameters
-        ----------
-        ingredient: List[Ingredient]
-            [ingredient](../../subobjects/ingredient) used in this process
-        type: str = ""
-            Process type must come from
-            [CRIPT Controlled vocabulary process type](https://app.criptapp.org/vocab/process_type/)
-        description: str = ""
-            description of this process
-        equipment: List[Equipment] = None
-            list of [equipment](../../subobjects/equipment) used in this process
-        product: List[Material] = None
-            product that this process created
-        waste: List[Material] = None
-            waste that this process created
-        condition: List[Condition] = None
-            list of [condition](../../subobjects/condition) that this process was created under
-        property: List[Property] = None
-            list of [properties](../../subobjects/property) for this process
-        keyword: List[str] = None
-            list of keywords for this process must come from
-            [CRIPT process keyword controlled keyword](https://app.criptapp.org/vocab/process_keyword/)
-        citation: List[Citation] = None
-            list of [citation](../../subobjects/citation)
-
-        Returns
-        -------
-        None
-            instantiate a process node
-        """
-
-        if ingredient is None:
-            ingredient = []
-
-        if equipment is None:
-            equipment = []
-
-        if product is None:
-            product = []
-
-        if waste is None:
-            waste = []
-
-        if prerequisite_process is None:
-            prerequisite_process = []
-
-        if condition is None:
-            condition = []
-
-        if property is None:
-            property = []
-
-        if keyword is None:
-            keyword = []
-
-        if citation is None:
-            citation = []
-
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        new_attrs = replace(
-            self._json_attrs,
-            ingredient=ingredient,
-            type=type,
-            description=description,
-            equipment=equipment,
-            product=product,
-            waste=waste,
-            condition=condition,
-            prerequisite_process=prerequisite_process,
-            property=property,
-            keyword=keyword,
-            citation=citation,
-        )
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        [Process type](https://app.criptapp.org/vocab/process_type) must come from the CRIPT controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_process.type = "affinity_pure"
-
-        Returns
-        -------
-        str
-            Select a [Process type](https://app.criptapp.org/vocab/process_type/) from CRIPT controlled vocabulary
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_process_type: str) -> None:
-        """
-        set process type from CRIPT controlled vocabulary
-
-        Parameters
-        ----------
-        new_process_type: str
-            new process type from CRIPT controlled vocabulary
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_process_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def ingredient(self) -> List[Any]:
-        """
-        List of [ingredient](../../subobjects/ingredient) for this process
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_identifier = [{"bigsmiles": "123456"}]
-        >>> my_material = cript.Material(name="my material", identifier=my_identifier)
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_ingredient = cript.Ingredient(
-        ...     material=my_material, quantity=[my_quantity], keyword=["catalyst"]
-        ... )
-        >>> my_process.ingredient = [my_ingredient]
-
-        Returns
-        -------
-        List[Ingredient]
-            list of ingredients for this process
-        """
-        return self._json_attrs.ingredient.copy()
-
-    @ingredient.setter
-    @beartype
-    def ingredient(self, new_ingredient_list: List[Any]) -> None:
-        """
-        set the list of the ingredients for this process
-
-        Parameters
-        ----------
-        new_ingredient_list
-            list of ingredients to replace the current list
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, ingredient=new_ingredient_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def description(self) -> str:
-        """
-        description of this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_process.description = "To oven-dried 20 mL glass vial, 5 mL of styrene and 10 ml of toluene was added"
-
-        Returns
-        -------
-        str
-            description of this process
-        """
-        return self._json_attrs.description
-
-    @description.setter
-    @beartype
-    def description(self, new_description: str) -> None:
-        """
-        set the description of this process
-
-        Parameters
-        ----------
-        new_description: str
-            new process description to replace the current one
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, description=new_description)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def equipment(self) -> List[Any]:
-        """
-        List of [equipment](../../subobjects/equipment) used for this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_equipment = cript.Equipment(key="burner")
-        >>> my_process.equipment = [my_equipment]
-
-        Returns
-        -------
-        List[Equipment]
-            list of equipment used for this process
-        """
-        return self._json_attrs.equipment.copy()
-
-    @equipment.setter
-    @beartype
-    def equipment(self, new_equipment_list: List[Any]) -> None:
-        """
-        set the list of equipment used for this process
-
-        Parameters
-        ----------
-        new_equipment_list
-            new equipment list to replace the current equipment list for this process
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, equipment=new_equipment_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def product(self) -> List[Any]:
-        """
-        List of product (material nodes) for this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_product_material = cript.Material(
-        ...     name="my product material",
-        ...     identifier=[{"amino_acid": "my material product amino_acid"}],
-        ... )
-        >>> my_process.product = [my_product_material]
-
-        Returns
-        -------
-        List[Material]
-            List of process product (Material nodes)
-        """
-        return self._json_attrs.product.copy()
-
-    @product.setter
-    @beartype
-    def product(self, new_product_list: List[Any]) -> None:
-        """
-        set the product list for this process
-
-        Parameters
-        ----------
-        new_product_list: List[Material]
-            replace the current list of process product
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, product=new_product_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def waste(self) -> List[Any]:
-        """
-        List of waste that resulted from this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_waste_material = cript.Material(
-        ...     name="my waste material",
-        ...     identifier=[{"bigsmiles": "123456"}],
-        ... )
-        >>> my_process.waste = [my_waste_material]
-
-        Returns
-        -------
-        List[Material]
-            list of waste materials that resulted from this product
-        """
-        return self._json_attrs.waste.copy()
-
-    @waste.setter
-    @beartype
-    def waste(self, new_waste_list: List[Any]) -> None:
-        """
-        set the list of waste (Material node) for that resulted from this process
-
-        Parameters
-        ----------
-        new_waste_list: List[Material]
-            replace the list waste that resulted from this process
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, waste=new_waste_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def prerequisite_process(self) -> List["Process"]:
-        """
-        list of prerequisite process nodes
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_prerequisite_process = [
-        ...     cript.Process(name="prerequisite processes 1", type="blow_molding"),
-        ...     cript.Process(name="prerequisite processes 2", type="centrifugation"),
-        ... ]
-        >>> my_process.prerequisite_process = my_prerequisite_process
-
-        Returns
-        -------
-        List[Process]
-            list of process that had to happen before this process
-        """
-        return self._json_attrs.prerequisite_process.copy()
-
-    @prerequisite_process.setter
-    @beartype
-    def prerequisite_process(self, new_prerequisite_process_list: List["Process"]) -> None:
-        """
-        set the prerequisite_process for the process node
-
-        Parameters
-        ----------
-        new_prerequisite_process_list: List["Process"]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, prerequisite_process=new_prerequisite_process_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def condition(self) -> List[Any]:
-        """
-        List of condition present for this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
-        >>> my_process.condition = [my_condition]
-
-        Returns
-        -------
-        List[Condition]
-            list of condition for this process node
-        """
-        return self._json_attrs.condition.copy()
-
-    @condition.setter
-    @beartype
-    def condition(self, new_condition_list: List[Any]) -> None:
-        """
-        set the list of condition for this process
-
-        Parameters
-        ----------
-        new_condition_list: List[Condition]
-            replace the condition list
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, condition=new_condition_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def keyword(self) -> List[str]:
-        """
-        List of keyword for this process
-        [Process keyword](https://app.criptapp.org/vocab/process_keyword/) must come from CRIPT controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_process.keyword = ["self_assembly"]
-
-        Returns
-        -------
-        List[str]
-            list of keywords for this process nod
-        """
-        return self._json_attrs.keyword.copy()  # type: ignore
-
-    @keyword.setter
-    @beartype
-    def keyword(self, new_keyword_list: List[str]) -> None:
-        """
-        set the list of keyword for this process from CRIPT controlled vocabulary
-
-        Parameters
-        ----------
-        new_keyword_list: List[str]
-            replace the current list of keyword
-
-        Returns
-        -------
-        None
-        """
-        # TODO validate with CRIPT controlled vocabulary
-        new_attrs = replace(self._json_attrs, keyword=new_keyword_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Any]:
-        """
-        List of [citation](../subobjects/citation.md) for this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
-        >>> my_process.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of citation for this process node
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation_list: List[Any]) -> None:
-        """
-        set the list of citation for this process
-
-        Parameters
-        ----------
-        new_citation_list: List[Citation]
-            replace the current list of citation
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def property(self) -> List[Any]:
-        """
-        List of [Property nodes](../../subobjects/property) for this process
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
-        >>> my_process.property = [my_property]
-
-        Returns
-        -------
-        List[Property]
-            list of properties for this process
-        """
-        return self._json_attrs.property.copy()
-
-    @property.setter
-    @beartype
-    def property(self, new_property_list: List[Any]) -> None:
-        """
-        set the list of Property nodes for this process
-
-        Parameters
-        ----------
-        new_property_list: List[Property]
-            replace the current list of properties
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, property=new_property_list)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import Any, List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.util.json import UIDProxy
+
+
+class Process(PrimaryBaseNode):
+    """
+    ## Definition
+    The process node contains a list of [ingredients](../../subobjects/ingredient),
+    [quantities](../../subobjects/quantity), and procedure information for an experimental
+    [material](../material) transformation (chemical and physical).
+
+    ## Attributes
+
+    | attribute               | type             | example                                                                         | description                                                         | required | vocab |
+    |-------------------------|------------------|---------------------------------------------------------------------------------|---------------------------------------------------------------------|----------|-------|
+    | type                    | str              | mix                                                                             | type of process                                                     | True     | True  |
+    | ingredient              | list[Ingredient] |                                                                                 | ingredients                                                         |          |       |
+    | description             | str              | To oven-dried 20 mL glass vial, 5 mL of styrene and 10 ml of toluene was added. | explanation of the process                                          |          |       |
+    | equipment               | list[Equipment]  |                                                                                 | equipment used in the process                                       |          |       |
+    | product                 | list[Material]   |                                                                                 | desired material produced from the process                          |          |       |
+    | waste                   | list[Material]   |                                                                                 | material sent to waste                                              |          |       |
+    | prerequisite_ processes | list[Process]    |                                                                                 | processes that must be completed prior to the start of this process |          |       |
+    | condition               | list[Condition]  |                                                                                 | global process condition                                            |          |       |
+    | property                | list[Property]   |                                                                                 | process properties                                                  |          |       |
+    | keyword                 | list[str]        |                                                                                 | words that classify the process                                     |          | True  |
+    | citation                | list[Citation]   |                                                                                 | reference to a book, paper, or scholarly work                       |          |       |
+    | notes                   | str              |                                                                                 | miscellaneous information, or custom data structure                 |          |       |
+
+    ## Can be added to
+    * [Experiment](../experiment)
+
+    ## Available Subobjects
+    * [Ingredient](../../subobjects/ingredient)
+    * [Equipment](../../subobjects/equipment)
+    * [Property](../../subobjects/property)
+    * [Condition](../../subobjects/condition)
+    * [Citation](../../subobjects/citation)
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my minimal process name",
+       "node":["Process"],
+       "type":"affinity_pure",
+       "keyword":[],
+       "uid":"_:f8ef33f3-677a-40f3-b24e-65ab2c99d796",
+       "uuid":"f8ef33f3-677a-40f3-b24e-65ab2c99d796"
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all Process attributes
+        """
+
+        type: str = ""
+        # TODO add proper typing in future, using Any for now to avoid circular import error
+        ingredient: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        description: str = ""
+        equipment: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        product: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        waste: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        prerequisite_process: List[Union["Process", UIDProxy]] = field(default_factory=list)
+        condition: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        property: List[Union[Any, UIDProxy]] = field(default_factory=list)
+        keyword: List[str] = field(default_factory=list)
+        citation: List[Union[Any, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        name: str,
+        type: str,
+        ingredient: Optional[List[Union[Any, UIDProxy]]] = None,
+        description: str = "",
+        equipment: Optional[List[Union[Any, UIDProxy]]] = None,
+        product: Optional[List[Union[Any, UIDProxy]]] = None,
+        waste: Optional[List[Union[Any, UIDProxy]]] = None,
+        prerequisite_process: Optional[List[Union["Process", UIDProxy]]] = None,
+        condition: Optional[List[Union[Any, UIDProxy]]] = None,
+        property: Optional[List[Union[Any, UIDProxy]]] = None,
+        keyword: Optional[List[str]] = None,
+        citation: Optional[List[Union[Any, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ) -> None:
+        """
+        create a process node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+
+        Parameters
+        ----------
+        ingredient: List[Ingredient]
+            [ingredient](../../subobjects/ingredient) used in this process
+        type: str = ""
+            Process type must come from
+            [CRIPT Controlled vocabulary process type](https://app.criptapp.org/vocab/process_type/)
+        description: str = ""
+            description of this process
+        equipment: List[Equipment] = None
+            list of [equipment](../../subobjects/equipment) used in this process
+        product: List[Material] = None
+            product that this process created
+        waste: List[Material] = None
+            waste that this process created
+        condition: List[Condition] = None
+            list of [condition](../../subobjects/condition) that this process was created under
+        property: List[Property] = None
+            list of [properties](../../subobjects/property) for this process
+        keyword: List[str] = None
+            list of keywords for this process must come from
+            [CRIPT process keyword controlled keyword](https://app.criptapp.org/vocab/process_keyword/)
+        citation: List[Citation] = None
+            list of [citation](../../subobjects/citation)
+
+        Returns
+        -------
+        None
+            instantiate a process node
+        """
+
+        if ingredient is None:
+            ingredient = []
+
+        if equipment is None:
+            equipment = []
+
+        if product is None:
+            product = []
+
+        if waste is None:
+            waste = []
+
+        if prerequisite_process is None:
+            prerequisite_process = []
+
+        if condition is None:
+            condition = []
+
+        if property is None:
+            property = []
+
+        if keyword is None:
+            keyword = []
+
+        if citation is None:
+            citation = []
+
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        new_attrs = replace(
+            self._json_attrs,
+            ingredient=ingredient,
+            type=type,
+            description=description,
+            equipment=equipment,
+            product=product,
+            waste=waste,
+            condition=condition,
+            prerequisite_process=prerequisite_process,
+            property=property,
+            keyword=keyword,
+            citation=citation,
+        )
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        [Process type](https://app.criptapp.org/vocab/process_type) must come from the CRIPT controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_process.type = "affinity_pure"
+
+        Returns
+        -------
+        str
+            Select a [Process type](https://app.criptapp.org/vocab/process_type/) from CRIPT controlled vocabulary
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_process_type: str) -> None:
+        """
+        set process type from CRIPT controlled vocabulary
+
+        Parameters
+        ----------
+        new_process_type: str
+            new process type from CRIPT controlled vocabulary
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_process_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def ingredient(self) -> List[Any]:
+        """
+        List of [ingredient](../../subobjects/ingredient) for this process
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_material = cript.Material(name="my material", bigsmiles = "material bigsmiles")
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_ingredient = cript.Ingredient(
+        ...     material=my_material, quantity=[my_quantity], keyword=["catalyst"]
+        ... )
+        >>> my_process.ingredient = [my_ingredient]
+
+        Returns
+        -------
+        List[Ingredient]
+            list of ingredients for this process
+        """
+        return self._json_attrs.ingredient.copy()
+
+    @ingredient.setter
+    @beartype
+    def ingredient(self, new_ingredient_list: List[Any]) -> None:
+        """
+        set the list of the ingredients for this process
+
+        Parameters
+        ----------
+        new_ingredient_list
+            list of ingredients to replace the current list
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, ingredient=new_ingredient_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def description(self) -> str:
+        """
+        description of this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_process.description = "To oven-dried 20 mL glass vial, 5 mL of styrene and 10 ml of toluene was added"
+
+        Returns
+        -------
+        str
+            description of this process
+        """
+        return self._json_attrs.description
+
+    @description.setter
+    @beartype
+    def description(self, new_description: str) -> None:
+        """
+        set the description of this process
+
+        Parameters
+        ----------
+        new_description: str
+            new process description to replace the current one
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, description=new_description)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def equipment(self) -> List[Any]:
+        """
+        List of [equipment](../../subobjects/equipment) used for this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_equipment = cript.Equipment(key="burner")
+        >>> my_process.equipment = [my_equipment]
+
+        Returns
+        -------
+        List[Equipment]
+            list of equipment used for this process
+        """
+        return self._json_attrs.equipment.copy()
+
+    @equipment.setter
+    @beartype
+    def equipment(self, new_equipment_list: List[Any]) -> None:
+        """
+        set the list of equipment used for this process
+
+        Parameters
+        ----------
+        new_equipment_list
+            new equipment list to replace the current equipment list for this process
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, equipment=new_equipment_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def product(self) -> List[Any]:
+        """
+        List of product (material nodes) for this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_product_material = cript.Material(
+        ...     name="my product material",
+        ...     amino_acid = "my material product amino_acid",
+        ... )
+        >>> my_process.product = [my_product_material]
+
+        Returns
+        -------
+        List[Material]
+            List of process product (Material nodes)
+        """
+        return self._json_attrs.product.copy()
+
+    @product.setter
+    @beartype
+    def product(self, new_product_list: List[Any]) -> None:
+        """
+        set the product list for this process
+
+        Parameters
+        ----------
+        new_product_list: List[Material]
+            replace the current list of process product
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, product=new_product_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def waste(self) -> List[Any]:
+        """
+        List of waste that resulted from this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_waste_material = cript.Material(
+        ...     name="my waste material",
+        ...     bigsmiles = "123456",
+        ... )
+        >>> my_process.waste = [my_waste_material]
+
+        Returns
+        -------
+        List[Material]
+            list of waste materials that resulted from this product
+        """
+        return self._json_attrs.waste.copy()
+
+    @waste.setter
+    @beartype
+    def waste(self, new_waste_list: List[Any]) -> None:
+        """
+        set the list of waste (Material node) for that resulted from this process
+
+        Parameters
+        ----------
+        new_waste_list: List[Material]
+            replace the list waste that resulted from this process
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, waste=new_waste_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def prerequisite_process(self) -> List[Union["Process", UIDProxy]]:
+        """
+        list of prerequisite process nodes
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_prerequisite_process = [
+        ...     cript.Process(name="prerequisite processes 1", type="blow_molding"),
+        ...     cript.Process(name="prerequisite processes 2", type="centrifugation"),
+        ... ]
+        >>> my_process.prerequisite_process = my_prerequisite_process
+
+        Returns
+        -------
+        List[Process]
+            list of process that had to happen before this process
+        """
+        return self._json_attrs.prerequisite_process.copy()
+
+    @prerequisite_process.setter
+    @beartype
+    def prerequisite_process(self, new_prerequisite_process_list: List[Union["Process", UIDProxy]]) -> None:
+        """
+        set the prerequisite_process for the process node
+
+        Parameters
+        ----------
+        new_prerequisite_process_list: List["Process"]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, prerequisite_process=new_prerequisite_process_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def condition(self) -> List[Any]:
+        """
+        List of condition present for this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_condition = cript.Condition(key="atm", type="min", value=1)
+        >>> my_process.condition = [my_condition]
+
+        Returns
+        -------
+        List[Condition]
+            list of condition for this process node
+        """
+        return self._json_attrs.condition.copy()
+
+    @condition.setter
+    @beartype
+    def condition(self, new_condition_list: List[Any]) -> None:
+        """
+        set the list of condition for this process
+
+        Parameters
+        ----------
+        new_condition_list: List[Condition]
+            replace the condition list
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, condition=new_condition_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def keyword(self) -> List[str]:
+        """
+        List of keyword for this process
+        [Process keyword](https://app.criptapp.org/vocab/process_keyword/) must come from CRIPT controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_process.keyword = ["self_assembly"]
+
+        Returns
+        -------
+        List[str]
+            list of keywords for this process nod
+        """
+        return self._json_attrs.keyword.copy()  # type: ignore
+
+    @keyword.setter
+    @beartype
+    def keyword(self, new_keyword_list: List[str]) -> None:
+        """
+        set the list of keyword for this process from CRIPT controlled vocabulary
+
+        Parameters
+        ----------
+        new_keyword_list: List[str]
+            replace the current list of keyword
+
+        Returns
+        -------
+        None
+        """
+        # TODO validate with CRIPT controlled vocabulary
+        new_attrs = replace(self._json_attrs, keyword=new_keyword_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Any]:
+        """
+        List of [citation](../subobjects/citation.md) for this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_citation = cript.Citation(type="derived_from", reference=my_reference)
+        >>> my_process.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of citation for this process node
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation_list: List[Any]) -> None:
+        """
+        set the list of citation for this process
+
+        Parameters
+        ----------
+        new_citation_list: List[Citation]
+            replace the current list of citation
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def property(self) -> List[Any]:
+        """
+        List of [Property nodes](../../subobjects/property) for this process
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_property = cript.Property(key="modulus_shear", type="min", value=1.23, unit="gram")
+        >>> my_process.property = [my_property]
+
+        Returns
+        -------
+        List[Property]
+            list of properties for this process
+        """
+        return self._json_attrs.property.copy()
+
+    @property.setter
+    @beartype
+    def property(self, new_property_list: List[Any]) -> None:
+        """
+        set the list of Property nodes for this process
+
+        Parameters
+        ----------
+        new_property_list: List[Property]
+            replace the current list of properties
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, property=new_property_list)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/project.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,235 +1,233 @@
-from dataclasses import dataclass, field, replace
-from typing import List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.collection import Collection
-from cript.nodes.primary_nodes.material import Material
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-from cript.nodes.supporting_nodes import User
-
-
-class Project(PrimaryBaseNode):
-    """
-    ## Definition
-    A [Project](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=7)
-    is the highest level node that is Not nested inside any other node.
-    A Project can be thought of as a folder that can contain [Collections](../collection) and
-    [Materials](../material).
-
-
-    | attribute  | type             | description                                         |
-    |------------|------------------|-----------------------------------------------------|
-    | collection | List[Collection] | collections that relate to the project              |
-    | materials  | List[Materials]  | materials owned by the project                      |
-    | notes      | str              | miscellaneous information, or custom data structure |
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"my project name",
-       "node":["Project"],
-       "uid":"_:270168b7-fc29-4c37-aa93-334212e1d962",
-       "uuid":"270168b7-fc29-4c37-aa93-334212e1d962",
-       "collection":[
-          {
-            "name":"my collection name",
-             "node":["Collection"],
-             "uid":"_:c60955a5-4de0-4da5-b2c8-77952b1d9bfa",
-             "uuid":"c60955a5-4de0-4da5-b2c8-77952b1d9bfa",
-             "experiment":[
-                {
-                   "name":"my experiment name",
-                   "node":["Experiment"],
-                   "uid":"_:a8cbc083-506e-45ce-bb8f-5e50917ab361",
-                   "uuid":"a8cbc083-506e-45ce-bb8f-5e50917ab361"
-                }
-             ],
-             "inventory":[],
-             "citation":[]
-          }
-       ]
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all Project attributes
-        """
-
-        member: List[User] = field(default_factory=list)
-        admin: List[User] = field(default_factory=list)
-        collection: List[Collection] = field(default_factory=list)
-        material: List[Material] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, collection: Optional[List[Collection]] = None, material: Optional[List[Material]] = None, notes: str = "", **kwargs):
-        """
-        Create a Project node with Project name
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_project = cript.Project(name="my Project name")
-
-
-        Parameters
-        ----------
-        name: str
-            project name
-        collection: List[Collection]
-            list of Collections that belongs to this Project
-         material: List[Material]
-            list of materials that belongs to this project
-        notes: str
-            notes for this project
-
-        Returns
-        -------
-        None
-            instantiate a Project node
-        """
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        if collection is None:
-            collection = []
-
-        if material is None:
-            material = []
-
-        self._json_attrs = replace(self._json_attrs, name=name, collection=collection, material=material)
-        self.validate()
-
-    def validate(self, api=None, is_patch=False, force_validation: bool = False):
-        from cript.nodes.exceptions import (
-            CRIPTOrphanedMaterialError,
-            get_orphaned_experiment_exception,
-        )
-
-        # First validate like other nodes
-        super().validate(api=api, is_patch=is_patch, force_validation=force_validation)
-
-        # Check graph for orphaned nodes, that should be listed in project
-        # Project.materials should contain all material nodes
-        project_graph_materials = self.find_children({"node": ["Material"]})
-        # Combine all materials listed in the project inventories
-        project_inventory_materials = []
-        for inventory in self.find_children({"node": ["Inventory"]}):
-            for material in inventory.material:
-                project_inventory_materials.append(material)
-        for material in project_graph_materials:
-            if material not in self.material and material not in project_inventory_materials:
-                raise CRIPTOrphanedMaterialError(material)
-
-        # Check graph for orphaned nodes, that should be listed in the experiments
-        project_experiments = self.find_children({"node": ["Experiment"]})
-        # There are 4 different types of nodes Experiments are collecting.
-        node_types = ("Process", "Computation", "ComputationProcess", "Data")
-        # We loop over them with the same logic
-        for node_type in node_types:
-            # All in the graph has to be in at least one experiment
-            project_graph_nodes = self.find_children({"node": [node_type]})
-            node_type_attr = node_type.lower()
-            # Non-consistent naming makes this necessary for Computation Process
-            if node_type == "ComputationProcess":
-                node_type_attr = "computation_process"
-
-            # Concatenation of all experiment attributes (process, computation, etc.)
-            # Every node of the graph must be present somewhere in this concatenated list.
-            experiment_nodes = []
-            for experiment in project_experiments:
-                for ex_node in getattr(experiment, node_type_attr):
-                    experiment_nodes.append(ex_node)
-            for node in project_graph_nodes:
-                if node not in experiment_nodes:
-                    raise get_orphaned_experiment_exception(node)
-
-    @property
-    @beartype
-    def member(self) -> List[User]:
-        return self._json_attrs.member.copy()
-
-    @property
-    @beartype
-    def admin(self) -> List[User]:
-        return self._json_attrs.admin
-
-    @property
-    @beartype
-    def collection(self) -> List[Collection]:
-        """
-        Collection is a Project node's property that can be set during creation in the constructor
-        or later by setting the project's property
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_project = cript.Project(name="my Project name")
-        >>> my_new_collection = cript.Collection(name="my collection name")
-        >>> my_project.collection = [my_new_collection]
-
-        Returns
-        -------
-        Collection: List[Collection]
-            the list of collections within this project
-        """
-        return self._json_attrs.collection
-
-    @collection.setter
-    @beartype
-    def collection(self, new_collection: List[Collection]) -> None:
-        """
-        set list of collections for the project node
-
-        Parameters
-        ----------
-        new_collection: List[Collection]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, collection=new_collection)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def material(self) -> List[Material]:
-        """
-        List of Materials that belong to this Project.
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_project = cript.Project(name="my Project name")
-        >>> identifier = [{"bigsmiles": "my big smiles"}]
-        >>> my_material = cript.Material(name="my material", identifier=identifier)
-        >>> my_project.material = [my_material]
-
-        Returns
-        -------
-        Material: List[Material]
-            List of materials that belongs to this project
-        """
-        return self._json_attrs.material
-
-    @material.setter
-    @beartype
-    def material(self, new_materials: List[Material]) -> None:
-        """
-        set the list of materials for this project
-
-        Parameters
-        ----------
-        new_materials: List[Material]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, material=new_materials)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.collection import Collection
+from cript.nodes.primary_nodes.material import Material
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+from cript.nodes.supporting_nodes import User
+from cript.nodes.util.json import UIDProxy
+
+
+class Project(PrimaryBaseNode):
+    """
+    ## Definition
+    A [Project](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=7)
+    is the highest level node that is Not nested inside any other node.
+    A Project can be thought of as a folder that can contain [Collections](../collection) and
+    [Materials](../material).
+
+
+    | attribute  | type             | description                                         |
+    |------------|------------------|-----------------------------------------------------|
+    | collection | List[Collection] | collections that relate to the project              |
+    | materials  | List[Materials]  | materials owned by the project                      |
+    | notes      | str              | miscellaneous information, or custom data structure |
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"my project name",
+       "node":["Project"],
+       "uid":"_:270168b7-fc29-4c37-aa93-334212e1d962",
+       "uuid":"270168b7-fc29-4c37-aa93-334212e1d962",
+       "collection":[
+          {
+            "name":"my collection name",
+             "node":["Collection"],
+             "uid":"_:c60955a5-4de0-4da5-b2c8-77952b1d9bfa",
+             "uuid":"c60955a5-4de0-4da5-b2c8-77952b1d9bfa",
+             "experiment":[
+                {
+                   "name":"my experiment name",
+                   "node":["Experiment"],
+                   "uid":"_:a8cbc083-506e-45ce-bb8f-5e50917ab361",
+                   "uuid":"a8cbc083-506e-45ce-bb8f-5e50917ab361"
+                }
+             ],
+             "inventory":[],
+             "citation":[]
+          }
+       ]
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all Project attributes
+        """
+
+        member: List[Union[User, UIDProxy]] = field(default_factory=list)
+        admin: List[Union[User, UIDProxy]] = field(default_factory=list)
+        collection: List[Union[Collection, UIDProxy]] = field(default_factory=list)
+        material: List[Union[Material, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, name: str, collection: Optional[List[Union[Collection, UIDProxy]]] = None, material: Optional[List[Union[Material, UIDProxy]]] = None, notes: str = "", **kwargs):
+        """
+        Create a Project node with Project name
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_project = cript.Project(name="my Project name")
+
+
+        Parameters
+        ----------
+        name: str
+            project name
+        collection: List[Collection]
+            list of Collections that belongs to this Project
+         material: List[Material]
+            list of materials that belongs to this project
+        notes: str
+            notes for this project
+
+        Returns
+        -------
+        None
+            instantiate a Project node
+        """
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        if collection is None:
+            collection = []
+
+        if material is None:
+            material = []
+
+        new_json_attrs = replace(self._json_attrs, name=name, collection=collection, material=material)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    def validate(self, api=None, is_patch=False, force_validation: bool = False):
+        from cript.nodes.exceptions import CRIPTOrphanedMaterialError
+        from cript.nodes.util.core import get_orphaned_experiment_exception
+
+        # First validate like other nodes
+        super().validate(api=api, is_patch=is_patch, force_validation=force_validation)
+
+        # Check graph for orphaned nodes, that should be listed in project
+        # Project.materials should contain all material nodes
+        project_graph_materials = self.find_children({"node": ["Material"]})
+        # Combine all materials listed in the project inventories
+        project_inventory_materials = []
+        for inventory in self.find_children({"node": ["Inventory"]}):
+            for material in inventory.material:
+                project_inventory_materials.append(material)
+        for material in project_graph_materials:
+            if material not in self.material and material not in project_inventory_materials:
+                raise CRIPTOrphanedMaterialError(material)
+
+        # Check graph for orphaned nodes, that should be listed in the experiments
+        project_experiments = self.find_children({"node": ["Experiment"]})
+        # There are 4 different types of nodes Experiments are collecting.
+        node_types = ("Process", "Computation", "ComputationProcess", "Data")
+        # We loop over them with the same logic
+        for node_type in node_types:
+            # All in the graph has to be in at least one experiment
+            project_graph_nodes = self.find_children({"node": [node_type]})
+            node_type_attr = node_type.lower()
+            # Non-consistent naming makes this necessary for Computation Process
+            if node_type == "ComputationProcess":
+                node_type_attr = "computation_process"
+
+            # Concatenation of all experiment attributes (process, computation, etc.)
+            # Every node of the graph must be present somewhere in this concatenated list.
+            experiment_nodes = []
+            for experiment in project_experiments:
+                for ex_node in getattr(experiment, node_type_attr):
+                    experiment_nodes.append(ex_node)
+            for node in project_graph_nodes:
+                if node not in experiment_nodes:
+                    raise get_orphaned_experiment_exception(node)
+
+    @property
+    @beartype
+    def member(self) -> List[Union[User, UIDProxy]]:
+        return self._json_attrs.member.copy()
+
+    @property
+    @beartype
+    def admin(self) -> List[Union[User, UIDProxy]]:
+        return self._json_attrs.admin
+
+    @property
+    @beartype
+    def collection(self) -> List[Union[Collection, UIDProxy]]:
+        """
+        Collection is a Project node's property that can be set during creation in the constructor
+        or later by setting the project's property
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_project = cript.Project(name="my Project name")
+        >>> my_new_collection = cript.Collection(name="my collection name")
+        >>> my_project.collection = [my_new_collection]
+
+        Returns
+        -------
+        Collection: List[Collection]
+            the list of collections within this project
+        """
+        return self._json_attrs.collection
+
+    @collection.setter
+    @beartype
+    def collection(self, new_collection: List[Union[Collection, UIDProxy]]) -> None:
+        """
+        set list of collections for the project node
+
+        Parameters
+        ----------
+        new_collection: List[Collection]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, collection=new_collection)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def material(self) -> List[Union[Material, UIDProxy]]:
+        """
+        List of Materials that belong to this Project.
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_project = cript.Project(name="my Project name")
+        >>> my_material = cript.Material(name="my material", bigsmiles="my bigsmiles")
+        >>> my_project.material = [my_material]
+
+        Returns
+        -------
+        Material: List[Material]
+            List of materials that belongs to this project
+        """
+        return self._json_attrs.material
+
+    @material.setter
+    @beartype
+    def material(self, new_materials: List[Union[Material, UIDProxy]]) -> None:
+        """
+        set the list of materials for this project
+
+        Parameters
+        ----------
+        new_materials: List[Material]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, material=new_materials)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/primary_nodes/reference.py` & `cript-2.3.0/src/cript/nodes/primary_nodes/reference.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,686 +1,685 @@
-from dataclasses import dataclass, field, replace
-from typing import List, Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Reference(UUIDBaseNode):
-    """
-    ## Definition
-
-    The
-    [Reference node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=15)
-    contains the metadata for a literature publication, book, or anything external to CRIPT.
-    The reference node does NOT contain the base attributes.
-
-    The reference node is always used inside the citation
-    sub-object to enable users to specify the context of the reference.
-
-    ## Attributes
-    | attribute | type      | example                                    | description                                   | required      | vocab |
-    |-----------|-----------|--------------------------------------------|-----------------------------------------------|---------------|-------|
-    | type      | str       | journal_article                            | type of literature                            | True          | True  |
-    | title     | str       | 'Living' Polymers                          | title of publication                          | True          |       |
-    | author    | list[str] | Michael Szwarc                             | list of authors                               |               |       |
-    | journal   | str       | Nature                                     | journal of the publication                    |               |       |
-    | publisher | str       | Springer                                   | publisher of publication                      |               |       |
-    | year      | int       | 1956                                       | year of publication                           |               |       |
-    | volume    | int       | 178                                        | volume of publication                         |               |       |
-    | issue     | int       | 0                                          | issue of publication                          |               |       |
-    | pages     | list[int] | [1168, 1169]                               | page range of publication                     |               |       |
-    | doi       | str       | 10.1038/1781168a0                          | DOI: digital object identifier                | Conditionally |       |
-    | issn      | str       | 1476-4687                                  | ISSN: international standard serial number    | Conditionally |       |
-    | arxiv_id  | str       | 1501                                       | arXiv identifier                              |               |       |
-    | pmid      | int       | ########                                   | PMID: PubMed ID                               |               |       |
-    | website   | str       | https://www.nature.com/artic les/1781168a0 | website where the publication can be accessed |               |       |
-
-
-    ## Can be added to
-    * [Citation](../../subobjects/citation)
-
-    ## Available Subobjects
-    * None
-
-    !!! warning "Reference will always be public"
-        Reference node is meant to always be public and static to allow globally link data to the reference
-
-    ## JSON Representation
-    ```json
-    {
-       "node":["Reference"],
-       "uid":"_:c681a947-0554-4acd-a01c-06ad76e34b87",
-       "uuid":"c681a947-0554-4acd-a01c-06ad76e34b87",
-       "author":["Ludwig Schneider","Marcus Müller"],
-       "doi":"10.1016/j.cpc.2018.08.011",
-       "issn":"0010-4655",
-       "journal":"Computer Physics Communications",
-       "pages":[463,476],
-       "publisher":"Elsevier",
-       "title":"Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
-       "type":"journal_article",
-       "website":"https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-       "year":2019
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        """
-        all reference nodes attributes
-
-        all int types are also None type in case they are not present it should be properly shown as None
-        instead of a placeholder number such as 0 or -1
-        """
-
-        type: str = ""
-        title: str = ""
-        author: List[str] = field(default_factory=list)
-        journal: str = ""
-        publisher: str = ""
-        year: Optional[int] = None
-        volume: Optional[int] = None
-        issue: Optional[int] = None
-        pages: List[int] = field(default_factory=list)
-        doi: str = ""
-        issn: str = ""
-        arxiv_id: str = ""
-        pmid: Optional[int] = None
-        website: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        type: str,
-        title: str,
-        author: Optional[List[str]] = None,
-        journal: str = "",
-        publisher: str = "",
-        year: Optional[int] = None,
-        volume: Optional[int] = None,
-        issue: Optional[int] = None,
-        pages: Optional[List[int]] = None,
-        doi: str = "",
-        issn: str = "",
-        arxiv_id: str = "",
-        pmid: Optional[int] = None,
-        website: str = "",
-        **kwargs,
-    ):
-        """
-        create a reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-
-        Parameters
-        ----------
-        type: str
-            type of literature.
-            The [reference type](https://app.criptapp.org/vocab/reference_type/)
-            must come from CRIPT controlled vocabulary
-        title: str
-            title of publication
-        author: List[str] default=""
-            list of authors
-        journal: str default=""
-            journal of publication
-        publisher: str default=""
-            publisher of publication
-        year: int default=None
-            year of publication
-        volume: int default=None
-            volume of publication
-        issue: int default=None
-            issue of publication
-        pages: List[int] default=None
-            page range of publication
-        doi: str default=""
-            DOI: digital object identifier
-        issn: str default=""
-            ISSN: international standard serial number
-        arxiv_id: str default=""
-            arXiv identifier
-        pmid: int default=None
-            PMID: PubMed ID
-        website: str default=""
-            website where the publication can be accessed
-
-        Returns
-        -------
-        None
-            Instantiate a reference node
-        """
-        if author is None:
-            author = []
-
-        if pages is None:
-            pages = []
-
-        super().__init__(**kwargs)
-
-        new_attrs = replace(self._json_attrs, type=type, title=title, author=author, journal=journal, publisher=publisher, year=year, volume=volume, issue=issue, pages=pages, doi=doi, issn=issn, arxiv_id=arxiv_id, pmid=pmid, website=website)
-
-        self._update_json_attrs_if_valid(new_attrs)
-        self.validate()
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        Type of reference.
-
-        The [reference type](https://app.criptapp.org/vocab/reference_type)
-        must come from the CRIPT controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.type = "web_site"
-
-        Returns
-        -------
-        str
-            reference type
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_reference_type: str) -> None:
-        """
-        set the reference type attribute
-
-        reference type must come from the CRIPT controlled vocabulary
-
-        Parameters
-        ----------
-        new_reference_type: str
-
-        Returns
-        -------
-        None
-        """
-        # TODO validate the reference type with CRIPT controlled vocabulary
-        new_attrs = replace(self._json_attrs, type=new_reference_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def title(self) -> str:
-        """
-        title of publication
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.title = "my new title"
-
-        Returns
-        -------
-        str
-            title of publication
-        """
-        return self._json_attrs.title
-
-    @title.setter
-    @beartype
-    def title(self, new_title: str) -> None:
-        """
-        set the title for the reference node
-
-        Parameters
-        ----------
-        new_title: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, title=new_title)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def author(self) -> List[str]:
-        """
-        List of authors for this reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.author += ["Navid Hariri"]
-
-        Returns
-        -------
-        List[str]
-            list of authors
-        """
-        return self._json_attrs.author.copy()
-
-    @author.setter
-    @beartype
-    def author(self, new_author: List[str]) -> None:
-        """
-        set the list of authors for the reference node
-
-        Parameters
-        ----------
-        new_author: List[str]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, author=new_author)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def journal(self) -> str:
-        """
-        journal of publication
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.journal = "my new journal"
-
-        Returns
-        -------
-        str
-            journal of publication
-        """
-        return self._json_attrs.journal
-
-    @journal.setter
-    @beartype
-    def journal(self, new_journal: str) -> None:
-        """
-        set the journal attribute for this reference node
-
-        Parameters
-        ----------
-        new_journal: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, journal=new_journal)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def publisher(self) -> str:
-        """
-        publisher for this reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.publisher = "my new publisher"
-
-        Returns
-        -------
-        str
-            publisher of this publication
-        """
-        return self._json_attrs.publisher
-
-    @publisher.setter
-    @beartype
-    def publisher(self, new_publisher: str) -> None:
-        """
-        set the publisher for this reference node
-
-        Parameters
-        ----------
-        new_publisher: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, publisher=new_publisher)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def year(self) -> Union[int, None]:
-        """
-        year for the scholarly work
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.year = 2023
-
-        Returns
-        -------
-        int
-        """
-        return self._json_attrs.year
-
-    @year.setter
-    @beartype
-    def year(self, new_year: Union[int, None]) -> None:
-        """
-        set the year for the scholarly work within the reference node
-
-        Parameters
-        ----------
-        new_year: int
-
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, year=new_year)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def volume(self) -> Union[int, None]:
-        """
-        Volume of the scholarly work from the reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.volume = 1
-
-        Returns
-        -------
-        int
-            volume number of the publishing
-        """
-        return self._json_attrs.volume
-
-    @volume.setter
-    @beartype
-    def volume(self, new_volume: Union[int, None]) -> None:
-        """
-        set the volume of the scholarly work for this reference node
-
-        Parameters
-        ----------
-        new_volume: int
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, volume=new_volume)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def issue(self) -> Union[int, None]:
-        """
-        issue of the scholarly work for the reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.issue = 2
-
-        Returns
-        -------
-        None
-        """
-        return self._json_attrs.issue
-
-    @issue.setter
-    @beartype
-    def issue(self, new_issue: Union[int, None]) -> None:
-        """
-        set the issue of the scholarly work
-
-        Parameters
-        ----------
-        new_issue: int
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, issue=new_issue)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def pages(self) -> List[int]:
-        """
-        pages of the scholarly work used in the reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.pages = [123, 456]
-
-        Returns
-        -------
-        int
-        """
-        return self._json_attrs.pages.copy()
-
-    @pages.setter
-    @beartype
-    def pages(self, new_pages_list: List[int]) -> None:
-        """
-        set the list of pages of the scholarly work for this reference node
-
-        Parameters
-        ----------
-        new_pages_list: List[int]
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, pages=new_pages_list)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def doi(self) -> str:
-        """
-        get the digital object identifier (DOI) for this reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.doi = "100.1038/1781168a0"
-
-        Returns
-        -------
-        str
-            digital object identifier (DOI) for this reference node
-        """
-        return self._json_attrs.doi
-
-    @doi.setter
-    @beartype
-    def doi(self, new_doi: str) -> None:
-        """
-        set the digital object identifier (DOI) for the scholarly work for this reference node
-
-        Parameters
-        ----------
-        new_doi: str
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.doi = "100.1038/1781168a0"
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, doi=new_doi)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def issn(self) -> str:
-        """
-        The international standard serial number (ISSN) for this reference node
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.issn = "1456-4687"
-
-        Returns
-        -------
-        str
-            ISSN for this reference node
-        """
-        return self._json_attrs.issn
-
-    @issn.setter
-    @beartype
-    def issn(self, new_issn: str) -> None:
-        """
-        set the international standard serial number (ISSN) for the scholarly work for this reference node
-
-        Parameters
-        ----------
-        new_issn: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, issn=new_issn)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def arxiv_id(self) -> str:
-        """
-        The arXiv identifier for the scholarly work for this reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.arxiv_id = "1501"
-
-        Returns
-        -------
-        str
-            arXiv identifier for the scholarly work for this publishing
-        """
-        return self._json_attrs.arxiv_id
-
-    @arxiv_id.setter
-    @beartype
-    def arxiv_id(self, new_arxiv_id: str) -> None:
-        """
-        set the arXiv identifier for the scholarly work for this reference node
-
-        Parameters
-        ----------
-        new_arxiv_id: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, arxiv_id=new_arxiv_id)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def pmid(self) -> Union[int, None]:
-        """
-        The PubMed ID (PMID) for this reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.pmid = 12345678
-
-        Returns
-        -------
-        int
-            the PubMedID of this publishing
-        """
-        return self._json_attrs.pmid
-
-    @pmid.setter
-    @beartype
-    def pmid(self, new_pmid: Union[int, None]) -> None:
-        """
-
-        Parameters
-        ----------
-        new_pmid
-
-        Returns
-        -------
-
-        """
-        # TODO can possibly add validations, possibly in forms of length checking
-        #  to be sure its the correct length
-        new_attrs = replace(self._json_attrs, pmid=new_pmid)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def website(self) -> str:
-        """
-        The website URL for the scholarly work
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
-        >>> my_reference.website = "https://criptapp.org"
-
-        Returns
-        -------
-        str
-            the website URL of this publishing
-        """
-        return self._json_attrs.website
-
-    @website.setter
-    @beartype
-    def website(self, new_website: str) -> None:
-        """
-        set the website URL for the scholarly work
-
-        Parameters
-        ----------
-        new_website: str
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, website=new_website)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Reference(UUIDBaseNode):
+    """
+    ## Definition
+
+    The
+    [Reference node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=15)
+    contains the metadata for a literature publication, book, or anything external to CRIPT.
+    The reference node does NOT contain the base attributes.
+
+    The reference node is always used inside the citation
+    sub-object to enable users to specify the context of the reference.
+
+    ## Attributes
+    | attribute | type      | example                                    | description                                   | required      | vocab |
+    |-----------|-----------|--------------------------------------------|-----------------------------------------------|---------------|-------|
+    | type      | str       | journal_article                            | type of literature                            | True          | True  |
+    | title     | str       | 'Living' Polymers                          | title of publication                          | True          |       |
+    | author    | list[str] | Michael Szwarc                             | list of authors                               |               |       |
+    | journal   | str       | Nature                                     | journal of the publication                    |               |       |
+    | publisher | str       | Springer                                   | publisher of publication                      |               |       |
+    | year      | int       | 1956                                       | year of publication                           |               |       |
+    | volume    | int       | 178                                        | volume of publication                         |               |       |
+    | issue     | int       | 0                                          | issue of publication                          |               |       |
+    | pages     | list[int] | [1168, 1169]                               | page range of publication                     |               |       |
+    | doi       | str       | 10.1038/1781168a0                          | DOI: digital object identifier                | Conditionally |       |
+    | issn      | str       | 1476-4687                                  | ISSN: international standard serial number    | Conditionally |       |
+    | arxiv_id  | str       | 1501                                       | arXiv identifier                              |               |       |
+    | pmid      | int       | ########                                   | PMID: PubMed ID                               |               |       |
+    | website   | str       | https://www.nature.com/artic les/1781168a0 | website where the publication can be accessed |               |       |
+
+
+    ## Can be added to
+    * [Citation](../../subobjects/citation)
+
+    ## Available Subobjects
+    * None
+
+    !!! warning "Reference will always be public"
+        Reference node is meant to always be public and static to allow globally link data to the reference
+
+    ## JSON Representation
+    ```json
+    {
+       "node":["Reference"],
+       "uid":"_:c681a947-0554-4acd-a01c-06ad76e34b87",
+       "uuid":"c681a947-0554-4acd-a01c-06ad76e34b87",
+       "author":["Ludwig Schneider","Marcus Müller"],
+       "doi":"10.1016/j.cpc.2018.08.011",
+       "issn":"0010-4655",
+       "journal":"Computer Physics Communications",
+       "pages":[463,476],
+       "publisher":"Elsevier",
+       "title":"Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
+       "type":"journal_article",
+       "website":"https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+       "year":2019
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        """
+        all reference nodes attributes
+
+        all int types are also None type in case they are not present it should be properly shown as None
+        instead of a placeholder number such as 0 or -1
+        """
+
+        type: str = ""
+        title: str = ""
+        author: List[str] = field(default_factory=list)
+        journal: str = ""
+        publisher: str = ""
+        year: Optional[int] = None
+        volume: Optional[int] = None
+        issue: Optional[int] = None
+        pages: List[int] = field(default_factory=list)
+        doi: str = ""
+        issn: str = ""
+        arxiv_id: str = ""
+        pmid: Optional[int] = None
+        website: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        type: str,
+        title: str,
+        author: Optional[List[str]] = None,
+        journal: str = "",
+        publisher: str = "",
+        year: Optional[int] = None,
+        volume: Optional[int] = None,
+        issue: Optional[int] = None,
+        pages: Optional[List[int]] = None,
+        doi: str = "",
+        issn: str = "",
+        arxiv_id: str = "",
+        pmid: Optional[int] = None,
+        website: str = "",
+        **kwargs,
+    ):
+        """
+        create a reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+
+        Parameters
+        ----------
+        type: str
+            type of literature.
+            The [reference type](https://app.criptapp.org/vocab/reference_type/)
+            must come from CRIPT controlled vocabulary
+        title: str
+            title of publication
+        author: List[str] default=""
+            list of authors
+        journal: str default=""
+            journal of publication
+        publisher: str default=""
+            publisher of publication
+        year: int default=None
+            year of publication
+        volume: int default=None
+            volume of publication
+        issue: int default=None
+            issue of publication
+        pages: List[int] default=None
+            page range of publication
+        doi: str default=""
+            DOI: digital object identifier
+        issn: str default=""
+            ISSN: international standard serial number
+        arxiv_id: str default=""
+            arXiv identifier
+        pmid: int default=None
+            PMID: PubMed ID
+        website: str default=""
+            website where the publication can be accessed
+
+        Returns
+        -------
+        None
+            Instantiate a reference node
+        """
+        if author is None:
+            author = []
+
+        if pages is None:
+            pages = []
+
+        super().__init__(**kwargs)
+
+        new_attrs = replace(self._json_attrs, type=type, title=title, author=author, journal=journal, publisher=publisher, year=year, volume=volume, issue=issue, pages=pages, doi=doi, issn=issn, arxiv_id=arxiv_id, pmid=pmid, website=website)
+
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        Type of reference.
+
+        The [reference type](https://app.criptapp.org/vocab/reference_type)
+        must come from the CRIPT controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.type = "web_site"
+
+        Returns
+        -------
+        str
+            reference type
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_reference_type: str) -> None:
+        """
+        set the reference type attribute
+
+        reference type must come from the CRIPT controlled vocabulary
+
+        Parameters
+        ----------
+        new_reference_type: str
+
+        Returns
+        -------
+        None
+        """
+        # TODO validate the reference type with CRIPT controlled vocabulary
+        new_attrs = replace(self._json_attrs, type=new_reference_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def title(self) -> str:
+        """
+        title of publication
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.title = "my new title"
+
+        Returns
+        -------
+        str
+            title of publication
+        """
+        return self._json_attrs.title
+
+    @title.setter
+    @beartype
+    def title(self, new_title: str) -> None:
+        """
+        set the title for the reference node
+
+        Parameters
+        ----------
+        new_title: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, title=new_title)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def author(self) -> List[str]:
+        """
+        List of authors for this reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.author += ["Navid Hariri"]
+
+        Returns
+        -------
+        List[str]
+            list of authors
+        """
+        return self._json_attrs.author.copy()
+
+    @author.setter
+    @beartype
+    def author(self, new_author: List[str]) -> None:
+        """
+        set the list of authors for the reference node
+
+        Parameters
+        ----------
+        new_author: List[str]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, author=new_author)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def journal(self) -> str:
+        """
+        journal of publication
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.journal = "my new journal"
+
+        Returns
+        -------
+        str
+            journal of publication
+        """
+        return self._json_attrs.journal
+
+    @journal.setter
+    @beartype
+    def journal(self, new_journal: str) -> None:
+        """
+        set the journal attribute for this reference node
+
+        Parameters
+        ----------
+        new_journal: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, journal=new_journal)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def publisher(self) -> str:
+        """
+        publisher for this reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.publisher = "my new publisher"
+
+        Returns
+        -------
+        str
+            publisher of this publication
+        """
+        return self._json_attrs.publisher
+
+    @publisher.setter
+    @beartype
+    def publisher(self, new_publisher: str) -> None:
+        """
+        set the publisher for this reference node
+
+        Parameters
+        ----------
+        new_publisher: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, publisher=new_publisher)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def year(self) -> Union[int, None]:
+        """
+        year for the scholarly work
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.year = 2023
+
+        Returns
+        -------
+        int
+        """
+        return self._json_attrs.year
+
+    @year.setter
+    @beartype
+    def year(self, new_year: Union[int, None]) -> None:
+        """
+        set the year for the scholarly work within the reference node
+
+        Parameters
+        ----------
+        new_year: int
+
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, year=new_year)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def volume(self) -> Union[int, None]:
+        """
+        Volume of the scholarly work from the reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.volume = 1
+
+        Returns
+        -------
+        int
+            volume number of the publishing
+        """
+        return self._json_attrs.volume
+
+    @volume.setter
+    @beartype
+    def volume(self, new_volume: Union[int, None]) -> None:
+        """
+        set the volume of the scholarly work for this reference node
+
+        Parameters
+        ----------
+        new_volume: int
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, volume=new_volume)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def issue(self) -> Union[int, None]:
+        """
+        issue of the scholarly work for the reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.issue = 2
+
+        Returns
+        -------
+        None
+        """
+        return self._json_attrs.issue
+
+    @issue.setter
+    @beartype
+    def issue(self, new_issue: Union[int, None]) -> None:
+        """
+        set the issue of the scholarly work
+
+        Parameters
+        ----------
+        new_issue: int
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, issue=new_issue)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def pages(self) -> List[int]:
+        """
+        pages of the scholarly work used in the reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.pages = [123, 456]
+
+        Returns
+        -------
+        int
+        """
+        return self._json_attrs.pages.copy()
+
+    @pages.setter
+    @beartype
+    def pages(self, new_pages_list: List[int]) -> None:
+        """
+        set the list of pages of the scholarly work for this reference node
+
+        Parameters
+        ----------
+        new_pages_list: List[int]
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, pages=new_pages_list)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def doi(self) -> str:
+        """
+        get the digital object identifier (DOI) for this reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.doi = "100.1038/1781168a0"
+
+        Returns
+        -------
+        str
+            digital object identifier (DOI) for this reference node
+        """
+        return self._json_attrs.doi
+
+    @doi.setter
+    @beartype
+    def doi(self, new_doi: str) -> None:
+        """
+        set the digital object identifier (DOI) for the scholarly work for this reference node
+
+        Parameters
+        ----------
+        new_doi: str
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.doi = "100.1038/1781168a0"
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, doi=new_doi)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def issn(self) -> str:
+        """
+        The international standard serial number (ISSN) for this reference node
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.issn = "1456-4687"
+
+        Returns
+        -------
+        str
+            ISSN for this reference node
+        """
+        return self._json_attrs.issn
+
+    @issn.setter
+    @beartype
+    def issn(self, new_issn: str) -> None:
+        """
+        set the international standard serial number (ISSN) for the scholarly work for this reference node
+
+        Parameters
+        ----------
+        new_issn: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, issn=new_issn)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def arxiv_id(self) -> str:
+        """
+        The arXiv identifier for the scholarly work for this reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.arxiv_id = "1501"
+
+        Returns
+        -------
+        str
+            arXiv identifier for the scholarly work for this publishing
+        """
+        return self._json_attrs.arxiv_id
+
+    @arxiv_id.setter
+    @beartype
+    def arxiv_id(self, new_arxiv_id: str) -> None:
+        """
+        set the arXiv identifier for the scholarly work for this reference node
+
+        Parameters
+        ----------
+        new_arxiv_id: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, arxiv_id=new_arxiv_id)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def pmid(self) -> Union[int, None]:
+        """
+        The PubMed ID (PMID) for this reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.pmid = 12345678
+
+        Returns
+        -------
+        int
+            the PubMedID of this publishing
+        """
+        return self._json_attrs.pmid
+
+    @pmid.setter
+    @beartype
+    def pmid(self, new_pmid: Union[int, None]) -> None:
+        """
+
+        Parameters
+        ----------
+        new_pmid
+
+        Returns
+        -------
+
+        """
+        # TODO can possibly add validations, possibly in forms of length checking
+        #  to be sure its the correct length
+        new_attrs = replace(self._json_attrs, pmid=new_pmid)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def website(self) -> str:
+        """
+        The website URL for the scholarly work
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_reference = cript.Reference(type="journal_article", title="'Living' Polymers")
+        >>> my_reference.website = "https://criptapp.org"
+
+        Returns
+        -------
+        str
+            the website URL of this publishing
+        """
+        return self._json_attrs.website
+
+    @website.setter
+    @beartype
+    def website(self, new_website: str) -> None:
+        """
+        set the website URL for the scholarly work
+
+        Parameters
+        ----------
+        new_website: str
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, website=new_website)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/__init__.py` & `cript-2.3.0/src/cript/nodes/subobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/algorithm.py` & `cript-2.3.0/src/cript/nodes/subobjects/algorithm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,264 +1,265 @@
-from dataclasses import dataclass, field, replace
-from typing import List, Optional
-
-from cript.nodes.subobjects.citation import Citation
-from cript.nodes.subobjects.parameter import Parameter
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Algorithm(UUIDBaseNode):
-    """
-    ## Definition
-
-    An [algorithm sub-object](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=25)
-    is a set of instructions that define a computational process.
-    An algorithm consists of parameters that are used in the computation and the computational process itself.
-
-
-    ## Attributes
-
-    | Keys      | Type            | Example                                      | Description                                            | Required | Vocab |
-    |-----------|-----------------|----------------------------------------------|--------------------------------------------------------|----------|-------|
-    | key       | str             | ensemble, thermo-barostat                    | system configuration, algorithms used in a computation | True     | True  |
-    | type      | str             | NPT for ensemble, Nose-Hoover for thermostat | specific type of configuration, algorithm              | True     |       |
-    | parameter | list[Parameter] |                                              | setup associated parameters                            |          |       |
-    | citation  | Citation        |                                              | reference to a book, paper, or scholarly work          |          |       |
-
-    ## Can be Added To
-    * [SoftwareConfiguration](../software_configuration)
-
-    ## Available sub-objects
-    * [Parameter](../parameter)
-    * [Citation](../citation)
-
-    ## JSON Representation
-    ```json
-    {
-        "node": ["Algorithm"],
-        "key": "mc_barostat",
-        "type": "barostat",
-        "parameter": {
-            "node": ["Parameter"],
-            "key": "update_frequency",
-            "value": 1000.0,
-            "unit": "1/second"
-        },
-        "citation": {
-            "node": ["Citation"],
-            "type": "reference"
-            "reference": {
-                    "node": ["Reference"],
-                    "type": "journal_article",
-                    "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
-                    "author": ["Ludwig Schneider", "Marcus Müller"],
-                    "journal": "Computer Physics Communications",
-                    "publisher": "Elsevier",
-                    "year": 2019,
-                    "pages": [463, 476],
-                    "doi": "10.1016/j.cpc.2018.08.011",
-                    "issn": "0010-4655",
-                    "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-            },
-        },
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        type: str = ""
-
-        parameter: List[Parameter] = field(default_factory=list)
-        citation: List[Citation] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    def __init__(self, key: str, type: str, parameter: Optional[List[Parameter]] = None, citation: Optional[List[Citation]] = None, **kwargs):  # ignored
-        """
-        Create algorithm sub-object
-
-        Parameters
-        ----------
-        key : str
-            algorithm key must come from
-            [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_key)
-        type : str
-            algorithm type must come from
-            [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_type)
-        parameter : List[Parameter], optional
-            parameter sub-object, by default None
-        citation : List[Citation], optional
-            citation sub-object, by default None
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-
-        Returns
-        -------
-        None
-            instantiate an algorithm node
-        """
-        if parameter is None:
-            parameter = []
-        if citation is None:
-            citation = []
-        super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, key=key, type=type, parameter=parameter)
-        self.validate()
-
-    @property
-    def key(self) -> str:
-        """
-        Algorithm key
-
-        Algorithm key must come from [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_key)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-        >>> my_algorithm.key = "amorphous_cell_module"
-
-        Returns
-        -------
-        str
-            algorithm key
-        """
-        return self._json_attrs.key
-
-    @key.setter
-    def key(self, new_key: str) -> None:
-        """
-        set the algorithm key
-
-        > Algorithm key must come from
-        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/algorithm_key)
-
-        Parameters
-        ----------
-        new_key : str
-            algorithm key
-        """
-        new_attrs = replace(self._json_attrs, key=new_key)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    def type(self) -> str:
-        """
-        Algorithm type
-
-        > Algorithm type must come from
-        [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_type)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-        >>> my_algorithm.type = "integration"
-
-        Returns
-        -------
-        str
-            algorithm type
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    def type(self, new_type: str) -> None:
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    def parameter(self) -> List[Parameter]:
-        """
-        list of [Parameter](../parameter) sub-objects for the algorithm sub-object
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-        >>> my_parameters = [
-        ...     cript.Parameter("update_frequency", 1000.0, "1/second"),
-        ...     cript.Parameter("damping_time", 1.0, "second"),
-        ... ]
-        >>> my_algorithm.parameter = my_parameters
-
-        Returns
-        -------
-        List[Parameter]
-            list of parameters for the algorithm sub-object
-        """
-        return self._json_attrs.parameter.copy()
-
-    @parameter.setter
-    def parameter(self, new_parameter: List[Parameter]) -> None:
-        """
-        set a list of cript.Parameter sub-objects
-
-        Parameters
-        ----------
-        new_parameter : List[Parameter]
-            list of Parameter sub-objects for the algorithm sub-object
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, parameter=new_parameter)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    def citation(self) -> Citation:
-        """
-        [citation](../citation) subobject for algorithm subobject
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-        >>> my_algorithm.citation = [my_citation]
-
-
-        Returns
-        -------
-        citation node: Citation
-            get the algorithm citation node
-        """
-        return self._json_attrs.citation.copy()  # type: ignore
-
-    @citation.setter
-    def citation(self, new_citation: List[Citation]) -> None:
-        """
-        set the algorithm citation subobject
-
-        Parameters
-        ----------
-        new_citation : Citation
-            new citation subobject to replace the current
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from cript.nodes.subobjects.citation import Citation
+from cript.nodes.subobjects.parameter import Parameter
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Algorithm(UUIDBaseNode):
+    """
+    ## Definition
+
+    An [algorithm sub-object](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=25)
+    is a set of instructions that define a computational process.
+    An algorithm consists of parameters that are used in the computation and the computational process itself.
+
+
+    ## Attributes
+
+    | Keys      | Type            | Example                                      | Description                                            | Required | Vocab |
+    |-----------|-----------------|----------------------------------------------|--------------------------------------------------------|----------|-------|
+    | key       | str             | ensemble, thermo-barostat                    | system configuration, algorithms used in a computation | True     | True  |
+    | type      | str             | NPT for ensemble, Nose-Hoover for thermostat | specific type of configuration, algorithm              | True     |       |
+    | parameter | list[Parameter] |                                              | setup associated parameters                            |          |       |
+    | citation  | Citation        |                                              | reference to a book, paper, or scholarly work          |          |       |
+
+    ## Can be Added To
+    * [SoftwareConfiguration](../software_configuration)
+
+    ## Available sub-objects
+    * [Parameter](../parameter)
+    * [Citation](../citation)
+
+    ## JSON Representation
+    ```json
+    {
+        "node": ["Algorithm"],
+        "key": "mc_barostat",
+        "type": "barostat",
+        "parameter": {
+            "node": ["Parameter"],
+            "key": "update_frequency",
+            "value": 1000.0,
+            "unit": "1/second"
+        },
+        "citation": {
+            "node": ["Citation"],
+            "type": "reference"
+            "reference": {
+                    "node": ["Reference"],
+                    "type": "journal_article",
+                    "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
+                    "author": ["Ludwig Schneider", "Marcus Müller"],
+                    "journal": "Computer Physics Communications",
+                    "publisher": "Elsevier",
+                    "year": 2019,
+                    "pages": [463, 476],
+                    "doi": "10.1016/j.cpc.2018.08.011",
+                    "issn": "0010-4655",
+                    "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+            },
+        },
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        type: str = ""
+
+        parameter: List[Union[Parameter, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Citation, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    def __init__(self, key: str, type: str, parameter: Optional[List[Union[Parameter, UIDProxy]]] = None, citation: Optional[List[Union[Citation, UIDProxy]]] = None, **kwargs):  # ignored
+        """
+        Create algorithm sub-object
+
+        Parameters
+        ----------
+        key : str
+            algorithm key must come from
+            [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_key)
+        type : str
+            algorithm type must come from
+            [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_type)
+        parameter : List[Parameter], optional
+            parameter sub-object, by default None
+        citation : List[Citation], optional
+            citation sub-object, by default None
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+
+        Returns
+        -------
+        None
+            instantiate an algorithm node
+        """
+        if parameter is None:
+            parameter = []
+        if citation is None:
+            citation = []
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, key=key, type=type, parameter=parameter)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    def key(self) -> str:
+        """
+        Algorithm key
+
+        Algorithm key must come from [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+        >>> my_algorithm.key = "amorphous_cell_module"
+
+        Returns
+        -------
+        str
+            algorithm key
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    def key(self, new_key: str) -> None:
+        """
+        set the algorithm key
+
+        > Algorithm key must come from
+        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/algorithm_key)
+
+        Parameters
+        ----------
+        new_key : str
+            algorithm key
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    def type(self) -> str:
+        """
+        Algorithm type
+
+        > Algorithm type must come from
+        [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/algorithm_type)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+        >>> my_algorithm.type = "integration"
+
+        Returns
+        -------
+        str
+            algorithm type
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    def type(self, new_type: str) -> None:
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    def parameter(self) -> List[Union[Parameter, UIDProxy]]:
+        """
+        list of [Parameter](../parameter) sub-objects for the algorithm sub-object
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+        >>> my_parameters = [
+        ...     cript.Parameter("update_frequency", 1000.0, "1/second"),
+        ...     cript.Parameter("damping_time", 1.0, "second"),
+        ... ]
+        >>> my_algorithm.parameter = my_parameters
+
+        Returns
+        -------
+        List[Parameter]
+            list of parameters for the algorithm sub-object
+        """
+        return self._json_attrs.parameter.copy()
+
+    @parameter.setter
+    def parameter(self, new_parameter: List[Union[Parameter, UIDProxy]]) -> None:
+        """
+        set a list of cript.Parameter sub-objects
+
+        Parameters
+        ----------
+        new_parameter : List[Parameter]
+            list of Parameter sub-objects for the algorithm sub-object
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, parameter=new_parameter)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    def citation(self) -> List[Union[Citation, UIDProxy]]:
+        """
+        [citation](../citation) subobject for algorithm subobject
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_algorithm.citation = [my_citation]
+
+
+        Returns
+        -------
+        citation node: Citation
+            get the algorithm citation node
+        """
+        return self._json_attrs.citation.copy()  # type: ignore
+
+    @citation.setter
+    def citation(self, new_citation: List[Union[Citation, UIDProxy]]) -> None:
+        """
+        set the algorithm citation subobject
+
+        Parameters
+        ----------
+        new_citation : Citation
+            new citation subobject to replace the current
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/citation.py` & `cript-2.3.0/src/cript/nodes/subobjects/citation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,231 +1,232 @@
-from dataclasses import dataclass, replace
-from typing import Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.reference import Reference
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Citation(UUIDBaseNode):
-    """
-    ## Definition
-    The [Citation sub-object](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=26)
-    essentially houses [Reference nodes](../../primary_nodes/reference). The citation subobject can then be added to CRIPT Primary nodes.
-
-    ## Attributes
-    | attribute | type      | example      | description                                   | required | vocab |
-    |-----------|-----------|--------------|-----------------------------------------------|----------|-------|
-    | type      | str       | derived_from | key for identifier                            | True     | True  |
-    | reference | Reference |              | reference to a book, paper, or scholarly work | True     |       |
-
-    ## Can Be Added To
-    * [Collection node](../../primary_nodes/collection)
-    * [Computation node](../../primary_nodes/computation)
-    * [Computation Process Node](../../primary_nodes/computation_process)
-    * [Data node](../../primary_nodes/data)
-
-    * [Computational Forcefield subobjects](../computational_forcefield)
-    * [Property subobject](../property)
-    * [Algorithm subobject](../algorithm)
-    * [Equipment subobject](../equipment)
-
-    ---
-
-    ## Available Subobjects
-    * `None`
-
-    ## JSON Representation
-    ```json
-    "citation": {
-            "node": ["Citation"],
-            "type": "reference",
-            "reference": {
-                    "node": ["Reference"],
-                    "type": "journal_article",
-                    "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
-                    "author": ["Ludwig Schneider", "Marcus Müller"],
-                    "journal": "Computer Physics Communications",
-                    "publisher": "Elsevier",
-                    "year": 2019,
-                    "pages": [463, 476],
-                    "doi": "10.1016/j.cpc.2018.08.011",
-                    "issn": "0010-4655",
-                    "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-            },
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        type: str = ""
-        reference: Optional[Reference] = None
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, type: str, reference: Reference, **kwargs):
-        """
-        create a Citation subobject
-
-        Parameters
-        ----------
-        type : citation type
-            citation type must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/citation_type)
-        reference : Reference
-            Reference node
-
-        Examples
-        -------
-        >>> import cript
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     "journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-
-
-        Returns
-        -------
-        None
-            Instantiate citation subobject
-        """
-        super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, type=type, reference=reference)
-        self.validate()
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        Citation type subobject
-
-        Citation type must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/citation_type)
-
-        Examples
-        --------
-        >>> import cript
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     "journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-        >>> my_citation.type = "extracted_by_algorithm"
-
-        Returns
-        -------
-        str
-            Citation type
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_type: str) -> None:
-        """
-        set the citation sub-object type
-
-        Parameters
-        ----------
-        new_type : str
-            citation type
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def reference(self) -> Union[Reference, None]:
-        """
-        citation reference node
-
-        Examples
-        --------
-        >>> import cript
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     "journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-        >>> my_new_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title="'Living' Polymers",
-        ...     author=["Dylan J. Walsh", "Bradley D. Olsen"],
-        ...     journal="Nature",
-        ...     publisher="Springer",
-        ...     year=2019,
-        ...     volume=3,
-        ...     issue=5,
-        ...     pages=[123, 456, 789],
-        ...     doi="10.1038/1781168a0",
-        ...     issn="1476-4687",
-        ...     arxiv_id="1501",
-        ...     pmid=12345678,
-        ...     website="https://criptapp.org",
-        ... )
-        >>> my_citation.reference = my_new_reference
-
-        Returns
-        -------
-        Reference
-            Reference node
-        """
-        return self._json_attrs.reference
-
-    @reference.setter
-    @beartype
-    def reference(self, new_reference: Reference) -> None:
-        """
-        replace the current Reference node for the citation subobject
-
-        Parameters
-        ----------
-        new_reference : Reference
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, reference=new_reference)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, replace
+from typing import Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.reference import Reference
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Citation(UUIDBaseNode):
+    """
+    ## Definition
+    The [Citation sub-object](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=26)
+    essentially houses [Reference nodes](../../primary_nodes/reference). The citation subobject can then be added to CRIPT Primary nodes.
+
+    ## Attributes
+    | attribute | type      | example      | description                                   | required | vocab |
+    |-----------|-----------|--------------|-----------------------------------------------|----------|-------|
+    | type      | str       | derived_from | key for identifier                            | True     | True  |
+    | reference | Reference |              | reference to a book, paper, or scholarly work | True     |       |
+
+    ## Can Be Added To
+    * [Collection node](../../primary_nodes/collection)
+    * [Computation node](../../primary_nodes/computation)
+    * [Computation Process Node](../../primary_nodes/computation_process)
+    * [Data node](../../primary_nodes/data)
+
+    * [Computational Forcefield subobjects](../computational_forcefield)
+    * [Property subobject](../property)
+    * [Algorithm subobject](../algorithm)
+    * [Equipment subobject](../equipment)
+
+    ---
+
+    ## Available Subobjects
+    * `None`
+
+    ## JSON Representation
+    ```json
+    "citation": {
+            "node": ["Citation"],
+            "type": "reference",
+            "reference": {
+                    "node": ["Reference"],
+                    "type": "journal_article",
+                    "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
+                    "author": ["Ludwig Schneider", "Marcus Müller"],
+                    "journal": "Computer Physics Communications",
+                    "publisher": "Elsevier",
+                    "year": 2019,
+                    "pages": [463, 476],
+                    "doi": "10.1016/j.cpc.2018.08.011",
+                    "issn": "0010-4655",
+                    "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+            },
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        type: str = ""
+        reference: Optional[Union[Reference, UIDProxy]] = None
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, type: str, reference: Union[Reference, UIDProxy], **kwargs):
+        """
+        create a Citation subobject
+
+        Parameters
+        ----------
+        type : citation type
+            citation type must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/citation_type)
+        reference : Reference
+            Reference node
+
+        Examples
+        -------
+        >>> import cript
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     "journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+
+
+        Returns
+        -------
+        None
+            Instantiate citation subobject
+        """
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, type=type, reference=reference)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        Citation type subobject
+
+        Citation type must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/citation_type)
+
+        Examples
+        --------
+        >>> import cript
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     "journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_citation.type = "extracted_by_algorithm"
+
+        Returns
+        -------
+        str
+            Citation type
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_type: str) -> None:
+        """
+        set the citation sub-object type
+
+        Parameters
+        ----------
+        new_type : str
+            citation type
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def reference(self) -> Union[Reference, None, UIDProxy]:
+        """
+        citation reference node
+
+        Examples
+        --------
+        >>> import cript
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     "journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_new_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title="'Living' Polymers",
+        ...     author=["Dylan J. Walsh", "Bradley D. Olsen"],
+        ...     journal="Nature",
+        ...     publisher="Springer",
+        ...     year=2019,
+        ...     volume=3,
+        ...     issue=5,
+        ...     pages=[123, 456, 789],
+        ...     doi="10.1038/1781168a0",
+        ...     issn="1476-4687",
+        ...     arxiv_id="1501",
+        ...     pmid=12345678,
+        ...     website="https://criptapp.org",
+        ... )
+        >>> my_citation.reference = my_new_reference
+
+        Returns
+        -------
+        Reference
+            Reference node
+        """
+        return self._json_attrs.reference
+
+    @reference.setter
+    @beartype
+    def reference(self, new_reference: Reference) -> None:
+        """
+        replace the current Reference node for the citation subobject
+
+        Parameters
+        ----------
+        new_reference : Reference
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, reference=new_reference)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/computational_forcefield.py` & `cript-2.3.0/src/cript/nodes/subobjects/computational_forcefield.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,496 +1,508 @@
-from dataclasses import dataclass, field, replace
-from typing import List, Optional
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.data import Data
-from cript.nodes.subobjects.citation import Citation
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class ComputationalForcefield(UUIDBaseNode):
-    """
-    ## Definition
-    A [Computational Forcefield Subobject](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=23)
-    is a mathematical model that describes the forces between atoms and molecules.
-    It is used in computational chemistry and molecular dynamics simulations to predict the behavior of materials.
-    Forcefields are typically based on experimental data or quantum mechanical calculations,
-    and they are often used to study the properties of materials such as their structure, dynamics, and reactivity.
-
-    ## Attributes
-    | attribute              | type           | example                                                                | description                                                              | required | vocab |
-    |------------------------|----------------|------------------------------------------------------------------------|--------------------------------------------------------------------------|----------|-------|
-    | key                    | str            | CHARMM27                                                               | type of forcefield                                                       | True     | True  |
-    | building_block         | str            | atom                                                                   | type of building block                                                   | True     | True  |
-    | coarse_grained_mapping | str            | SC3 beads in MARTINI forcefield                                        | atom to beads mapping                                                    |          |       |
-    | implicit_solvent       | str            | water                                                                  | Name of implicit solvent                                                 |          |       |
-    | source                 | str            | package in GROMACS                                                     | source of forcefield                                                     |          |       |
-    | description            | str            | OPLS forcefield with partial charges calculated via the LBCC algorithm | description of the forcefield and any modifications that have been added |          |       |
-    | data                   | Data           |                                                                        | details of mapping schema and forcefield parameters                      |          |       |
-    | citation               | list[Citation] |                                                                        | reference to a book, paper, or scholarly work                            |          |       |
-
-
-    ## Can be Added To Primary Node:
-    * Material node
-
-    ## JSON Representation
-    ```json
-    {
-        "node": ["ComputationalForcefield"],
-        "key": "opls_aa",
-        "building_block": "atom",
-        "coarse_grained_mapping": "atom -> atom",
-        "implicit_solvent": "no implicit solvent",
-        "source": "local LigParGen installation",
-        "description": "this is a test forcefield",
-        "data": {
-            "node":["Data"],
-            "name":"my data name",
-            "type":"afm_amp",
-            "file":[
-                {
-                    "node":["File"],
-                    "type":"calibration",
-                    "source":"https://criptapp.org",
-                    "extension":".csv",
-                    "data_dictionary":"my file's data dictionary"
-                }
-            ]
-        },
-        "citation": {
-            "node": ["Citation"],
-            "type": "reference"
-            "reference": {
-                "node": ["Reference"],
-                "type": "journal_article",
-                "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
-                "author": ["Ludwig Schneider", "Marcus Müller"],
-                "journal": "Computer Physics Communications",
-                "publisher": "Elsevier",
-                "year": 2019,
-                "pages": [463, 476],
-                "doi": "10.1016/j.cpc.2018.08.011",
-                "issn": "0010-4655",
-                "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-            }
-    }
-
-
-    ```
-
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        building_block: str = ""
-        coarse_grained_mapping: str = ""
-        implicit_solvent: str = ""
-        source: str = ""
-        description: str = ""
-        data: List[Data] = field(default_factory=list)
-        citation: List[Citation] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, key: str, building_block: str, coarse_grained_mapping: str = "", implicit_solvent: str = "", source: str = "", description: str = "", data: Optional[List[Data]] = None, citation: Optional[List[Citation]] = None, **kwargs):
-        """
-        instantiate a computational_forcefield subobject
-
-        Parameters
-        ----------
-        key : str
-            type of forcefield key must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/computational_forcefield_key)
-        building_block : str
-            type of computational_forcefield building_block must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/building_block)
-        coarse_grained_mapping : str, optional
-            atom to beads mapping, by default ""
-        implicit_solvent : str, optional
-            Name of implicit solvent, by default ""
-        source : str, optional
-            source of forcefield, by default ""
-        description : str, optional
-            description of the forcefield and any modifications that have been added, by default ""
-        data : List[Data], optional
-            details of mapping schema and forcefield parameters, by default None
-        citation : Union[List[Citation], None], optional
-            reference to a book, paper, or scholarly work, by default None
-
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-
-        Returns
-        -------
-        None
-            Instantiate a computational_forcefield subobject
-        """
-        if citation is None:
-            citation = []
-        super().__init__(**kwargs)
-
-        if data is None:
-            data = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            key=key,
-            building_block=building_block,
-            coarse_grained_mapping=coarse_grained_mapping,
-            implicit_solvent=implicit_solvent,
-            source=source,
-            description=description,
-            data=data,
-            citation=citation,
-        )
-        self.validate()
-
-    @property
-    @beartype
-    def key(self) -> str:
-        """
-        type of forcefield
-
-        Computational_Forcefield key must come from
-        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/computational_forcefield_key)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.key = "amber"
-
-        Returns
-        -------
-        str
-            type of forcefield
-        """
-        return self._json_attrs.key
-
-    @key.setter
-    @beartype
-    def key(self, new_key: str) -> None:
-        """
-        set key for this computational_forcefield
-
-        Parameters
-        ----------
-        new_key : str
-            computational_forcefield key
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, key=new_key)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def building_block(self) -> str:
-        """
-        type of building block
-
-        Computational_Forcefield building_block must come from
-        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/building_block)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.building_block = "non_atomistic"
-
-        Returns
-        -------
-        str
-            type of building block
-        """
-        return self._json_attrs.building_block
-
-    @building_block.setter
-    @beartype
-    def building_block(self, new_building_block: str) -> None:
-        """
-        type of building block
-
-        Parameters
-        ----------
-        new_building_block : str
-            new type of building block
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, building_block=new_building_block)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def coarse_grained_mapping(self) -> str:
-        """
-        atom to beads mapping
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.coarse_grained_mapping = "SC3 beads in MARTINI forcefield"
-
-        Returns
-        -------
-        str
-            coarse_grained_mapping
-        """
-        return self._json_attrs.coarse_grained_mapping
-
-    @coarse_grained_mapping.setter
-    @beartype
-    def coarse_grained_mapping(self, new_coarse_grained_mapping: str) -> None:
-        """
-        atom to beads mapping
-
-        Parameters
-        ----------
-        new_coarse_grained_mapping : str
-            new coarse_grained_mapping
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, coarse_grained_mapping=new_coarse_grained_mapping)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def implicit_solvent(self) -> str:
-        """
-        Name of implicit solvent
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.implicit_solvent = "water"
-
-        Returns
-        -------
-        str
-            _description_
-        """
-        return self._json_attrs.implicit_solvent
-
-    @implicit_solvent.setter
-    @beartype
-    def implicit_solvent(self, new_implicit_solvent: str) -> None:
-        """
-        set the implicit_solvent
-
-        Parameters
-        ----------
-        new_implicit_solvent : str
-            new implicit_solvent
-        """
-        new_attrs = replace(self._json_attrs, implicit_solvent=new_implicit_solvent)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def source(self) -> str:
-        """
-        source of forcefield
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.source = "package in GROMACS"
-
-        Returns
-        -------
-        str
-            source of forcefield
-        """
-        return self._json_attrs.source
-
-    @source.setter
-    @beartype
-    def source(self, new_source: str) -> None:
-        """
-        set the computational_forcefield
-
-        Parameters
-        ----------
-        new_source : str
-            new source of forcefield
-        """
-        new_attrs = replace(self._json_attrs, source=new_source)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def description(self) -> str:
-        """
-        description of the forcefield and any modifications that have been added
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_computational_forcefield.description = "OPLS forcefield with partial charges calculated via the LBCC algorithm"
-
-        Returns
-        -------
-        str
-            description of the forcefield and any modifications that have been added
-        """
-        return self._json_attrs.description
-
-    @description.setter
-    @beartype
-    def description(self, new_description: str) -> None:
-        """
-        set this computational_forcefields description
-
-        Parameters
-        ----------
-        new_description : str
-            new computational_forcefields description
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, description=new_description)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def data(self) -> List[Data]:
-        """
-        details of mapping schema and forcefield parameters
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
-        ...     type="calibration",
-        ...     extension=".pdf",
-        ... )
-        >>> my_data = cript.Data(
-        ...     name="my data node name",
-        ...     type="afm_amp",
-        ...     file=[my_file],
-        ... )
-        >>> my_computational_forcefield.data = [my_data]
-
-        Returns
-        -------
-        List[Data]
-            list of data nodes for this computational_forcefield subobject
-        """
-        return self._json_attrs.data.copy()
-
-    @data.setter
-    @beartype
-    def data(self, new_data: List[Data]) -> None:
-        """
-        set the data attribute of this computational_forcefield node
-
-        Parameters
-        ----------
-        new_data : List[Data]
-            new list of data nodes
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, data=new_data)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Citation]:
-        """
-        reference to a book, paper, or scholarly work
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_computational_forcefield = cript.ComputationalForcefield(
-        ...     key="opls_aa",
-        ...     building_block="atom",
-        ... )
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "SOft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     "journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-        >>> my_computational_forcefield.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            computational_forcefield list of citations
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation: List[Citation]) -> None:
-        """
-        set the citation subobject of the computational_forcefield subobject
-
-        Parameters
-        ----------
-        new_citation : List[Citation]
-            new citation subobject
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.data import Data
+from cript.nodes.subobjects.citation import Citation
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class ComputationalForcefield(UUIDBaseNode):
+    """
+    ## Definition
+    A [Computational Forcefield Subobject](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=23)
+    is a mathematical model that describes the forces between atoms and molecules.
+    It is used in computational chemistry and molecular dynamics simulations to predict the behavior of materials.
+    Forcefields are typically based on experimental data or quantum mechanical calculations,
+    and they are often used to study the properties of materials such as their structure, dynamics, and reactivity.
+
+    ## Attributes
+    | attribute              | type           | example                                                                | description                                                              | required | vocab |
+    |------------------------|----------------|------------------------------------------------------------------------|--------------------------------------------------------------------------|----------|-------|
+    | key                    | str            | CHARMM27                                                               | type of forcefield                                                       | True     | True  |
+    | building_block         | str            | atom                                                                   | type of building block                                                   | True     | True  |
+    | coarse_grained_mapping | str            | SC3 beads in MARTINI forcefield                                        | atom to beads mapping                                                    |          |       |
+    | implicit_solvent       | str            | water                                                                  | Name of implicit solvent                                                 |          |       |
+    | source                 | str            | package in GROMACS                                                     | source of forcefield                                                     |          |       |
+    | description            | str            | OPLS forcefield with partial charges calculated via the LBCC algorithm | description of the forcefield and any modifications that have been added |          |       |
+    | data                   | Data           |                                                                        | details of mapping schema and forcefield parameters                      |          |       |
+    | citation               | list[Citation] |                                                                        | reference to a book, paper, or scholarly work                            |          |       |
+
+
+    ## Can be Added To Primary Node:
+    * Material node
+
+    ## JSON Representation
+    ```json
+    {
+        "node": ["ComputationalForcefield"],
+        "key": "opls_aa",
+        "building_block": "atom",
+        "coarse_grained_mapping": "atom -> atom",
+        "implicit_solvent": "no implicit solvent",
+        "source": "local LigParGen installation",
+        "description": "this is a test forcefield",
+        "data": {
+            "node":["Data"],
+            "name":"my data name",
+            "type":"afm_amp",
+            "file":[
+                {
+                    "node":["File"],
+                    "type":"calibration",
+                    "source":"https://criptapp.org",
+                    "extension":".csv",
+                    "data_dictionary":"my file's data dictionary"
+                }
+            ]
+        },
+        "citation": {
+            "node": ["Citation"],
+            "type": "reference"
+            "reference": {
+                "node": ["Reference"],
+                "type": "journal_article",
+                "title": "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: SOft coarse grained Monte-Carlo Acceleration (SOMA)",
+                "author": ["Ludwig Schneider", "Marcus Müller"],
+                "journal": "Computer Physics Communications",
+                "publisher": "Elsevier",
+                "year": 2019,
+                "pages": [463, 476],
+                "doi": "10.1016/j.cpc.2018.08.011",
+                "issn": "0010-4655",
+                "website": "https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+            }
+    }
+
+
+    ```
+
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        building_block: str = ""
+        coarse_grained_mapping: str = ""
+        implicit_solvent: str = ""
+        source: str = ""
+        description: str = ""
+        data: List[Union[Data, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Citation, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        key: str,
+        building_block: str,
+        coarse_grained_mapping: str = "",
+        implicit_solvent: str = "",
+        source: str = "",
+        description: str = "",
+        data: Optional[List[Union[Data, UIDProxy]]] = None,
+        citation: Optional[List[Union[Citation, UIDProxy]]] = None,
+        **kwargs
+    ):
+        """
+        instantiate a computational_forcefield subobject
+
+        Parameters
+        ----------
+        key : str
+            type of forcefield key must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/computational_forcefield_key)
+        building_block : str
+            type of computational_forcefield building_block must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/building_block)
+        coarse_grained_mapping : str, optional
+            atom to beads mapping, by default ""
+        implicit_solvent : str, optional
+            Name of implicit solvent, by default ""
+        source : str, optional
+            source of forcefield, by default ""
+        description : str, optional
+            description of the forcefield and any modifications that have been added, by default ""
+        data : List[Data], optional
+            details of mapping schema and forcefield parameters, by default None
+        citation : Union[List[Citation], None], optional
+            reference to a book, paper, or scholarly work, by default None
+
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+
+        Returns
+        -------
+        None
+            Instantiate a computational_forcefield subobject
+        """
+        if citation is None:
+            citation = []
+        super().__init__(**kwargs)
+
+        if data is None:
+            data = []
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            key=key,
+            building_block=building_block,
+            coarse_grained_mapping=coarse_grained_mapping,
+            implicit_solvent=implicit_solvent,
+            source=source,
+            description=description,
+            data=data,
+            citation=citation,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        type of forcefield
+
+        Computational_Forcefield key must come from
+        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/computational_forcefield_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.key = "amber"
+
+        Returns
+        -------
+        str
+            type of forcefield
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    @beartype
+    def key(self, new_key: str) -> None:
+        """
+        set key for this computational_forcefield
+
+        Parameters
+        ----------
+        new_key : str
+            computational_forcefield key
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def building_block(self) -> str:
+        """
+        type of building block
+
+        Computational_Forcefield building_block must come from
+        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/building_block)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.building_block = "non_atomistic"
+
+        Returns
+        -------
+        str
+            type of building block
+        """
+        return self._json_attrs.building_block
+
+    @building_block.setter
+    @beartype
+    def building_block(self, new_building_block: str) -> None:
+        """
+        type of building block
+
+        Parameters
+        ----------
+        new_building_block : str
+            new type of building block
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, building_block=new_building_block)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def coarse_grained_mapping(self) -> str:
+        """
+        atom to beads mapping
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.coarse_grained_mapping = "SC3 beads in MARTINI forcefield"
+
+        Returns
+        -------
+        str
+            coarse_grained_mapping
+        """
+        return self._json_attrs.coarse_grained_mapping
+
+    @coarse_grained_mapping.setter
+    @beartype
+    def coarse_grained_mapping(self, new_coarse_grained_mapping: str) -> None:
+        """
+        atom to beads mapping
+
+        Parameters
+        ----------
+        new_coarse_grained_mapping : str
+            new coarse_grained_mapping
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, coarse_grained_mapping=new_coarse_grained_mapping)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def implicit_solvent(self) -> str:
+        """
+        Name of implicit solvent
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.implicit_solvent = "water"
+
+        Returns
+        -------
+        str
+            _description_
+        """
+        return self._json_attrs.implicit_solvent
+
+    @implicit_solvent.setter
+    @beartype
+    def implicit_solvent(self, new_implicit_solvent: str) -> None:
+        """
+        set the implicit_solvent
+
+        Parameters
+        ----------
+        new_implicit_solvent : str
+            new implicit_solvent
+        """
+        new_attrs = replace(self._json_attrs, implicit_solvent=new_implicit_solvent)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def source(self) -> str:
+        """
+        source of forcefield
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.source = "package in GROMACS"
+
+        Returns
+        -------
+        str
+            source of forcefield
+        """
+        return self._json_attrs.source
+
+    @source.setter
+    @beartype
+    def source(self, new_source: str) -> None:
+        """
+        set the computational_forcefield
+
+        Parameters
+        ----------
+        new_source : str
+            new source of forcefield
+        """
+        new_attrs = replace(self._json_attrs, source=new_source)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def description(self) -> str:
+        """
+        description of the forcefield and any modifications that have been added
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_computational_forcefield.description = "OPLS forcefield with partial charges calculated via the LBCC algorithm"
+
+        Returns
+        -------
+        str
+            description of the forcefield and any modifications that have been added
+        """
+        return self._json_attrs.description
+
+    @description.setter
+    @beartype
+    def description(self, new_description: str) -> None:
+        """
+        set this computational_forcefields description
+
+        Parameters
+        ----------
+        new_description : str
+            new computational_forcefields description
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, description=new_description)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def data(self) -> List[Union[Data, UIDProxy]]:
+        """
+        details of mapping schema and forcefield parameters
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
+        ...     type="calibration",
+        ...     extension=".pdf",
+        ... )
+        >>> my_data = cript.Data(
+        ...     name="my data node name",
+        ...     type="afm_amp",
+        ...     file=[my_file],
+        ... )
+        >>> my_computational_forcefield.data = [my_data]
+
+        Returns
+        -------
+        List[Data]
+            list of data nodes for this computational_forcefield subobject
+        """
+        return self._json_attrs.data.copy()
+
+    @data.setter
+    @beartype
+    def data(self, new_data: List[Union[Data, UIDProxy]]) -> None:
+        """
+        set the data attribute of this computational_forcefield node
+
+        Parameters
+        ----------
+        new_data : List[Data]
+            new list of data nodes
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, data=new_data)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Union[Citation, UIDProxy]]:
+        """
+        reference to a book, paper, or scholarly work
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_computational_forcefield = cript.ComputationalForcefield(
+        ...     key="opls_aa",
+        ...     building_block="atom",
+        ... )
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "SOft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     "journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_computational_forcefield.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            computational_forcefield list of citations
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation: List[Union[Citation, UIDProxy]]) -> None:
+        """
+        set the citation subobject of the computational_forcefield subobject
+
+        Parameters
+        ----------
+        new_citation : List[Citation]
+            new citation subobject
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/condition.py` & `cript-2.3.0/src/cript/nodes/subobjects/condition.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,556 +1,557 @@
-from dataclasses import dataclass, field, replace
-from numbers import Number
-from typing import List, Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.data import Data
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Condition(UUIDBaseNode):
-    """
-    ## Definition
-
-    A [Condition](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=21) sub-object
-    is the conditions under which the experiment was conducted.
-    Some examples include temperature, mixing_rate, stirring, time_duration.
-
-    ----
-
-    ## Can Be Added To:
-    ### Primary Nodes
-    * [Process](../../primary_nodes/process)
-    * [Computation_Process](../../primary_nodes/computation_process)
-
-    ### Subobjects
-    * [Property](../property)
-    * [Equipment](../equipment)
-
-    ---
-
-    ## Attributes
-
-    | attribute        | type   | example                 | description                                                                            | required | vocab |
-    |------------------|--------|-------------------------|----------------------------------------------------------------------------------------|----------|-------|
-    | key              | str    | temp                    | type of condition                                                                      | True     | True  |
-    | type             | str    | min                     | type of value stored, 'value' is just the number, 'min', 'max', 'avg', etc. for series | True     | True  |
-    | descriptor       | str    | upper temperature probe | freeform description for condition                                                     |          |       |
-    | value            | Number | 1.23                    | value or quantity                                                                      | True     |       |
-    | unit             | str    | gram                    | unit for value                                                                         |          |       |
-    | uncertainty      | Number | 0.1                     | uncertainty of value                                                                   |          |       |
-    | uncertainty_type | str    | std                     | type of uncertainty                                                                    |          | True  |
-    | set_id           | int    | 0                       | ID of set (used to link measurements in as series)                                     |          |       |
-    | measurement _id  | int    | 0                       | ID for a single measurement (used to link multiple condition at a single instance)     |          |       |
-    | data             | List[Data] |                         | detailed data associated with the condition                                            |          |       |
-
-    ## JSON Representation
-    ```json
-    {
-        "node": ["Condition"],
-        "key": "temperature",
-        "type": "value",
-        "descriptor": "room temperature of lab",
-        "value": 22,
-        "unit": "C",
-        "uncertainty": 5,
-        "uncertainty_type": "stdev",
-        "set_id": 0,
-        "measurement_id": 2,
-        "data": [{
-            "node":["Data"],
-            "name":"my data name",
-            "type":"afm_amp",
-            "file":[
-                {
-                    "node":["File"],
-                    "type":"calibration",
-                    "source":"https://criptapp.org",
-                    "extension":".csv",
-                    "data_dictionary":"my file's data dictionary"
-                }
-            ]
-        }],
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        type: str = ""
-        descriptor: str = ""
-        value: Optional[Union[Number, str]] = None
-        unit: str = ""
-        uncertainty: Optional[Union[Number, str]] = None
-        uncertainty_type: str = ""
-        set_id: Optional[int] = None
-        measurement_id: Optional[int] = None
-        data: List[Data] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        key: str,
-        type: str,
-        value: Union[Number, str],
-        unit: str = "",
-        descriptor: str = "",
-        uncertainty: Optional[Union[Number, str]] = None,
-        uncertainty_type: str = "",
-        set_id: Optional[int] = None,
-        measurement_id: Optional[int] = None,
-        data: Optional[List[Data]] = None,
-        **kwargs
-    ):
-        """
-        create Condition sub-object
-
-        Parameters
-        ----------
-        key : str
-            type of condition
-        type : str
-            type of value stored
-        value : Number
-            value or quantity
-        unit : str, optional
-            unit for value, by default ""
-        descriptor : str, optional
-            freeform description for condition, by default ""
-        uncertainty : Union[Number, None], optional
-           uncertainty of value, by default None
-        uncertainty_type : str, optional
-            type of uncertainty, by default ""
-        set_id : Union[int, None], optional
-            ID of set (used to link measurements in as series), by default None
-        measurement_id : Union[int, None], optional
-            ID for a single measurement (used to link multiple condition at a single instance), by default None
-        data : List[Data], optional
-            detailed data associated with the condition, by default None
-
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-
-        Returns
-        -------
-        None
-        """
-        super().__init__(**kwargs)
-
-        if data is None:
-            data = []
-
-        self._json_attrs = replace(
-            self._json_attrs,
-            key=key,
-            type=type,
-            value=value,
-            descriptor=descriptor,
-            unit=unit,
-            uncertainty=uncertainty,
-            uncertainty_type=uncertainty_type,
-            set_id=set_id,
-            measurement_id=measurement_id,
-            data=data,
-        )
-        self.validate()
-
-    @property
-    @beartype
-    def key(self) -> str:
-        """
-        type of condition
-
-        > Condition key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/condition_key)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.key = "energy_threshold"
-
-        Returns
-        -------
-        condition key: str
-            type of condition
-        """
-        return self._json_attrs.key
-
-    @key.setter
-    @beartype
-    def key(self, new_key: str) -> None:
-        """
-        set this Condition sub-object key
-
-        Parameters
-        ----------
-        new_key : str
-            type of condition
-
-        Returns
-        --------
-        None
-        """
-        new_attrs = replace(self._json_attrs, key=new_key)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        description for the value stored for this Condition node
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.type = "min"
-
-        Returns
-        -------
-        condition type: str
-            description for the value
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_type: str) -> None:
-        """
-        set the type attribute for this Condition node
-
-        Parameters
-        ----------
-        new_type : str
-            new description of the Condition value
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def descriptor(self) -> str:
-        """
-        freeform description for Condition
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.descriptor = "my condition description"
-
-        Returns
-        -------
-        description: str
-            description of this Condition sub-object
-        """
-        return self._json_attrs.descriptor
-
-    @descriptor.setter
-    @beartype
-    def descriptor(self, new_descriptor: str) -> None:
-        """
-        set the description of this Condition sub-object
-
-        Parameters
-        ----------
-        new_descriptor : str
-            new description describing the Condition subobject
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, descriptor=new_descriptor)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def value(self) -> Optional[Union[Number, str]]:
-        """
-        value or quantity
-
-        Returns
-        -------
-        Union[Number, None]
-            new value or quantity
-        """
-        return self._json_attrs.value
-
-    def set_value(self, new_value: Union[Number, str], new_unit: str) -> None:
-        """
-        set the value for this Condition subobject
-
-        Parameters
-        ----------
-        new_value : Number
-            new value
-        new_unit : str
-            units for the new value
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.set_value(new_value=1, new_unit="gram")
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, value=new_value, unit=new_unit)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def unit(self) -> str:
-        """
-        set units for this Condition subobject
-
-        Returns
-        -------
-        unit: str
-            units
-        """
-        return self._json_attrs.unit
-
-    @property
-    @beartype
-    def uncertainty(self) -> Optional[Union[Number, str]]:
-        """
-        set uncertainty value for this Condition subobject
-
-        Returns
-        -------
-        uncertainty: Union[Number, None]
-            uncertainty
-        """
-        return self._json_attrs.uncertainty
-
-    @beartype
-    def set_uncertainty(self, new_uncertainty: Union[Number, str, None], new_uncertainty_type: str) -> None:
-        """
-        set uncertainty and uncertainty type
-
-        Parameters
-        ----------
-        new_uncertainty : Number
-            new uncertainty value
-        new_uncertainty_type : str
-            new uncertainty type
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.set_uncertainty(new_uncertainty=0.2, new_uncertainty_type="stdev")
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, uncertainty=new_uncertainty, uncertainty_type=new_uncertainty_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def uncertainty_type(self) -> str:
-        """
-        Uncertainty type for the uncertainty value
-
-        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type) must come from CRIPT controlled vocabulary
-
-        Returns
-        -------
-        uncertainty_type: str
-            uncertainty type
-        """
-        return self._json_attrs.uncertainty_type
-
-    @property
-    @beartype
-    def set_id(self) -> Union[int, None]:
-        """
-        ID of set (used to link measurements in as series)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.set_id = 0
-
-        Returns
-        -------
-        set_id: Union[int, None]
-            ID of set
-        """
-        return self._json_attrs.set_id
-
-    @set_id.setter
-    @beartype
-    def set_id(self, new_set_id: Union[int, None]) -> None:
-        """
-         set this Condition subobjects set_id
-
-        Parameters
-        ----------
-        new_set_id : Union[int, None]
-            ID of set
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, set_id=new_set_id)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def measurement_id(self) -> Union[int, None]:
-        """
-        ID for a single measurement (used to link multiple condition at a single instance)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.measurement_id = 0
-
-        Returns
-        -------
-        measurement_id: Union[int, None]
-            ID for a single measurement
-        """
-        return self._json_attrs.measurement_id
-
-    @measurement_id.setter
-    @beartype
-    def measurement_id(self, new_measurement_id: Union[int, None]) -> None:
-        """
-        set the set_id for this Condition subobject
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_condition.measurement_id = 1
-
-        Parameters
-        ----------
-        new_measurement_id : Union[int, None]
-            ID for a single measurement
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, measurement_id=new_measurement_id)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def data(self) -> List[Data]:
-        """
-        detailed data associated with the condition
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_condition = cript.Condition(
-        ...     key="temperature",
-        ...     type="value",
-        ...     value=22,
-        ...     unit="C",
-        ... )
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
-        ...     type="calibration",
-        ...     extension=".pdf",
-        ... )
-        >>> my_data = cript.Data(
-        ...     name="my data node name",
-        ...     type="afm_amp",
-        ...     file=[my_file],
-        ... )
-        >>> my_condition.data = [my_data]
-
-        Returns
-        -------
-        Condition: Union[Data, None]
-            detailed data associated with the condition
-        """
-        return self._json_attrs.data.copy()
-
-    @data.setter
-    @beartype
-    def data(self, new_data: List[Data]) -> None:
-        """
-        set the data node for this Condition Subobject
-
-        Parameters
-        ----------
-        new_data : List[Data]
-            new Data node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, data=new_data)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from numbers import Number
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.data import Data
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Condition(UUIDBaseNode):
+    """
+    ## Definition
+
+    A [Condition](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=21) sub-object
+    is the conditions under which the experiment was conducted.
+    Some examples include temperature, mixing_rate, stirring, time_duration.
+
+    ----
+
+    ## Can Be Added To:
+    ### Primary Nodes
+    * [Process](../../primary_nodes/process)
+    * [Computation_Process](../../primary_nodes/computation_process)
+
+    ### Subobjects
+    * [Property](../property)
+    * [Equipment](../equipment)
+
+    ---
+
+    ## Attributes
+
+    | attribute        | type   | example                 | description                                                                            | required | vocab |
+    |------------------|--------|-------------------------|----------------------------------------------------------------------------------------|----------|-------|
+    | key              | str    | temp                    | type of condition                                                                      | True     | True  |
+    | type             | str    | min                     | type of value stored, 'value' is just the number, 'min', 'max', 'avg', etc. for series | True     | True  |
+    | descriptor       | str    | upper temperature probe | freeform description for condition                                                     |          |       |
+    | value            | Number | 1.23                    | value or quantity                                                                      | True     |       |
+    | unit             | str    | gram                    | unit for value                                                                         |          |       |
+    | uncertainty      | Number | 0.1                     | uncertainty of value                                                                   |          |       |
+    | uncertainty_type | str    | std                     | type of uncertainty                                                                    |          | True  |
+    | set_id           | int    | 0                       | ID of set (used to link measurements in as series)                                     |          |       |
+    | measurement _id  | int    | 0                       | ID for a single measurement (used to link multiple condition at a single instance)     |          |       |
+    | data             | List[Data] |                         | detailed data associated with the condition                                            |          |       |
+
+    ## JSON Representation
+    ```json
+    {
+        "node": ["Condition"],
+        "key": "temperature",
+        "type": "value",
+        "descriptor": "room temperature of lab",
+        "value": 22,
+        "unit": "C",
+        "uncertainty": 5,
+        "uncertainty_type": "stdev",
+        "set_id": 0,
+        "measurement_id": 2,
+        "data": [{
+            "node":["Data"],
+            "name":"my data name",
+            "type":"afm_amp",
+            "file":[
+                {
+                    "node":["File"],
+                    "type":"calibration",
+                    "source":"https://criptapp.org",
+                    "extension":".csv",
+                    "data_dictionary":"my file's data dictionary"
+                }
+            ]
+        }],
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        type: str = ""
+        descriptor: str = ""
+        value: Optional[Union[Number, str]] = None
+        unit: str = ""
+        uncertainty: Optional[Union[Number, str]] = None
+        uncertainty_type: str = ""
+        set_id: Optional[int] = None
+        measurement_id: Optional[int] = None
+        data: List[Union[Data, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        key: str,
+        type: str,
+        value: Union[Number, str],
+        unit: str = "",
+        descriptor: str = "",
+        uncertainty: Optional[Union[Number, str]] = None,
+        uncertainty_type: str = "",
+        set_id: Optional[int] = None,
+        measurement_id: Optional[int] = None,
+        data: Optional[List[Union[Data, UIDProxy]]] = None,
+        **kwargs
+    ):
+        """
+        create Condition sub-object
+
+        Parameters
+        ----------
+        key : str
+            type of condition
+        type : str
+            type of value stored
+        value : Number
+            value or quantity
+        unit : str, optional
+            unit for value, by default ""
+        descriptor : str, optional
+            freeform description for condition, by default ""
+        uncertainty : Union[Number, None], optional
+           uncertainty of value, by default None
+        uncertainty_type : str, optional
+            type of uncertainty, by default ""
+        set_id : Union[int, None], optional
+            ID of set (used to link measurements in as series), by default None
+        measurement_id : Union[int, None], optional
+            ID for a single measurement (used to link multiple condition at a single instance), by default None
+        data : List[Data], optional
+            detailed data associated with the condition, by default None
+
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+
+        Returns
+        -------
+        None
+        """
+        super().__init__(**kwargs)
+
+        if data is None:
+            data = []
+
+        new_json_attrs = replace(
+            self._json_attrs,
+            key=key,
+            type=type,
+            value=value,
+            descriptor=descriptor,
+            unit=unit,
+            uncertainty=uncertainty,
+            uncertainty_type=uncertainty_type,
+            set_id=set_id,
+            measurement_id=measurement_id,
+            data=data,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        type of condition
+
+        > Condition key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/condition_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.key = "energy_threshold"
+
+        Returns
+        -------
+        condition key: str
+            type of condition
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    @beartype
+    def key(self, new_key: str) -> None:
+        """
+        set this Condition sub-object key
+
+        Parameters
+        ----------
+        new_key : str
+            type of condition
+
+        Returns
+        --------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        description for the value stored for this Condition node
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.type = "min"
+
+        Returns
+        -------
+        condition type: str
+            description for the value
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_type: str) -> None:
+        """
+        set the type attribute for this Condition node
+
+        Parameters
+        ----------
+        new_type : str
+            new description of the Condition value
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def descriptor(self) -> str:
+        """
+        freeform description for Condition
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.descriptor = "my condition description"
+
+        Returns
+        -------
+        description: str
+            description of this Condition sub-object
+        """
+        return self._json_attrs.descriptor
+
+    @descriptor.setter
+    @beartype
+    def descriptor(self, new_descriptor: str) -> None:
+        """
+        set the description of this Condition sub-object
+
+        Parameters
+        ----------
+        new_descriptor : str
+            new description describing the Condition subobject
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, descriptor=new_descriptor)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def value(self) -> Optional[Union[Number, str]]:
+        """
+        value or quantity
+
+        Returns
+        -------
+        Union[Number, None]
+            new value or quantity
+        """
+        return self._json_attrs.value
+
+    def set_value(self, new_value: Union[Number, str], new_unit: str) -> None:
+        """
+        set the value for this Condition subobject
+
+        Parameters
+        ----------
+        new_value : Number
+            new value
+        new_unit : str
+            units for the new value
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.set_value(new_value=1, new_unit="gram")
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, value=new_value, unit=new_unit)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def unit(self) -> str:
+        """
+        set units for this Condition subobject
+
+        Returns
+        -------
+        unit: str
+            units
+        """
+        return self._json_attrs.unit
+
+    @property
+    @beartype
+    def uncertainty(self) -> Optional[Union[Number, str]]:
+        """
+        set uncertainty value for this Condition subobject
+
+        Returns
+        -------
+        uncertainty: Union[Number, None]
+            uncertainty
+        """
+        return self._json_attrs.uncertainty
+
+    @beartype
+    def set_uncertainty(self, new_uncertainty: Union[Number, str, None], new_uncertainty_type: str) -> None:
+        """
+        set uncertainty and uncertainty type
+
+        Parameters
+        ----------
+        new_uncertainty : Number
+            new uncertainty value
+        new_uncertainty_type : str
+            new uncertainty type
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.set_uncertainty(new_uncertainty=0.2, new_uncertainty_type="stdev")
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, uncertainty=new_uncertainty, uncertainty_type=new_uncertainty_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def uncertainty_type(self) -> str:
+        """
+        Uncertainty type for the uncertainty value
+
+        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type) must come from CRIPT controlled vocabulary
+
+        Returns
+        -------
+        uncertainty_type: str
+            uncertainty type
+        """
+        return self._json_attrs.uncertainty_type
+
+    @property
+    @beartype
+    def set_id(self) -> Union[int, None]:
+        """
+        ID of set (used to link measurements in as series)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.set_id = 0
+
+        Returns
+        -------
+        set_id: Union[int, None]
+            ID of set
+        """
+        return self._json_attrs.set_id
+
+    @set_id.setter
+    @beartype
+    def set_id(self, new_set_id: Union[int, None]) -> None:
+        """
+         set this Condition subobjects set_id
+
+        Parameters
+        ----------
+        new_set_id : Union[int, None]
+            ID of set
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, set_id=new_set_id)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def measurement_id(self) -> Union[int, None]:
+        """
+        ID for a single measurement (used to link multiple condition at a single instance)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.measurement_id = 0
+
+        Returns
+        -------
+        measurement_id: Union[int, None]
+            ID for a single measurement
+        """
+        return self._json_attrs.measurement_id
+
+    @measurement_id.setter
+    @beartype
+    def measurement_id(self, new_measurement_id: Union[int, None]) -> None:
+        """
+        set the set_id for this Condition subobject
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_condition.measurement_id = 1
+
+        Parameters
+        ----------
+        new_measurement_id : Union[int, None]
+            ID for a single measurement
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, measurement_id=new_measurement_id)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def data(self) -> List[Union[Data, UIDProxy]]:
+        """
+        detailed data associated with the condition
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_condition = cript.Condition(
+        ...     key="temperature",
+        ...     type="value",
+        ...     value=22,
+        ...     unit="C",
+        ... )
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
+        ...     type="calibration",
+        ...     extension=".pdf",
+        ... )
+        >>> my_data = cript.Data(
+        ...     name="my data node name",
+        ...     type="afm_amp",
+        ...     file=[my_file],
+        ... )
+        >>> my_condition.data = [my_data]
+
+        Returns
+        -------
+        Condition: Union[Data, None]
+            detailed data associated with the condition
+        """
+        return self._json_attrs.data.copy()
+
+    @data.setter
+    @beartype
+    def data(self, new_data: List[Union[Data, UIDProxy]]) -> None:
+        """
+        set the data node for this Condition Subobject
+
+        Parameters
+        ----------
+        new_data : List[Data]
+            new Data node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, data=new_data)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/parameter.py` & `cript-2.3.0/src/cript/nodes/subobjects/parameter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-from dataclasses import dataclass, replace
-from numbers import Number
-from typing import Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Parameter(UUIDBaseNode):
-    """
-    ## Definition
-
-    A [parameter](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=25)
-    is an input value to an algorithm.
-
-    ??? note "Difference between `Parameter` and `Condition`"
-        For typical computations, the difference between
-        parameter and condition lies in whether it changes the thermodynamic state of the simulated
-        system: Variables that are part of defining a thermodynamic state should be defined as a condition
-        in a parent node.
-
-        Therefore, `number` and `volume` need to be listed as conditions while
-        `boundaries` and `origin` are parameters of ensemble size
-
-    ---
-    ## Can Be Added To:
-    * [Algorithm sub-object](../algorithm)
-
-    ## Available sub-objects:
-    * None
-
-    ---
-
-    ## Attributes
-
-    | attribute | type | example | description        | required | vocab |
-    |-----------|------|---------|--------------------|----------|-------|
-    | key       | str  |         | key for identifier | True     | True  |
-    | value     | Any  |         | value              | True     |       |
-    | unit      | str  |         | unit for parameter |          |       |
-
-
-    ## JSON Representation
-    ```json
-    {
-       "key":"update_frequency",
-       "node":["Parameter"],
-       "unit":"1/second",
-       "value":1000.0
-       "uid":"_:6af3b3aa-1dbc-4ce7-be8b-1896b375001c",
-       "uuid":"6af3b3aa-1dbc-4ce7-be8b-1896b375001c",
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        value: Optional[Number] = None
-        # We explicitly allow None for unit here (instead of empty str),
-        # this presents number without physical unit, like counting
-        # particles or dimensionless numbers.
-        unit: Union[str, None] = None
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    # Note that the key word args are ignored.
-    # They are just here, such that we can feed more kwargs in that we get from the back end.
-    @beartype
-    def __init__(self, key: str, value: Number, unit: Optional[str] = None, **kwargs):
-        """
-        create new Parameter sub-object
-
-        Parameters
-        ----------
-        key : str
-            Parameter key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/parameter_key)
-        value : Union[int, float]
-            Parameter value
-        unit : Union[str, None], optional
-            Parameter unit, by default None
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
-
-        Returns
-        -------
-        None
-            create Parameter sub-object
-        """
-        super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, key=key, value=value, unit=unit)
-        self.validate()
-
-    @classmethod
-    def _from_json(cls, json_dict: dict):
-        # TODO: remove this temporary fix, once back end is working correctly
-        try:
-            json_dict["value"] = float(json_dict["value"])
-        except KeyError:
-            pass
-        return super(Parameter, cls)._from_json(json_dict)
-
-    @property
-    @beartype
-    def key(self) -> str:
-        """
-        Parameter key must come from the [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/parameter_key)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
-        >>> my_parameter.key = "damping_time"
-
-        Returns
-        -------
-        str
-            parameter key
-        """
-        return self._json_attrs.key
-
-    @key.setter
-    @beartype
-    def key(self, new_key: str) -> None:
-        """
-        set new key for the Parameter sub-object
-
-        Parameters
-        ----------
-        new_key : str
-            new Parameter key
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, key=new_key)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def value(self) -> Optional[Number]:
-        """
-        Parameter value
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
-        >>> my_parameter.value = 1
-
-        Returns
-        -------
-        Union[int, float, str]
-            parameter value
-        """
-        return self._json_attrs.value
-
-    @value.setter
-    @beartype
-    def value(self, new_value: Number) -> None:
-        """
-        set the Parameter value
-
-        Parameters
-        ----------
-        new_value : Union[int, float, str]
-            new parameter value
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, value=new_value)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def unit(self) -> Union[str, None]:
-        """
-        Parameter unit
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
-        >>> my_parameter.unit = "gram"
-
-        Returns
-        -------
-        str
-            parameter unit
-        """
-        return self._json_attrs.unit
-
-    @unit.setter
-    @beartype
-    def unit(self, new_unit: str) -> None:
-        """
-        set the unit attribute for the Parameter sub-object
-
-        Parameters
-        ----------
-        new_unit : str
-            new Parameter unit
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, unit=new_unit)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, replace
+from numbers import Number
+from typing import Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Parameter(UUIDBaseNode):
+    """
+    ## Definition
+
+    A [parameter](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=25)
+    is an input value to an algorithm.
+
+    ??? note "Difference between `Parameter` and `Condition`"
+        For typical computations, the difference between
+        parameter and condition lies in whether it changes the thermodynamic state of the simulated
+        system: Variables that are part of defining a thermodynamic state should be defined as a condition
+        in a parent node.
+
+        Therefore, `number` and `volume` need to be listed as conditions while
+        `boundaries` and `origin` are parameters of ensemble size
+
+    ---
+    ## Can Be Added To:
+    * [Algorithm sub-object](../algorithm)
+
+    ## Available sub-objects:
+    * None
+
+    ---
+
+    ## Attributes
+
+    | attribute | type | example | description        | required | vocab |
+    |-----------|------|---------|--------------------|----------|-------|
+    | key       | str  |         | key for identifier | True     | True  |
+    | value     | Any  |         | value              | True     |       |
+    | unit      | str  |         | unit for parameter |          |       |
+
+
+    ## JSON Representation
+    ```json
+    {
+       "key":"update_frequency",
+       "node":["Parameter"],
+       "unit":"1/second",
+       "value":1000.0
+       "uid":"_:6af3b3aa-1dbc-4ce7-be8b-1896b375001c",
+       "uuid":"6af3b3aa-1dbc-4ce7-be8b-1896b375001c",
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        value: Optional[Number] = None
+        # We explicitly allow None for unit here (instead of empty str),
+        # this presents number without physical unit, like counting
+        # particles or dimensionless numbers.
+        unit: Union[str, None] = None
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    # Note that the key word args are ignored.
+    # They are just here, such that we can feed more kwargs in that we get from the back end.
+    @beartype
+    def __init__(self, key: str, value: Number, unit: Optional[str] = None, **kwargs):
+        """
+        create new Parameter sub-object
+
+        Parameters
+        ----------
+        key : str
+            Parameter key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/parameter_key)
+        value : Union[int, float]
+            Parameter value
+        unit : Union[str, None], optional
+            Parameter unit, by default None
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
+
+        Returns
+        -------
+        None
+            create Parameter sub-object
+        """
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, key=key, value=value, unit=unit)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @classmethod
+    def _from_json(cls, json_dict: dict):
+        # TODO: remove this temporary fix, once back end is working correctly
+        try:
+            json_dict["value"] = float(json_dict["value"])
+        except KeyError:
+            pass
+        return super(Parameter, cls)._from_json(json_dict)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        Parameter key must come from the [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/parameter_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
+        >>> my_parameter.key = "damping_time"
+
+        Returns
+        -------
+        str
+            parameter key
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    @beartype
+    def key(self, new_key: str) -> None:
+        """
+        set new key for the Parameter sub-object
+
+        Parameters
+        ----------
+        new_key : str
+            new Parameter key
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def value(self) -> Optional[Number]:
+        """
+        Parameter value
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
+        >>> my_parameter.value = 1
+
+        Returns
+        -------
+        Union[int, float, str]
+            parameter value
+        """
+        return self._json_attrs.value
+
+    @value.setter
+    @beartype
+    def value(self, new_value: Number) -> None:
+        """
+        set the Parameter value
+
+        Parameters
+        ----------
+        new_value : Union[int, float, str]
+            new parameter value
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, value=new_value)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def unit(self) -> Union[str, None]:
+        """
+        Parameter unit
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_parameter = cript.Parameter("update_frequency", 1000.0, "1/second")
+        >>> my_parameter.unit = "gram"
+
+        Returns
+        -------
+        str
+            parameter unit
+        """
+        return self._json_attrs.unit
+
+    @unit.setter
+    @beartype
+    def unit(self, new_unit: str) -> None:
+        """
+        set the unit attribute for the Parameter sub-object
+
+        Parameters
+        ----------
+        new_unit : str
+            new Parameter unit
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, unit=new_unit)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/property.py` & `cript-2.3.0/src/cript/nodes/subobjects/property.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,735 +1,736 @@
-from dataclasses import dataclass, field, replace
-from numbers import Number
-from typing import List, Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.computation import Computation
-from cript.nodes.primary_nodes.data import Data
-from cript.nodes.primary_nodes.material import Material
-from cript.nodes.primary_nodes.process import Process
-from cript.nodes.subobjects.citation import Citation
-from cript.nodes.subobjects.condition import Condition
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Property(UUIDBaseNode):
-    """
-    ## Definition
-    [Property](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=18)
-    sub-objects are qualities/traits of a [material](../../primary_nodes/material) or
-    [Process](../../primary_nodes/process)
-
-    ---
-
-    ## Can Be Added To:
-    * [Material](../../primary_nodes/material)
-    * [Process](../../primary_nodes/process)
-    * [Computation_Process](../../primary_nodes/computation_process)
-
-    ## Available sub-objects:
-    * [Condition](../condition)
-    * [Citation](../citation)
-
-    ---
-
-    ## Attributes
-
-    | attribute          | type              | example                                 | description                                                                  | required | vocab |
-    |--------------------|-------------------|-----------------------------------------|------------------------------------------------------------------------------|----------|-------|
-    | key                | str               | modulus_shear                           | type of property                                                             | True     | True  |
-    | type               | str               | min                                     | type of value stored                                                         | True     | True  |
-    | value              | Any               | 1.23                                    | value or quantity                                                            | True     |       |
-    | unit               | str               | gram                                    | unit for value                                                               | True     |       |
-    | uncertainty        | Number            | 0.1                                     | uncertainty of value                                                         |          |       |
-    | uncertainty_type   | str               | standard_deviation                      | type of uncertainty                                                          |          | True  |
-    | component          | list[Material]    |                                         | material that the property relates to**                                      |          |       |
-    | structure          | str               | {\\[\\]\\[$\\]\\[C:1\\]\\[C:1\\]\\[$\\] | specific chemical structure associate with the property with atom mappings** |          |       |
-    | method             | str               | sec                                     | approach or source of property data                                          |          | True  |
-    | sample_preparation | Process           |                                         | sample preparation                                                           |          |       |
-    | condition          | list[Condition]   |                                         | conditions under which the property was measured                             |          |       |
-    | data               | Data              |                                         | data node                                                                    |          |       |
-    | computation        | list[Computation] |                                         | computation method that produced property                                    |          |       |
-    | citation           | list[Citation]    |                                         | reference to a book, paper, or scholarly work                                |          |       |
-    | notes              | str               |                                         | miscellaneous information, or custom data structure (e.g.; JSON)             |          |       |
-
-
-    ## JSON Representation
-    ```json
-    {
-       "key":"modulus_shear",
-       "node":["Property"],
-       "type":"value",
-       "unit":"GPa",
-       "value":5.0
-       "uid":"_:bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
-       "uuid":"bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        type: str = ""
-        value: Union[Number, str, None] = None
-        unit: Optional[str] = ""
-        uncertainty: Optional[Number] = None
-        uncertainty_type: str = ""
-        component: List[Material] = field(default_factory=list)
-        structure: str = ""
-        method: str = ""
-        sample_preparation: Optional[Process] = None
-        condition: List[Condition] = field(default_factory=list)
-        data: List[Data] = field(default_factory=list)
-        computation: List[Computation] = field(default_factory=list)
-        citation: List[Citation] = field(default_factory=list)
-        notes: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(
-        self,
-        key: str,
-        type: str,
-        value: Union[Number, str, None],
-        unit: Union[str, None],
-        uncertainty: Optional[Number] = None,
-        uncertainty_type: str = "",
-        component: Optional[List[Material]] = None,
-        structure: str = "",
-        method: str = "",
-        sample_preparation: Optional[Process] = None,
-        condition: Optional[List[Condition]] = None,
-        data: Optional[List[Data]] = None,
-        computation: Optional[List[Computation]] = None,
-        citation: Optional[List[Citation]] = None,
-        notes: str = "",
-        **kwargs
-    ):
-        """
-        create a property sub-object
-
-        Parameters
-        ----------
-        key : str
-            type of property, Property key must come from the CRIPT Controlled Vocabulary
-        type : str
-            type of value stored, Property type must come from the CRIPT Controlled Vocabulary
-        value : Union[Number, None]
-            value or quantity
-        unit : str
-            unit for value
-        uncertainty : Union[Number, None], optional
-            uncertainty value of the value, by default None
-        uncertainty_type : str, optional
-            type of uncertainty, by default ""
-        component : Union[List[Material], None], optional
-            List of Material nodes, by default None
-        structure : str, optional
-            specific chemical structure associate with the property with atom mappings**, by default ""
-        method : str, optional
-            approach or source of property data, by default ""
-        sample_preparation : Union[Process, None], optional
-            sample preparation, by default None
-        condition : Union[List[Condition], None], optional
-            conditions under which the property was measured, by default None
-        data : Union[List[Data], None], optional
-            Data node, by default None
-        computation : Union[List[Computation], None], optional
-            computation method that produced property, by default None
-        citation : Union[List[Citation], None], optional
-            reference scholarly work, by default None
-        notes : str, optional
-            miscellaneous information, or custom data structure (e.g.; JSON), by default ""
-
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-
-        Returns
-        -------
-        None
-            create a Property sub-object
-        """
-        if component is None:
-            component = []
-        if condition is None:
-            condition = []
-        if computation is None:
-            computation = []
-        if data is None:
-            data = []
-        if citation is None:
-            citation = []
-
-        super().__init__(**kwargs)
-        self._json_attrs = replace(
-            self._json_attrs,
-            key=key,
-            type=type,
-            value=value,
-            unit=unit,
-            uncertainty=uncertainty,
-            uncertainty_type=uncertainty_type,
-            component=component,
-            structure=structure,
-            method=method,
-            sample_preparation=sample_preparation,
-            condition=condition,
-            data=data,
-            computation=computation,
-            citation=citation,
-            notes=notes,
-        )
-        self.validate()
-
-    @property
-    @beartype
-    def key(self) -> str:
-        """
-        Property key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.key = "angle_rdist"
-
-        Returns
-        -------
-        str
-            Property Key
-        """
-        return self._json_attrs.key
-
-    @key.setter
-    @beartype
-    def key(self, new_key: str) -> None:
-        """
-        set the key for this Property sub-object
-
-        Parameters
-        ----------
-        new_key : str
-            new Property key
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, key=new_key)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        type of value for this Property sub-object
-
-        [property type](https://app.criptapp.org/vocab/) must come from CRIPT controlled vocabulary
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.type = "max"
-
-        Returns
-        -------
-        str
-            type of value for this Property sub-object
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_type: str) -> None:
-        """
-        set the Property type for this subobject
-
-        Parameters
-        ----------
-        new_type : str
-            new Property type
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def value(self) -> Union[Number, str, None]:
-        """
-        get the Property value
-
-        Returns
-        -------
-        Union[Number, None]
-            Property value
-        """
-        return self._json_attrs.value
-
-    @beartype
-    def set_value(self, new_value: Union[Number, str, None], new_unit: str) -> None:
-        """
-        set the value attribute of the Property subobject
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.set_value(new_value=1, new_unit="gram")
-
-        Parameters
-        ----------
-        new_value : Number
-            new value
-        new_unit : str
-            new unit for the value
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, value=new_value, unit=new_unit)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def unit(self) -> Optional[str]:
-        """
-        get the Property unit for the value
-
-        Returns
-        -------
-        str
-            unit
-        """
-        return self._json_attrs.unit
-
-    @property
-    @beartype
-    def uncertainty(self) -> Union[Number, None]:
-        """
-        get the uncertainty value of the Property node
-
-        Returns
-        -------
-        Union[Number, None]
-            uncertainty value
-        """
-        return self._json_attrs.uncertainty
-
-    @beartype
-    def set_uncertainty(self, new_uncertainty: Optional[Number], new_uncertainty_type: str) -> None:
-        """
-        set the uncertainty value and type
-
-        Uncertainty type must come from [CRIPT Controlled Vocabulary]
-
-        Parameters
-        ----------
-        new_uncertainty : Number
-            new uncertainty value
-        new_uncertainty_type : str
-            new uncertainty type
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.set_uncertainty(new_uncertainty=2, new_uncertainty_type="fwhm")
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, uncertainty=new_uncertainty, uncertainty_type=new_uncertainty_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def uncertainty_type(self) -> str:
-        """
-        get the uncertainty_type for this Property subobject
-
-        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type)
-        must come from CRIPT Controlled Vocabulary
-
-        Returns
-        -------
-        str
-            Uncertainty type
-        """
-        return self._json_attrs.uncertainty_type
-
-    @property
-    @beartype
-    def component(self) -> List[Material]:
-        """
-        list of Materials that the Property relates to
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_material = cript.Material(name="my material", identifier=[{"bigsmiles": "123456"}])
-        >>> my_property.component = [my_material]
-
-        Returns
-        -------
-        List[Material]
-            list of Materials that the Property relates to
-        """
-        return self._json_attrs.component.copy()
-
-    @component.setter
-    @beartype
-    def component(self, new_component: List[Material]) -> None:
-        """
-        set the list of Materials as components for the Property subobject
-
-        Parameters
-        ----------
-        new_component : List[Material]
-            new list of Materials to for the Property subobject
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, component=new_component)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def structure(self) -> str:
-        """
-        specific chemical structure associate with the property with atom mappings
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.structure = "{[][$][C:1][C:1][$],[$][C:2][C:2]([C:2])[$][]}"
-
-        Returns
-        -------
-        str
-            Property structure string
-        """
-        return self._json_attrs.structure
-
-    @structure.setter
-    @beartype
-    def structure(self, new_structure: str) -> None:
-        """
-        set the this Property's structure
-
-        Parameters
-        ----------
-        new_structure : str
-            new structure
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, structure=new_structure)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def method(self) -> str:
-        """
-        approach or source of property data True sample_preparation Process sample preparation
-
-        [Property method](https://app.criptapp.org/vocab/property_method) must come from CRIPT Controlled Vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.method = "ASTM_D3574_Test_A"
-
-        Returns
-        -------
-        str
-            Property method
-        """
-        return self._json_attrs.method
-
-    @method.setter
-    @beartype
-    def method(self, new_method: str) -> None:
-        """
-        set the Property method
-
-        Parameters
-        ----------
-        new_method : str
-            new Property method
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, method=new_method)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def sample_preparation(self) -> Union[Process, None]:
-        """
-        sample_preparation
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
-        >>> my_property.sample_preparation = my_process
-
-        Returns
-        -------
-        Union[Process, None]
-            Property linking back to the Process that has it as subobject
-        """
-        return self._json_attrs.sample_preparation
-
-    @sample_preparation.setter
-    @beartype
-    def sample_preparation(self, new_sample_preparation: Union[Process, None]) -> None:
-        """
-        set the sample_preparation for the Property subobject
-
-        Parameters
-        ----------
-        new_sample_preparation : Union[Process, None]
-            back link to the Process that has this Property as its subobject
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, sample_preparation=new_sample_preparation)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def condition(self) -> List[Condition]:
-        """
-        list of Conditions under which the property was measured
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_condition = cript.Condition(key="atm", type="max", value=1)
-        >>> my_property.condition = [my_condition]
-
-        Returns
-        -------
-        List[Condition]
-            list of Conditions
-        """
-        return self._json_attrs.condition.copy()
-
-    @condition.setter
-    @beartype
-    def condition(self, new_condition: List[Condition]) -> None:
-        """
-        set the list of Conditions for this property subobject
-
-        Parameters
-        ----------
-        new_condition : List[Condition]
-            new list of Condition Subobjects
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, condition=new_condition)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def data(self) -> List[Data]:
-        """
-        List of Data nodes for this Property subobjects
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary",
-        ... )
-        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
-        >>> my_property.data = [my_data]
-
-        Returns
-        -------
-        List[Data]
-            list of Data nodes
-        """
-        return self._json_attrs.data.copy()
-
-    @data.setter
-    @beartype
-    def data(self, new_data: List[Data]) -> None:
-        """
-        set the Data node for the Property subobject
-
-        Parameters
-        ----------
-        new_data : List[Data]
-            new list of Data nodes
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, data=new_data)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def computation(self) -> List[Computation]:
-        """
-        list of Computation nodes that produced this property
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
-        >>> my_property.computation = [my_computation]
-
-        Returns
-        -------
-        List[Computation]
-            list of Computation nodes
-        """
-        return self._json_attrs.computation.copy()
-
-    @computation.setter
-    @beartype
-    def computation(self, new_computation: List[Computation]) -> None:
-        """
-        set the list of Computation nodes that produced this property
-
-        Parameters
-        ----------
-        new_computation : List[Computation]
-            new list of Computation nodes
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, computation=new_computation)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Citation]:
-        """
-        list of Citation subobjects for this Property subobject
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
-        >>> my_property.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of Citation subobjects for this Property subobject
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation: List[Citation]) -> None:
-        """
-        set the list of Citation subobjects for the Property subobject
-
-        Parameters
-        ----------
-        new_citation : List[Citation]
-            new list of Citation subobjects
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def notes(self) -> str:
-        """
-        notes for this Property subobject
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
-        >>> my_property.notes = "these are my notes"
-
-        Returns
-        -------
-        str
-            notes for this property subobject
-        """
-        return self._json_attrs.notes
-
-    @notes.setter
-    @beartype
-    def notes(self, new_notes: str) -> None:
-        """
-        set the notes for this Property sub-object
-
-        Parameters
-        ----------
-        new_notes : str
-            new notes
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, notes=new_notes)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from numbers import Number
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.computation import Computation
+from cript.nodes.primary_nodes.data import Data
+from cript.nodes.primary_nodes.material import Material
+from cript.nodes.primary_nodes.process import Process
+from cript.nodes.subobjects.citation import Citation
+from cript.nodes.subobjects.condition import Condition
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Property(UUIDBaseNode):
+    """
+    ## Definition
+    [Property](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=18)
+    sub-objects are qualities/traits of a [material](../../primary_nodes/material) or
+    [Process](../../primary_nodes/process)
+
+    ---
+
+    ## Can Be Added To:
+    * [Material](../../primary_nodes/material)
+    * [Process](../../primary_nodes/process)
+    * [Computation_Process](../../primary_nodes/computation_process)
+
+    ## Available sub-objects:
+    * [Condition](../condition)
+    * [Citation](../citation)
+
+    ---
+
+    ## Attributes
+
+    | attribute          | type              | example                                 | description                                                                  | required | vocab |
+    |--------------------|-------------------|-----------------------------------------|------------------------------------------------------------------------------|----------|-------|
+    | key                | str               | modulus_shear                           | type of property                                                             | True     | True  |
+    | type               | str               | min                                     | type of value stored                                                         | True     | True  |
+    | value              | Any               | 1.23                                    | value or quantity                                                            | True     |       |
+    | unit               | str               | gram                                    | unit for value                                                               | True     |       |
+    | uncertainty        | Number            | 0.1                                     | uncertainty of value                                                         |          |       |
+    | uncertainty_type   | str               | standard_deviation                      | type of uncertainty                                                          |          | True  |
+    | component          | list[Material]    |                                         | material that the property relates to**                                      |          |       |
+    | structure          | str               | {\\[\\]\\[$\\]\\[C:1\\]\\[C:1\\]\\[$\\] | specific chemical structure associate with the property with atom mappings** |          |       |
+    | method             | str               | sec                                     | approach or source of property data                                          |          | True  |
+    | sample_preparation | Process           |                                         | sample preparation                                                           |          |       |
+    | condition          | list[Condition]   |                                         | conditions under which the property was measured                             |          |       |
+    | data               | Data              |                                         | data node                                                                    |          |       |
+    | computation        | list[Computation] |                                         | computation method that produced property                                    |          |       |
+    | citation           | list[Citation]    |                                         | reference to a book, paper, or scholarly work                                |          |       |
+    | notes              | str               |                                         | miscellaneous information, or custom data structure (e.g.; JSON)             |          |       |
+
+
+    ## JSON Representation
+    ```json
+    {
+       "key":"modulus_shear",
+       "node":["Property"],
+       "type":"value",
+       "unit":"GPa",
+       "value":5.0
+       "uid":"_:bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
+       "uuid":"bc3abb68-25b5-4144-aa1b-85d82b7c77e1",
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        type: str = ""
+        value: Union[Number, str, None] = None
+        unit: Optional[str] = ""
+        uncertainty: Optional[Number] = None
+        uncertainty_type: str = ""
+        component: List[Union[Material, UIDProxy]] = field(default_factory=list)
+        structure: str = ""
+        method: str = ""
+        sample_preparation: Optional[Union[Process, UIDProxy]] = None
+        condition: List[Union[Condition, UIDProxy]] = field(default_factory=list)
+        data: List[Union[Data, UIDProxy]] = field(default_factory=list)
+        computation: List[Union[Computation, UIDProxy]] = field(default_factory=list)
+        citation: List[Union[Citation, UIDProxy]] = field(default_factory=list)
+        notes: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(
+        self,
+        key: str,
+        type: str,
+        value: Union[Number, str, None],
+        unit: Union[str, None],
+        uncertainty: Optional[Number] = None,
+        uncertainty_type: str = "",
+        component: Optional[List[Union[Material, UIDProxy]]] = None,
+        structure: str = "",
+        method: str = "",
+        sample_preparation: Optional[Union[Process, UIDProxy]] = None,
+        condition: Optional[List[Union[Condition, UIDProxy]]] = None,
+        data: Optional[List[Union[Data, UIDProxy]]] = None,
+        computation: Optional[List[Union[Computation, UIDProxy]]] = None,
+        citation: Optional[List[Union[Citation, UIDProxy]]] = None,
+        notes: str = "",
+        **kwargs
+    ):
+        """
+        create a property sub-object
+
+        Parameters
+        ----------
+        key : str
+            type of property, Property key must come from the CRIPT Controlled Vocabulary
+        type : str
+            type of value stored, Property type must come from the CRIPT Controlled Vocabulary
+        value : Union[Number, None]
+            value or quantity
+        unit : str
+            unit for value
+        uncertainty : Union[Number, None], optional
+            uncertainty value of the value, by default None
+        uncertainty_type : str, optional
+            type of uncertainty, by default ""
+        component : Union[List[Material], None], optional
+            List of Material nodes, by default None
+        structure : str, optional
+            specific chemical structure associate with the property with atom mappings**, by default ""
+        method : str, optional
+            approach or source of property data, by default ""
+        sample_preparation : Union[Process, None], optional
+            sample preparation, by default None
+        condition : Union[List[Condition], None], optional
+            conditions under which the property was measured, by default None
+        data : Union[List[Data], None], optional
+            Data node, by default None
+        computation : Union[List[Computation], None], optional
+            computation method that produced property, by default None
+        citation : Union[List[Citation], None], optional
+            reference scholarly work, by default None
+        notes : str, optional
+            miscellaneous information, or custom data structure (e.g.; JSON), by default ""
+
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+
+        Returns
+        -------
+        None
+            create a Property sub-object
+        """
+        if component is None:
+            component = []
+        if condition is None:
+            condition = []
+        if computation is None:
+            computation = []
+        if data is None:
+            data = []
+        if citation is None:
+            citation = []
+
+        super().__init__(**kwargs)
+        new_json_attrs = replace(
+            self._json_attrs,
+            key=key,
+            type=type,
+            value=value,
+            unit=unit,
+            uncertainty=uncertainty,
+            uncertainty_type=uncertainty_type,
+            component=component,
+            structure=structure,
+            method=method,
+            sample_preparation=sample_preparation,
+            condition=condition,
+            data=data,
+            computation=computation,
+            citation=citation,
+            notes=notes,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        Property key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.key = "angle_rdist"
+
+        Returns
+        -------
+        str
+            Property Key
+        """
+        return self._json_attrs.key
+
+    @key.setter
+    @beartype
+    def key(self, new_key: str) -> None:
+        """
+        set the key for this Property sub-object
+
+        Parameters
+        ----------
+        new_key : str
+            new Property key
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        type of value for this Property sub-object
+
+        [property type](https://app.criptapp.org/vocab/) must come from CRIPT controlled vocabulary
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.type = "max"
+
+        Returns
+        -------
+        str
+            type of value for this Property sub-object
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_type: str) -> None:
+        """
+        set the Property type for this subobject
+
+        Parameters
+        ----------
+        new_type : str
+            new Property type
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def value(self) -> Union[Number, str, None]:
+        """
+        get the Property value
+
+        Returns
+        -------
+        Union[Number, None]
+            Property value
+        """
+        return self._json_attrs.value
+
+    @beartype
+    def set_value(self, new_value: Union[Number, str, None], new_unit: str) -> None:
+        """
+        set the value attribute of the Property subobject
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.set_value(new_value=1, new_unit="gram")
+
+        Parameters
+        ----------
+        new_value : Number
+            new value
+        new_unit : str
+            new unit for the value
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, value=new_value, unit=new_unit)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def unit(self) -> Optional[str]:
+        """
+        get the Property unit for the value
+
+        Returns
+        -------
+        str
+            unit
+        """
+        return self._json_attrs.unit
+
+    @property
+    @beartype
+    def uncertainty(self) -> Union[Number, None]:
+        """
+        get the uncertainty value of the Property node
+
+        Returns
+        -------
+        Union[Number, None]
+            uncertainty value
+        """
+        return self._json_attrs.uncertainty
+
+    @beartype
+    def set_uncertainty(self, new_uncertainty: Optional[Number], new_uncertainty_type: str) -> None:
+        """
+        set the uncertainty value and type
+
+        Uncertainty type must come from [CRIPT Controlled Vocabulary]
+
+        Parameters
+        ----------
+        new_uncertainty : Number
+            new uncertainty value
+        new_uncertainty_type : str
+            new uncertainty type
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.set_uncertainty(new_uncertainty=2, new_uncertainty_type="fwhm")
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, uncertainty=new_uncertainty, uncertainty_type=new_uncertainty_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def uncertainty_type(self) -> str:
+        """
+        get the uncertainty_type for this Property subobject
+
+        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type)
+        must come from CRIPT Controlled Vocabulary
+
+        Returns
+        -------
+        str
+            Uncertainty type
+        """
+        return self._json_attrs.uncertainty_type
+
+    @property
+    @beartype
+    def component(self) -> List[Union[Material, UIDProxy]]:
+        """
+        list of Materials that the Property relates to
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_material = cript.Material(name="my material", bigsmiles = "123456")
+        >>> my_property.component = [my_material]
+
+        Returns
+        -------
+        List[Material]
+            list of Materials that the Property relates to
+        """
+        return self._json_attrs.component.copy()
+
+    @component.setter
+    @beartype
+    def component(self, new_component: List[Union[Material, UIDProxy]]) -> None:
+        """
+        set the list of Materials as components for the Property subobject
+
+        Parameters
+        ----------
+        new_component : List[Material]
+            new list of Materials to for the Property subobject
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, component=new_component)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def structure(self) -> str:
+        """
+        specific chemical structure associate with the property with atom mappings
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.structure = "{[][$][C:1][C:1][$],[$][C:2][C:2]([C:2])[$][]}"
+
+        Returns
+        -------
+        str
+            Property structure string
+        """
+        return self._json_attrs.structure
+
+    @structure.setter
+    @beartype
+    def structure(self, new_structure: str) -> None:
+        """
+        set the this Property's structure
+
+        Parameters
+        ----------
+        new_structure : str
+            new structure
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, structure=new_structure)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def method(self) -> str:
+        """
+        approach or source of property data True sample_preparation Process sample preparation
+
+        [Property method](https://app.criptapp.org/vocab/property_method) must come from CRIPT Controlled Vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.method = "ASTM_D3574_Test_A"
+
+        Returns
+        -------
+        str
+            Property method
+        """
+        return self._json_attrs.method
+
+    @method.setter
+    @beartype
+    def method(self, new_method: str) -> None:
+        """
+        set the Property method
+
+        Parameters
+        ----------
+        new_method : str
+            new Property method
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, method=new_method)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def sample_preparation(self) -> Union[Process, None, UIDProxy]:
+        """
+        sample_preparation
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_process = cript.Process(name="my process name", type="affinity_pure")
+        >>> my_property.sample_preparation = my_process
+
+        Returns
+        -------
+        Union[Process, None]
+            Property linking back to the Process that has it as subobject
+        """
+        return self._json_attrs.sample_preparation
+
+    @sample_preparation.setter
+    @beartype
+    def sample_preparation(self, new_sample_preparation: Union[Process, None, UIDProxy]) -> None:
+        """
+        set the sample_preparation for the Property subobject
+
+        Parameters
+        ----------
+        new_sample_preparation : Union[Process, None]
+            back link to the Process that has this Property as its subobject
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, sample_preparation=new_sample_preparation)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def condition(self) -> List[Union[Condition, UIDProxy]]:
+        """
+        list of Conditions under which the property was measured
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_condition = cript.Condition(key="atm", type="max", value=1)
+        >>> my_property.condition = [my_condition]
+
+        Returns
+        -------
+        List[Condition]
+            list of Conditions
+        """
+        return self._json_attrs.condition.copy()
+
+    @condition.setter
+    @beartype
+    def condition(self, new_condition: List[Union[Condition, UIDProxy]]) -> None:
+        """
+        set the list of Conditions for this property subobject
+
+        Parameters
+        ----------
+        new_condition : List[Condition]
+            new list of Condition Subobjects
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, condition=new_condition)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def data(self) -> List[Union[Data, UIDProxy]]:
+        """
+        List of Data nodes for this Property subobjects
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary",
+        ... )
+        >>> my_data = cript.Data(name="my data name", type="afm_amp", file=[my_file])
+        >>> my_property.data = [my_data]
+
+        Returns
+        -------
+        List[Data]
+            list of Data nodes
+        """
+        return self._json_attrs.data.copy()
+
+    @data.setter
+    @beartype
+    def data(self, new_data: List[Union[Data, UIDProxy]]) -> None:
+        """
+        set the Data node for the Property subobject
+
+        Parameters
+        ----------
+        new_data : List[Data]
+            new list of Data nodes
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, data=new_data)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def computation(self) -> List[Union[Computation, UIDProxy]]:
+        """
+        list of Computation nodes that produced this property
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_computation = cript.Computation(name="my computation name", type="analysis")
+        >>> my_property.computation = [my_computation]
+
+        Returns
+        -------
+        List[Computation]
+            list of Computation nodes
+        """
+        return self._json_attrs.computation.copy()
+
+    @computation.setter
+    @beartype
+    def computation(self, new_computation: List[Union[Computation, UIDProxy]]) -> None:
+        """
+        set the list of Computation nodes that produced this property
+
+        Parameters
+        ----------
+        new_computation : List[Computation]
+            new list of Computation nodes
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, computation=new_computation)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Union[Citation, UIDProxy]]:
+        """
+        list of Citation subobjects for this Property subobject
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = cript.Citation(type="reference", reference=my_reference)
+        >>> my_property.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of Citation subobjects for this Property subobject
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation: List[Union[Citation, UIDProxy]]) -> None:
+        """
+        set the list of Citation subobjects for the Property subobject
+
+        Parameters
+        ----------
+        new_citation : List[Citation]
+            new list of Citation subobjects
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def notes(self) -> str:
+        """
+        notes for this Property subobject
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_property = cript.Property(key="air_flow", type="min", value=1.00, unit="gram")
+        >>> my_property.notes = "these are my notes"
+
+        Returns
+        -------
+        str
+            notes for this property subobject
+        """
+        return self._json_attrs.notes
+
+    @notes.setter
+    @beartype
+    def notes(self, new_notes: str) -> None:
+        """
+        set the notes for this Property sub-object
+
+        Parameters
+        ----------
+        new_notes : str
+            new notes
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, notes=new_notes)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/quantity.py` & `cript-2.3.0/src/cript/nodes/subobjects/quantity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-from dataclasses import dataclass, replace
-from numbers import Number
-from typing import Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Quantity(UUIDBaseNode):
-    """
-    ## Definition
-    The [Quantity](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=22)
-    sub-objects are the amount of material involved in a process
-
-    ---
-
-    ## Can Be Added To:
-    * [Ingredient](../ingredient)
-
-    ## Available sub-objects
-    * None
-
-    ----
-
-    ## Attributes
-
-    | attribute        | type    | example | description          | required | vocab |
-    |------------------|---------|---------|----------------------|----------|-------|
-    | key              | str     | mass    | type of quantity     | True     | True  |
-    | value            | Any     | 1.23    | amount of material   | True     |       |
-    | unit             | str     | gram    | unit for quantity    | True     |       |
-    | uncertainty      | Number  | 0.1     | uncertainty of value |          |       |
-    | uncertainty_type | str     | std     | type of uncertainty  |          | True  |
-
-
-
-
-    ## JSON Representation
-    ```json
-    {
-     "node":["Quantity"],
-     "key":"mass",
-     "value":11.2
-     "uncertainty":0.2,
-     "uncertainty_type":"stdev",
-     "unit":"kg",
-     "uid":"_:c95ee781-923b-4699-ba3b-923ce186ac5d",
-     "uuid":"c95ee781-923b-4699-ba3b-923ce186ac5d",
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        key: str = ""
-        value: Union[Number, str, None] = None
-        unit: str = ""
-        uncertainty: Optional[Number] = None
-        uncertainty_type: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, key: str, value: Number, unit: str, uncertainty: Optional[Number] = None, uncertainty_type: str = "", **kwargs):
-        """
-        create Quantity sub-object
-
-        Parameters
-        ----------
-        key : str
-            type of quantity. Quantity key must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
-        value : Number
-            amount of material
-        unit : str
-            unit for quantity
-        uncertainty : Union[Number, None], optional
-            uncertainty of value, by default None
-        uncertainty_type : str, optional
-            type of uncertainty. Quantity uncertainty type must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type), by default ""
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-
-        Returns
-        -------
-        None
-            create Quantity sub-object
-        """
-        super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, key=key, value=value, unit=unit, uncertainty=uncertainty, uncertainty_type=uncertainty_type)
-        self.validate()
-
-    @classmethod
-    def _from_json(cls, json_dict: dict):
-        # TODO: remove this temporary fix, once back end is working correctly
-        for key in ["value", "uncertainty"]:
-            try:
-                json_dict[key] = float(json_dict[key])
-            except KeyError:
-                pass
-        return super(Quantity, cls)._from_json(json_dict)
-
-    @beartype
-    def set_key_unit(self, new_key: str, new_unit: str) -> None:
-        """
-        set the Quantity key and unit attributes
-
-        Quantity key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_quantity.set_key_unit(new_key="mass", new_unit="kg")
-
-        Parameters
-        ----------
-        new_key : str
-            new Quantity key. Quantity key must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
-        new_unit : str
-            new unit
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, key=new_key, unit=new_unit)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def key(self) -> str:
-        """
-        get the Quantity sub-object key attribute
-
-        [Quantity type](https://app.criptapp.org/vocab/quantity_key) must come from CRIPT controlled vocabulary
-
-        Returns
-        -------
-        str
-            this Quantity key attribute
-        """
-        return self._json_attrs.key
-
-    @property
-    @beartype
-    def value(self) -> Union[int, float, str]:
-        """
-        amount of Material
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-        >>> my_quantity.value = 1
-
-        Returns
-        -------
-        Union[int, float, str]
-            amount of Material
-        """
-        return self._json_attrs.value  # type: ignore
-
-    @value.setter
-    @beartype
-    def value(self, new_value: Union[Number, str, None]) -> None:
-        """
-        set the amount of Material
-
-        Parameters
-        ----------
-        new_value : Union[int, float, str]
-            amount of Material
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, value=new_value)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def unit(self) -> str:
-        """
-        get the Quantity unit attribute
-
-        Returns
-        -------
-        str
-            unit for the Quantity value attribute
-        """
-        return self._json_attrs.unit
-
-    @property
-    @beartype
-    def uncertainty(self) -> Optional[Number]:
-        """
-        get the uncertainty value
-
-        Returns
-        -------
-        Number
-            uncertainty value
-        """
-        return self._json_attrs.uncertainty  # type: ignore
-
-    @property
-    @beartype
-    def uncertainty_type(self) -> str:
-        """
-        get the uncertainty type attribute for the Quantity sub-object
-
-        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type) must come from CRIPT controlled vocabulary
-
-        Returns
-        -------
-        str
-            uncertainty type
-        """
-        return self._json_attrs.uncertainty_type
-
-    @beartype
-    def set_uncertainty(self, uncertainty: Optional[Number], type: str) -> None:
-        """
-        set the `uncertainty value` and `uncertainty_type`
-
-        Uncertainty and uncertainty type are set at the same time to keep the value and type in sync
-
-        `uncertainty_type` must come from
-        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type)
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_quantity = cript.Quantity(
-        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
-        ... )
-
-        Parameters
-        ----------
-        uncertainty : Number
-            uncertainty value
-        type : str
-            type of uncertainty, uncertainty_type must come from
-            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type)
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, uncertainty=uncertainty, uncertainty_type=type)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, replace
+from numbers import Number
+from typing import Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Quantity(UUIDBaseNode):
+    """
+    ## Definition
+    The [Quantity](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=22)
+    sub-objects are the amount of material involved in a process
+
+    ---
+
+    ## Can Be Added To:
+    * [Ingredient](../ingredient)
+
+    ## Available sub-objects
+    * None
+
+    ----
+
+    ## Attributes
+
+    | attribute        | type    | example | description          | required | vocab |
+    |------------------|---------|---------|----------------------|----------|-------|
+    | key              | str     | mass    | type of quantity     | True     | True  |
+    | value            | Any     | 1.23    | amount of material   | True     |       |
+    | unit             | str     | gram    | unit for quantity    | True     |       |
+    | uncertainty      | Number  | 0.1     | uncertainty of value |          |       |
+    | uncertainty_type | str     | std     | type of uncertainty  |          | True  |
+
+
+
+
+    ## JSON Representation
+    ```json
+    {
+     "node":["Quantity"],
+     "key":"mass",
+     "value":11.2
+     "uncertainty":0.2,
+     "uncertainty_type":"stdev",
+     "unit":"kg",
+     "uid":"_:c95ee781-923b-4699-ba3b-923ce186ac5d",
+     "uuid":"c95ee781-923b-4699-ba3b-923ce186ac5d",
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        key: str = ""
+        value: Union[Number, str, None] = None
+        unit: str = ""
+        uncertainty: Optional[Number] = None
+        uncertainty_type: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, key: str, value: Number, unit: str, uncertainty: Optional[Number] = None, uncertainty_type: str = "", **kwargs):
+        """
+        create Quantity sub-object
+
+        Parameters
+        ----------
+        key : str
+            type of quantity. Quantity key must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
+        value : Number
+            amount of material
+        unit : str
+            unit for quantity
+        uncertainty : Union[Number, None], optional
+            uncertainty of value, by default None
+        uncertainty_type : str, optional
+            type of uncertainty. Quantity uncertainty type must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type), by default ""
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+
+        Returns
+        -------
+        None
+            create Quantity sub-object
+        """
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, key=key, value=value, unit=unit, uncertainty=uncertainty, uncertainty_type=uncertainty_type)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @classmethod
+    def _from_json(cls, json_dict: dict):
+        # TODO: remove this temporary fix, once back end is working correctly
+        for key in ["value", "uncertainty"]:
+            try:
+                json_dict[key] = float(json_dict[key])
+            except KeyError:
+                pass
+        return super(Quantity, cls)._from_json(json_dict)
+
+    @beartype
+    def set_key_unit(self, new_key: str, new_unit: str) -> None:
+        """
+        set the Quantity key and unit attributes
+
+        Quantity key must come from [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_quantity.set_key_unit(new_key="mass", new_unit="kg")
+
+        Parameters
+        ----------
+        new_key : str
+            new Quantity key. Quantity key must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/quantity_key)
+        new_unit : str
+            new unit
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, key=new_key, unit=new_unit)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def key(self) -> str:
+        """
+        get the Quantity sub-object key attribute
+
+        [Quantity type](https://app.criptapp.org/vocab/quantity_key) must come from CRIPT controlled vocabulary
+
+        Returns
+        -------
+        str
+            this Quantity key attribute
+        """
+        return self._json_attrs.key
+
+    @property
+    @beartype
+    def value(self) -> Union[int, float, str]:
+        """
+        amount of Material
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+        >>> my_quantity.value = 1
+
+        Returns
+        -------
+        Union[int, float, str]
+            amount of Material
+        """
+        return self._json_attrs.value  # type: ignore
+
+    @value.setter
+    @beartype
+    def value(self, new_value: Union[Number, str, None]) -> None:
+        """
+        set the amount of Material
+
+        Parameters
+        ----------
+        new_value : Union[int, float, str]
+            amount of Material
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, value=new_value)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def unit(self) -> str:
+        """
+        get the Quantity unit attribute
+
+        Returns
+        -------
+        str
+            unit for the Quantity value attribute
+        """
+        return self._json_attrs.unit
+
+    @property
+    @beartype
+    def uncertainty(self) -> Optional[Number]:
+        """
+        get the uncertainty value
+
+        Returns
+        -------
+        Number
+            uncertainty value
+        """
+        return self._json_attrs.uncertainty  # type: ignore
+
+    @property
+    @beartype
+    def uncertainty_type(self) -> str:
+        """
+        get the uncertainty type attribute for the Quantity sub-object
+
+        [Uncertainty type](https://app.criptapp.org/vocab/uncertainty_type) must come from CRIPT controlled vocabulary
+
+        Returns
+        -------
+        str
+            uncertainty type
+        """
+        return self._json_attrs.uncertainty_type
+
+    @beartype
+    def set_uncertainty(self, uncertainty: Optional[Number], type: str) -> None:
+        """
+        set the `uncertainty value` and `uncertainty_type`
+
+        Uncertainty and uncertainty type are set at the same time to keep the value and type in sync
+
+        `uncertainty_type` must come from
+        [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type)
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_quantity = cript.Quantity(
+        ...     key="mass", value=11.2, unit="kg", uncertainty=0.2, uncertainty_type="stdev"
+        ... )
+
+        Parameters
+        ----------
+        uncertainty : Number
+            uncertainty value
+        type : str
+            type of uncertainty, uncertainty_type must come from
+            [CRIPT Controlled Vocabulary](https://app.criptapp.org/vocab/uncertainty_type)
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, uncertainty=uncertainty, uncertainty_type=type)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/software.py` & `cript-2.3.0/src/cript/nodes/subobjects/software.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-from dataclasses import dataclass, replace
-
-from beartype import beartype
-
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class Software(UUIDBaseNode):
-    """
-    ## Definition
-
-    The [Software](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=16)
-    node contains metadata for a computation tool, code, programming language, or software package.
-
-    Similar to the [reference](../../primary_nodes/reference) node, the software node does not contain the base
-    attributes and is meant to always be public and static.
-
-    ---
-
-    ## Can Be Added To:
-    * [Software_Configuration](../../subobjects/software_configuration)
-
-    ## Available sub-objects
-    * None
-
-    ---
-
-    ## Attributes
-
-    | attribute | type | example    | description                   | required | vocab |
-    |-----------|------|------------|-------------------------------|----------|-------|
-    | name      | str  | LAMMPS     | type of literature            | True     |       |
-    | version   | str  | 23Jun22    | software version              | True     |       |
-    | source    | str  | lammps.org | source of software            |          |       |
-
-    ## JSON Representation
-    ```json
-    {
-       "name":"SOMA",
-       "node":["Software"],
-       "version":"0.7.0"
-       "source":"https://gitlab.com/InnocentBug/SOMA",
-       "uid":"_:f2ec4bf2-96aa-48a3-bfbc-d1d3f090583b",
-       "uuid":"f2ec4bf2-96aa-48a3-bfbc-d1d3f090583b",
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        name: str = ""
-        version: str = ""
-        source: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, version: str, source: str = "", **kwargs):
-        """
-        create Software node
-
-        Parameters
-        ----------
-        name : str
-            Software name
-        version : str
-            Software version
-        source : str, optional
-            Software source, by default ""
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(
-        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
-        ... )
-
-        Returns
-        -------
-        None
-            create Software node
-        """
-        super().__init__(**kwargs)
-
-        self._json_attrs = replace(self._json_attrs, name=name, version=version, source=source)
-        self.validate()
-
-    @property
-    @beartype
-    def name(self) -> str:
-        """
-        Software name
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(
-        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
-        ... )
-        >>> my_software.name = "my software name"
-
-        Returns
-        -------
-        str
-            Software name
-        """
-        return self._json_attrs.name
-
-    @name.setter
-    @beartype
-    def name(self, new_name: str) -> None:
-        """
-        set the name of the Software node
-
-        Parameters
-        ----------
-        new_name : str
-            new Software name
-
-        Returns
-        -------
-        None
-        """
-        new_attr = replace(self._json_attrs, name=new_name)
-        self._update_json_attrs_if_valid(new_attr)
-
-    @property
-    @beartype
-    def version(self) -> str:
-        """
-        Software version
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(
-        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
-        ... )
-        >>> my_software.version = "1.2.3"
-
-        Returns
-        -------
-        str
-            Software version
-        """
-        return self._json_attrs.version
-
-    @version.setter
-    @beartype
-    def version(self, new_version: str) -> None:
-        """
-        set the Software version
-
-        Parameters
-        ----------
-        new_version : str
-            new Software version
-
-        Returns
-        -------
-        None
-        """
-        new_attr = replace(self._json_attrs, version=new_version)
-        self._update_json_attrs_if_valid(new_attr)
-
-    @property
-    @beartype
-    def source(self) -> str:
-        """
-        Software source
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(
-        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
-        ... )
-        >>> my_software.source = "https://myNewWebsite.com"
-
-        Returns
-        -------
-        str
-            Software source
-        """
-        return self._json_attrs.source
-
-    @source.setter
-    @beartype
-    def source(self, new_source: str) -> None:
-        """
-        set the Software source
-
-        Parameters
-        ----------
-        new_source : str
-            new Software source
-
-        Returns
-        -------
-        None
-        """
-        new_attr = replace(self._json_attrs, source=new_source)
-        self._update_json_attrs_if_valid(new_attr)
+from dataclasses import dataclass, replace
+
+from beartype import beartype
+
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class Software(UUIDBaseNode):
+    """
+    ## Definition
+
+    The [Software](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=16)
+    node contains metadata for a computation tool, code, programming language, or software package.
+
+    Similar to the [reference](../../primary_nodes/reference) node, the software node does not contain the base
+    attributes and is meant to always be public and static.
+
+    ---
+
+    ## Can Be Added To:
+    * [Software_Configuration](../../subobjects/software_configuration)
+
+    ## Available sub-objects
+    * None
+
+    ---
+
+    ## Attributes
+
+    | attribute | type | example    | description                   | required | vocab |
+    |-----------|------|------------|-------------------------------|----------|-------|
+    | name      | str  | LAMMPS     | type of literature            | True     |       |
+    | version   | str  | 23Jun22    | software version              | True     |       |
+    | source    | str  | lammps.org | source of software            |          |       |
+
+    ## JSON Representation
+    ```json
+    {
+       "name":"SOMA",
+       "node":["Software"],
+       "version":"0.7.0"
+       "source":"https://gitlab.com/InnocentBug/SOMA",
+       "uid":"_:f2ec4bf2-96aa-48a3-bfbc-d1d3f090583b",
+       "uuid":"f2ec4bf2-96aa-48a3-bfbc-d1d3f090583b",
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        name: str = ""
+        version: str = ""
+        source: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, name: str, version: str, source: str = "", **kwargs):
+        """
+        create Software node
+
+        Parameters
+        ----------
+        name : str
+            Software name
+        version : str
+            Software version
+        source : str, optional
+            Software source, by default ""
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(
+        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
+        ... )
+
+        Returns
+        -------
+        None
+            create Software node
+        """
+        super().__init__(**kwargs)
+
+        new_json_attrs = replace(self._json_attrs, name=name, version=version, source=source)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def name(self) -> str:
+        """
+        Software name
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(
+        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
+        ... )
+        >>> my_software.name = "my software name"
+
+        Returns
+        -------
+        str
+            Software name
+        """
+        return self._json_attrs.name
+
+    @name.setter
+    @beartype
+    def name(self, new_name: str) -> None:
+        """
+        set the name of the Software node
+
+        Parameters
+        ----------
+        new_name : str
+            new Software name
+
+        Returns
+        -------
+        None
+        """
+        new_attr = replace(self._json_attrs, name=new_name)
+        self._update_json_attrs_if_valid(new_attr)
+
+    @property
+    @beartype
+    def version(self) -> str:
+        """
+        Software version
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(
+        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
+        ... )
+        >>> my_software.version = "1.2.3"
+
+        Returns
+        -------
+        str
+            Software version
+        """
+        return self._json_attrs.version
+
+    @version.setter
+    @beartype
+    def version(self, new_version: str) -> None:
+        """
+        set the Software version
+
+        Parameters
+        ----------
+        new_version : str
+            new Software version
+
+        Returns
+        -------
+        None
+        """
+        new_attr = replace(self._json_attrs, version=new_version)
+        self._update_json_attrs_if_valid(new_attr)
+
+    @property
+    @beartype
+    def source(self) -> str:
+        """
+        Software source
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(
+        ...     name="my software name", version="v1.0.0", source="https://myurl.com"
+        ... )
+        >>> my_software.source = "https://myNewWebsite.com"
+
+        Returns
+        -------
+        str
+            Software source
+        """
+        return self._json_attrs.source
+
+    @source.setter
+    @beartype
+    def source(self, new_source: str) -> None:
+        """
+        set the Software source
+
+        Parameters
+        ----------
+        new_source : str
+            new Software source
+
+        Returns
+        -------
+        None
+        """
+        new_attr = replace(self._json_attrs, source=new_source)
+        self._update_json_attrs_if_valid(new_attr)
```

### Comparing `cript-2.2.0/src/cript/nodes/subobjects/software_configuration.py` & `cript-2.3.0/src/cript/nodes/subobjects/software_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,279 @@
-from dataclasses import dataclass, field, replace
-from typing import List, Optional, Union
-
-from beartype import beartype
-
-from cript.nodes.subobjects.algorithm import Algorithm
-from cript.nodes.subobjects.citation import Citation
-from cript.nodes.subobjects.software import Software
-from cript.nodes.uuid_base import UUIDBaseNode
-
-
-class SoftwareConfiguration(UUIDBaseNode):
-    """
-    ## Definition
-
-    The [software_configuration](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=24)
-    sub-object includes software and the set of algorithms to execute computation or computational_process.
-
-    ---
-
-    ## Can Be Added To:
-    * [Computation](../../primary_nodes/computation)
-    * [Computation_Process](../../primary_nodes/computation_process)
-
-    ## Available sub-objects:
-    * [Algorithm](../algorithm)
-    * [Citation](../citation)
-
-    ---
-
-    ## Attributes
-
-    | keys                                             | type            | example | description                                                      | required | vocab |
-    |--------------------------------------------------|-----------------|---------|------------------------------------------------------------------|----------|-------|
-    | software                                         | Software        |         | software used                                                    | True     |       |
-    | algorithms                                       | list[Algorithm] |         | algorithms used                                                  |          |       |
-    | notes                                            | str             |         | miscellaneous information, or custom data structure (e.g.; JSON) |          |       |
-    | citation                                         | list[Citation]  |         | reference to a book, paper, or scholarly work                    |          |       |
-
-
-    ## JSON Representation
-    ```json
-    {
-       "node":["SoftwareConfiguration"],
-       "uid":"_:f0dc3415-635d-4590-8b1f-cd65ad8ab3fe"
-       "software":{
-          "name":"SOMA",
-          "node":["Software"],
-          "source":"https://gitlab.com/InnocentBug/SOMA",
-          "uid":"_:5bf9cb33-f029-4d1b-ba53-3602036e4f75",
-          "uuid":"5bf9cb33-f029-4d1b-ba53-3602036e4f75",
-          "version":"0.7.0"
-       }
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(UUIDBaseNode.JsonAttributes):
-        software: Union[Software, None] = None
-        algorithm: List[Algorithm] = field(default_factory=list)
-        notes: str = ""
-        citation: List[Citation] = field(default_factory=list)
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, software: Software, algorithm: Optional[List[Algorithm]] = None, notes: str = "", citation: Union[List[Citation], None] = None, **kwargs):
-        """
-        Create Software_Configuration sub-object
-
-
-        Parameters
-        ----------
-        software : Software
-            Software node used for the Software_Configuration
-        algorithm : Union[List[Algorithm], None], optional
-            algorithm used for the Software_Configuration, by default None
-        notes : str, optional
-            plain text notes, by default ""
-        citation : Union[List[Citation], None], optional
-            list of Citation sub-object, by default None
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-
-        Returns
-        -------
-        None
-            Create Software_Configuration sub-object
-        """
-        if algorithm is None:
-            algorithm = []
-        if citation is None:
-            citation = []
-        super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, software=software, algorithm=algorithm, notes=notes, citation=citation)
-        self.validate()
-
-    @property
-    @beartype
-    def software(self) -> Union[Software, None]:
-        """
-        Software used
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_software_configuration.software = my_software
-
-        Returns
-        -------
-        Union[Software, None]
-            Software node used
-        """
-        return self._json_attrs.software
-
-    @software.setter
-    @beartype
-    def software(self, new_software: Union[Software, None]) -> None:
-        """
-        set the Software used
-
-        Parameters
-        ----------
-        new_software : Union[Software, None]
-            new Software node
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, software=new_software)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def algorithm(self) -> List[Algorithm]:
-        """
-        list of Algorithms used
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_software_configuration.algorithm = [my_algorithm]
-
-        Returns
-        -------
-        List[Algorithm]
-            list of algorithms used
-        """
-        return self._json_attrs.algorithm.copy()
-
-    @algorithm.setter
-    @beartype
-    def algorithm(self, new_algorithm: List[Algorithm]) -> None:
-        """
-        set the list of Algorithms
-
-        Parameters
-        ----------
-        new_algorithm : List[Algorithm]
-            list of algorithms
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, algorithm=new_algorithm)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def notes(self) -> str:
-        """
-        miscellaneous information, or custom data structure (e.g.; JSON). Notes can be written in plain text or JSON
-
-        Examples
-        --------
-        ### Plain Text
-        ```json
-        my_software_configuration.notes = "these are my awesome notes!"
-        ```
-
-        Examples
-        -------
-        >>> import cript
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_software_configuration.notes = "{'notes subject': 'notes contents'}"
-
-        Returns
-        -------
-        str
-            notes
-        """
-        return self._json_attrs.notes
-
-    @notes.setter
-    @beartype
-    def notes(self, new_notes: str) -> None:
-        """
-        set notes for Software_configuration
-
-        Parameters
-        ----------
-        new_notes : str
-            new notes in plain text or JSON
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, notes=new_notes)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def citation(self) -> List[Citation]:
-        """
-        list of Citation sub-objects for the Software_Configuration
-
-        Examples
-        --------
-        >>> import cript
-        >>> title = (
-        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
-        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
-        ... )
-        >>> my_reference = cript.Reference(
-        ...     type="journal_article",
-        ...     title=title,
-        ...     author=["Ludwig Schneider", "Marcus Müller"],
-        ...     journal="Computer Physics Communications",
-        ...     publisher="Elsevier",
-        ...     year=2019,
-        ...     pages=[463, 476],
-        ...     doi="10.1016/j.cpc.2018.08.011",
-        ...     issn="0010-4655",
-        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
-        ... )
-        >>> my_citation = Citation("reference", my_reference)
-        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
-        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
-        >>> my_software_configuration.citation = [my_citation]
-
-        Returns
-        -------
-        List[Citation]
-            list of Citations
-        """
-        return self._json_attrs.citation.copy()
-
-    @citation.setter
-    @beartype
-    def citation(self, new_citation: List[Citation]) -> None:
-        """
-        set the Citation sub-object
-
-        Parameters
-        ----------
-        new_citation : List[Citation]
-            new list of Citation sub-objects
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, citation=new_citation)
-        self._update_json_attrs_if_valid(new_attrs)
+from dataclasses import dataclass, field, replace
+from typing import List, Optional, Union
+
+from beartype import beartype
+
+from cript.nodes.subobjects.algorithm import Algorithm
+from cript.nodes.subobjects.citation import Citation
+from cript.nodes.subobjects.software import Software
+from cript.nodes.util.json import UIDProxy
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+class SoftwareConfiguration(UUIDBaseNode):
+    """
+    ## Definition
+
+    The [software_configuration](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf#page=24)
+    sub-object includes software and the set of algorithms to execute computation or computational_process.
+
+    ---
+
+    ## Can Be Added To:
+    * [Computation](../../primary_nodes/computation)
+    * [Computation_Process](../../primary_nodes/computation_process)
+
+    ## Available sub-objects:
+    * [Algorithm](../algorithm)
+    * [Citation](../citation)
+
+    ---
+
+    ## Attributes
+
+    | keys                                             | type            | example | description                                                      | required | vocab |
+    |--------------------------------------------------|-----------------|---------|------------------------------------------------------------------|----------|-------|
+    | software                                         | Software        |         | software used                                                    | True     |       |
+    | algorithms                                       | list[Algorithm] |         | algorithms used                                                  |          |       |
+    | notes                                            | str             |         | miscellaneous information, or custom data structure (e.g.; JSON) |          |       |
+    | citation                                         | list[Citation]  |         | reference to a book, paper, or scholarly work                    |          |       |
+
+
+    ## JSON Representation
+    ```json
+    {
+       "node":["SoftwareConfiguration"],
+       "uid":"_:f0dc3415-635d-4590-8b1f-cd65ad8ab3fe"
+       "software":{
+          "name":"SOMA",
+          "node":["Software"],
+          "source":"https://gitlab.com/InnocentBug/SOMA",
+          "uid":"_:5bf9cb33-f029-4d1b-ba53-3602036e4f75",
+          "uuid":"5bf9cb33-f029-4d1b-ba53-3602036e4f75",
+          "version":"0.7.0"
+       }
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(UUIDBaseNode.JsonAttributes):
+        software: Optional[Union[Software, UIDProxy]] = None
+        algorithm: List[Union[Algorithm, UIDProxy]] = field(default_factory=list)
+        notes: str = ""
+        citation: List[Union[Citation, UIDProxy]] = field(default_factory=list)
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, software: Union[Software, UIDProxy], algorithm: Optional[List[Union[Algorithm, UIDProxy]]] = None, notes: str = "", citation: Union[List[Union[Citation, UIDProxy]], None] = None, **kwargs):
+        """
+        Create Software_Configuration sub-object
+
+
+        Parameters
+        ----------
+        software : Software
+            Software node used for the Software_Configuration
+        algorithm : Union[List[Algorithm], None], optional
+            algorithm used for the Software_Configuration, by default None
+        notes : str, optional
+            plain text notes, by default ""
+        citation : Union[List[Citation], None], optional
+            list of Citation sub-object, by default None
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+
+        Returns
+        -------
+        None
+            Create Software_Configuration sub-object
+        """
+        if algorithm is None:
+            algorithm = []
+        if citation is None:
+            citation = []
+        super().__init__(**kwargs)
+        new_json_attrs = replace(self._json_attrs, software=software, algorithm=algorithm, notes=notes, citation=citation)
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    @property
+    @beartype
+    def software(self) -> Union[Software, None, UIDProxy]:
+        """
+        Software used
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_software_configuration.software = my_software
+
+        Returns
+        -------
+        Union[Software, None]
+            Software node used
+        """
+        return self._json_attrs.software
+
+    @software.setter
+    @beartype
+    def software(self, new_software: Union[Software, None, UIDProxy]) -> None:
+        """
+        set the Software used
+
+        Parameters
+        ----------
+        new_software : Union[Software, None]
+            new Software node
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, software=new_software)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def algorithm(self) -> List[Union[Algorithm, UIDProxy]]:
+        """
+        list of Algorithms used
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_algorithm = cript.Algorithm(key="mc_barostat", type="barostat")
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_software_configuration.algorithm = [my_algorithm]
+
+        Returns
+        -------
+        List[Algorithm]
+            list of algorithms used
+        """
+        return self._json_attrs.algorithm.copy()
+
+    @algorithm.setter
+    @beartype
+    def algorithm(self, new_algorithm: List[Union[Algorithm, UIDProxy]]) -> None:
+        """
+        set the list of Algorithms
+
+        Parameters
+        ----------
+        new_algorithm : List[Algorithm]
+            list of algorithms
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, algorithm=new_algorithm)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def notes(self) -> str:
+        """
+        miscellaneous information, or custom data structure (e.g.; JSON). Notes can be written in plain text or JSON
+
+        Examples
+        --------
+        ### Plain Text
+        ```json
+        my_software_configuration.notes = "these are my awesome notes!"
+        ```
+
+        Examples
+        -------
+        >>> import cript
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_software_configuration.notes = "{'notes subject': 'notes contents'}"
+
+        Returns
+        -------
+        str
+            notes
+        """
+        return self._json_attrs.notes
+
+    @notes.setter
+    @beartype
+    def notes(self, new_notes: str) -> None:
+        """
+        set notes for Software_configuration
+
+        Parameters
+        ----------
+        new_notes : str
+            new notes in plain text or JSON
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, notes=new_notes)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def citation(self) -> List[Union[Citation, UIDProxy]]:
+        """
+        list of Citation sub-objects for the Software_Configuration
+
+        Examples
+        --------
+        >>> import cript
+        >>> title = (
+        ...     "Multi-architecture Monte-Carlo (MC) simulation of soft coarse-grained polymeric materials: "
+        ...     "Soft coarse grained Monte-Carlo Acceleration (SOMA)"
+        ... )
+        >>> my_reference = cript.Reference(
+        ...     type="journal_article",
+        ...     title=title,
+        ...     author=["Ludwig Schneider", "Marcus Müller"],
+        ...     journal="Computer Physics Communications",
+        ...     publisher="Elsevier",
+        ...     year=2019,
+        ...     pages=[463, 476],
+        ...     doi="10.1016/j.cpc.2018.08.011",
+        ...     issn="0010-4655",
+        ...     website="https://www.sciencedirect.com/science/article/pii/S0010465518303072",
+        ... )
+        >>> my_citation = Citation("reference", my_reference)
+        >>> my_software = cript.Software(name="LAMMPS", version="23Jun22", source="lammps.org")
+        >>> my_software_configuration = cript.SoftwareConfiguration(software=my_software)
+        >>> my_software_configuration.citation = [my_citation]
+
+        Returns
+        -------
+        List[Citation]
+            list of Citations
+        """
+        return self._json_attrs.citation.copy()
+
+    @citation.setter
+    @beartype
+    def citation(self, new_citation: List[Union[Citation, UIDProxy]]) -> None:
+        """
+        set the Citation sub-object
+
+        Parameters
+        ----------
+        new_citation : List[Citation]
+            new list of Citation sub-objects
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, citation=new_citation)
+        self._update_json_attrs_if_valid(new_attrs)
```

### Comparing `cript-2.2.0/src/cript/nodes/supporting_nodes/file.py` & `cript-2.3.0/src/cript/nodes/supporting_nodes/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,479 +1,478 @@
-import os
-from dataclasses import dataclass, replace
-from pathlib import Path
-from typing import Union
-
-from beartype import beartype
-
-from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
-
-
-def _is_local_file(file_source: str) -> bool:
-    """
-    Determines if the file the user is uploading is a local file or a link.
-
-    It basically tests if the path exists, and it is specifically a file
-    on the local storage and not just a valid directory
-
-    Notes
-    -----
-    since checking for URL is very easy because it has to start with HTTP it checks that as well
-    if it starts with http then it makes the work easy, and it is automatically web URL
-
-    Parameters
-    ----------
-    file_source: str
-        The source of the file.
-
-    Returns
-    -------
-    bool
-        True if the file is local, False if it's a link or s3 object_name.
-    """
-
-    # convert local or relative file path str into a path object and resolve it to always get an absolute path
-    file_source_abs_path: str = str(Path(file_source).resolve())
-
-    # if it doesn't start with HTTP and exists on disk
-    # checking "http" so it works with both "https://" and "http://"
-    if not file_source.startswith("http") and os.path.isfile(file_source_abs_path):
-        return True
-
-    else:
-        return False
-
-
-def _upload_file_and_get_object_name(source: Union[str, Path], api=None) -> str:
-    """
-    uploads file to cloud storage and returns the file link
-
-    1.  checks if the source is a local file path and not a web url
-    1. if it is a local file path, then it uploads it to cloud storage
-        * returns the file link in cloud storage
-    1. else it returns the same file link because it is already on the web
-
-    Parameters
-    ----------
-    source: str
-        file source can be a relative or absolute file string or pathlib object
-
-    Returns
-    -------
-    str
-        file AWS S3 link
-    """
-    from cript.api.api import _get_global_cached_api
-
-    # convert source to str for `_is_local_file` and to return str
-    source = str(source)
-
-    if _is_local_file(file_source=source):
-        if api is None:
-            api = _get_global_cached_api()
-        object_name = api.upload_file(file_path=source)
-        # always getting a string for object_name
-        source = str(object_name)
-
-    # always returning a string
-    return source
-
-
-class File(PrimaryBaseNode):
-    """
-    ## Definition
-
-    The [File node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001
-    .pdf#page=28) provides a link to scholarly work and allows users to specify in what way the work relates to that
-    data. More specifically, users can specify that the data was directly extracted from, inspired by, derived from,
-    etc.
-
-    The file node is held in the [Data node](../../primary_nodes/data).
-
-    ## Attributes
-
-    | Attribute       | Type | Example                                                                                               | Description                                                                 | Required |
-    |-----------------|------|-------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|----------|
-    | name            | str  | `"my file name"`                                                                                      | descriptive name for the file node                                          | True     |
-    | source          | str  | `"path/to/my/file"` or `"https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system"` | source to the file can be URL or local path                                 | True     |
-    | type            | str  | `"logs"`                                                                                              | Pick from [CRIPT File Types](https://app.criptapp.org/vocab/file_type/)     | True     |
-    | extension       | str  | `".csv"`                                                                                              | file extension                                                              | False    |
-    | data_dictionary | str  | `"my extra info in my data dictionary"`                                                               | set of information describing the contents, format, and structure of a file | False    |
-    | notes           | str  |                                                                                                       | miscellaneous information, or custom data structure (e.g.; JSON)            |          |
-
-    ## JSON
-    ``` json
-    {
-        "node": ["File"],
-        "name": "my file node name",
-        "source": "https://criptapp.org",
-        "type": "calibration",
-        "extension": ".csv",
-        "data_dictionary": "my file's data dictionary",
-    }
-    ```
-    """
-
-    @dataclass(frozen=True)
-    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
-        """
-        all file attributes
-        """
-
-        source: str = ""
-        type: str = ""
-        extension: str = ""
-        data_dictionary: str = ""
-
-    _json_attrs: JsonAttributes = JsonAttributes()
-
-    @beartype
-    def __init__(self, name: str, source: str, type: str, extension: str, data_dictionary: str = "", notes: str = "", **kwargs):
-        """
-        create a File node
-
-        Parameters
-        ----------
-        name: str
-            File node name
-        source: str
-            link or path to local file
-        type: str
-            Pick a file type from CRIPT controlled vocabulary
-            [File types](https://app.criptapp.org/vocab/file_type)
-        extension:str
-            file extension
-        data_dictionary:str
-            extra information describing the file
-        notes: str
-            notes for the file node
-        **kwargs:dict
-            for internal use. Any extra data needed to create this file node
-            when deserializing the JSON response from the API
-
-        Examples
-        --------
-        ### Web URL File Node
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
-        ...     type="calibration",
-        ...     extension=".pdf",
-        ...     data_dictionary="my file's data dictionary",
-        ...     notes="my notes for this file",
-        ... )
-
-        ### Local Source File Node
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="/home/user/MIT/project/my_file.csv",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ...     data_dictionary="my file's data dictionary",
-        ...     notes="my notes for this file",
-        ... )
-        """
-
-        super().__init__(name=name, notes=notes, **kwargs)
-
-        # setting every attribute except for source, which will be handled via setter
-        self._json_attrs = replace(
-            self._json_attrs,
-            type=type,
-            # always giving the function the required str regardless if the input `Path` or `str`
-            source=str(source),
-            extension=extension,
-            data_dictionary=data_dictionary,
-        )
-
-        self.validate()
-
-    def ensure_uploaded(self, api=None):
-        """
-        Ensure that a local file is being uploaded into CRIPT accessible cloud storage.
-        After this call, non-local files (file names that do not start with `http`) are uploaded.
-        It is not necessary to call this function manually.
-        A saved project automatically ensures uploaded files, it is recommend to rely on the automatic upload.
-
-        Parameters
-        -----------
-        api: cript.API, optional
-           API object that performs the upload.
-           If None, the globally cached object is being used.
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="/local/path/to/file",
-        ...     type="calibration",
-        ...     extension="csv",
-        ... )
-        >>> my_file.ensure_uploaded()   # doctest: +SKIP
-        >>> my_file.source # changed to cloud storage object name   # doctest: +SKIP
-        """
-
-        if _is_local_file(file_source=self.source):
-            # upload file source if local file
-            self.source = _upload_file_and_get_object_name(source=self.source)
-
-    # TODO can be made into a function
-
-    # --------------- Properties ---------------
-    @property
-    @beartype
-    def source(self) -> str:
-        """
-        The File node source can be set to be either a path to a local file on disk
-        or a URL path to a file on the web.
-
-        Examples
-        --------
-        URL File Source
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ... )
-        >>> my_file.source = "/home/user/project/my_file.csv"
-
-        Returns
-        -------
-        source: str
-            A string representing the file source.
-        """
-        return self._json_attrs.source
-
-    @source.setter
-    @beartype
-    def source(self, new_source: str) -> None:
-        """
-        sets the source of the file node
-        the source can either be a path to a file on local storage or a link to a file
-
-        1. checks if the file source is a link or a local file path
-        2. if the source is a link such as `https://wikipedia.com` then it sets the URL as the file source
-        3. if the file source is a local file path such as
-                `C:\\Users\\my_username\\Desktop\\cript\\file.txt`
-            1. then it opens the file and reads it
-            2. uploads it to the cloud storage
-            3. gets back a URL from where in the cloud the file is found
-            4. sets that as the source
-
-        Parameters
-        ----------
-        new_source: str
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file.source = "https://pubs.acs.org/doi/10.1021/acscentsci.3c00011"
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, source=new_source)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def type(self) -> str:
-        """
-        The [File type](https://app.criptapp.org/vocab/file_type) must come from CRIPT controlled vocabulary
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".csv",
-        ... )
-        >>> my_file.type = "calibration"
-
-        Returns
-        -------
-        file type: str
-            file type must come from [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/file_type)
-        """
-        return self._json_attrs.type
-
-    @type.setter
-    @beartype
-    def type(self, new_type: str) -> None:
-        """
-        set the file type
-
-        file type must come from CRIPT controlled vocabulary
-
-        Parameters
-        -----------
-        new_type: str
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file.type = "computation_config"
-
-        Returns
-        -------
-        None
-        """
-        # TODO check vocabulary is valid
-        # is_vocab_valid("file type", self._json_attrs.type)
-        new_attrs = replace(self._json_attrs, type=new_type)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def extension(self) -> str:
-        """
-        The file extension property explicitly states what is the file extension of the file node.
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".text",
-        ... )
-        >>> my_file.extension = ".csv"
-
-        !!! Note "file extensions must start with a dot"
-            File extensions must start with a dot, for example `.csv` or `.pdf`
-
-        Returns
-        -------
-        extension: str
-            file extension
-        """
-        return self._json_attrs.extension
-
-    @extension.setter
-    @beartype
-    def extension(self, new_extension) -> None:
-        """
-        sets the new file extension
-
-        Parameters
-        ----------
-        new_extension: str
-            new file extension to overwrite the current file extension
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file.extension = ".pdf"
-
-        Returns
-        -------
-            None
-        """
-        new_attrs = replace(self._json_attrs, extension=new_extension)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @property
-    @beartype
-    def data_dictionary(self) -> str:
-        # TODO data dictionary needs documentation describing it and how to use it
-        """
-        The data dictionary contains additional information
-        that the scientist needs to describe their file.
-
-        Notes
-        ------
-        It is advised for this field to be written in JSON format
-
-        Examples
-        ---------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file name",
-        ...     source="https://criptapp.org",
-        ...     type="calibration",
-        ...     extension=".png",
-        ... )
-        >>> my_file.data_dictionary = "{'notes': 'This is something that describes my file node.'}"
-
-        Returns
-        -------
-        data_dictionary: str
-            the file data dictionary attribute
-        """
-        return self._json_attrs.data_dictionary
-
-    @data_dictionary.setter
-    @beartype
-    def data_dictionary(self, new_data_dictionary: str) -> None:
-        """
-        Sets the data dictionary for the file node.
-
-        Parameters
-        ----------
-        new_data_dictionary: str
-            The new data dictionary to be set.
-
-        Returns
-        -------
-        None
-        """
-        new_attrs = replace(self._json_attrs, data_dictionary=new_data_dictionary)
-        self._update_json_attrs_if_valid(new_attrs)
-
-    @beartype
-    def download(
-        self,
-        destination_directory_path: Union[str, Path] = ".",
-    ) -> None:
-        """
-        download this file to current working directory or a specific destination.
-        The file name will come from the file_node.name and the extension will come from file_node.extension
-
-        Examples
-        --------
-        >>> import cript
-        >>> my_file = cript.File(
-        ...     name="my file node name",
-        ...     source="/local/path/to/file",
-        ...     type="calibration",
-        ...     extension=".jpeg",
-        ... )
-        >>> my_file.ensure_uploaded()   # doctest: +SKIP
-        >>> my_file.source # changed to cloud storage object name   # doctest: +SKIP
-        >>> my_file.download()  # doctest: +SKIP
-
-        Notes
-        -----
-        Whether the file extension is written like `.csv` or `csv` the program will work correctly
-
-        Parameters
-        ----------
-        destination_directory_path: Union[str, Path]
-            where you want the file to be stored and what you want the name to be
-            by default it is the current working directory
-
-        Returns
-        -------
-        None
-        """
-        from cript.api.api import _get_global_cached_api
-
-        api = _get_global_cached_api()
-
-        # convert the path from str to Path in case it was given as a str and resolve it to get the absolute path
-        existing_folder_path = Path(destination_directory_path).resolve()
-
-        # stripping dot from extension to make all extensions uniform, in case a user puts `.csv` or `csv` it will work
-        file_name = f"{self.name}.{self.extension.lstrip('.')}"
-
-        absolute_file_path = str((existing_folder_path / file_name).resolve())
-
-        api.download_file(file_source=self.source, destination_path=absolute_file_path)
+import os
+from dataclasses import dataclass, replace
+from pathlib import Path
+from typing import Union
+
+from beartype import beartype
+
+from cript.nodes.primary_nodes.primary_base_node import PrimaryBaseNode
+
+
+def _is_local_file(file_source: str) -> bool:
+    """
+    Determines if the file the user is uploading is a local file or a link.
+
+    It basically tests if the path exists, and it is specifically a file
+    on the local storage and not just a valid directory
+
+    Notes
+    -----
+    since checking for URL is very easy because it has to start with HTTP it checks that as well
+    if it starts with http then it makes the work easy, and it is automatically web URL
+
+    Parameters
+    ----------
+    file_source: str
+        The source of the file.
+
+    Returns
+    -------
+    bool
+        True if the file is local, False if it's a link or s3 object_name.
+    """
+
+    # convert local or relative file path str into a path object and resolve it to always get an absolute path
+    file_source_abs_path: str = str(Path(file_source).resolve())
+
+    # if it doesn't start with HTTP and exists on disk
+    # checking "http" so it works with both "https://" and "http://"
+    if not file_source.startswith("http") and os.path.isfile(file_source_abs_path):
+        return True
+
+    else:
+        return False
+
+
+def _upload_file_and_get_object_name(source: Union[str, Path], api=None) -> str:
+    """
+    uploads file to cloud storage and returns the file link
+
+    1.  checks if the source is a local file path and not a web url
+    1. if it is a local file path, then it uploads it to cloud storage
+        * returns the file link in cloud storage
+    1. else it returns the same file link because it is already on the web
+
+    Parameters
+    ----------
+    source: str
+        file source can be a relative or absolute file string or pathlib object
+
+    Returns
+    -------
+    str
+        file AWS S3 link
+    """
+    from cript.api.api import _get_global_cached_api
+
+    # convert source to str for `_is_local_file` and to return str
+    source = str(source)
+
+    if _is_local_file(file_source=source):
+        if api is None:
+            api = _get_global_cached_api()
+        object_name = api.upload_file(file_path=source)
+        # always getting a string for object_name
+        source = str(object_name)
+
+    # always returning a string
+    return source
+
+
+class File(PrimaryBaseNode):
+    """
+    ## Definition
+
+    The [File node](https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001
+    .pdf#page=28) provides a link to scholarly work and allows users to specify in what way the work relates to that
+    data. More specifically, users can specify that the data was directly extracted from, inspired by, derived from,
+    etc.
+
+    The file node is held in the [Data node](../../primary_nodes/data).
+
+    ## Attributes
+
+    | Attribute       | Type | Example                                                                                               | Description                                                                 | Required |
+    |-----------------|------|-------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|----------|
+    | name            | str  | `"my file name"`                                                                                      | descriptive name for the file node                                          | True     |
+    | source          | str  | `"path/to/my/file"` or `"https://en.wikipedia.org/wiki/Simplified_molecular-input_line-entry_system"` | source to the file can be URL or local path                                 | True     |
+    | type            | str  | `"logs"`                                                                                              | Pick from [CRIPT File Types](https://app.criptapp.org/vocab/file_type/)     | True     |
+    | extension       | str  | `".csv"`                                                                                              | file extension                                                              | False    |
+    | data_dictionary | str  | `"my extra info in my data dictionary"`                                                               | set of information describing the contents, format, and structure of a file | False    |
+    | notes           | str  |                                                                                                       | miscellaneous information, or custom data structure (e.g.; JSON)            |          |
+
+    ## JSON
+    ``` json
+    {
+        "node": ["File"],
+        "name": "my file node name",
+        "source": "https://criptapp.org",
+        "type": "calibration",
+        "extension": ".csv",
+        "data_dictionary": "my file's data dictionary",
+    }
+    ```
+    """
+
+    @dataclass(frozen=True)
+    class JsonAttributes(PrimaryBaseNode.JsonAttributes):
+        """
+        all file attributes
+        """
+
+        source: str = ""
+        type: str = ""
+        extension: str = ""
+        data_dictionary: str = ""
+
+    _json_attrs: JsonAttributes = JsonAttributes()
+
+    @beartype
+    def __init__(self, name: str, source: str, type: str, extension: str, data_dictionary: str = "", notes: str = "", **kwargs):
+        """
+        create a File node
+
+        Parameters
+        ----------
+        name: str
+            File node name
+        source: str
+            link or path to local file
+        type: str
+            Pick a file type from CRIPT controlled vocabulary
+            [File types](https://app.criptapp.org/vocab/file_type)
+        extension:str
+            file extension
+        data_dictionary:str
+            extra information describing the file
+        notes: str
+            notes for the file node
+        **kwargs:dict
+            for internal use. Any extra data needed to create this file node
+            when deserializing the JSON response from the API
+
+        Examples
+        --------
+        ### Web URL File Node
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="https://pubs.acs.org/doi/suppl/10.1021/acscentsci.3c00011/suppl_file/oc3c00011_si_001.pdf",
+        ...     type="calibration",
+        ...     extension=".pdf",
+        ...     data_dictionary="my file's data dictionary",
+        ...     notes="my notes for this file",
+        ... )
+
+        ### Local Source File Node
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="/home/user/MIT/project/my_file.csv",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ...     data_dictionary="my file's data dictionary",
+        ...     notes="my notes for this file",
+        ... )
+        """
+
+        super().__init__(name=name, notes=notes, **kwargs)
+
+        # setting every attribute except for source, which will be handled via setter
+        new_json_attrs = replace(
+            self._json_attrs,
+            type=type,
+            # always giving the function the required str regardless if the input `Path` or `str`
+            source=str(source),
+            extension=extension,
+            data_dictionary=data_dictionary,
+        )
+        self._update_json_attrs_if_valid(new_json_attrs)
+
+    def ensure_uploaded(self, api=None):
+        """
+        Ensure that a local file is being uploaded into CRIPT accessible cloud storage.
+        After this call, non-local files (file names that do not start with `http`) are uploaded.
+        It is not necessary to call this function manually.
+        A saved project automatically ensures uploaded files, it is recommend to rely on the automatic upload.
+
+        Parameters
+        -----------
+        api: cript.API, optional
+           API object that performs the upload.
+           If None, the globally cached object is being used.
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="/local/path/to/file",
+        ...     type="calibration",
+        ...     extension="csv",
+        ... )
+        >>> my_file.ensure_uploaded()   # doctest: +SKIP
+        >>> my_file.source # changed to cloud storage object name   # doctest: +SKIP
+        """
+
+        if _is_local_file(file_source=self.source):
+            # upload file source if local file
+            self.source = _upload_file_and_get_object_name(source=self.source)
+
+    # TODO can be made into a function
+
+    # --------------- Properties ---------------
+    @property
+    @beartype
+    def source(self) -> str:
+        """
+        The File node source can be set to be either a path to a local file on disk
+        or a URL path to a file on the web.
+
+        Examples
+        --------
+        URL File Source
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ... )
+        >>> my_file.source = "/home/user/project/my_file.csv"
+
+        Returns
+        -------
+        source: str
+            A string representing the file source.
+        """
+        return self._json_attrs.source
+
+    @source.setter
+    @beartype
+    def source(self, new_source: str) -> None:
+        """
+        sets the source of the file node
+        the source can either be a path to a file on local storage or a link to a file
+
+        1. checks if the file source is a link or a local file path
+        2. if the source is a link such as `https://wikipedia.com` then it sets the URL as the file source
+        3. if the file source is a local file path such as
+                `C:\\Users\\my_username\\Desktop\\cript\\file.txt`
+            1. then it opens the file and reads it
+            2. uploads it to the cloud storage
+            3. gets back a URL from where in the cloud the file is found
+            4. sets that as the source
+
+        Parameters
+        ----------
+        new_source: str
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file.source = "https://pubs.acs.org/doi/10.1021/acscentsci.3c00011"
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, source=new_source)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def type(self) -> str:
+        """
+        The [File type](https://app.criptapp.org/vocab/file_type) must come from CRIPT controlled vocabulary
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".csv",
+        ... )
+        >>> my_file.type = "calibration"
+
+        Returns
+        -------
+        file type: str
+            file type must come from [CRIPT controlled vocabulary](https://app.criptapp.org/vocab/file_type)
+        """
+        return self._json_attrs.type
+
+    @type.setter
+    @beartype
+    def type(self, new_type: str) -> None:
+        """
+        set the file type
+
+        file type must come from CRIPT controlled vocabulary
+
+        Parameters
+        -----------
+        new_type: str
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file.type = "computation_config"
+
+        Returns
+        -------
+        None
+        """
+        # TODO check vocabulary is valid
+        # is_vocab_valid("file type", self._json_attrs.type)
+        new_attrs = replace(self._json_attrs, type=new_type)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def extension(self) -> str:
+        """
+        The file extension property explicitly states what is the file extension of the file node.
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".text",
+        ... )
+        >>> my_file.extension = ".csv"
+
+        !!! Note "file extensions must start with a dot"
+            File extensions must start with a dot, for example `.csv` or `.pdf`
+
+        Returns
+        -------
+        extension: str
+            file extension
+        """
+        return self._json_attrs.extension
+
+    @extension.setter
+    @beartype
+    def extension(self, new_extension) -> None:
+        """
+        sets the new file extension
+
+        Parameters
+        ----------
+        new_extension: str
+            new file extension to overwrite the current file extension
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file.extension = ".pdf"
+
+        Returns
+        -------
+            None
+        """
+        new_attrs = replace(self._json_attrs, extension=new_extension)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @property
+    @beartype
+    def data_dictionary(self) -> str:
+        # TODO data dictionary needs documentation describing it and how to use it
+        """
+        The data dictionary contains additional information
+        that the scientist needs to describe their file.
+
+        Notes
+        ------
+        It is advised for this field to be written in JSON format
+
+        Examples
+        ---------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file name",
+        ...     source="https://criptapp.org",
+        ...     type="calibration",
+        ...     extension=".png",
+        ... )
+        >>> my_file.data_dictionary = "{'notes': 'This is something that describes my file node.'}"
+
+        Returns
+        -------
+        data_dictionary: str
+            the file data dictionary attribute
+        """
+        return self._json_attrs.data_dictionary
+
+    @data_dictionary.setter
+    @beartype
+    def data_dictionary(self, new_data_dictionary: str) -> None:
+        """
+        Sets the data dictionary for the file node.
+
+        Parameters
+        ----------
+        new_data_dictionary: str
+            The new data dictionary to be set.
+
+        Returns
+        -------
+        None
+        """
+        new_attrs = replace(self._json_attrs, data_dictionary=new_data_dictionary)
+        self._update_json_attrs_if_valid(new_attrs)
+
+    @beartype
+    def download(
+        self,
+        destination_directory_path: Union[str, Path] = ".",
+    ) -> None:
+        """
+        download this file to current working directory or a specific destination.
+        The file name will come from the file_node.name and the extension will come from file_node.extension
+
+        Examples
+        --------
+        >>> import cript
+        >>> my_file = cript.File(
+        ...     name="my file node name",
+        ...     source="/local/path/to/file",
+        ...     type="calibration",
+        ...     extension=".jpeg",
+        ... )
+        >>> my_file.ensure_uploaded()   # doctest: +SKIP
+        >>> my_file.source # changed to cloud storage object name   # doctest: +SKIP
+        >>> my_file.download()  # doctest: +SKIP
+
+        Notes
+        -----
+        Whether the file extension is written like `.csv` or `csv` the program will work correctly
+
+        Parameters
+        ----------
+        destination_directory_path: Union[str, Path]
+            where you want the file to be stored and what you want the name to be
+            by default it is the current working directory
+
+        Returns
+        -------
+        None
+        """
+        from cript.api.api import _get_global_cached_api
+
+        api = _get_global_cached_api()
+
+        # convert the path from str to Path in case it was given as a str and resolve it to get the absolute path
+        existing_folder_path = Path(destination_directory_path).resolve()
+
+        # stripping dot from extension to make all extensions uniform, in case a user puts `.csv` or `csv` it will work
+        file_name = f"{self.name}.{self.extension.lstrip('.')}"
+
+        absolute_file_path = str((existing_folder_path / file_name).resolve())
+
+        api.download_file(file_source=self.source, destination_path=absolute_file_path)
```

### Comparing `cript-2.2.0/src/cript/nodes/supporting_nodes/user.py` & `cript-2.3.0/src/cript/nodes/supporting_nodes/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,16 @@
             user username
         email: str
             user email
         orcid: str
             user ORCID
         """
         super().__init__(**kwargs)
-        self._json_attrs = replace(self._json_attrs, username=username, email=email, orcid=orcid)
-
-        self.validate()
+        new_json_attrs = replace(self._json_attrs, username=username, email=email, orcid=orcid)
+        self._update_json_attrs_if_valid(new_json_attrs)
 
     @property
     @beartype
     def created_at(self) -> str:
         return self._json_attrs.created_at
 
     @property
```

### Comparing `cript-2.2.0/src/cript/nodes/util/__init__.py` & `cript-2.3.0/src/cript/nodes/util/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,518 +1,463 @@
-import dataclasses
-import inspect
-import json
-import uuid
-from typing import Dict, List, Optional, Set, Union
-
-import cript.nodes
-from cript.nodes.core import BaseNode
-from cript.nodes.exceptions import (
-    CRIPTDeserializationUIDError,
-    CRIPTJsonDeserializationError,
-    CRIPTJsonNodeError,
-    CRIPTOrphanedComputationalProcessError,
-    CRIPTOrphanedComputationError,
-    CRIPTOrphanedDataError,
-    CRIPTOrphanedMaterialError,
-    CRIPTOrphanedProcessError,
-)
-from cript.nodes.primary_nodes.experiment import Experiment
-from cript.nodes.primary_nodes.project import Project
-
-
-class NodeEncoder(json.JSONEncoder):
-    """
-    Custom JSON encoder for serializing CRIPT nodes to JSON.
-
-    This encoder is used to convert CRIPT nodes into JSON format while handling unique identifiers (UUIDs) and
-    condensed representations to avoid redundancy in the JSON output.
-    It also allows suppressing specific attributes from being included in the serialized JSON.
-
-    Attributes
-    ----------
-    handled_ids : Set[str]
-        A set to store the UIDs of nodes that have been processed during serialization.
-    known_uuid : Set[str]
-        A set to store the UUIDs of nodes that have been previously encountered in the JSON.
-    condense_to_uuid : Dict[str, Set[str]]
-        A set to store the node types that should be condensed to UUID edges in the JSON.
-    suppress_attributes : Optional[Dict[str, Set[str]]]
-        A dictionary that allows suppressing specific attributes for nodes with the corresponding UUIDs.
-
-    Methods
-    -------
-    ```python
-    default(self, obj: Any) -> Any:
-        # Convert CRIPT nodes and other objects to their JSON representation.
-    ```
-
-    ```python
-    _apply_modifications(self, serialize_dict: dict) -> Tuple[dict, List[str]]:
-        # Apply modifications to the serialized dictionary based on node types
-        # and attributes to be condensed. This internal function handles node
-        # condensation and attribute suppression during serialization.
-    ```
-    """
-
-    handled_ids: Set[str] = set()
-    known_uuid: Set[str] = set()
-    condense_to_uuid: Dict[str, Set[str]] = dict()
-    suppress_attributes: Optional[Dict[str, Set[str]]] = None
-
-    def default(self, obj):
-        """
-        Convert CRIPT nodes and other objects to their JSON representation.
-
-        This method is called during JSON serialization.
-        It customizes the serialization process for CRIPT nodes and handles unique identifiers (UUIDs)
-        to avoid redundant data in the JSON output.
-        It also allows for attribute suppression for specific nodes.
-
-        Parameters
-        ----------
-        obj : Any
-            The object to be serialized to JSON.
-
-        Returns
-        -------
-        dict
-            The JSON representation of the input object, which can be a string, a dictionary, or any other JSON-serializable type.
-
-        Raises
-        ------
-        CRIPTJsonDeserializationError
-            If there is an issue with the JSON deserialization process for CRIPT nodes.
-
-        Notes
-        -----
-        * If the input object is a UUID, it is converted to a string representation and returned.
-        * If the input object is a CRIPT node (an instance of `BaseNode`), it is serialized into a dictionary
-          representation. The node is first checked for uniqueness based on its UID (unique identifier), and if
-          it has already been serialized, it is represented as a UUID edge only. If not, the node's attributes
-          are added to the dictionary representation, and any default attribute values are removed to reduce
-          redundancy in the JSON output.
-        * The method `_apply_modifications()` is called to check if further modifications are needed before
-          considering the dictionary representation done. This includes condensing certain node types to UUID edges
-          and suppressing specific attributes for nodes.
-        """
-        if isinstance(obj, uuid.UUID):
-            return str(obj)
-        if isinstance(obj, BaseNode):
-            try:
-                uid = obj.uid
-            except AttributeError:
-                pass
-            else:
-                if uid in NodeEncoder.handled_ids:
-                    return {"uid": uid}
-
-            # When saving graphs, some nodes can be pre-saved.
-            # If that happens, we want to represent them as a UUID edge only
-            try:
-                uuid_str = str(obj.uuid)
-            except AttributeError:
-                pass
-            else:
-                if uuid_str in NodeEncoder.known_uuid:
-                    return {"uuid": uuid_str}
-
-            default_dataclass = obj.JsonAttributes()
-            serialize_dict = {}
-            # Remove default values from serialization
-            for field_name in [field.name for field in dataclasses.fields(default_dataclass)]:
-                if getattr(default_dataclass, field_name) != getattr(obj._json_attrs, field_name):
-                    serialize_dict[field_name] = getattr(obj._json_attrs, field_name)
-            # add the default node type
-            serialize_dict["node"] = obj._json_attrs.node
-
-            # check if further modifications to the dict is needed before considering it done
-            serialize_dict, condensed_uid = self._apply_modifications(serialize_dict)
-            if uid not in condensed_uid:  # We can uid (node) as handled if we don't condense it to uuid
-                NodeEncoder.handled_ids.add(uid)
-
-            # Remove suppressed attributes
-            if NodeEncoder.suppress_attributes is not None and str(obj.uuid) in NodeEncoder.suppress_attributes:
-                for attr in NodeEncoder.suppress_attributes[str(obj.uuid)]:
-                    del serialize_dict[attr]
-
-            return serialize_dict
-        return json.JSONEncoder.default(self, obj)
-
-    def _apply_modifications(self, serialize_dict: Dict):
-        """
-        Checks the serialize_dict to see if any other operations are required before it
-        can be considered done. If other operations are required, then it passes it to the other operations
-        and at the end returns the fully finished dict.
-
-        This function is essentially a big switch case that checks the node type
-        and determines what other operations are required for it.
-
-        Parameters
-        ----------
-        serialize_dict: dict
-
-        Returns
-        -------
-        serialize_dict: dict
-        """
-
-        def process_attribute(attribute):
-            def strip_to_edge_uuid(element):
-                # Extracts UUID and UID information from the element
-                try:
-                    uuid = getattr(element, "uuid")
-                except AttributeError:
-                    uuid = element["uuid"]
-                    if len(element) == 1:  # Already a condensed element
-                        return element, None
-                try:
-                    uid = getattr(element, "uid")
-                except AttributeError:
-                    uid = element["uid"]
-
-                element = {"uuid": str(uuid)}
-                return element, uid
-
-            # Processes an attribute based on its type (list or single element)
-            if isinstance(attribute, list):
-                processed_elements = []
-                for element in attribute:
-                    processed_element, uid = strip_to_edge_uuid(element)
-                    if uid is not None:
-                        uid_of_condensed.append(uid)
-                    processed_elements.append(processed_element)
-                return processed_elements
-            else:
-                processed_attribute, uid = strip_to_edge_uuid(attribute)
-                if uid is not None:
-                    uid_of_condensed.append(uid)
-                return processed_attribute
-
-        uid_of_condensed: List = []
-
-        nodes_to_condense = serialize_dict["node"]
-        for node_type in nodes_to_condense:
-            if node_type in self.condense_to_uuid:
-                attributes_to_process = self.condense_to_uuid[node_type]  # type: ignore
-                for attribute in attributes_to_process:
-                    if attribute in serialize_dict:
-                        attribute_to_condense = serialize_dict[attribute]
-                        processed_attribute = process_attribute(attribute_to_condense)
-                        serialize_dict[attribute] = processed_attribute
-
-        # Check if the node is "Material" and convert the identifiers list to JSON fields
-        if serialize_dict["node"] == ["Material"]:
-            serialize_dict = _material_identifiers_list_to_json_fields(serialize_dict)
-
-        return serialize_dict, uid_of_condensed
-
-
-class _UIDProxy:
-    """
-    Proxy class for unresolvable UID nodes.
-    This is going to be replaced by actual nodes.
-
-    Report a bug if you find this class in production.
-    """
-
-    def __init__(self, uid: str):
-        self.uid = uid
-        print("proxy", uid)
-
-
-class _NodeDecoderHook:
-    def __init__(self, uid_cache: Optional[Dict] = None):
-        """
-        Initialize the custom JSON object hook used for CRIPT node deserialization.
-
-        Parameters
-        ----------
-        uid_cache : Optional[Dict], optional
-            A dictionary to cache Python objects with shared UIDs, by default None.
-
-        Notes
-        -----
-        The `_NodeDecoderHook` class is used as an object hook for JSON deserialization,
-        handling the conversion of JSON nodes into Python objects based on their node types.
-        The `uid_cache` is an optional dictionary to store cached objects with shared UIDs
-        to never create two different python nodes with the same uid.
-        """
-        if uid_cache is None:
-            uid_cache = {}
-        self._uid_cache = uid_cache
-
-    def __call__(self, node_str: Union[dict, str]) -> dict:
-        """
-        Internal function, used as a hook for json deserialization.
-
-        This function is called recursively to convert every JSON of a node and its children from node to JSON.
-
-        If given a JSON without a "node" field then it is assumed that it is not a node
-        and just a key value pair data, and the JSON string is then just converted from string to dict and returned
-        applicable for places where the data is something like
-
-        ```json
-        { "bigsmiles": "123456" }
-        ```
-
-        no serialization is needed in this case and just needs to be converted from str to dict
-
-        if the node field is present, then continue and convert the JSON node into a Python object
-
-        Parameters
-        ----------
-        node_str : Union[dict, str]
-            The JSON representation of a node or a regular dictionary.
-
-        Returns
-        -------
-        Union[CRIPT Node, dict]
-            Either returns a regular dictionary if the input JSON or input dict is NOT a node.
-            If it is a node, it returns the appropriate CRIPT node object, such as `cript.Material`
-
-        Raises
-        ------
-        CRIPTJsonNodeError
-            If there is an issue with the JSON structure or the node type is invalid.
-        CRIPTJsonDeserializationError
-            If there is an error during deserialization of a specific node type.
-        CRIPTDeserializationUIDError
-            If there is an issue with the UID used for deserialization, like circular references.
-        """
-        node_dict = dict(node_str)  # type: ignore
-
-        # Handle UID objects.
-        if len(node_dict) == 1 and "uid" in node_dict:
-            try:
-                return self._uid_cache[node_dict["uid"]]
-            except KeyError:
-                # TODO if we convince beartype to accept Proxy temporarily, enable return instead of raise
-                raise CRIPTDeserializationUIDError("Unknown", node_dict["uid"])
-                # return _UIDProxy(node_dict["uid"])
-
-        try:
-            node_type_list = node_dict["node"]
-        except KeyError:  # Not a node, just a regular dictionary
-            return node_dict
-
-        # TODO consider putting this into the try because it might need error handling for the dict
-        if _is_node_field_valid(node_type_list):
-            node_type_str = node_type_list[0]
-        else:
-            raise CRIPTJsonNodeError(node_type_list, str(node_str))
-
-        # Iterate over all nodes in cript to find the correct one here
-        for key, pyclass in inspect.getmembers(cript.nodes, inspect.isclass):
-            if BaseNode in inspect.getmro(pyclass):
-                if key == node_type_str:
-                    try:
-                        json_node = pyclass._from_json(node_dict)
-                        self._uid_cache[json_node.uid] = json_node
-                        return json_node
-                    except Exception as exc:
-                        raise CRIPTJsonDeserializationError(key, str(node_type_str)) from exc
-        # Fall back
-        return node_dict
-
-
-def _material_identifiers_list_to_json_fields(serialize_dict: dict) -> dict:
-    """
-    input:
-    ```json
-        {
-            "node":["Material"],
-            "name":"my material",
-            "identifier":[ {"cas":"my material cas"} ],
-            "uid":"_:a78203cb-82ea-4376-910e-dee74088cd37"
-        }
-    ```
-
-    output:
-    ```json
-    {
-        "node":["Material"],
-        "name":"my material",
-        "cas":"my material cas",
-        "uid":"_:08018f4a-e8e3-4ac0-bdad-fa704fdc0145"
-    }
-    ```
-
-    Parameters
-    ----------
-    serialize_dict: dict
-        the serialized dictionary of the node
-
-    Returns
-    -------
-    serialized_dict = dict
-        new dictionary that has converted the list of dictionary identifiers into the dictionary as fields
-
-    """
-
-    # TODO this if statement might not be needed in future
-    if "identifier" in serialize_dict:
-        for identifier in serialize_dict["identifier"]:
-            for key, value in identifier.items():
-                serialize_dict[key] = value
-
-        # remove identifiers list of objects after it has been flattened
-        del serialize_dict["identifier"]
-
-    return serialize_dict
-
-
-def _rename_field(serialize_dict: dict, old_name: str, new_name: str) -> dict:
-    """
-    renames `property_` to `property` the JSON
-    """
-    if "property_" in serialize_dict:
-        serialize_dict[new_name] = serialize_dict.pop(old_name)
-
-    return serialize_dict
-
-
-def _is_node_field_valid(node_type_list: list) -> bool:
-    """
-    a simple function that checks if the node field has only a single node type in there
-    and not 2 or None
-
-    Parameters
-    ----------
-    node_type_list: list
-        e.g. "node": ["Material"]
-
-    Returns
-    ------
-    bool
-        if all tests pass then it returns true, otherwise false
-    """
-
-    # TODO consider having exception handling for the dict
-    if isinstance(node_type_list, list) and len(node_type_list) == 1 and isinstance(node_type_list[0], str) and len(node_type_list[0]) > 0:
-        return True
-    else:
-        return False
-
-
-def load_nodes_from_json(nodes_json: Union[str, Dict]):
-    """
-    User facing function, that return a node and all its children from a json string input.
-
-    Parameters
-    ----------
-    nodes_json: Union[str, dict]
-        JSON string representation of a CRIPT node
-
-    Examples
-    --------
-    >>> import cript
-    >>> # Get updated project from API
-    >>> my_paginator = api.search(
-    ...     node_type=cript.Project,
-    ...     search_mode=cript.SearchModes.EXACT_NAME,
-    ...     value_to_search="my project name",
-    ... ) # doctest: +SKIP
-    >>> # Take specific Project you want from paginator
-    >>> my_project_from_api_dict: dict = my_paginator.current_page_results[0] # doctest: +SKIP
-    >>> # Deserialize your Project dict into a Project node
-    >>> my_project_node_from_api = cript.load_nodes_from_json( # doctest: +SKIP
-    ...     nodes_json=my_project_from_api_dict
-    ... )
-
-    Raises
-    ------
-    CRIPTJsonNodeError
-        If there is an issue with the JSON of the node field.
-    CRIPTJsonDeserializationError
-        If there is an error during deserialization of a specific node.
-    CRIPTDeserializationUIDError
-        If there is an issue with the UID used for deserialization, like circular references.
-
-    Notes
-    -----
-    This function uses a custom `_NodeDecoderHook` to convert JSON nodes into Python objects.
-    The `_NodeDecoderHook` class is responsible for handling the deserialization of nodes
-    and caching objects with shared UIDs to avoid redundant deserialization.
-
-    The function is intended for deserializing CRIPT nodes and should not be used for generic JSON.
-
-    Returns
-    -------
-    Union[CRIPT Node, List[CRIPT Node]]
-        Typically returns a single CRIPT node,
-        but if given a list of nodes, then it will serialize them and return a list of CRIPT nodes
-    """
-    # Initialize the custom decoder hook for JSON deserialization
-    node_json_hook = _NodeDecoderHook()
-
-    # Check if the input is already a Python dictionary
-    if isinstance(nodes_json, Dict):
-        # If it's a dictionary, directly use the decoder hook to deserialize it
-        return node_json_hook(nodes_json)
-
-    # Check if the input is a JSON-formatted string
-    elif isinstance(nodes_json, str):
-        # If it's a JSON string, parse and deserialize it using the decoder hook
-        return json.loads(nodes_json, object_hook=node_json_hook)
-
-    # Raise an error if the input type is unsupported
-    else:
-        raise TypeError(f"Unsupported type for nodes_json: {type(nodes_json)}")
-    # TODO: enable this logic to replace proxies, once beartype is OK with that.
-    # def recursive_proxy_replacement(node, handled_nodes):
-    #     if isinstance(node, _UIDProxy):
-    #         try:
-    #             node = node_json_hook._uid_cache[node.uid]
-    #         except KeyError as exc:
-    #             raise CRIPTDeserializationUIDError(node.node_type, node.uid)
-    #         return node
-    #     handled_nodes.add(node.uid)
-    #     for field in node._json_attrs.__dict__:
-    #         child_node = getattr(node._json_attrs, field)
-    #         if not isinstance(child_node, list):
-    #             if hasattr(cn, "__bases__") and BaseNode in child_node.__bases__:
-    #                 child_node = recursive_proxy_replacement(child_node, handled_nodes)
-    #                 node._json_attrs = replace(node._json_attrs, field=child_node)
-    #         else:
-    #             for i, cn in enumerate(child_node):
-    #                 if hasattr(cn, "__bases__") and BaseNode in cn.__bases__:
-    #                     if cn.uid not in handled_nodes:
-    #                         child_node[i] = recursive_proxy_replacement(cn, handled_nodes)
-
-    #     return node
-    # handled_nodes = set()
-    # recursive_proxy_replacement(json_nodes, handled_nodes)
-
-
-def add_orphaned_nodes_to_project(project: Project, active_experiment: Experiment, max_iteration: int = -1):
-    """
-    Helper function that adds all orphaned material nodes of the project graph to the
-    `project.materials` attribute.
-    Material additions only is permissible with `active_experiment is None`.
-    This function also adds all orphaned data, process, computation and computational process nodes
-    of the project graph to the `active_experiment`.
-    This functions call `project.validate` and might raise Exceptions from there.
-    """
-    if active_experiment is not None and active_experiment not in project.find_children({"node": ["Experiment"]}):
-        raise RuntimeError(f"The provided active experiment {active_experiment} is not part of the project graph. Choose an active experiment that is part of a collection of this project.")
-
-    counter = 0
-    while True:
-        if counter > max_iteration >= 0:
-            break  # Emergency stop
-        try:
-            project.validate()
-        except CRIPTOrphanedMaterialError as exc:
-            # because calling the setter calls `validate` we have to force add the material.
-            project._json_attrs.material.append(exc.orphaned_node)
-        except CRIPTOrphanedDataError as exc:
-            active_experiment.data += [exc.orphaned_node]
-        except CRIPTOrphanedProcessError as exc:
-            active_experiment.process += [exc.orphaned_node]
-        except CRIPTOrphanedComputationError as exc:
-            active_experiment.computation += [exc.orphaned_node]
-        except CRIPTOrphanedComputationalProcessError as exc:
-            active_experiment.computation_process += [exc.orphaned_node]
-        else:
-            break
-        counter += 1
+"""
+This module contains classes and functions that help with the json serialization and deserialization of nodes.
+"""
+import dataclasses
+import inspect
+import json
+import uuid
+from typing import Dict, List, Optional, Set, Union
+
+import cript.nodes
+from cript.nodes.core import BaseNode
+from cript.nodes.exceptions import (
+    CRIPTDeserializationUIDError,
+    CRIPTJsonDeserializationError,
+    CRIPTJsonNodeError,
+)
+from cript.nodes.util.core import iterate_leaves
+from cript.nodes.uuid_base import UUIDBaseNode
+
+
+@dataclasses.dataclass(frozen=True)
+class UIDProxy:
+    """Helper class that store temporarily unresolved UIDs."""
+
+    uid: Optional[str] = None
+
+    def __post_init__(self):
+        if self.uid is None:
+            raise RuntimeError("UID needs to be initialized")
+
+
+class NodeEncoder(json.JSONEncoder):
+    """
+    Custom JSON encoder for serializing CRIPT nodes to JSON.
+
+    This encoder is used to convert CRIPT nodes into JSON format while handling unique identifiers (UUIDs) and
+    condensed representations to avoid redundancy in the JSON output.
+    It also allows suppressing specific attributes from being included in the serialized JSON.
+
+    Attributes
+    ----------
+    handled_ids : set[str]
+        A set to store the UIDs of nodes that have been processed during serialization.
+    known_uuid : set[str]
+        A set to store the UUIDs of nodes that have been previously encountered in the JSON.
+    condense_to_uuid : dict[str, set[str]]
+        A set to store the node types that should be condensed to UUID edges in the JSON.
+    suppress_attributes : Optional[dict[str, set[str]]]
+
+    Methods
+    -------
+    ```python
+    default(self, obj: Any) -> Any:
+        # Convert CRIPT nodes and other objects to their JSON representation.
+    ```
+
+    ```python
+    _apply_modifications(self, serialize_dict: dict) -> Tuple[dict, list[str]]:
+        # Apply modifications to the serialized dictionary based on node types
+        # and attributes to be condensed. This internal function handles node
+        # condensation and attribute suppression during serialization.
+    ```
+    """
+
+    handled_ids: Set[str] = set()
+    known_uuid: Set[str] = set()
+    condense_to_uuid: Dict[str, Set[str]] = dict()
+    suppress_attributes: Optional[Dict[str, Set[str]]] = None
+
+    def default(self, obj):
+        """
+        Convert CRIPT nodes and other objects to their JSON representation.
+
+        This method is called during JSON serialization.
+        It customizes the serialization process for CRIPT nodes and handles unique identifiers (UUIDs)
+        to avoid redundant data in the JSON output.
+        It also allows for attribute suppression for specific nodes.
+
+        Parameters
+        ----------
+        obj : Any
+            The object to be serialized to JSON.
+
+        Returns
+        -------
+        dict
+            The JSON representation of the input object, which can be a string, a dictionary, or any other JSON-serializable type.
+
+        Raises
+        ------
+        CRIPTJsonDeserializationError
+            If there is an issue with the JSON deserialization process for CRIPT nodes.
+
+        Notes
+        -----
+        * If the input object is a UUID, it is converted to a string representation and returned.
+        * If the input object is a CRIPT node (an instance of `BaseNode`), it is serialized into a dictionary
+          representation. The node is first checked for uniqueness based on its UID (unique identifier), and if
+          it has already been serialized, it is represented as a UUID edge only. If not, the node's attributes
+          are added to the dictionary representation, and any default attribute values are removed to reduce
+          redundancy in the JSON output.
+        * The method `_apply_modifications()` is called to check if further modifications are needed before
+          considering the dictionary representation done. This includes condensing certain node types to UUID edges
+          and suppressing specific attributes for nodes.
+        """
+        if isinstance(obj, uuid.UUID):
+            return str(obj)
+
+        if isinstance(obj, UIDProxy):
+            return obj.uid
+
+        if isinstance(obj, BaseNode):
+            try:
+                uid = obj.uid
+            except AttributeError:
+                pass
+            else:
+                if uid in NodeEncoder.handled_ids:
+                    return {"uid": uid}
+
+            # When saving graphs, some nodes can be pre-saved.
+            # If that happens, we want to represent them as a UUID edge only
+            try:
+                uuid_str = str(obj.uuid)
+            except AttributeError:
+                pass
+            else:
+                if uuid_str in NodeEncoder.known_uuid:
+                    return {"uuid": uuid_str}
+
+            default_dataclass = obj.JsonAttributes()
+            serialize_dict = {}
+            # Remove default values from serialization
+            for field_name in [field.name for field in dataclasses.fields(default_dataclass)]:
+                if getattr(default_dataclass, field_name) != getattr(obj._json_attrs, field_name):
+                    serialize_dict[field_name] = getattr(obj._json_attrs, field_name)
+            # add the default node type
+            serialize_dict["node"] = obj._json_attrs.node
+
+            # check if further modifications to the dict is needed before considering it done
+            serialize_dict, condensed_uid = self._apply_modifications(serialize_dict)
+            if uid not in condensed_uid:  # We can uid (node) as handled if we don't condense it to uuid
+                NodeEncoder.handled_ids.add(uid)
+
+            # Remove suppressed attributes
+            if NodeEncoder.suppress_attributes is not None and str(obj.uuid) in NodeEncoder.suppress_attributes:
+                for attr in NodeEncoder.suppress_attributes[str(obj.uuid)]:
+                    del serialize_dict[attr]
+
+            return serialize_dict
+        return json.JSONEncoder.default(self, obj)
+
+    def _apply_modifications(self, serialize_dict: Dict):
+        """
+        Checks the serialize_dict to see if any other operations are required before it
+        can be considered done. If other operations are required, then it passes it to the other operations
+        and at the end returns the fully finished dict.
+
+        This function is essentially a big switch case that checks the node type
+        and determines what other operations are required for it.
+
+        Parameters
+        ----------
+        serialize_dict: Dict
+
+        Returns
+        -------
+        serialize_dict: Dict
+        """
+
+        def process_attribute(attribute):
+            def strip_to_edge_uuid(element):
+                # Extracts UUID and UID information from the element
+                try:
+                    uuid = getattr(element, "uuid")
+                except AttributeError:
+                    uuid = element["uuid"]
+                    if len(element) == 1:  # Already a condensed element
+                        return element, None
+                try:
+                    uid = getattr(element, "uid")
+                except AttributeError:
+                    uid = element["uid"]
+
+                element = {"uuid": str(uuid)}
+                return element, uid
+
+            # Processes an attribute based on its type (list or single element)
+            if isinstance(attribute, List):
+                processed_elements = []
+                for element in attribute:
+                    processed_element, uid = strip_to_edge_uuid(element)
+                    if uid is not None:
+                        uid_of_condensed.append(uid)
+                    processed_elements.append(processed_element)
+                return processed_elements
+            else:
+                processed_attribute, uid = strip_to_edge_uuid(attribute)
+                if uid is not None:
+                    uid_of_condensed.append(uid)
+                return processed_attribute
+
+        uid_of_condensed: List = []
+
+        nodes_to_condense = serialize_dict["node"]
+        for node_type in nodes_to_condense:
+            if node_type in self.condense_to_uuid:
+                attributes_to_process = self.condense_to_uuid[node_type]  # type: ignore
+                for attribute in attributes_to_process:
+                    if attribute in serialize_dict:
+                        attribute_to_condense = serialize_dict[attribute]
+                        processed_attribute = process_attribute(attribute_to_condense)
+                        serialize_dict[attribute] = processed_attribute
+
+        return serialize_dict, uid_of_condensed
+
+
+class _NodeDecoderHook:
+    def __init__(self, uid_cache: Optional[Dict] = None):
+        """
+        Initialize the custom JSON object hook used for CRIPT node deserialization.
+
+        Parameters
+        ----------
+        uid_cache : Optional[dict], optional
+            A dictionary to cache Python objects with shared UIDs, by default None.
+
+        Notes
+        -----
+        The `_NodeDecoderHook` class is used as an object hook for JSON deserialization,
+        handling the conversion of JSON nodes into Python objects based on their node types.
+        The `uid_cache` is an optional dictionary to store cached objects with shared UIDs
+        to never create two different python nodes with the same uid.
+        """
+        if uid_cache is None:
+            uid_cache = {}
+        self._uid_cache = uid_cache
+
+    @property
+    def uid_cache(self):
+        return self._uid_cache
+
+    def __call__(self, node_str: Union[Dict, str]) -> Union[Dict, UIDProxy]:
+        """
+        Internal function, used as a hook for json deserialization.
+
+        This function is called recursively to convert every JSON of a node and its children from node to JSON.
+
+        If given a JSON without a "node" field then it is assumed that it is not a node
+        and just a key value pair data, and the JSON string is then just converted from string to dict and returned
+        applicable for places where the data is something like
+
+        ```json
+        { "bigsmiles": "123456" }
+        ```
+
+        no serialization is needed in this case and just needs to be converted from str to dict
+
+        if the node field is present, then continue and convert the JSON node into a Python object
+
+        Parameters
+        ----------
+        node_str : Union[Dict, str]
+            The JSON representation of a node or a regular dictionary.
+
+        Returns
+        -------
+        Union[CRIPT Node, dict]
+            Either returns a regular dictionary if the input JSON or input dict is NOT a node.
+            If it is a node, it returns the appropriate CRIPT node object, such as `cript.Material`
+
+        Raises
+        ------
+        CRIPTJsonNodeError
+            If there is an issue with the JSON structure or the node type is invalid.
+        CRIPTJsonDeserializationError
+            If there is an error during deserialization of a specific node type.
+        CRIPTDeserializationUIDError
+            If there is an issue with the UID used for deserialization, like circular references.
+        """
+        node_dict = dict(node_str)  # type: ignore
+
+        # Handle UID objects.
+        if len(node_dict) == 1 and "uid" in node_dict:
+            try:
+                return self._uid_cache[node_dict["uid"]]
+            except KeyError:
+                # raise CRIPTDeserializationUIDError("Unknown", node_dict["uid"])
+                proxy = UIDProxy(uid=node_dict["uid"])
+                return proxy
+
+        try:
+            node_type_list = node_dict["node"]
+        except KeyError:  # Not a node, just a regular dictionary
+            return node_dict
+
+        # TODO consider putting this into the try because it might need error handling for the dict
+        if _is_node_field_valid(node_type_list):
+            node_type_str = node_type_list[0]
+        else:
+            raise CRIPTJsonNodeError(node_type_list, str(node_str))
+
+        # Iterate over all nodes in cript to find the correct one here
+        for key, pyclass in inspect.getmembers(cript.nodes, inspect.isclass):
+            if BaseNode in inspect.getmro(pyclass):
+                if key == node_type_str:
+                    try:
+                        json_node = pyclass._from_json(node_dict)
+                        self._uid_cache[json_node.uid] = json_node
+                        return json_node
+                    except Exception as exc:
+                        raise CRIPTJsonDeserializationError(key, str(node_type_str)) from exc
+        # Fall back
+        return node_dict
+
+    def resolve_unresolved_uids(self, node_iter):
+        def handle_uid_replacement(node, name, attr):
+            if isinstance(attr, UIDProxy):
+                unresolved_uid = attr.uid
+                try:
+                    uid_node = self.uid_cache[unresolved_uid]
+                except KeyError as exc:
+                    raise CRIPTDeserializationUIDError("Unknown", unresolved_uid) from exc
+                updated_attrs = dataclasses.replace(node._json_attrs, **{name: uid_node})
+                node._update_json_attrs_if_valid(updated_attrs)
+
+        for node_leaves in iterate_leaves(node_iter):
+            if isinstance(node_leaves, BaseNode):
+                for node in node_leaves:
+                    field_names = [field.name for field in dataclasses.fields(node._json_attrs)]
+                    for field_name in field_names:
+                        field_attr = getattr(node._json_attrs, field_name)
+                        handle_uid_replacement(node, field_name, field_attr)
+                        if isinstance(field_attr, list):
+                            for i in range(len(field_attr)):
+                                if isinstance(field_attr[i], UIDProxy):
+                                    try:
+                                        field_attr[i] = self.uid_cache[field_attr[i].uid]
+                                    except KeyError as exc:
+                                        raise CRIPTDeserializationUIDError("Unknown", field_attr[i].uid) from exc
+        return node_iter
+
+
+def load_nodes_from_json(nodes_json: Union[str, Dict], api=None, _use_uuid_cache: Optional[Dict] = None, skip_validation: bool = False):
+    """
+    User facing function, that return a node and all its children from a json string input.
+
+    Parameters
+    ----------
+    nodes_json: Union[str, dict]
+        JSON string representation of a CRIPT node
+
+    Examples
+    --------
+    >>> import cript
+    >>> # Get updated project from API
+    >>> my_paginator = api.search(
+    ...     node_type=cript.Project,
+    ...     search_mode=cript.SearchModes.EXACT_NAME,
+    ...     value_to_search="my project name",
+    ... ) # doctest: +SKIP
+    >>> # Take specific Project you want from paginator
+    >>> my_project_from_api_dict: dict = my_paginator.current_page_results[0] # doctest: +SKIP
+    >>> # Deserialize your Project dict into a Project node
+    >>> my_project_node_from_api = cript.load_nodes_from_json( # doctest: +SKIP
+    ...     nodes_json=my_project_from_api_dict
+    ... )
+
+    Raises
+    ------
+    CRIPTJsonNodeError
+        If there is an issue with the JSON of the node field.
+    CRIPTJsonDeserializationError
+        If there is an error during deserialization of a specific node.
+    CRIPTDeserializationUIDError
+        If there is an issue with the UID used for deserialization, like circular references.
+
+    Notes
+    -----
+    This function uses a custom `_NodeDecoderHook` to convert JSON nodes into Python objects.
+    The `_NodeDecoderHook` class is responsible for handling the deserialization of nodes
+    and caching objects with shared UIDs to avoid redundant deserialization.
+
+    The function is intended for deserializing CRIPT nodes and should not be used for generic JSON.
+
+    Returns
+    -------
+    Union[CRIPT Node, List[CRIPT Node]]
+        Typically returns a single CRIPT node,
+        but if given a list of nodes, then it will serialize them and return a list of CRIPT nodes
+    """
+    from cript.api.api import _get_global_cached_api
+
+    if api is None:
+        api = _get_global_cached_api()
+
+    # Initialize the custom decoder hook for JSON deserialization
+    node_json_hook = _NodeDecoderHook()
+
+    # Convert everything into a string. This is slightly inefficient for already encoded dicts,
+    # but catches a lot of odd cases. And at the moment performance is not bottle necked here
+    if not isinstance(nodes_json, str):
+        nodes_json = json.dumps(nodes_json)
+
+    # Store previous UUIDBaseNode Cache state
+    previous_uuid_cache = UUIDBaseNode._uuid_cache
+
+    if _use_uuid_cache is not None:  # If requested use a custom cache.
+        UUIDBaseNode._uuid_cache = _use_uuid_cache
+
+    previous_skip_validation = api.schema.skip_validation
+    # Temporarily disable validation while loading nodes from JSON
+    api.schema.skip_validation = True
+    try:
+        loaded_nodes = json.loads(nodes_json, object_hook=node_json_hook)
+        loaded_nodes = node_json_hook.resolve_unresolved_uids(loaded_nodes)
+    finally:
+        # Definitively restore the old cache state
+        UUIDBaseNode._uuid_cache = previous_uuid_cache
+        api.schema.skip_validation = previous_skip_validation
+
+    # If nodes are actually expected to be checked, do it now
+    if not previous_skip_validation and not skip_validation:
+        for node in iterate_leaves(loaded_nodes):
+            if isinstance(node, BaseNode):
+                node.validate()
+
+    if _use_uuid_cache is not None:
+        return loaded_nodes, _use_uuid_cache
+    return loaded_nodes
+
+
+def _rename_field(serialize_dict: Dict, old_name: str, new_name: str) -> Dict:
+    """
+    renames `property_` to `property` the JSON
+    """
+    if "property_" in serialize_dict:
+        serialize_dict[new_name] = serialize_dict.pop(old_name)
+
+    return serialize_dict
+
+
+def _is_node_field_valid(node_type_list: List) -> bool:
+    """
+    a simple function that checks if the node field has only a single node type in there
+    and not 2 or None
+
+    Parameters
+    ----------
+    node_type_list: List
+        e.g. "node": ["Material"]
+
+    Returns
+    ------
+    bool
+        if all tests pass then it returns true, otherwise false
+    """
+
+    # TODO consider having exception handling for the dict
+    if isinstance(node_type_list, list) and len(node_type_list) == 1 and isinstance(node_type_list[0], str) and len(node_type_list[0]) > 0:
+        return True
+    else:
+        return False
```

### Comparing `cript-2.2.0/src/cript/nodes/uuid_base.py` & `cript-2.3.0/src/cript/nodes/uuid_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import uuid
 from abc import ABC
 from dataclasses import dataclass, field, replace
-from typing import Any, Dict
-
-from cript.nodes.core import BaseNode
+from typing import Any, Dict, Optional
 
+from beartype import beartype
 
-def get_uuid_from_uid(uid):
-    return str(uuid.UUID(uid[2:]))
+from cript.nodes.core import BaseNode
+from cript.nodes.exceptions import CRIPTUUIDException
+from cript.nodes.node_iterator import NodeIterator
 
 
 class UUIDBaseNode(BaseNode, ABC):
     """
     Base node that handles UUIDs and URLs.
     """
 
@@ -28,40 +28,50 @@
         updated_by: Any = None
         created_by: Any = None
         created_at: str = ""
         updated_at: str = ""
 
     _json_attrs: JsonAttributes = JsonAttributes()
 
+    def __new__(cls, *args, **kwargs):
+        uuid: Optional[str] = str(kwargs.get("uuid"))
+        if uuid and uuid in UUIDBaseNode._uuid_cache:
+            existing_node_to_overwrite = UUIDBaseNode._uuid_cache[uuid]
+            if type(existing_node_to_overwrite) is not cls:
+                raise CRIPTUUIDException(uuid, type(existing_node_to_overwrite), cls)
+            return existing_node_to_overwrite
+        new_uuid_node = super().__new__(cls)
+        return new_uuid_node
+
     def __init__(self, **kwargs):
+        from cript.nodes.util.core import get_uuid_from_uid
+
         # initialize Base class with node
         super().__init__(**kwargs)
         # Respect uuid if passed as argument, otherwise construct uuid from uid
-        uuid = kwargs.get("uuid", get_uuid_from_uid(self.uid))
+        uuid: str = kwargs.get("uuid", get_uuid_from_uid(self.uid))
         # replace name and notes within PrimaryBase
         self._json_attrs = replace(self._json_attrs, uuid=uuid)
-
-        # Place successfully created node in the UUID cache
-        self._uuid_cache[uuid] = self
+        UUIDBaseNode._uuid_cache[uuid] = self
 
     @property
-    def uuid(self) -> uuid.UUID:
-        return uuid.UUID(self._json_attrs.uuid)
+    @beartype
+    def uuid(self) -> str:
+        if not isinstance(self._json_attrs.uuid, str):
+            # Some JSON decoding automatically converted this to UUID objects, which we don't want
+            self._json_attrs = replace(self._json_attrs, uuid=str(self._json_attrs.uuid))
+
+        return self._json_attrs.uuid
 
     @property
     def url(self):
         from cript.api.api import _get_global_cached_api
 
         api = _get_global_cached_api()
-        return f"{api.host}/{self.uuid}"
-
-    def __deepcopy__(self, memo):
-        node = super().__deepcopy__(memo)
-        node._json_attrs = replace(node._json_attrs, uuid=get_uuid_from_uid(node.uid))
-        return node
+        return f"{api.host}/{api.api_prefix}/{api.api_version}/{self.uuid}"
 
     @property
     def updated_by(self):
         return self._json_attrs.updated_by
 
     @property
     def created_by(self):
@@ -70,7 +80,11 @@
     @property
     def updated_at(self):
         return self._json_attrs.updated_at
 
     @property
     def created_at(self):
         return self._json_attrs.created_at
+
+    def __iter__(self) -> NodeIterator:
+        """Enables DFS iteration over all children."""
+        return NodeIterator(self)
```

### Comparing `cript-2.2.0/src/cript.egg-info/PKG-INFO` & `cript-2.3.0/src/cript.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-Metadata-Version: 2.1
-Name: cript
-Version: 2.2.0
-Summary: CRIPT Python SDK
-Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
-Author: CRIPT Development Team
-License: MIT
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Scientific/Engineering
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests==2.31.0
-Requires-Dist: jsonschema>=4.17.3
-Requires-Dist: beartype==0.14.1
-Requires-Dist: boto3==1.28.39
-
-# CRIPT Python SDK
-
-[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-
-[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
-[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
-[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
-[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
-[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
-[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
-[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
-[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
-
-[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
-[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
-[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
-[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
-
-<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
-
-<!-- just shows pass/fail instead of percentage
-[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
--->
-
-## CRIPT Availability
-
-Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
-
----
-
-## What is it?
-
-The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
-
----
-
-## Installation
-
-CRIPT Python SDK requires Python 3.8+
-
-The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
-
-```bash
-pip install cript
-```
-
----
-
-## Documentation
-
-To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
-
-To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
-
----
-
-## Release Notes
-
-Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
-
----
-
-## We Invite Contribution
-
-To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
-a detailed guide on how to contribute to our repository and become a part of our community.
-
-Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
-
-For development documentation to better understand the Python SDK code please visit the
-[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
-If you encounter any issues please let us know via
-[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
-[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
-
-To learn more about our great community and all the open source plugins made by our fantastic community available
-for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
-[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
-
-We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
-
-Happy coding!
+Metadata-Version: 2.1
+Name: cript
+Version: 2.3.0
+Summary: CRIPT Python SDK
+Home-page: https://github.com/C-Accel-CRIPT/Python-SDK
+Author: CRIPT Development Team
+License: MIT
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: requests==2.31.0
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: beartype==0.14.1
+Requires-Dist: boto3==1.28.39
+
+# CRIPT Python SDK
+
+[![License](./CRIPT_full_logo_colored_transparent.png)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+
+[![License](https://img.shields.io/github/license/C-Accel-CRIPT/cript?style=flat-square)](https://github.com/C-Accel-CRIPT/Python-SDK/blob/develop/LICENSE.md)
+[![Python](https://img.shields.io/badge/Language-Python%203.8+-blue?style=flat-square&logo=python)](https://www.python.org/)
+[![Code style is black](https://img.shields.io/badge/Code%20Style-black-000000.svg?style=flat-square&logo=python)](https://github.com/psf/black)
+[![Link to CRIPT website](https://img.shields.io/badge/platform-criptapp.org-blueviolet?style=flat-square)](https://criptapp.org/)
+[![Using Pytest](https://img.shields.io/badge/Dependencies-pytest-green?style=flat-square&logo=Pytest)](https://docs.pytest.org/en/7.2.x/)
+[![Using JSONSchema](https://img.shields.io/badge/Dependencies-jsonschema-blueviolet?style=flat-square&logo=json)](https://python-JSONSchema.readthedocs.io/en/stable/)
+[![Using Requests Library](https://img.shields.io/badge/Dependencies-Requests-blueviolet?style=flat-square&logo=python)](https://requests.readthedocs.io/en/latest/)
+[![Material MkDocs](https://img.shields.io/badge/Docs-mkdocs--material-blueviolet?style=flat-square&logo=markdown)](https://squidfunk.github.io/mkdocs-material/)
+
+[![trunk CI](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/trunk.yml)
+[![Tests](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/codeql.yml)
+[![mypy](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/mypy_check.yaml)
+
+<!-- [![Safe Dependencies](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/dependency-review.yml) -->
+
+<!-- just shows pass/fail instead of percentage
+[![Test Coverage](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml/badge.svg)](https://github.com/C-Accel-CRIPT/Python-SDK/actions/workflows/test_coverage.yaml)
+-->
+
+## CRIPT Availability
+
+Currently, CRIPT is only available for users in the USA, and it is equipped with geo-blocking functionality that restricts access for users outside the USA. We are diligently working towards making CRIPT accessible worldwide. We appreciate your patience as we strive to achieve this goal!
+
+---
+
+## What is it?
+
+The CRIPT Python SDK allows programmatic access to the [CRIPT platform](https://criptapp.org). It can help automate uploading your data to CRIPT, and aims to allow for manipulation of your CRIPT data through the python language. This is a perfect tool for users who have python experience and have large amount of data to upload to [CRIPT](https://criptapp.org).
+
+---
+
+## Installation
+
+CRIPT Python SDK requires Python 3.8+
+
+The latest released of CRIPT Python SDK is available on [Python Package Index (PyPI)](https://pypi.org/project/cript/)
+
+```bash
+pip install cript
+```
+
+---
+
+## Documentation
+
+To learn more about the CRIPT Python SDK please check the [CRIPT Python SDK user documentation](https://c-accel-cript.github.io/Python-SDK/)
+
+To learn more about the internal workings of the CRIPT Python SDK please check the [CRIPT Python SDK internal documentation](https://github.com/C-Accel-CRIPT/Python-SDK/wiki)
+
+---
+
+## Release Notes
+
+Please visit the [GitHub Releases page](https://github.com/C-Accel-CRIPT/Python-SDK/releases/latest) for a detailed release notes.
+
+---
+
+## We Invite Contribution
+
+To get started, feel free to take a look at our [Contribution Guidelines](CONTRIBUTING.md) for
+a detailed guide on how to contribute to our repository and become a part of our community.
+
+Whether you want to report a bug, propose a new feature, or submit a pull request, your contribution is highly valued.
+
+For development documentation to better understand the Python SDK code please visit the
+[Python SDK Wiki](https://github.com/C-Accel-CRIPT/Python-SDK/wiki).
+If you encounter any issues please let us know via
+[issues section](https://github.com/C-Accel-CRIPT/Python-SDK/issues) or
+[discussion sections](https://github.com/C-Accel-CRIPT/Python-SDK/discussions).
+
+To learn more about our great community and all the open source plugins made by our fantastic community available
+for the [CRIPT Python SDK](https://github.com/C-Accel-CRIPT/Python-SDK) please take a look at the
+[plugins section](https://github.com/C-Accel-CRIPT/Python-SDK/discussions/categories/plugins).
+
+We appreciate your interest in contributing to our project! Together, let's make it even better! 🚀
+
+Happy coding!
```

### Comparing `cript-2.2.0/src/cript.egg-info/SOURCES.txt` & `cript-2.3.0/src/cript.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 src/cript.egg-info/SOURCES.txt
 src/cript.egg-info/dependency_links.txt
 src/cript.egg-info/requires.txt
 src/cript.egg-info/top_level.txt
 src/cript/api/__init__.py
 src/cript/api/api.py
 src/cript/api/api_config.py
+src/cript/api/data_schema.py
 src/cript/api/exceptions.py
 src/cript/api/paginator.py
 src/cript/api/valid_search_modes.py
 src/cript/api/vocabulary_categories.py
 src/cript/api/utils/__init__.py
 src/cript/api/utils/aws_s3_utils.py
 src/cript/api/utils/get_host_token.py
 src/cript/api/utils/helper_functions.py
 src/cript/api/utils/save_helper.py
 src/cript/api/utils/web_file_downloader.py
 src/cript/nodes/__init__.py
 src/cript/nodes/core.py
 src/cript/nodes/exceptions.py
+src/cript/nodes/node_iterator.py
 src/cript/nodes/uuid_base.py
 src/cript/nodes/primary_nodes/__init__.py
 src/cript/nodes/primary_nodes/collection.py
 src/cript/nodes/primary_nodes/computation.py
 src/cript/nodes/primary_nodes/computation_process.py
 src/cript/nodes/primary_nodes/data.py
 src/cript/nodes/primary_nodes/experiment.py
@@ -51,9 +53,10 @@
 src/cript/nodes/subobjects/quantity.py
 src/cript/nodes/subobjects/software.py
 src/cript/nodes/subobjects/software_configuration.py
 src/cript/nodes/supporting_nodes/__init__.py
 src/cript/nodes/supporting_nodes/file.py
 src/cript/nodes/supporting_nodes/user.py
 src/cript/nodes/util/__init__.py
-src/cript/nodes/util/material_deserialization.py
+src/cript/nodes/util/core.py
+src/cript/nodes/util/json.py
 tests/test_node_util.py
```

### Comparing `cript-2.2.0/tests/test_node_util.py` & `cript-2.3.0/tests/test_node_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,347 +1,366 @@
-import copy
-import json
-from dataclasses import replace
-
-import pytest
-
-import cript
-from cript.nodes.core import get_new_uid
-from cript.nodes.exceptions import (
-    CRIPTJsonNodeError,
-    CRIPTJsonSerializationError,
-    CRIPTNodeSchemaError,
-    CRIPTOrphanedComputationalProcessError,
-    CRIPTOrphanedComputationError,
-    CRIPTOrphanedDataError,
-    CRIPTOrphanedMaterialError,
-    CRIPTOrphanedProcessError,
-)
-from tests.utils.util import strip_uid_from_dict
-
-
-def test_removing_nodes(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
-    a = simple_algorithm_node
-    p = complex_parameter_node
-    a.parameter += [p]
-    assert strip_uid_from_dict(json.loads(a.json)) != simple_algorithm_dict
-    a.remove_child(p)
-    assert strip_uid_from_dict(json.loads(a.json)) == simple_algorithm_dict
-
-
-def test_uid_deserialization(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
-    identifier = [{"bigsmiles": "123456"}]
-    material = cript.Material(name="my material", identifier=identifier)
-
-    computation = cript.Computation(name="my computation name", type="analysis")
-    property1 = cript.Property("modulus_shear", "value", 5.0, "GPa", computation=[computation])
-    property2 = cript.Property("modulus_loss", "value", 5.0, "GPa", computation=[computation])
-    material.property = [property1, property2]
-
-    material2 = cript.load_nodes_from_json(material.json)
-    assert json.loads(material.json) == json.loads(material2.json)
-
-    material3_dict = {
-        "node": ["Material"],
-        "uid": "_:f6d56fdc-9df7-49a1-a843-cf92681932ad",
-        "uuid": "f6d56fdc-9df7-49a1-a843-cf92681932ad",
-        "name": "my material",
-        "property": [
-            {
-                "node": ["Property"],
-                "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
-                "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
-                "key": "modulus_shear",
-                "type": "value",
-                "value": 5.0,
-                "unit": "GPa",
-                "computation": [{"uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef"}],
-            },
-            {
-                "node": ["Property"],
-                "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-                "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-                "key": "modulus_loss",
-                "type": "value",
-                "value": 5.0,
-                "unit": "GPa",
-                "computation": [
-                    {
-                        "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
-                    }
-                ],
-            },
-        ],
-        "bigsmiles": "123456",
-    }
-
-    with pytest.raises(cript.nodes.exceptions.CRIPTDeserializationUIDError):
-        cript.load_nodes_from_json(json.dumps(material3_dict))
-
-    # TODO convince beartype to allow _ProxyUID as well
-    # material4_dict = {
-    #     "node": [
-    #         "Material"
-    #     ],
-    #     "uid": "_:f6d56fdc-9df7-49a1-a843-cf92681932ad",
-    #     "uuid": "f6d56fdc-9df7-49a1-a843-cf92681932ad",
-    #     "name": "my material",
-    #     "property": [
-    #         {
-    #             "node": [
-    #                 "Property"
-    #             ],
-    #             "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
-    #             "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
-    #             "key": "modulus_shear",
-    #             "type": "value",
-    #             "value": 5.0,
-    #             "unit": "GPa",
-    #             "computation": [
-    #                 {
-    #                     "node": [
-    #                         "Computation"
-    #                     ],
-    #                     "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef"
-    #                 }
-    #             ]
-    #         },
-    #         {
-    #             "node": [
-    #                 "Property"
-    #             ],
-    #             "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-    #             "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
-    #             "key": "modulus_loss",
-    #             "type": "value",
-    #             "value": 5.0,
-    #             "unit": "GPa",
-    #             "computation": [
-    #                 {
-    #                     "node": [
-    #                         "Computation"
-    #                     ],
-    #                     "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
-    #                     "uuid": "9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
-    #                     "name": "my computation name",
-    #                     "type": "analysis",
-    #                     "citation": []
-    #                 }
-    #             ]
-    #         }
-    #     ],
-    #     "bigsmiles": "123456"
-    # }
-
-    # material4 = cript.load_nodes_from_json(json.dumps(material4_dict))
-    # assert json.loads(material.json) == json.loads(material4.json)
-
-
-def test_json_error(complex_parameter_node):
-    parameter = complex_parameter_node
-    # Let's break the node by violating the data model
-    parameter._json_attrs = replace(parameter._json_attrs, value="abc")
-    with pytest.raises(CRIPTNodeSchemaError):
-        parameter.validate()
-    # Let's break it completely
-    parameter._json_attrs = None
-    with pytest.raises(CRIPTJsonSerializationError):
-        parameter.json
-
-
-def test_local_search(simple_algorithm_node, complex_parameter_node):
-    a = simple_algorithm_node
-    # Check if we can use search to find the algorithm node, but specifying node and key
-    find_algorithms = a.find_children({"node": "Algorithm", "key": "mc_barostat"})
-    assert find_algorithms == [a]
-    # Check if it correctly exclude the algorithm if key is specified to non-existent value
-    find_algorithms = a.find_children({"node": "Algorithm", "key": "mc"})
-    assert find_algorithms == []
-
-    # Adding 2 separate parameters to test deeper search
-    p1 = complex_parameter_node
-    p2 = copy.deepcopy(complex_parameter_node)
-    p2.key = "damping_time"
-    p2.value = 15.0
-    p2.unit = "m"
-    a.parameter += [p1, p2]
-
-    # Test if we can find a specific one of the parameters
-    find_parameter = a.find_children({"key": "damping_time"})
-    assert find_parameter == [p2]
-
-    # Test to find the other parameter
-    find_parameter = a.find_children({"key": "update_frequency"})
-    assert find_parameter == [p1]
-
-    # Test if correctly find no parameter if we are searching for a non-existent parameter
-    find_parameter = a.find_children({"key": "update"})
-    assert find_parameter == []
-
-    # Test nested search. Here we are looking for any node that has a child node parameter as specified.
-    find_algorithms = a.find_children({"parameter": {"key": "damping_time"}})
-    assert find_algorithms == [a]
-    # Same as before, but specifying two children that have to be present (AND condition)
-    find_algorithms = a.find_children({"parameter": [{"key": "damping_time"}, {"key": "update_frequency"}]})
-    assert find_algorithms == [a]
-
-    # Test that the main node is correctly excluded if we specify an additionally non-existent parameter
-    find_algorithms = a.find_children({"parameter": [{"key": "damping_time"}, {"key": "update_frequency"}, {"foo": "bar"}]})
-    assert find_algorithms == []
-
-
-def test_cycles(complex_data_node, simple_computation_node):
-    # We create a wrong cycle with parameters here.
-    # TODO replace this with nodes that actually can form a cycle
-    d = copy.deepcopy(complex_data_node)
-    c = copy.deepcopy(simple_computation_node)
-    d.computation += [c]
-    # Using input and output data guarantees a cycle here.
-    c.output_data += [d]
-    c.input_data += [d]
-
-    # # Test the repetition of a citation.
-    # # Notice that we do not use a deepcopy here, as we want the citation to be the exact same node.
-    # citation = d.citation[0]
-    # # c._json_attrs.citation.append(citation)
-    # c.citation += [citation]
-    # # print(c.get_json(indent=2).json)
-    # # c.validate()
-
-    # Generate json with an implicit cycle
-    c.json
-    d.json
-
-
-def test_uid_serial(simple_inventory_node):
-    simple_inventory_node.material += simple_inventory_node.material
-    json_dict = json.loads(simple_inventory_node.get_json(condense_to_uuid={}).json)
-    assert len(json_dict["material"]) == 4
-    assert isinstance(json_dict["material"][2]["uid"], str)
-    assert json_dict["material"][2]["uid"].startswith("_:")
-    assert len(json_dict["material"][2]["uid"]) == len(get_new_uid())
-    assert isinstance(json_dict["material"][3]["uid"], str)
-    assert json_dict["material"][3]["uid"].startswith("_:")
-    assert len(json_dict["material"][3]["uid"]) == len(get_new_uid())
-    assert json_dict["material"][3]["uid"] != json_dict["material"][2]["uid"]
-
-
-def test_invalid_json_load():
-    def raise_node_dict(node_dict):
-        node_str = json.dumps(node_dict)
-        with pytest.raises(CRIPTJsonNodeError):
-            cript.load_nodes_from_json(node_str)
-
-    node_dict = {"node": "Computation"}
-    raise_node_dict(node_dict)
-    node_dict = {"node": []}
-    raise_node_dict(node_dict)
-    node_dict = {"node": ["asdf", "asdf"]}
-    raise_node_dict(node_dict)
-    node_dict = {"node": [None]}
-    raise_node_dict(node_dict)
-
-
-def test_invalid_project_graphs(simple_project_node, simple_material_node, simple_process_node, simple_property_node, simple_data_node, simple_computation_node, simple_computation_process_node):
-    project = copy.deepcopy(simple_project_node)
-    process = copy.deepcopy(simple_process_node)
-    material = copy.deepcopy(simple_material_node)
-
-    ingredient = cript.Ingredient(material=material, quantity=[cript.Quantity(key="mass", value=1.23, unit="kg")])
-    process.ingredient += [ingredient]
-
-    # Add the process to the experiment, but not in inventory or materials
-    # Invalid graph
-    project.collection[0].experiment[0].process += [process]
-    with pytest.raises(CRIPTOrphanedMaterialError):
-        project.validate()
-
-    # First fix add material to inventory
-    project.collection[0].inventory += [cript.Inventory("test_inventory", material=[material])]
-    project.validate()
-    # Reverse this fix
-    project.collection[0].inventory = []
-    with pytest.raises(CRIPTOrphanedMaterialError):
-        project.validate()
-
-    # Fix by add to the materials list instead.
-    # Using the util helper function for this.
-    cript.add_orphaned_nodes_to_project(project, active_experiment=None, max_iteration=10)
-    project.validate()
-
-    # Now add an orphan process to the graph
-    process2 = copy.deepcopy(simple_process_node)
-    process.prerequisite_process += [process2]
-    with pytest.raises(CRIPTOrphanedProcessError):
-        project.validate()
-
-    # Wrong fix it helper node
-    dummy_experiment = copy.deepcopy(project.collection[0].experiment[0])
-    with pytest.raises(RuntimeError):
-        cript.add_orphaned_nodes_to_project(project, dummy_experiment)
-    # Problem still persists
-    with pytest.raises(CRIPTOrphanedProcessError):
-        project.validate()
-    # Fix by using the helper function correctly
-    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
-
-    # We add property to the material, because that adds the opportunity for orphaned data and computation
-    property = copy.deepcopy(simple_property_node)
-    material.property += [property]
-    project.validate()
-    # Now add an orphan data
-    data = copy.deepcopy(simple_data_node)
-    property.data = [data]
-    with pytest.raises(CRIPTOrphanedDataError):
-        project.validate()
-    # Fix with the helper function
-    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
-
-    # Add an orphan Computation
-    computation = copy.deepcopy(simple_computation_node)
-    property.computation += [computation]
-    with pytest.raises(CRIPTOrphanedComputationError):
-        project.validate()
-    # Fix with the helper function
-    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
-
-    # Add orphan computational process
-    comp_proc = copy.deepcopy(simple_computation_process_node)
-    data.computation_process += [comp_proc]
-    with pytest.raises(CRIPTOrphanedComputationalProcessError):
-        while True:
-            try:  # Do trigger not orphan materials
-                project.validate()
-            except CRIPTOrphanedMaterialError as exc:
-                project._json_attrs.material.append(exc.orphaned_node)
-            except CRIPTOrphanedProcessError as exc:
-                project.collection[0].experiment[0]._json_attrs.process.append(exc.orphaned_node)
-            else:
-                break
-
-    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
-    project.validate()
-
-
-def test_expanded_json(complex_project_node):
-    """
-    Tests the generation and deserialization of expanded JSON for a complex project node.
-
-    This test verifies 2 key aspects:
-        1. A complex project node can be serialized into an expanded JSON string, without UUID placeholders.
-        2. The expanded JSON can be deserialized into a node  that is equivalent to the original node.
-    """
-    project_expanded_json: str = complex_project_node.get_expanded_json()
-    deserialized_project_node: cript.Project = cript.load_nodes_from_json(project_expanded_json)
-
-    # assert the expanded JSON was correctly deserialized to project node
-    assert deserialized_project_node == complex_project_node
-
-    condensed_json: str = complex_project_node.json
-
-    # since short JSON has UUID it will not be able to deserialize correctly and will
-    # raise CRIPTJsonDeserializationError
-    with pytest.raises(cript.nodes.exceptions.CRIPTJsonDeserializationError):
-        cript.load_nodes_from_json(condensed_json)
+import copy
+import json
+from dataclasses import replace
+
+import pytest
+
+import cript
+from cript.nodes.core import get_new_uid
+from cript.nodes.exceptions import (
+    CRIPTJsonNodeError,
+    CRIPTJsonSerializationError,
+    CRIPTNodeSchemaError,
+    CRIPTOrphanedComputationalProcessError,
+    CRIPTOrphanedComputationError,
+    CRIPTOrphanedDataError,
+    CRIPTOrphanedMaterialError,
+    CRIPTOrphanedProcessError,
+)
+from tests.utils.util import strip_uid_from_dict
+
+
+def test_removing_nodes(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
+    a = simple_algorithm_node
+    p = complex_parameter_node
+    a.parameter += [p]
+    assert strip_uid_from_dict(json.loads(a.json)) != simple_algorithm_dict
+    a.remove_child(p)
+    assert strip_uid_from_dict(json.loads(a.json)) == simple_algorithm_dict
+
+
+def test_uid_deserialization(simple_algorithm_node, complex_parameter_node, simple_algorithm_dict):
+    material = cript.Material(name="my material", bigsmiles="{[][$]CC[$][]}")
+
+    computation = cript.Computation(name="my computation name", type="analysis")
+    property1 = cript.Property("modulus_shear", "value", 5.0, "GPa", computation=[computation])
+    property2 = cript.Property("modulus_loss", "value", 5.0, "GPa", computation=[computation])
+    material.property = [property1, property2]
+
+    material2 = cript.load_nodes_from_json(material.json)
+    assert json.loads(material.json) == json.loads(material2.json)
+
+    material3_dict = {
+        "node": ["Material"],
+        "uid": "_:f6d56fdc-9df7-49a1-a843-cf92681932ad",
+        "uuid": "f6d56fdc-9df7-49a1-a843-cf92681932ad",
+        "name": "my material",
+        "property": [
+            {
+                "node": ["Property"],
+                "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
+                "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
+                "key": "modulus_shear",
+                "type": "value",
+                "value": 5.0,
+                "unit": "GPa",
+                "computation": [{"uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef"}],
+            },
+            {
+                "node": ["Property"],
+                "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
+                "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
+                "key": "modulus_loss",
+                "type": "value",
+                "value": 5.0,
+                "unit": "GPa",
+                "computation": [
+                    {
+                        "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
+                    }
+                ],
+            },
+        ],
+        "bigsmiles": "123456",
+    }
+
+    with pytest.raises(cript.nodes.exceptions.CRIPTDeserializationUIDError):
+        cript.load_nodes_from_json(json.dumps(material3_dict))
+
+    # TODO convince beartype to allow _ProxyUID as well
+    # material4_dict = {
+    #     "node": [
+    #         "Material"
+    #     ],
+    #     "uid": "_:f6d56fdc-9df7-49a1-a843-cf92681932ad",
+    #     "uuid": "f6d56fdc-9df7-49a1-a843-cf92681932ad",
+    #     "name": "my material",
+    #     "property": [
+    #         {
+    #             "node": [
+    #                 "Property"
+    #             ],
+    #             "uid": "_:82e7270e-9f35-4b35-80a2-faa6e7f670be",
+    #             "uuid": "82e7270e-9f35-4b35-80a2-faa6e7f670be",
+    #             "key": "modulus_shear",
+    #             "type": "value",
+    #             "value": 5.0,
+    #             "unit": "GPa",
+    #             "computation": [
+    #                 {
+    #                     "node": [
+    #                         "Computation"
+    #                     ],
+    #                     "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef"
+    #                 }
+    #             ]
+    #         },
+    #         {
+    #             "node": [
+    #                 "Property"
+    #             ],
+    #             "uid": "_:fc4dfa5e-742c-4d0b-bb66-2185461f4582",
+    #             "uuid": "fc4dfa5e-742c-4d0b-bb66-2185461f4582",
+    #             "key": "modulus_loss",
+    #             "type": "value",
+    #             "value": 5.0,
+    #             "unit": "GPa",
+    #             "computation": [
+    #                 {
+    #                     "node": [
+    #                         "Computation"
+    #                     ],
+    #                     "uid": "_:9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
+    #                     "uuid": "9ddda2c0-ff8c-4ce3-beb0-e0cafb6169ef",
+    #                     "name": "my computation name",
+    #                     "type": "analysis",
+    #                     "citation": []
+    #                 }
+    #             ]
+    #         }
+    #     ],
+    #     "bigsmiles": "123456"
+    # }
+
+    # material4 = cript.load_nodes_from_json(json.dumps(material4_dict))
+    # assert json.loads(material.json) == json.loads(material4.json)
+
+
+def test_json_error(complex_parameter_node):
+    parameter = complex_parameter_node
+    # Let's break the node by violating the data model
+    parameter._json_attrs = replace(parameter._json_attrs, value="abc")
+    with pytest.raises(CRIPTNodeSchemaError):
+        parameter.validate()
+    # Let's break it completely
+    parameter._json_attrs = None
+    with pytest.raises(CRIPTJsonSerializationError):
+        parameter.json
+
+
+def test_local_search(simple_algorithm_node, complex_parameter_node):
+    a = simple_algorithm_node
+    # Check if we can use search to find the algorithm node, but specifying node and key
+    find_algorithms = a.find_children({"node": "Algorithm", "key": "mc_barostat"})
+    assert find_algorithms == [a]
+    # Check if it correctly exclude the algorithm if key is specified to non-existent value
+    find_algorithms = a.find_children({"node": "Algorithm", "key": "mc"})
+    assert find_algorithms == []
+
+    # Adding 2 separate parameters to test deeper search
+    p1 = complex_parameter_node
+    p2 = copy.deepcopy(complex_parameter_node)
+    p2.key = "damping_time"
+    p2.value = 15.0
+    p2.unit = "m"
+    a.parameter += [p1, p2]
+
+    # Test if we can find a specific one of the parameters
+    find_parameter = a.find_children({"key": "damping_time"})
+    assert find_parameter == [p2]
+
+    # Test to find the other parameter
+    find_parameter = a.find_children({"key": "update_frequency"})
+    assert find_parameter == [p1]
+
+    # Test if correctly find no parameter if we are searching for a non-existent parameter
+    find_parameter = a.find_children({"key": "update"})
+    assert find_parameter == []
+
+    # Test nested search. Here we are looking for any node that has a child node parameter as specified.
+    find_algorithms = a.find_children({"parameter": {"key": "damping_time"}})
+    assert find_algorithms == [a]
+    # Same as before, but specifying two children that have to be present (AND condition)
+    find_algorithms = a.find_children({"parameter": [{"key": "damping_time"}, {"key": "update_frequency"}]})
+    assert find_algorithms == [a]
+
+    # Test that the main node is correctly excluded if we specify an additionally non-existent parameter
+    find_algorithms = a.find_children({"parameter": [{"key": "damping_time"}, {"key": "update_frequency"}, {"foo": "bar"}]})
+    assert find_algorithms == []
+
+    # Test search depth exclusions
+    find_algorithms = a.find_children({"node": "Algorithm", "key": "mc_barostat"}, search_depth=0)
+    assert find_algorithms == [a]
+    find_parameter = a.find_children({"node": ["Parameter"]}, search_depth=1)
+    assert find_parameter == [p1, p2]
+    find_parameter = a.find_children({"node": ["Parameter"]}, search_depth=0)
+    assert find_parameter == []
+
+
+def test_cycles(fixed_cyclic_project_node):
+    new_project = fixed_cyclic_project_node
+    new_json = new_project.get_expanded_json()
+
+    reloaded_project, cache = cript.load_nodes_from_json(new_json, _use_uuid_cache=dict())
+    assert reloaded_project is not new_project
+    assert reloaded_project.uuid == new_project.uuid
+
+
+def test_uid_serial(simple_inventory_node):
+    simple_inventory_node.material += simple_inventory_node.material
+    json_dict = json.loads(simple_inventory_node.get_json(condense_to_uuid={}).json)
+    assert len(json_dict["material"]) == 4
+    assert isinstance(json_dict["material"][2]["uid"], str)
+    assert json_dict["material"][2]["uid"].startswith("_:")
+    assert len(json_dict["material"][2]["uid"]) == len(get_new_uid())
+    assert isinstance(json_dict["material"][3]["uid"], str)
+    assert json_dict["material"][3]["uid"].startswith("_:")
+    assert len(json_dict["material"][3]["uid"]) == len(get_new_uid())
+    assert json_dict["material"][3]["uid"] != json_dict["material"][2]["uid"]
+
+
+def test_invalid_json_load():
+    def raise_node_dict(node_dict):
+        node_str = json.dumps(node_dict)
+        with pytest.raises(CRIPTJsonNodeError):
+            cript.load_nodes_from_json(node_str)
+
+    node_dict = {"node": "Computation"}
+    raise_node_dict(node_dict)
+    node_dict = {"node": []}
+    raise_node_dict(node_dict)
+    node_dict = {"node": ["asdf", "asdf"]}
+    raise_node_dict(node_dict)
+    node_dict = {"node": [None]}
+    raise_node_dict(node_dict)
+
+
+def test_invalid_project_graphs(simple_project_node, simple_material_node, simple_process_node, simple_property_node, simple_data_node, simple_computation_node, simple_computation_process_node):
+    project = copy.deepcopy(simple_project_node)
+    process = copy.deepcopy(simple_process_node)
+    material = copy.deepcopy(simple_material_node)
+
+    ingredient = cript.Ingredient(material=material, quantity=[cript.Quantity(key="mass", value=1.23, unit="kg")])
+    process.ingredient += [ingredient]
+
+    # Add the process to the experiment, but not in inventory or materials
+    # Invalid graph
+    project.collection[0].experiment[0].process += [process]
+    with pytest.raises(CRIPTOrphanedMaterialError):
+        project.validate()
+
+    # First fix add material to inventory
+    project.collection[0].inventory += [cript.Inventory("test_inventory", material=[material])]
+    project.validate()
+    # Reverse this fix
+    project.collection[0].inventory = []
+    with pytest.raises(CRIPTOrphanedMaterialError):
+        project.validate()
+
+    # Fix by add to the materials list instead.
+    # Using the util helper function for this.
+    cript.add_orphaned_nodes_to_project(project, active_experiment=None, max_iteration=10)
+    project.validate()
+
+    # Now add an orphan process to the graph
+    process2 = copy.deepcopy(simple_process_node)
+    process.prerequisite_process += [process2]
+    with pytest.raises(CRIPTOrphanedProcessError):
+        project.validate()
+
+    # Wrong fix it helper node
+    dummy_experiment = copy.deepcopy(project.collection[0].experiment[0])
+    with pytest.raises(RuntimeError):
+        cript.add_orphaned_nodes_to_project(project, dummy_experiment)
+    # Problem still persists
+    with pytest.raises(CRIPTOrphanedProcessError):
+        project.validate()
+    # Fix by using the helper function correctly
+    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
+    project.validate()
+
+    # We add property to the material, because that adds the opportunity for orphaned data and computation
+    property = copy.deepcopy(simple_property_node)
+    material.property += [property]
+    project.validate()
+    # Now add an orphan data
+    data = copy.deepcopy(simple_data_node)
+    property.data = [data]
+
+    with pytest.raises(CRIPTOrphanedDataError):
+        project.validate()
+    # Fix with the helper function
+    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
+    project.validate()
+
+    # Add an orphan Computation
+    computation = copy.deepcopy(simple_computation_node)
+    property.computation += [computation]
+    with pytest.raises(CRIPTOrphanedComputationError):
+        project.validate()
+    # Fix with the helper function
+    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
+    project.validate()
+
+    # Add orphan computational process
+    comp_proc = copy.deepcopy(simple_computation_process_node)
+    data.computation_process += [comp_proc]
+    with pytest.raises(CRIPTOrphanedComputationalProcessError):
+        while True:
+            try:  # Do trigger not orphan materials
+                project.validate()
+            except CRIPTOrphanedMaterialError as exc:
+                project._json_attrs.material.append(exc.orphaned_node)
+            except CRIPTOrphanedProcessError as exc:
+                project.collection[0].experiment[0]._json_attrs.process.append(exc.orphaned_node)
+            else:
+                break
+
+    cript.add_orphaned_nodes_to_project(project, project.collection[0].experiment[0], 10)
+    project.validate()
+
+
+def test_expanded_json(complex_project_node):
+    """
+    Tests the generation and deserialization of expanded JSON for a complex project node.
+
+    This test verifies 2 key aspects:
+        1. A complex project node can be serialized into an expanded JSON string, without UUID placeholders.
+        2. The expanded JSON can be deserialized into a node  that is equivalent to the original node.
+    """
+    project_expanded_json: str = complex_project_node.get_expanded_json()
+    deserialized_project_node: cript.Project = cript.load_nodes_from_json(project_expanded_json)
+
+    # assert the expanded JSON was correctly deserialized to project node
+    assert deserialized_project_node == complex_project_node
+
+    condensed_json: str = complex_project_node.json
+
+    # since short JSON has UUID it will not be able to deserialize correctly and will
+    # raise CRIPTJsonDeserializationError
+    with pytest.raises(cript.nodes.exceptions.CRIPTJsonDeserializationError):
+        cript.load_nodes_from_json(condensed_json)
+
+
+def test_uuid_cache_override(complex_project_node):
+    normal_serial = complex_project_node.get_expanded_json()
+    reloaded_project = cript.load_nodes_from_json(normal_serial)
+
+    # For a normal load, the reloaded node as to be the same as before.
+    assert reloaded_project is complex_project_node
+
+    # Load with custom cache override
+    custom_project, cache = cript.load_nodes_from_json(normal_serial, _use_uuid_cache=dict())
+
+    assert custom_project is not reloaded_project
+
+    # Make sure that the nodes in the different caches are different
+    for key in cache:
+        old_node = cript.nodes.uuid_base.UUIDBaseNode._uuid_cache[key]
+        new_node = cache[key]
+        assert old_node.uuid == new_node.uuid
+        assert old_node is not new_node
+
+
+def test_dfs_order(fixed_cyclic_project_node, fixed_cyclic_project_dfs_uuid_order):
+    for i, node in enumerate(fixed_cyclic_project_node):
+        assert node.uuid == fixed_cyclic_project_dfs_uuid_order[i]
```

