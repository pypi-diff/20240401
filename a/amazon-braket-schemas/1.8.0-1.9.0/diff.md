# Comparing `tmp/amazon-braket-schemas-1.8.0.tar.gz` & `tmp/amazon-braket-schemas-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-schemas-1.8.0.tar", last modified: Mon Mar  7 19:24:32 2022, max compression
+gzip compressed data, was "amazon-braket-schemas-1.9.0.tar", last modified: Wed Apr  6 16:23:49 2022, max compression
```

## Comparing `amazon-braket-schemas-1.8.0.tar` & `amazon-braket-schemas-1.9.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.695036 amazon-braket-schemas-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-03-07 19:24:32.695036 amazon-braket-schemas-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7300 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-03-07 19:24:32.695036 amazon-braket-schemas-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.683035 amazon-braket-schemas-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.683035 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-03-07 19:24:32.000000 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-03-07 19:24:32.000000 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-07 19:24:32.000000 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-03-07 19:24:32.000000 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-07 19:24:32.000000 amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.683035 amazon-braket-schemas-1.8.0/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.683035 amazon-braket-schemas-1.8.0/src/braket/_schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/_schemas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/device_action_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/device_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/device_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/device_execution_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     4403 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/device_service_properties_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_2000Q_device_level_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_2000Q_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4316 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_advantage_device_level_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_advantage_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_device_capabilities_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_provider_level_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_provider_properties_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/gate_model_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/gate_model_qpu_paradigm_properties_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_device_capabilities_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_provider_properties_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/jaqcd_device_action_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/openqasm_device_action_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4771 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_device_capabilities_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_provider_properties_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/result_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_device_capabilities_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_provider_properties_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_device_capabilities_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_device_parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_paradigm_properties_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.683035 amazon-braket-schemas-1.8.0/src/braket/ir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/ir/annealing/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/annealing/problem_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27444 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/instructions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6825 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/program_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/results.py
--rw-r--r--   0 runner    (1001) docker     (121)    11369 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/shared_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/ir/openqasm/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/openqasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/ir/openqasm/program_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/jobs_data/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/jobs_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/jobs_data/persisted_job_data_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.687035 amazon-braket-schemas-1.8.0/src/braket/schema_common/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/schema_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/schema_common/schema_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/schema_common/schema_header.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-07 19:24:32.695036 amazon-braket-schemas-1.8.0/src/braket/task_result/
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/additional_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/annealing_task_result_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/dwave_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/gate_model_task_result_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/oqc_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/rigetti_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/simulator_metadata_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-03-07 19:24:22.000000 amazon-braket-schemas-1.8.0/src/braket/task_result/task_metadata_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7300 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.123307 amazon-braket-schemas-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8134 2022-04-06 16:23:48.000000 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-04-06 16:23:49.000000 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 16:23:48.000000 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-04-06 16:23:48.000000 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-06 16:23:48.000000 amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.123307 amazon-braket-schemas-1.9.0/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/_schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/_schemas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1536 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/device_action_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/device_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/device_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/device_execution_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4403 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/device_service_properties_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5127 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_2000Q_device_level_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_2000Q_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4316 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_advantage_device_level_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_advantage_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_device_capabilities_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_provider_level_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_provider_properties_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/gate_model_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/gate_model_qpu_paradigm_properties_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4696 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_device_capabilities_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_provider_properties_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/jaqcd_device_action_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/openqasm_device_action_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5221 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_device_capabilities_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_provider_properties_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/result_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_device_capabilities_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3059 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_provider_properties_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_device_capabilities_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_device_parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_paradigm_properties_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7858 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/device_schema/standardized_gate_model_qpu_device_properties_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.123307 amazon-braket-schemas-1.9.0/src/braket/ir/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/ir/annealing/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/annealing/problem_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.127307 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27444 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6825 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/program_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/results.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11369 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/shared_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/src/braket/ir/openqasm/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/openqasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/ir/openqasm/program_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/src/braket/jobs_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/jobs_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/jobs_data/persisted_job_data_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/src/braket/schema_common/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/schema_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/schema_common/schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/schema_common/schema_header.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 16:23:49.131307 amazon-braket-schemas-1.9.0/src/braket/task_result/
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/additional_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/annealing_task_result_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/dwave_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/gate_model_task_result_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/oqc_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/rigetti_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/simulator_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-04-06 16:23:34.000000 amazon-braket-schemas-1.9.0/src/braket/task_result/task_metadata_v1.py
```

### Comparing `amazon-braket-schemas-1.8.0/LICENSE` & `amazon-braket-schemas-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/PKG-INFO` & `amazon-braket-schemas-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-schemas
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source library that contains the schemas for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-schemas-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amazon-braket-schemas-1.8.0/README.md` & `amazon-braket-schemas-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/setup.cfg` & `amazon-braket-schemas-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/setup.py` & `amazon-braket-schemas-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/PKG-INFO` & `amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-schemas
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source library that contains the schemas for Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-schemas-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amazon-braket-schemas-1.8.0/src/amazon_braket_schemas.egg-info/SOURCES.txt` & `amazon-braket-schemas-1.9.0/src/amazon_braket_schemas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/braket/device_schema/device_execution_window.py
 src/braket/device_schema/device_service_properties_v1.py
 src/braket/device_schema/gate_model_parameters_v1.py
 src/braket/device_schema/gate_model_qpu_paradigm_properties_v1.py
 src/braket/device_schema/jaqcd_device_action_properties.py
 src/braket/device_schema/openqasm_device_action_properties.py
 src/braket/device_schema/result_type.py
