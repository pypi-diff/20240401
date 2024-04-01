# Comparing `tmp/amazon-braket-algorithm-library-1.4.8.tar.gz` & `tmp/amazon-braket-algorithm-library-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-braket-algorithm-library-1.4.8.tar", last modified: Tue Mar  5 16:04:46 2024, max compression
+gzip compressed data, was "amazon-braket-algorithm-library-1.4.9.tar", last modified: Mon Apr  1 16:04:56 2024, max compression
```

## Comparing `amazon-braket-algorithm-library-1.4.8.tar` & `amazon-braket-algorithm-library-1.4.9.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.748557 amazon-braket-algorithm-library-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-05 16:04:46.748557 amazon-braket-algorithm-library-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-05 16:04:46.748557 amazon-braket-algorithm-library-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.736557 amazon-braket-algorithm-library-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-05 16:04:46.000000 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-05 16:04:46.000000 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 16:04:46.000000 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-05 16:04:46.000000 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 16:04:46.000000 amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.736557 amazon-braket-algorithm-library-1.4.8/src/braket/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/_algos/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/_algos/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bells_inequality/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bells_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bernstein_vazirani/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/chsh_inequality/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/chsh_inequality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/deutsch_jozsa/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.740557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/grovers_search/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/grovers_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/grovers_search/grovers_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19663 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_approximate_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_circuit_born_machine/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_fourier_transform/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_phase_estimation/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_walk/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_walk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/shors/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/shors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/shors/shors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 16:04:46.744557 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/simons/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/simons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-03-05 16:04:23.000000 amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/simons/simons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.882473 amazon-braket-algorithm-library-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-01 16:04:56.882473 amazon-braket-algorithm-library-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-01 16:04:56.882473 amazon-braket-algorithm-library-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.870473 amazon-braket-algorithm-library-1.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-01 16:04:56.000000 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-01 16:04:56.000000 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:04:56.000000 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-01 16:04:56.000000 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 16:04:56.000000 amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.870473 amazon-braket-algorithm-library-1.4.9/src/braket/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/_algos/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/_algos/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bells_inequality/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bells_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bernstein_vazirani/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/chsh_inequality/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/chsh_inequality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/deutsch_jozsa/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.874472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/grovers_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/grovers_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/grovers_search/grovers_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19663 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_approximate_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_circuit_born_machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_fourier_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_phase_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10830 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_walk/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_walk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/shors/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/shors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/shors/shors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/simons/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/simons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/simons/simons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/auxiliary_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/auxiliary_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:04:56.878472 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/auxiliary_functions/random_circuit/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/auxiliary_functions/random_circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-01 16:04:47.000000 amazon-braket-algorithm-library-1.4.9/src/braket/experimental/auxiliary_functions/random_circuit/random_circuit.py
```

### Comparing `amazon-braket-algorithm-library-1.4.8/LICENSE` & `amazon-braket-algorithm-library-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/setup.py` & `amazon-braket-algorithm-library-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt` & `amazon-braket-algorithm-library-1.4.9/src/amazon_braket_algorithm_library.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,11 @@
 src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py
 src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py
 src/braket/experimental/algorithms/quantum_walk/__init__.py
 src/braket/experimental/algorithms/quantum_walk/quantum_walk.py
 src/braket/experimental/algorithms/shors/__init__.py
 src/braket/experimental/algorithms/shors/shors.py
 src/braket/experimental/algorithms/simons/__init__.py
-src/braket/experimental/algorithms/simons/simons.py
+src/braket/experimental/algorithms/simons/simons.py
+src/braket/experimental/auxiliary_functions/__init__.py
+src/braket/experimental/auxiliary_functions/random_circuit/__init__.py
+src/braket/experimental/auxiliary_functions/random_circuit/random_circuit.py
```

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/_algos/_version.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/_algos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # language governing permissions and limitations under the License.
 
 """Version information.
 
 Version number (major.minor.patch[-label])
 """
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
```

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bells_inequality/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bells_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bells_inequality/bells_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bernstein_vazirani/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/bernstein_vazirani/bernstein_vazirani.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/chsh_inequality/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/chsh_inequality/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/chsh_inequality/chsh_inequality.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/deutsch_jozsa/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/deutsch_jozsa/deutsch_jozsa.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/grovers_search/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/grovers_search/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/grovers_search/grovers_search.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/grovers_search/grovers_search.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/classical_qmc.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/qc_qmc/qc_qmc.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_approximate_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_approximate_optimization/quantum_approximate_optimization.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_circuit_born_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_circuit_born_machine/qcbm.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_fourier_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_fourier_transform/quantum_fourier_transform.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_phase_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_phase_estimation/quantum_phase_estimation.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_walk/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_walk/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/quantum_walk/quantum_walk.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/shors/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/shors/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/shors/shors.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/shors/shors.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/simons/__init__.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/simons/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-braket-algorithm-library-1.4.8/src/braket/experimental/algorithms/simons/simons.py` & `amazon-braket-algorithm-library-1.4.9/src/braket/experimental/algorithms/simons/simons.py`

 * *Files identical despite different names*

