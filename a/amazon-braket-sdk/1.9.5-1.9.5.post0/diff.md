# Comparing `tmp/amazon-braket-sdk-1.9.5.tar.gz` & `tmp/amazon-braket-sdk-1.9.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-sdk-1.9.5.tar", last modified: Tue Oct  5 18:50:53 2021, max compression
+gzip compressed data, was "amazon-braket-sdk-1.9.5.post0.tar", last modified: Thu Nov  4 18:19:40 2021, max compression
```

## Comparing `amazon-braket-sdk-1.9.5.tar` & `amazon-braket-sdk-1.9.5.post0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.456288 amazon-braket-sdk-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)    10142 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)    12911 2021-10-05 18:50:53.456288 amazon-braket-sdk-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12063 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      534 2021-10-05 18:50:53.456288 amazon-braket-sdk-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.448288 amazon-braket-sdk-1.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.448288 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12911 2021-10-05 18:50:53.000000 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2021-10-05 18:50:53.000000 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 18:50:53.000000 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-10-05 18:50:53.000000 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-05 18:50:53.000000 amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.448288 amazon-braket-sdk-1.9.5/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.448288 amazon-braket-sdk-1.9.5/src/braket/_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.448288 amazon-braket-sdk-1.9.5/src/braket/annealing/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4729 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/annealing/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.452288 amazon-braket-sdk-1.9.5/src/braket/aws/
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17770 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/aws/aws_device.py
--rw-r--r--   0 runner    (1001) docker     (121)    22063 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/aws/aws_quantum_task.py
--rw-r--r--   0 runner    (1001) docker     (121)    11801 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/aws/aws_quantum_task_batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     6861 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/aws/aws_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.452288 amazon-braket-sdk-1.9.5/src/braket/circuits/
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/angled_gate.py
--rw-r--r--   0 runner    (1001) docker     (121)    10034 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/ascii_circuit_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)    45577 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/circuit_diagram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/circuit_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/compiler_directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/compiler_directives.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/gate.py
--rw-r--r--   0 runner    (1001) docker     (121)    40931 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/gates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5844 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/instruction.py
--rw-r--r--   0 runner    (1001) docker     (121)    11472 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/moments.py
--rw-r--r--   0 runner    (1001) docker     (121)    15178 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/noise.py
--rw-r--r--   0 runner    (1001) docker     (121)    12015 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/noise_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    27823 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/noises.py
--rw-r--r--   0 runner    (1001) docker     (121)     3533 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/observable.py
--rw-r--r--   0 runner    (1001) docker     (121)    13466 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/observables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/quantum_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/quantum_operator_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/qubit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/qubit_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     7588 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/result_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    18081 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/result_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/circuits/unitary_calculation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.456288 amazon-braket-sdk-1.9.5/src/braket/devices/
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/devices/local_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/ipython_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 18:50:53.456288 amazon-braket-sdk-1.9.5/src/braket/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6530 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/tasks/annealing_quantum_task_result.py
--rw-r--r--   0 runner    (1001) docker     (121)    20756 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/tasks/gate_model_quantum_task_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/tasks/local_quantum_task.py
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2021-10-05 18:50:44.000000 amazon-braket-sdk-1.9.5/src/braket/tasks/quantum_task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/
+-rw-r--r--   0 runner    (1001) docker     (121)    10142 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)    12917 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12063 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2403 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.473055 amazon-braket-sdk-1.9.5.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.473055 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12917 2021-11-04 18:19:40.000000 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1783 2021-11-04 18:19:40.000000 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-04 18:19:40.000000 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-11-04 18:19:40.000000 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-04 18:19:40.000000 amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.473055 amazon-braket-sdk-1.9.5.post0/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.473055 amazon-braket-sdk-1.9.5.post0/src/braket/_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.473055 amazon-braket-sdk-1.9.5.post0/src/braket/annealing/
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4729 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/annealing/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.477055 amazon-braket-sdk-1.9.5.post0/src/braket/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17770 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_device.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22063 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_quantum_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11801 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_quantum_task_batch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6861 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_session.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/angled_gate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10034 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/ascii_circuit_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45577 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1924 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/compiler_directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/compiler_directives.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2797 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/gate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40931 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/gates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5844 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11472 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/moments.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15178 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noise.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12015 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noise_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27823 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noises.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3533 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/observable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13466 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/observables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5895 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/quantum_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3889 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/quantum_operator_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/qubit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/qubit_set.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7588 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/result_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18081 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/result_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3121 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/circuits/unitary_calculation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/src/braket/devices/
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/devices/local_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/ipython_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 18:19:40.481055 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6530 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/annealing_quantum_task_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20756 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/gate_model_quantum_task_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1669 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/local_quantum_task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2073 2021-11-04 18:19:27.000000 amazon-braket-sdk-1.9.5.post0/src/braket/tasks/quantum_task.py
```

### Comparing `amazon-braket-sdk-1.9.5/LICENSE` & `amazon-braket-sdk-1.9.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/PKG-INFO` & `amazon-braket-sdk-1.9.5.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-sdk
-Version: 1.9.5
+Version: 1.9.5.post0
 Summary: An open source library for interacting with quantum computing devices on Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-sdk-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amazon-braket-sdk-1.9.5/README.md` & `amazon-braket-sdk-1.9.5.post0/README.md`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/setup.cfg` & `amazon-braket-sdk-1.9.5.post0/setup.cfg`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/setup.py` & `amazon-braket-sdk-1.9.5.post0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/PKG-INFO` & `amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-sdk