+src/braket/device_schema/standardized_gate_model_qpu_device_properties_v1.py
 src/braket/device_schema/dwave/__init__.py
 src/braket/device_schema/dwave/dwave_2000Q_device_level_parameters_v1.py
 src/braket/device_schema/dwave/dwave_2000Q_device_parameters_v1.py
 src/braket/device_schema/dwave/dwave_advantage_device_level_parameters_v1.py
 src/braket/device_schema/dwave/dwave_advantage_device_parameters_v1.py
 src/braket/device_schema/dwave/dwave_device_capabilities_v1.py
 src/braket/device_schema/dwave/dwave_device_parameters_v1.py
```

### Comparing `amazon-braket-schemas-1.8.0/src/braket/_schemas/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/_schemas/_version.py` & `amazon-braket-schemas-1.9.0/src/braket/_schemas/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
```

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,7 +28,10 @@
 )
 from braket.device_schema.jaqcd_device_action_properties import (  # noqa: F401
     JaqcdDeviceActionProperties,
 )
 from braket.device_schema.openqasm_device_action_properties import (  # noqa: F401
     OpenQASMDeviceActionProperties,
 )
+from braket.device_schema.standardized_gate_model_qpu_device_properties_v1 import (  # noqa: F401
+    StandardizedGateModelQpuDeviceProperties,
+)
```

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/device_action_properties.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/device_action_properties.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/device_capabilities.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/device_capabilities.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/device_connectivity.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/device_execution_window.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/device_execution_window.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/device_service_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/device_service_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_2000Q_device_level_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_2000Q_device_level_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_2000Q_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_2000Q_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_advantage_device_level_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_advantage_device_level_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_advantage_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_advantage_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_device_capabilities_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_device_capabilities_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_provider_level_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_provider_level_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/dwave/dwave_provider_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/dwave/dwave_provider_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/gate_model_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/gate_model_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/gate_model_qpu_paradigm_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/gate_model_qpu_paradigm_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_device_capabilities_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_device_capabilities_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/ionq/ionq_provider_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/ionq/ionq_provider_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/jaqcd_device_action_properties.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/jaqcd_device_action_properties.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/openqasm_device_action_properties.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/openqasm_device_action_properties.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_device_capabilities_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_device_capabilities_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from braket.device_schema.device_capabilities import DeviceCapabilities
 from braket.device_schema.gate_model_qpu_paradigm_properties_v1 import (
     GateModelQpuParadigmProperties,
 )
 from braket.device_schema.jaqcd_device_action_properties import JaqcdDeviceActionProperties
 from braket.device_schema.openqasm_device_action_properties import OpenQASMDeviceActionProperties
 from braket.device_schema.oqc.oqc_provider_properties_v1 import OqcProviderProperties
+from braket.device_schema.standardized_gate_model_qpu_device_properties_v1 import (
+    StandardizedGateModelQpuDeviceProperties,
+)
 from braket.schema_common import BraketSchemaBase, BraketSchemaHeader
 
 # TODO: Update the device and topology details when we have information from the provider
 
 
 class OqcDeviceCapabilities(BraketSchemaBase, DeviceCapabilities):
     """
@@ -34,14 +37,17 @@
 
     Attributes:
         action(Dict[Union[DeviceActionType, str],
             Union[OpenQASMDeviceActionProperties, JaqcdDeviceActionProperties]]): Actions that an
             OQC device can support
         paradigm(GateModelQpuParadigmProperties): Paradigm properties
         provider(Optional[OqcProviderProperties]): OQC provider specific properties
+        standardized
+            (StandardizedGateModelQpuDeviceProperties): Braket standarized device
+            properties for OQC
 
     Examples:
         >>> import json
         >>> input_json = {
         ...    "braketSchemaHeader": {
         ...        "name": "braket.device_schema.oqc.oqc_device_capabilities",
         ...        "version": "1",
@@ -93,21 +99,24 @@
         ...        "nativeGateSet": ["ccnot", "cy"],
         ...        "connectivity": {
         ...            "fullyConnected": False,
         ...            "connectivityGraph": {"1": ["2", "3"]},
         ...        },
         ...    },
         ...    "deviceParameters": {OqcDeviceParameters.schema_json()},
+        ...    "standardized": \
+        ...            {StandardizedGateModelQpuDeviceProperties.schema_json()},,
         ... }
         >>> OqcDeviceCapabilities.parse_raw_schema(json.dumps(input_json))
     """
 
     _PROGRAM_HEADER = BraketSchemaHeader(
         name="braket.device_schema.oqc.oqc_device_capabilities", version="1"
     )
     braketSchemaHeader: BraketSchemaHeader = Field(default=_PROGRAM_HEADER, const=_PROGRAM_HEADER)
     action: Dict[
         Union[DeviceActionType, str],
         Union[OpenQASMDeviceActionProperties, JaqcdDeviceActionProperties],
     ]
     paradigm: GateModelQpuParadigmProperties
     provider: Optional[OqcProviderProperties]
+    standardized: Optional[StandardizedGateModelQpuDeviceProperties]
```

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/oqc/oqc_provider_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/oqc/oqc_provider_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/result_type.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/result_type.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_device_capabilities_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_device_capabilities_v1.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,27 +19,33 @@
 from braket.device_schema.device_capabilities import DeviceCapabilities
 from braket.device_schema.gate_model_qpu_paradigm_properties_v1 import (
     GateModelQpuParadigmProperties,
 )
 from braket.device_schema.jaqcd_device_action_properties import JaqcdDeviceActionProperties
 from braket.device_schema.openqasm_device_action_properties import OpenQASMDeviceActionProperties
 from braket.device_schema.rigetti.rigetti_provider_properties_v1 import RigettiProviderProperties
+from braket.device_schema.standardized_gate_model_qpu_device_properties_v1 import (
+    StandardizedGateModelQpuDeviceProperties,
+)
 from braket.schema_common import BraketSchemaBase, BraketSchemaHeader
 
 
 class RigettiDeviceCapabilities(BraketSchemaBase, DeviceCapabilities):
     """
     This defines the capabilities of a Rigetti device.
 
     Attributes:
         action(Dict[Union[DeviceActionType, str],
             Union[OpenQASMDeviceActionProperties, JaqcdDeviceActionProperties]]): Actions that a
             Rigetti device can support
         paradigm(GateModelQpuParadigmProperties): Paradigm properties of a Rigetti
         provider(Optional[RigettiProviderProperties]): Rigetti provider specific properties
+        standardized
+            (StandardizedGateModelQpuDeviceProperties): Braket standarized device
+            properties for Rigetti
 
     Examples:
         >>> import json
         >>> input_json = {
         ...    "braketSchemaHeader": {
         ...        "name": "braket.device_schema.rigetti.rigetti_device_capabilities",
         ...        "version": "1",
@@ -91,14 +97,16 @@
         ...        "nativeGateSet": ["ccnot", "cy"],
         ...        "connectivity": {
         ...            "fullyConnected": False,
         ...            "connectivityGraph": {"1": ["2", "3"]},
         ...        },
         ...    },
         ...    "deviceParameters": {RigettiDeviceParameters.schema_json()},
+        ...    "standardized": \
+        ...            {StandardizedGateModelQpuDeviceProperties.schema_json()},
         ... }
         >>> RigettiDeviceCapabilities.parse_raw_schema(json.dumps(input_json))
 
     """
 
     _PROGRAM_HEADER = BraketSchemaHeader(
         name="braket.device_schema.rigetti.rigetti_device_capabilities", version="1"
@@ -106,7 +114,8 @@
     braketSchemaHeader: BraketSchemaHeader = Field(default=_PROGRAM_HEADER, const=_PROGRAM_HEADER)
     action: Dict[
         Union[DeviceActionType, str],
         Union[OpenQASMDeviceActionProperties, JaqcdDeviceActionProperties],
     ]
     paradigm: GateModelQpuParadigmProperties
     provider: Optional[RigettiProviderProperties]
+    standardized: Optional[StandardizedGateModelQpuDeviceProperties]
```

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/rigetti/rigetti_provider_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/rigetti/rigetti_provider_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_device_capabilities_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_device_capabilities_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_device_parameters_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_device_parameters_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/device_schema/simulators/gate_model_simulator_paradigm_properties_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/device_schema/simulators/gate_model_simulator_paradigm_properties_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/annealing/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/annealing/problem_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/annealing/problem_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/instructions.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/instructions.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/program_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/program_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/results.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/results.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/jaqcd/shared_models.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/jaqcd/shared_models.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/ir/openqasm/program_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/ir/openqasm/program_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/jobs_data/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/jobs_data/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/jobs_data/persisted_job_data_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/jobs_data/persisted_job_data_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/schema_common/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/schema_common/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/schema_common/schema_base.py` & `amazon-braket-schemas-1.9.0/src/braket/schema_common/schema_base.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/schema_common/schema_header.py` & `amazon-braket-schemas-1.9.0/src/braket/schema_common/schema_header.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/__init__.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/additional_metadata.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/additional_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/annealing_task_result_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/annealing_task_result_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/dwave_metadata_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/dwave_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/gate_model_task_result_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/gate_model_task_result_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/oqc_metadata_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/oqc_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/rigetti_metadata_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/rigetti_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/simulator_metadata_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/simulator_metadata_v1.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-schemas-1.8.0/src/braket/task_result/task_metadata_v1.py` & `amazon-braket-schemas-1.9.0/src/braket/task_result/task_metadata_v1.py`

 * *Files identical despite different names*