-Version: 1.9.5
+Version: 1.9.5.post0
 Summary: An open source library for interacting with quantum computing devices on Amazon Braket
 Home-page: https://github.com/aws/amazon-braket-sdk-python
 Author: Amazon Web Services
 License: Apache License 2.0
 Keywords: Amazon AWS Quantum
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amazon-braket-sdk-1.9.5/src/amazon_braket_sdk.egg-info/SOURCES.txt` & `amazon-braket-sdk-1.9.5.post0/src/amazon_braket_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/_sdk/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/_sdk/_version.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/_sdk/_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.9.5"
+__version__ = "1.9.5.post0"
```

### Comparing `amazon-braket-sdk-1.9.5/src/braket/annealing/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/annealing/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/annealing/problem.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/annealing/problem.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/aws/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/aws/aws_device.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_device.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/aws/aws_quantum_task.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_quantum_task.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/aws/aws_quantum_task_batch.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_quantum_task_batch.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/aws/aws_session.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/aws/aws_session.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/angled_gate.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/angled_gate.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/ascii_circuit_diagram.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/ascii_circuit_diagram.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/circuit.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/circuit_diagram.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit_diagram.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/circuit_helpers.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/circuit_helpers.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/compiler_directive.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/compiler_directive.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/compiler_directives.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/compiler_directives.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/gate.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/gate.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/gates.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/gates.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/instruction.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/instruction.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/moments.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/moments.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/noise.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noise.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/noise_helpers.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noise_helpers.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/noises.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/noises.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/observable.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/observable.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/observables.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/observables.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/operator.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/operator.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/quantum_operator.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/quantum_operator.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/quantum_operator_helpers.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/quantum_operator_helpers.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/qubit.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/qubit.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/qubit_set.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/qubit_set.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/result_type.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/result_type.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/result_types.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/result_types.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/circuits/unitary_calculation.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/circuits/unitary_calculation.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/devices/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/devices/device.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/devices/device.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/devices/local_simulator.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/devices/local_simulator.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/ipython_utils.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/tasks/__init__.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/tasks/annealing_quantum_task_result.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/tasks/annealing_quantum_task_result.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/tasks/gate_model_quantum_task_result.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/tasks/gate_model_quantum_task_result.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/tasks/local_quantum_task.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/tasks/local_quantum_task.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-sdk-1.9.5/src/braket/tasks/quantum_task.py` & `amazon-braket-sdk-1.9.5.post0/src/braket/tasks/quantum_task.py`

 * *Files identical despite different names*

