# Comparing `tmp/qiskit-aer-0.9.0.tar.gz` & `tmp/qiskit-aer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-aer-0.9.0.tar", last modified: Thu Sep 16 10:24:36 2021, max compression
+gzip compressed data, was "qiskit-aer-0.9.1.tar", last modified: Mon Oct 11 20:40:39 2021, max compression
```

## Comparing `qiskit-aer-0.9.0.tar` & `qiskit-aer-0.9.1.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.369367 qiskit-aer-0.9.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)    14844 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6964 2021-09-16 10:24:36.369367 qiskit-aer-0.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     5058 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/FindPybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    21390 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/FindPythonExtensions.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/Linter.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/compiler_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    24973 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/conan.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/conan_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/dependency_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/findBLASInSpecificPath.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/nvcc_add_compiler_options.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    16669 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/cmake/targetLinkLibrariesWithDynamicLookup.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.333366 qiskit-aer-0.9.0/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/contrib/standalone/
--rwxr-xr-x   0 runner    (1001) docker     (121)     5661 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/contrib/standalone/qasm_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/contrib/standalone/version.hpp.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/qiskit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/__init__.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/__init__.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/aererror.py
--rw-r--r--   0 runner    (1001) docker     (121)     3245 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/aerprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      755 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33452 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/aer_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    16616 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/aerbackend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13505 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/pulse_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    30602 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12149 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/statevector_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12577 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/unitary_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/backends/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/wrappers/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/backends/wrappers/bindings.cc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5980 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_density_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_expectation_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_probabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_stabilizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_statevector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/jobs/
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/jobs/aerjob.py
--rw-r--r--   0 runner    (1001) docker     (121)    13079 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/jobs/aerjobset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/jobs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.341366 qiskit-aer-0.9.0/qiskit/providers/aer/library/
--rw-r--r--   0 runner    (1001) docker     (121)     5888 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/default_qubits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/instructions_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6917 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5440 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_density_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    10420 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_expectation_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_matrix_product_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     6443 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_probabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_stabilizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_statevector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_superop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_unitary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/
--rw-r--r--   0 runner    (1001) docker     (121)      917 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2737 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_density_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_matrix_product_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_stabilizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_statevector.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_superop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_unitary.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/noise/
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/
--rw-r--r--   0 runner    (1001) docker     (121)      895 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10846 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22122 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/errorutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    26093 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/quantum_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    12190 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/readout_error.py
--rw-r--r--   0 runner    (1001) docker     (121)    22143 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/standard_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    42334 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/noise_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/noise/noiseerror.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      735 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18592 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/digest_pulse_qobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/mc_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    18088 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_de_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     4892 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_sim_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/unitary_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/
--rw-r--r--   0 runner    (1001) docker     (121)    14320 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/DE_Methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/DE_Options.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.345366 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19793 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/duffing_model_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    12488 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/hamiltonian_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8645 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/pulse_system_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.349367 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/apply_str_func_to_qobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/gen_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_from_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     4544 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_generators.py
--rw-r--r--   0 runner    (1001) docker     (121)    16112 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/string_model_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.349367 qiskit-aer-0.9.0/qiskit/providers/aer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_model_inserter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4944 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_remapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    29913 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/qiskit/providers/aer/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.349367 qiskit-aer-0.9.0/src/controllers/
--rwxr-xr-x   0 runner    (1001) docker     (121)    69672 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/controllers/aer_controller.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1456 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/controllers/controller_execute.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.349367 qiskit-aer-0.9.0/src/framework/
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/avx2_detect.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     7381 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/blas_protos.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    15816 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/circuit.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     9820 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/creg.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     9700 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/json.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/json_parser.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.349367 qiskit-aer-0.9.0/src/framework/linalg/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2194 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/almost_equal.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/eigensystem.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1469 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/enable_if_numeric.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1140 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linalg.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/linalg/linops/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4217 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_aer_vector.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     5103 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_array.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3641 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_generic.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6737 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_json.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6772 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_map.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     4560 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_matrix.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     7124 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_unordered_map.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6507 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/linops/linops_vector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)    13546 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/matrix_defs.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    10977 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/smatrix_defs.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    12921 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/vmatrix_defs.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)      780 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/matrix_utils.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6724 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/square.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    12220 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/vector.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/linalg/vector_json.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    28383 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/noise_utils.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    43603 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/operations.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     9277 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/opset.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6844 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/pybind_basics.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/pybind_casts.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    10085 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/pybind_json.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/python_parser.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6157 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/qobj.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/results/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/results/data/
--rw-r--r--   0 runner    (1001) docker     (121)     9637 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/data.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4955 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/metadata.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/results/data/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cdict.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cmatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_creg.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cvector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_json.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2462 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_mps.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rdict.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rvalue.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rvector.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2137 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cdict.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3455 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cmatrix.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1821 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_creg.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2587 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cvector.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2004 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_json.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2603 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_mps.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rdict.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2216 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rvalue.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2303 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rvector.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2314 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/pybind_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1472 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/pybind_metadata.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.353366 qiskit-aer-0.9.0/src/framework/results/data/subtypes/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2003 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/accum_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2695 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/average_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     5943 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/data_map.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1925 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/list_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2515 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/pybind_data_map.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2095 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/pybind_subtypes.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1870 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/data/subtypes/single_data.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/experiment_result.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/framework/results/legacy/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7442 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/average_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     4488 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/average_snapshot.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     8451 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/data_container.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2792 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/pershot_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3511 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/pershot_snapshot.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    13490 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/pybind_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    12857 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/legacy/snapshot_data.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     4074 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/pybind_result.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2992 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/results/result.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3483 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/rng.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     4689 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/stl_ostream.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1922 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/types.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    38926 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/framework/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/misc/
--rw-r--r--   0 runner    (1001) docker     (121)    18973 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/clang_omp_symbols.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/common_macros.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/gcc_omp_symbols.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/hacks.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/warnings.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/misc/wrap_thrust.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/noise/
--rw-r--r--   0 runner    (1001) docker     (121)    37552 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/noise/noise_model.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    13524 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/noise/quantum_error.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4247 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/noise/readout_error.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/open_pulse/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/eval_hamiltonian.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/iterators.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/log.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     9987 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/numeric_integrator.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/numeric_integrator.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/ordered_map.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/pulse_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/pulse_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/pulse_utils_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    13808 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/python_to_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/test_python_to_cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/test_python_to_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/types.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7295 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/zspmv.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/open_pulse/zspmv.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/simulators/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/simulators/density_matrix/
--rwxr-xr-x   0 runner    (1001) docker     (121)    18448 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    42030 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    59191 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_state_chunk.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    32373 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_thrust.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/
--rw-r--r--   0 runner    (1001) docker     (121)    22914 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/ch_runner.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.357367 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/chlib/
--rw-r--r--   0 runner    (1001) docker     (121)    28227 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/chlib/chstabilizer.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12207 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/chlib/core.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    36948 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/extended_stabilizer_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/extended_stabilizer/gates.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/matrix_product_state/
--rw-r--r--   0 runner    (1001) docker     (121)    42263 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    64098 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_internal.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    21232 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_internal.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    21365 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    13528 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/svd.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/matrix_product_state/svd.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/stabilizer/
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/stabilizer/binary_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    16043 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/stabilizer/clifford.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     3761 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/stabilizer/pauli.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    32524 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/stabilizer/stabilizer_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    21889 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    49597 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/state_chunk.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/statevector/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/statevector/chunk/
--rw-r--r--   0 runner    (1001) docker     (121)     6811 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    19056 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk_container.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     9658 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk_manager.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    33340 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/chunk/device_chunk_container.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12774 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/chunk/host_chunk_container.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12391 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/indexes.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    75146 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/qubitvector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    96756 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/qubitvector_thrust.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    50994 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/qv_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/qv_avx2.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    53204 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/statevector_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    70330 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/statevector_state_chunk.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    14004 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/transformer.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     3804 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/statevector/transformer_avx2.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/superoperator/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6515 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/superoperator/superoperator.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    21778 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/superoperator/superoperator_state.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     6650 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/superoperator/superoperator_thrust.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/simulators/unitary/
--rwxr-xr-x   0 runner    (1001) docker     (121)    22607 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/unitary/unitary_state.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    25303 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/unitary/unitary_state_chunk.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    11892 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/unitary/unitarymatrix.hpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    12204 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/simulators/unitary/unitarymatrix_thrust.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/src/third-party/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/src/third-party/win32/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.361367 qiskit-aer-0.9.0/src/third-party/win32/lib/
--rw-r--r--   0 runner    (1001) docker     (121)  2484913 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/third-party/win32/lib/openblas.7z
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.337366 qiskit-aer-0.9.0/src/third-party/win64/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.365367 qiskit-aer-0.9.0/src/third-party/win64/lib/
--rw-r--r--   0 runner    (1001) docker     (121)  3492408 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/third-party/win64/lib/openblas.7z
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-16 10:24:36.369367 qiskit-aer-0.9.0/src/transpile/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/transpile/basic_opts.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    25091 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/transpile/cacheblocking.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/transpile/circuitopt.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    36813 2021-09-16 10:24:13.000000 qiskit-aer-0.9.0/src/transpile/fusion.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.654826 qiskit-aer-0.9.1/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14844 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6964 2021-10-11 20:40:39.654826 qiskit-aer-0.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5058 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.606826 qiskit-aer-0.9.1/cmake/
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/FindPybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    21390 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/FindPythonExtensions.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/Linter.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/compiler_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    24973 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/conan.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/conan_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/dependency_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/findBLASInSpecificPath.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/nvcc_add_compiler_options.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    16669 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/cmake/targetLinkLibrariesWithDynamicLookup.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.598826 qiskit-aer-0.9.1/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.606826 qiskit-aer-0.9.1/contrib/standalone/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5661 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/contrib/standalone/qasm_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/contrib/standalone/version.hpp.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.606826 qiskit-aer-0.9.1/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.606826 qiskit-aer-0.9.1/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.606826 qiskit-aer-0.9.1/qiskit/providers/aer/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/aererror.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3245 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/aerprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.610826 qiskit-aer-0.9.1/qiskit/providers/aer/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32178 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/aer_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17017 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/aerbackend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13505 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/pulse_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29658 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11920 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/statevector_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12348 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/unitary_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.610826 qiskit-aer-0.9.1/qiskit/providers/aer/backends/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/wrappers/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/backends/wrappers/bindings.cc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.610826 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5980 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_density_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6916 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_expectation_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3384 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3284 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_stabilizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3371 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_statevector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.610826 qiskit-aer-0.9.1/qiskit/providers/aer/jobs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4520 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/jobs/aerjob.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13079 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/jobs/aerjobset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2853 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/jobs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.610826 qiskit-aer-0.9.1/qiskit/providers/aer/library/
+-rw-r--r--   0 runner    (1001) docker     (121)     5888 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/default_qubits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/instructions_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1652 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6917 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5440 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_density_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10420 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_expectation_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2903 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_matrix_product_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6443 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_stabilizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3213 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5064 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_statevector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2156 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_superop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2737 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_density_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2977 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_matrix_product_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_stabilizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_statevector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2693 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_superop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2646 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_unitary.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/noise/
+-rw-r--r--   0 runner    (1001) docker     (121)     5825 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10846 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6741 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1096 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22122 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/errorutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26093 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/quantum_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12190 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/readout_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22109 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/standard_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42334 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/noise/noiseerror.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.614826 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18592 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/digest_pulse_qobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8454 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/mc_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18088 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_de_solver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4892 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_sim_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5059 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/unitary_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/
+-rw-r--r--   0 runner    (1001) docker     (121)    14320 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/DE_Methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/DE_Options.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6194 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19793 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/duffing_model_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12488 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/hamiltonian_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8645 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/pulse_system_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/apply_str_func_to_qobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3847 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/gen_operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_from_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4544 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_generators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16112 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/string_model_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/qiskit/providers/aer/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3527 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_model_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4944 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_remapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29913 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/qiskit/providers/aer/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.602826 qiskit-aer-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.618826 qiskit-aer-0.9.1/src/controllers/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    69467 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/controllers/aer_controller.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1456 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/controllers/controller_execute.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.622826 qiskit-aer-0.9.1/src/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/avx2_detect.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7381 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/blas_protos.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15842 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/circuit.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9820 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/creg.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9700 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/json.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2463 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/json_parser.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.622826 qiskit-aer-0.9.1/src/framework/linalg/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2194 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/almost_equal.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/eigensystem.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1469 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/enable_if_numeric.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1140 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linalg.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.626826 qiskit-aer-0.9.1/src/framework/linalg/linops/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4217 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_aer_vector.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5103 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_array.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3641 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_generic.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6737 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_json.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6772 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_map.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4560 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_matrix.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7124 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_unordered_map.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6507 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/linops/linops_vector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.626826 qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13546 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/matrix_defs.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10977 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/smatrix_defs.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12921 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/vmatrix_defs.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)      780 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/matrix_utils.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6724 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/square.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12220 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/vector.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1727 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/linalg/vector_json.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    28383 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4743 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/noise_utils.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    43603 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/operations.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9277 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/opset.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6844 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/pybind_basics.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/pybind_casts.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    10085 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/pybind_json.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4602 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/python_parser.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6157 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/qobj.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.626826 qiskit-aer-0.9.1/src/framework/results/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.626826 qiskit-aer-0.9.1/src/framework/results/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     9637 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/data.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4955 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/metadata.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.630826 qiskit-aer-0.9.1/src/framework/results/data/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cdict.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4871 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cmatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_creg.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3319 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cvector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_json.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2462 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_mps.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rdict.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2731 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rvalue.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3055 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rvector.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2137 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cdict.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3455 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cmatrix.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1821 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_creg.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2587 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cvector.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2004 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_json.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2603 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_mps.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2345 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rdict.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2216 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rvalue.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2303 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rvector.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2314 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/pybind_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1472 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/pybind_metadata.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.630826 qiskit-aer-0.9.1/src/framework/results/data/subtypes/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2003 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/accum_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2695 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/average_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5943 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/data_map.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1925 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/list_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2515 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/pybind_data_map.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2095 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/pybind_subtypes.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1870 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/data/subtypes/single_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3118 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/experiment_result.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.634826 qiskit-aer-0.9.1/src/framework/results/legacy/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7442 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/average_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4488 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/average_snapshot.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8451 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/data_container.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2792 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/pershot_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3511 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/pershot_snapshot.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13490 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/pybind_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12857 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/legacy/snapshot_data.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4074 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/pybind_result.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3083 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/results/result.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3483 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/rng.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4689 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/stl_ostream.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1922 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/types.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    38926 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/framework/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.634826 qiskit-aer-0.9.1/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)    18973 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/clang_omp_symbols.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/common_macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4688 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/gcc_omp_symbols.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2729 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/hacks.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/warnings.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/misc/wrap_thrust.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.634826 qiskit-aer-0.9.1/src/noise/
+-rw-r--r--   0 runner    (1001) docker     (121)    37637 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/noise/noise_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13524 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/noise/quantum_error.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/noise/readout_error.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.638826 qiskit-aer-0.9.1/src/open_pulse/
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4132 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/eval_hamiltonian.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2278 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/iterators.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2808 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/log.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9987 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/numeric_integrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/numeric_integrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3802 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/ordered_map.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5426 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/pulse_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/pulse_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2445 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/pulse_utils_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13808 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/python_to_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/test_python_to_cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2678 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/test_python_to_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/types.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     7295 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/zspmv.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/open_pulse/zspmv.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.638826 qiskit-aer-0.9.1/src/simulators/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.638826 qiskit-aer-0.9.1/src/simulators/density_matrix/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    18448 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    42030 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    59191 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_state_chunk.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    32373 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_thrust.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.638826 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/
+-rw-r--r--   0 runner    (1001) docker     (121)    22914 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/ch_runner.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.638826 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/chlib/
+-rw-r--r--   0 runner    (1001) docker     (121)    28227 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/chlib/chstabilizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12207 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/chlib/core.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    36948 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/extended_stabilizer_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/extended_stabilizer/gates.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.642826 qiskit-aer-0.9.1/src/simulators/matrix_product_state/
+-rw-r--r--   0 runner    (1001) docker     (121)    42263 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    64098 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_internal.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)    21232 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_internal.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    21365 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    13563 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/svd.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/matrix_product_state/svd.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.642826 qiskit-aer-0.9.1/src/simulators/stabilizer/
+-rw-r--r--   0 runner    (1001) docker     (121)     7407 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/stabilizer/binary_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    16043 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/stabilizer/clifford.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3761 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/stabilizer/pauli.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    32524 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/stabilizer/stabilizer_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    21889 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    49597 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/state_chunk.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.642826 qiskit-aer-0.9.1/src/simulators/statevector/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.646826 qiskit-aer-0.9.1/src/simulators/statevector/chunk/
+-rw-r--r--   0 runner    (1001) docker     (121)     6811 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    19056 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk_container.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     9658 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    33340 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/chunk/device_chunk_container.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12774 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/chunk/host_chunk_container.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    12391 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/indexes.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    75146 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/qubitvector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    96756 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/qubitvector_thrust.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    50994 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/qv_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/qv_avx2.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    53204 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/statevector_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    70330 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/statevector_state_chunk.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14004 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/transformer.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3804 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/statevector/transformer_avx2.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.646826 qiskit-aer-0.9.1/src/simulators/superoperator/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6515 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/superoperator/superoperator.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    21778 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/superoperator/superoperator_state.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6650 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/superoperator/superoperator_thrust.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.646826 qiskit-aer-0.9.1/src/simulators/unitary/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    22607 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/unitary/unitary_state.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    25303 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/unitary/unitary_state_chunk.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11892 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/unitary/unitarymatrix.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12204 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/simulators/unitary/unitarymatrix_thrust.hpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.602826 qiskit-aer-0.9.1/src/third-party/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.602826 qiskit-aer-0.9.1/src/third-party/win32/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.646826 qiskit-aer-0.9.1/src/third-party/win32/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)  2484913 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/third-party/win32/lib/openblas.7z
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.602826 qiskit-aer-0.9.1/src/third-party/win64/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.650826 qiskit-aer-0.9.1/src/third-party/win64/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)  3492408 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/third-party/win64/lib/openblas.7z
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 20:40:39.654826 qiskit-aer-0.9.1/src/transpile/
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/transpile/basic_opts.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    25091 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/transpile/cacheblocking.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/transpile/circuitopt.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)    36813 2021-10-11 20:40:17.000000 qiskit-aer-0.9.1/src/transpile/fusion.hpp
```

### Comparing `qiskit-aer-0.9.0/CMakeLists.txt` & `qiskit-aer-0.9.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/MANIFEST.in` & `qiskit-aer-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/PKG-INFO` & `qiskit-aer-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-aer
-Version: 0.9.0
+Version: 0.9.1
 Summary: Qiskit Aer - High performance simulators for Qiskit
 Home-page: https://github.com/Qiskit/qiskit-aer
 Author: AER Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Description: # Qiskit Aer
```

### Comparing `qiskit-aer-0.9.0/README.md` & `qiskit-aer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/FindPybind11.cmake` & `qiskit-aer-0.9.1/cmake/FindPybind11.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/FindPythonExtensions.cmake` & `qiskit-aer-0.9.1/cmake/FindPythonExtensions.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/Linter.cmake` & `qiskit-aer-0.9.1/cmake/Linter.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/compiler_utils.cmake` & `qiskit-aer-0.9.1/cmake/compiler_utils.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/conan.cmake` & `qiskit-aer-0.9.1/cmake/conan.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/conan_utils.cmake` & `qiskit-aer-0.9.1/cmake/conan_utils.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/dependency_utils.cmake` & `qiskit-aer-0.9.1/cmake/dependency_utils.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/findBLASInSpecificPath.cmake` & `qiskit-aer-0.9.1/cmake/findBLASInSpecificPath.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/cmake/targetLinkLibrariesWithDynamicLookup.cmake` & `qiskit-aer-0.9.1/cmake/targetLinkLibrariesWithDynamicLookup.cmake`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/contrib/standalone/qasm_simulator.cpp` & `qiskit-aer-0.9.1/contrib/standalone/qasm_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/contrib/standalone/version.hpp.in` & `qiskit-aer-0.9.1/contrib/standalone/version.hpp.in`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/aererror.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/aererror.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/aerprovider.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/aerprovider.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/aer_simulator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/aer_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,24 +199,14 @@
 
     * ``max_memory_mb`` (int): Sets the maximum size of memory
       to store a state vector. If a state vector needs more, an error
       is thrown. In general, a state vector of n-qubits uses 2^n complex
       values (16 Bytes). If set to 0, the maximum will be automatically
       set to the system memory size (Default: 0).
 
-    * ``optimize_ideal_threshold`` (int): Sets the qubit threshold for
-      applying circuit optimization passes on ideal circuits.
-      Passes include gate fusion and truncation of unused qubits
-      (Default: 5).
-
-    * ``optimize_noise_threshold`` (int): Sets the qubit threshold for
-      applying circuit optimization passes on ideal circuits.
-      Passes include gate fusion and truncation of unused qubits
-      (Default: 12).
-
     These backend options only apply when using the ``"statevector"``
     simulation method:
 
     * ``statevector_parallel_threshold`` (int): Sets the threshold that
       the number of qubits must be greater than to enable OpenMP
       parallelization for matrix multiplication during execution of
       an experiment. If parallel circuit or shot execution is enabled
@@ -515,16 +505,14 @@
             enable_truncation=True,
             zero_threshold=1e-10,
             validation_threshold=None,
             max_parallel_threads=None,
             max_parallel_experiments=None,
             max_parallel_shots=None,
             max_memory_mb=None,
-            optimize_ideal_threshold=5,
-            optimize_noise_threshold=12,
             fusion_enable=True,
             fusion_verbose=False,
             fusion_max_qubit=5,
             fusion_threshold=14,
             accept_distributed_results=None,
             blocking_qubits=None,
             blocking_enable=False,
@@ -633,41 +621,26 @@
             qobj (QasmQobj): simulator input.
 
         Returns:
             dict: return a dictionary of results.
         """
         return cpp_execute(self._controller, qobj)
 
-    def set_options(self, **fields):
-        out_options = {}
-        update_basis_gates = False
-        for key, value in fields.items():
-            if key == 'method':
-                if (value is not None and value not in self.available_methods()):
-                    raise AerError(
-                        "Invalid simulation method {}. Available methods"
-                        " are: {}".format(value, self.available_methods()))
-                self._set_method_config(value)
-                update_basis_gates = True
-                out_options[key] = value
-            elif key in ['noise_model', 'basis_gates']:
-                update_basis_gates = True
-                out_options[key] = value
-            elif key == 'device':
-                if value is not None and value not in self._AVAILABLE_DEVICES:
-                    raise AerError(
-                        "Invalid simulation device {}. Available devices"
-                        " are: {}".format(value, self._AVAILABLE_DEVICES))
-                out_options[key] = value
-            elif key == 'custom_instructions':
-                self._set_configuration_option(key, value)
-            else:
-                out_options[key] = value
-        super().set_options(**out_options)
-        if update_basis_gates:
+    def set_option(self, key, value):
+        if key == "custom_instructions":
+            self._set_configuration_option(key, value)
+            return
+        if key == "method":
+            if (value is not None and value not in self.available_methods()):
+                raise AerError(
+                    "Invalid simulation method {}. Available methods"
+                    " are: {}".format(value, self.available_methods()))
+            self._set_method_config(value)
+        super().set_option(key, value)
+        if key in ["method", "noise_model", "basis_gates"]:
             self._cached_basis_gates = self._basis_gates()
 
     def _validate(self, qobj):
         """Semantic validations of the qobj which cannot be done via schemas.
 
         Warn if no measure or save instructions in run circuits.
         """
@@ -720,15 +693,14 @@
                 "simulation method basis gates (%s), and "
                 "noise model basis gates (%s) is empty",
                 config_gates, method_gates, noise_gates)
         return sorted(basis_gates)
 
     def _set_method_config(self, method=None):
         """Set non-basis gate options when setting method"""
-        super().set_options(method=method)
         # Update configuration description and number of qubits
         if method == 'statevector':
             description = 'A C++ statevector simulator with noise'
             n_qubits = MAX_QUBITS_STATEVECTOR
         elif method == 'density_matrix':
             description = 'A C++ density matrix simulator with noise'
             n_qubits = MAX_QUBITS_STATEVECTOR // 2
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/aerbackend.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/aerbackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
         parameterizations = []
         for index, inst_tuple in enumerate(circuit.data):
             if inst_tuple[0].is_parameterized():
                 for bind_pos, param in enumerate(inst_tuple[0].params):
                     if param in binds:
                         parameterizations.append([[index, bind_pos], binds[param]])
                     elif isinstance(param, ParameterExpression):
+                        # If parameter expression has no unbound parameters
+                        # it's already bound and should be skipped
+                        if not param.parameters:
+                            continue
                         local_binds = {k: v for k, v in binds.items() if k in param.parameters}
                         bind_list = [dict(zip(local_binds, t)) for t in zip(*local_binds.values())]
                         bound_values = [float(param.bind(x)) for x in bind_list]
                         parameterizations.append([[index, bind_pos], bound_values])
         return parameterizations
 
     def _convert_binds(self, circuits, parameter_binds):
@@ -203,27 +207,40 @@
         else:
             qobj = self._assemble(circuits, parameter_binds=parameter_binds, **run_options)
 
         # Optional validation
         if validate:
             self._validate(qobj)
 
+        # Get executor from qobj config and delete attribute so qobj can still be serialized
+        executor = getattr(qobj.config, 'executor', None)
+        if hasattr(qobj.config, 'executor'):
+            delattr(qobj.config, 'executor')
+
         # Optionally split the job
         experiments = split_qobj(qobj, max_size=getattr(qobj.config, 'max_job_size', None))
 
-        # Get the executor
-        executor = self._get_executor(**run_options)
+        # Temporarily remove any executor from options so that job submission
+        # can work with Dask client executors which can't be pickled
+        opts_executor = getattr(self._options, 'executor', None)
+        if hasattr(self._options, 'executor'):
+            self._options.executor = None
 
         # Submit job
         job_id = str(uuid.uuid4())
         if isinstance(experiments, list):
             aer_job = AerJobSet(self, job_id, self._run, experiments, executor)
         else:
             aer_job = AerJob(self, job_id, self._run, experiments, executor)
         aer_job.submit()
+
+        # Restore removed executor after submission
+        if hasattr(self._options, 'executor'):
+            self._options.executor = opts_executor
+
         return aer_job
 
     def configuration(self):
         """Return the simulator backend configuration.
 
         Returns:
             BackendConfiguration: the configuration for the backend.
@@ -341,28 +358,16 @@
             if val is not None:
                 setattr(qobj.config, key, val)
 
         # Override with run-time options
         for key, val in run_options.items():
             setattr(qobj.config, key, val)
 
-        # We need to remove the executor from the qobj config
-        # since it can't be serialized though JSON/Pybind.
-        if hasattr(qobj.config, 'executor'):
-            delattr(qobj.config, 'executor')
-
         return qobj
 
-    def _get_executor(self, **run_options):
-        """Get the executor"""
-        if 'executor' in run_options:
-            return run_options['executor']
-        else:
-            return getattr(self._options, 'executor', None)
-
     @abstractmethod
     def _execute(self, qobj):
         """Execute a qobj on the backend.
 
         Args:
             qobj (QasmQobj or PulseQobj): simulator input.
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/backend_utils.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/pulse_simulator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/pulse_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/qasm_simulator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/qasm_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,24 +162,14 @@
 
     * ``max_memory_mb`` (int): Sets the maximum size of memory
       to store a state vector. If a state vector needs more, an error
       is thrown. In general, a state vector of n-qubits uses 2^n complex
       values (16 Bytes). If set to 0, the maximum will be automatically
       set to the system memory size (Default: 0).
 
-    * ``optimize_ideal_threshold`` (int): Sets the qubit threshold for
-      applying circuit optimization passes on ideal circuits.
-      Passes include gate fusion and truncation of unused qubits
-      (Default: 5).
-
-    * ``optimize_noise_threshold`` (int): Sets the qubit threshold for
-      applying circuit optimization passes on ideal circuits.
-      Passes include gate fusion and truncation of unused qubits
-      (Default: 12).
-
     These backend options only apply when using the ``"statevector"``
     simulation method:
 
     * ``statevector_parallel_threshold`` (int): Sets the threshold that
       the number of qubits must be greater than to enable OpenMP
       parallelization for matrix multiplication during execution of
       an experiment. If parallel circuit or shot execution is enabled
@@ -414,16 +404,14 @@
             enable_truncation=True,
             zero_threshold=1e-10,
             validation_threshold=None,
             max_parallel_threads=None,
             max_parallel_experiments=None,
             max_parallel_shots=None,
             max_memory_mb=None,
-            optimize_ideal_threshold=5,
-            optimize_noise_threshold=12,
             fusion_enable=True,
             fusion_verbose=False,
             fusion_max_qubit=5,
             fusion_threshold=14,
             accept_distributed_results=None,
             blocking_qubits=None,
             blocking_enable=False,
@@ -510,38 +498,29 @@
 
         Returns:
             dict: return a dictionary of results.
         """
         qobj = map_legacy_method_options(qobj)
         return cpp_execute(self._controller, qobj)
 
-    def set_options(self, **fields):
-        out_options = {}
-        update_basis_gates = False
-        for key, value in fields.items():
-            if key == 'method':
-                if value in LEGACY_METHOD_MAP:
-                    value, device = LEGACY_METHOD_MAP[value]
-                    out_options["device"] = device
-                self._set_method_config(value)
-                update_basis_gates = True
-                out_options[key] = value
-                if (value is not None and value not in self.available_methods()):
-                    raise AerError(
-                        "Invalid simulation method {}. Available methods"
-                        " are: {}".format(value, self.available_methods()))
-            elif key in ['noise_model', 'basis_gates']:
-                update_basis_gates = True
-                out_options[key] = value
-            elif key == 'custom_instructions':
-                self._set_configuration_option(key, value)
-            else:
-                out_options[key] = value
-        super().set_options(**out_options)
-        if update_basis_gates:
+    def set_option(self, key, value):
+        if key == "custom_instructions":
+            self._set_configuration_option(key, value)
+            return
+        if key == "method":
+            if value in LEGACY_METHOD_MAP:
+                value, device = LEGACY_METHOD_MAP[value]
+                self.set_option("device", device)
+            if (value is not None and value not in self.available_methods()):
+                raise AerError(
+                    "Invalid simulation method {}. Available methods"
+                    " are: {}".format(value, self.available_methods()))
+            self._set_method_config(value)
+        super().set_option(key, value)
+        if key in ["method", "noise_model", "basis_gates"]:
             self._cached_basis_gates = self._basis_gates()
 
     def _validate(self, qobj):
         """Semantic validations of the qobj which cannot be done via schemas.
 
         Warn if no measurements in circuit with classical registers.
         """
@@ -666,15 +645,14 @@
             ])
         if method == 'extended_stabilizer':
             return sorted(['roerror', 'snapshot', 'save_statevector'])
         return QasmSimulator._DEFAULT_CUSTOM_INSTR
 
     def _set_method_config(self, method=None):
         """Set non-basis gate options when setting method"""
-        super().set_options(method=method)
         # Update configuration description and number of qubits
         if method in ['statevector', 'statevector_gpu', 'statevector_thrust']:
             description = 'A C++ statevector simulator with noise'
             n_qubits = MAX_QUBITS_STATEVECTOR
         elif method in ['density_matrix', 'density_matrix_gpu', 'density_matrix_thrust']:
             description = 'A C++ density matrix simulator with noise'
             n_qubits = MAX_QUBITS_STATEVECTOR // 2
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/statevector_simulator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/statevector_simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -203,42 +203,37 @@
             max_job_size=None,
             zero_threshold=1e-10,
             validation_threshold=None,
             max_parallel_threads=None,
             max_parallel_experiments=None,
             max_parallel_shots=None,
             max_memory_mb=None,
-            optimize_ideal_threshold=5,
-            optimize_noise_threshold=12,
             seed_simulator=None,
             fusion_enable=True,
             fusion_verbose=False,
             fusion_max_qubit=5,
             fusion_threshold=14,
             # statevector options
             statevector_parallel_threshold=14)
 
-    def set_options(self, **fields):
-        if "method" in fields:
+    def set_option(self, key, value):
+        if key == "method":
             # Handle deprecation of method option for device option
             warn("The method option of the `StatevectorSimulator` has been"
                  " deprecated as of qiskit-aer 0.9.0. To run a GPU statevector"
                  " simulation use the option `device='GPU'` instead",
                  DeprecationWarning)
-            fields = copy.copy(fields)
-            method = fields["method"]
-            if method in LEGACY_METHOD_MAP:
-                new_method, device = LEGACY_METHOD_MAP[method]
-                fields["method"] = new_method
-                fields["device"] = device
-            if fields["method"] != "statevector":
+            if value in LEGACY_METHOD_MAP:
+                value, device = LEGACY_METHOD_MAP[value]
+                self.set_option("device", device)
+            if value != "statevector":
                 raise AerError(
                     "only the 'statevector' method is supported for the StatevectorSimulator")
-            fields.pop("method")
-        super().set_options(**fields)
+            return
+        super().set_option(key, value)
 
     def available_methods(self):
         """Return the available simulation methods."""
         warn("The `available_methods` method of the StatevectorSimulator"
              " is deprecated as of qiskit-aer 0.9.0 as this simulator only"
              " supports a single method. To check if GPU simulation is available"
              " use the `available_devices` method instead.",
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/unitary_simulator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/unitary_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,43 +202,38 @@
             zero_threshold=1e-10,
             seed_simulator=None,
             validation_threshold=None,
             max_parallel_threads=None,
             max_parallel_experiments=None,
             max_parallel_shots=None,
             max_memory_mb=None,
-            optimize_ideal_threshold=5,
-            optimize_noise_threshold=12,
             fusion_enable=True,
             fusion_verbose=False,
             fusion_max_qubit=5,
             fusion_threshold=14,
             blocking_qubits=None,
             blocking_enable=False,
             # statevector options
             statevector_parallel_threshold=14)
 
-    def set_options(self, **fields):
-        if "method" in fields:
+    def set_option(self, key, value):
+        if key == "method":
             # Handle deprecation of method option for device option
             warn("The method option of the `UnitarySimulator` has been"
                  " deprecated as of qiskit-aer 0.9.0. To run a GPU statevector"
                  " simulation use the option `device='GPU'` instead",
                  DeprecationWarning)
-            fields = copy.copy(fields)
-            method = fields["method"]
-            if method in LEGACY_METHOD_MAP:
-                new_method, device = LEGACY_METHOD_MAP[method]
-                fields["method"] = new_method
-                fields["device"] = device
-            if fields["method"] != "unitary":
+            if value in LEGACY_METHOD_MAP:
+                value, device = LEGACY_METHOD_MAP[value]
+                self.set_option("device", device)
+            if value != "unitary":
                 raise AerError(
                     "only the 'unitary' method is supported for the UnitarySimulator")
-            fields.pop("method")
-        super().set_options(**fields)
+            return
+        super().set_option(key, value)
 
     def available_methods(self):
         """Return the available simulation methods."""
         warn("The `available_methods` method of the UnitarySimulator"
              " is deprecated as of qiskit-aer 0.9.0 as this simulator only"
              " supports a single method. To check if GPU simulation is available"
              " use the `available_devices` method instead.",
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/wrappers/CMakeLists.txt` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/wrappers/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/backends/wrappers/bindings.cc` & `qiskit-aer-0.9.1/qiskit/providers/aer/backends/wrappers/bindings.cc`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_density_matrix.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_density_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_expectation_value.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_expectation_value.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_probabilities.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_probabilities.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_stabilizer.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_stabilizer.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/extensions/snapshot_statevector.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/extensions/snapshot_statevector.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/jobs/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/jobs/aerjob.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/jobs/aerjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/jobs/aerjobset.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/jobs/aerjobset.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/jobs/utils.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/default_qubits.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/default_qubits.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/instructions_table.csv` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/instructions_table.csv`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_amplitudes.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_amplitudes.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_data.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_density_matrix.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_density_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_expectation_value.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_expectation_value.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_matrix_product_state.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_matrix_product_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_probabilities.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_probabilities.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_stabilizer.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_stabilizer.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_state.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_statevector.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_statevector.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_superop.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_superop.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/save_instructions/save_unitary.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/save_instructions/save_unitary.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_density_matrix.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_density_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_matrix_product_state.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_matrix_product_state.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_stabilizer.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_stabilizer.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_statevector.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_statevector.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_superop.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_superop.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/library/set_instructions/set_unitary.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/library/set_instructions/set_unitary.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/models.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/models.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/device/parameters.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/device/parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/errorutils.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/errorutils.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/quantum_error.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/quantum_error.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/readout_error.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/readout_error.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/errors/standard_errors.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/errors/standard_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,18 +586,18 @@
         0,
         excited_state_population=excited_state_population,
         canonical_kraus=canonical_kraus)
 
 
 def phase_damping_error(param_phase, canonical_kraus=True):
     r"""
-    Return a single-qubit combined phase and amplitude damping quantum error channel.
+    Return a single-qubit generalized phase damping quantum error channel.
 
-    The single-qubit combined phase and amplitude damping channel is
-    described by the following Kraus matrices:
+    The single-qubit phase damping channel is described by the
+    following Kraus matrices:
 
     .. code-block:: python
 
         A0 = [[1, 0], [0, sqrt(1 - b)]]
         A2 = [[0, 0], [0, sqrt(b)]]
 
     where ``b = param_phase``.
```

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/noise_model.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/noise_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/noise/noiseerror.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/noise/noiseerror.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/digest_pulse_qobj.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/digest_pulse_qobj.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/mc_controller.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/mc_controller.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_controller.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_controller.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_de_solver.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_de_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/pulse_sim_options.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/pulse_sim_options.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/controllers/unitary_controller.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/controllers/unitary_controller.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/DE_Methods.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/DE_Methods.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/DE_Options.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/DE_Options.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/de/type_utils.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/de/type_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/duffing_model_generators.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/duffing_model_generators.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/hamiltonian_model.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/hamiltonian_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/pulse_system_model.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/pulse_system_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/apply_str_func_to_qobj.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/apply_str_func_to_qobj.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/gen_operator.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/gen_operator.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_from_string.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_from_string.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_generators.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/operator_generators.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/pulse/system_models/string_model_parser/string_model_parser.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/pulse/system_models/string_model_parser/string_model_parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/utils/__init__.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_model_inserter.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_model_inserter.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_remapper.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_remapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/utils/noise_transformation.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/utils/noise_transformation.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/qiskit/providers/aer/version.py` & `qiskit-aer-0.9.1/qiskit/providers/aer/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/setup.py` & `qiskit-aer-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,34 +64,30 @@
 
 
 # These are requirements that are both runtime/install dependencies and
 # also build time/setup requirements and will be added to both lists
 # of requirements
 common_requirements = [
     'numpy>=1.16.3',
-    'scipy>=1.0',
-    'pybind11>=2.6'  # This isn't really an install requirement,
-                     # Pybind11 is required to be pre-installed for
-                     # CMake to successfully find header files.
-                     # This should be fixed in the CMake build files.
 ]
 
 setup_requirements = common_requirements + [
     'scikit-build>=0.11.0',
     'cmake!=3.17,!=3.17.0',
+    'pybind11>=2.6',
 ]
 
 extras_requirements = {
     "dask": ["dask", "distributed"]
 }
 
 if not _DISABLE_CONAN:
     setup_requirements.append('conan>=1.22.2')
 
-requirements = common_requirements + ['qiskit-terra>=0.17.0']
+requirements = common_requirements + ['qiskit-terra>=0.17.0', 'scipy>=1.0']
 
 if not hasattr(setuptools,
                'find_namespace_packages') or not inspect.ismethod(
                     setuptools.find_namespace_packages):
     print("Your setuptools version:'{}' does not support PEP 420 "
           "(find_namespace_packages). Upgrade it to version >='40.1.0' and "
           "repeat install.".format(setuptools.__version__))
```

### Comparing `qiskit-aer-0.9.0/src/controllers/aer_controller.hpp` & `qiskit-aer-0.9.1/src/controllers/aer_controller.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1784,26 +1784,18 @@
                                      Method::superop});
   for (const auto& method : methods) {
     if (validate_method(method, circ, noise_model, false))
       return method;
   }
 
   // If we got here, circuit isn't compatible with any of the simulation
-  // methods
-  std::stringstream msg;
-  msg << "AerSimulator: ";
-  if (noise_model.is_ideal()) {
-    msg << "circuit with instructions " << circ.opset();
-  } else {
-    auto opset = circ.opset();
-    opset.insert(noise_model.opset());
-    msg << "circuit and noise model with instructions" << opset;
-  }
-  msg << " is not compatible with any available simulation methods";
-  throw std::runtime_error(msg.str());
+  // method so fallback to a default method of statevector. The execution will
+  // fail but we will get partial result generation and generate a user facing
+  // error message
+  return Method::statevector;
 }
 
 bool Controller::validate_method(Method method,
                                  const Circuit &circ, 
                                  const Noise::NoiseModel &noise_model,
                                  bool throw_except) const {
   // Switch wrapper for templated function validate_state
```

### Comparing `qiskit-aer-0.9.0/src/controllers/controller_execute.hpp` & `qiskit-aer-0.9.1/src/controllers/controller_execute.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/avx2_detect.hpp` & `qiskit-aer-0.9.1/src/framework/avx2_detect.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/blas_protos.hpp` & `qiskit-aer-0.9.1/src/framework/blas_protos.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/circuit.hpp` & `qiskit-aer-0.9.1/src/framework/circuit.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -248,47 +248,46 @@
   }
 }
 
 
 void Circuit::set_params(bool truncation) {
   // Clear current circuit metadata  
   reset_metadata();
-  
+  if (ops.empty()) return;
+
   // Analyze input ops from tail to head to get locations of ancestor,
   // first measurement position and last initialize position
   const auto size = ops.size();
   std::vector<bool> ancestor(size, false);
   first_measure_pos = size;
   bool has_measure = false;
   size_t num_ancestors = 0;
   size_t last_ancestor_pos = 0;
   size_t last_initialize_pos = 0;
   bool ops_to_remove = false;
 
-  if (!ops.empty()) {
-    std::unordered_set<uint_t> ancestor_qubits;
-    for (size_t i = 0; i < size; ++ i) {
-      const size_t rpos = size - i - 1;
-      const auto& op = ops[rpos];
-      if (!truncation || check_result_ancestor(op, ancestor_qubits)) {
-        add_op_metadata(op);
-        ancestor[rpos] = true;
-        num_ancestors++;
-        if (op.type == OpType::measure) {
-          first_measure_pos = rpos;
-          has_measure = true;
-        } else if (op.type == OpType::initialize && last_initialize_pos == 0) {
-          last_initialize_pos = rpos;
-        }
-        if (last_ancestor_pos == 0) {
-          last_ancestor_pos = rpos;
-        }
-      } else if (truncation && !ops_to_remove){
-        ops_to_remove = true;
+  std::unordered_set<uint_t> ancestor_qubits;
+  for (size_t i = 0; i < size; ++ i) {
+    const size_t rpos = size - i - 1;
+    const auto& op = ops[rpos];
+    if (!truncation || check_result_ancestor(op, ancestor_qubits)) {
+      add_op_metadata(op);
+      ancestor[rpos] = true;
+      num_ancestors++;
+      if (op.type == OpType::measure) {
+        first_measure_pos = rpos;
+        has_measure = true;
+      } else if (op.type == OpType::initialize && last_initialize_pos == 0) {
+        last_initialize_pos = rpos;
       }
+      if (last_ancestor_pos == 0) {
+        last_ancestor_pos = rpos;
+      }
+    } else if (truncation && !ops_to_remove){
+      ops_to_remove = true;
     }
   }
 
   // Set qubit size and check for truncaiton
   remapped_qubits = false;
   if (truncation) {
     // Generate mapping of original qubits to ancestor set
@@ -377,15 +376,20 @@
         break;
       }
     }
   }
 
   // Counter for current position in ops as we shuffle ops
   size_t op_idx = 0;
-  const size_t head_end = (has_measure && can_sample) ? first_measure_pos : last_ancestor_pos + 1;
+  size_t head_end = 0;
+  if (has_measure && can_sample) {
+    head_end = first_measure_pos;
+  } else if (num_ancestors > 0) {
+    head_end = last_ancestor_pos + 1;
+  }
   for (size_t pos = 0; pos < head_end; ++pos) {
     if (ops_to_remove && !ancestor[pos]) {
       // Skip if not ancestor
       continue;
     }
     if (remapped_qubits) {
       remap_qubits(ops[pos]);
```

### Comparing `qiskit-aer-0.9.0/src/framework/creg.hpp` & `qiskit-aer-0.9.1/src/framework/creg.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/json.hpp` & `qiskit-aer-0.9.1/src/framework/json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/json_parser.hpp` & `qiskit-aer-0.9.1/src/framework/json_parser.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/almost_equal.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/almost_equal.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/eigensystem.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/eigensystem.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/enable_if_numeric.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/enable_if_numeric.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linalg.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linalg.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_aer_vector.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_aer_vector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_array.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_array.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_generic.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_generic.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_json.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_map.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_map.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_matrix.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_matrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_unordered_map.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_unordered_map.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/linops/linops_vector.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/linops/linops_vector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/matrix_defs.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/matrix_defs.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/smatrix_defs.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/smatrix_defs.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/matrix_utils/vmatrix_defs.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/matrix_utils/vmatrix_defs.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/matrix_utils.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/matrix_utils.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/square.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/square.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/vector.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/vector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/linalg/vector_json.hpp` & `qiskit-aer-0.9.1/src/framework/linalg/vector_json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/matrix.hpp` & `qiskit-aer-0.9.1/src/framework/matrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/noise_utils.hpp` & `qiskit-aer-0.9.1/src/framework/noise_utils.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/operations.hpp` & `qiskit-aer-0.9.1/src/framework/operations.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/opset.hpp` & `qiskit-aer-0.9.1/src/framework/opset.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/pybind_basics.hpp` & `qiskit-aer-0.9.1/src/framework/pybind_basics.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/pybind_casts.hpp` & `qiskit-aer-0.9.1/src/framework/pybind_casts.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/pybind_json.hpp` & `qiskit-aer-0.9.1/src/framework/pybind_json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/python_parser.hpp` & `qiskit-aer-0.9.1/src/framework/python_parser.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/qobj.hpp` & `qiskit-aer-0.9.1/src/framework/qobj.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/metadata.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/metadata.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cdict.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cdict.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cmatrix.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cmatrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_creg.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_creg.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_cvector.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_cvector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_json.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_mps.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_mps.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rdict.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rdict.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rvalue.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rvalue.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/data_rvector.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/data_rvector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cdict.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cdict.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cmatrix.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cmatrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_creg.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_creg.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_cvector.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_cvector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_json.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_json.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_mps.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_mps.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rdict.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rdict.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rvalue.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rvalue.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/mixins/pybind_data_rvector.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/mixins/pybind_data_rvector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/pybind_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/pybind_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/pybind_metadata.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/pybind_metadata.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/accum_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/accum_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/average_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/average_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/data_map.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/data_map.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/list_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/list_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/pybind_data_map.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/pybind_data_map.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/pybind_subtypes.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/pybind_subtypes.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/data/subtypes/single_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/data/subtypes/single_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/experiment_result.hpp` & `qiskit-aer-0.9.1/src/framework/results/experiment_result.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/average_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/average_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/average_snapshot.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/average_snapshot.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/data_container.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/data_container.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/pershot_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/pershot_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/pershot_snapshot.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/pershot_snapshot.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/pybind_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/pybind_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/legacy/snapshot_data.hpp` & `qiskit-aer-0.9.1/src/framework/results/legacy/snapshot_data.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/pybind_result.hpp` & `qiskit-aer-0.9.1/src/framework/results/pybind_result.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/results/result.hpp` & `qiskit-aer-0.9.1/src/framework/results/result.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -69,16 +69,20 @@
   json_t js;
   js["qobj_id"] = qobj_id;
   
   js["backend_name"] = backend_name;
   js["backend_version"] = backend_version;
   js["date"] = date;
   js["job_id"] = job_id;
-  for (auto& res : results) {
-    js["results"].push_back(res.to_json());
+  if (results.empty()) {
+    js["results"] = json_t::array({});
+  } else {
+      for (auto& res : results) {
+        js["results"].push_back(res.to_json());
+      }
   }
   if (header.empty() == false)
     js["header"] = header;
   js["metadata"] = metadata.to_json();
   js["success"] = (status == Status::completed);
   switch (status) {
     case Status::completed:
```

### Comparing `qiskit-aer-0.9.0/src/framework/rng.hpp` & `qiskit-aer-0.9.1/src/framework/rng.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/stl_ostream.hpp` & `qiskit-aer-0.9.1/src/framework/stl_ostream.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/types.hpp` & `qiskit-aer-0.9.1/src/framework/types.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/framework/utils.hpp` & `qiskit-aer-0.9.1/src/framework/utils.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/clang_omp_symbols.hpp` & `qiskit-aer-0.9.1/src/misc/clang_omp_symbols.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/common_macros.hpp` & `qiskit-aer-0.9.1/src/misc/common_macros.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/gcc_omp_symbols.hpp` & `qiskit-aer-0.9.1/src/misc/gcc_omp_symbols.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/hacks.hpp` & `qiskit-aer-0.9.1/src/misc/hacks.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/warnings.hpp` & `qiskit-aer-0.9.1/src/misc/warnings.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/misc/wrap_thrust.hpp` & `qiskit-aer-0.9.1/src/misc/wrap_thrust.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/noise/noise_model.hpp` & `qiskit-aer-0.9.1/src/noise/noise_model.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,18 @@
 //=========================================================================
 // Noise sampling
 //=========================================================================
 
 Circuit NoiseModel::sample_noise(const Circuit &circ,
                                  RngEngine &rng,
                                  const Method method) const {
+  // Check edge case of empty circuit
+  if (circ.ops.empty()) {
+    return circ;
+  }
   // Check if sampling method is enabled
   if (enabled_methods_.find(method) == enabled_methods_.end()) {
     throw std::runtime_error(
       "Kraus or superoperator noise sampling method has not been enabled.");
   }
   return sample_noise_circuit(circ, rng, method);                   
 }
```

### Comparing `qiskit-aer-0.9.0/src/noise/quantum_error.hpp` & `qiskit-aer-0.9.1/src/noise/quantum_error.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/noise/readout_error.hpp` & `qiskit-aer-0.9.1/src/noise/readout_error.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/CMakeLists.txt` & `qiskit-aer-0.9.1/src/open_pulse/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/eval_hamiltonian.hpp` & `qiskit-aer-0.9.1/src/open_pulse/eval_hamiltonian.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/iterators.hpp` & `qiskit-aer-0.9.1/src/open_pulse/iterators.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/log.hpp` & `qiskit-aer-0.9.1/src/open_pulse/log.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/numeric_integrator.cpp` & `qiskit-aer-0.9.1/src/open_pulse/numeric_integrator.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/numeric_integrator.hpp` & `qiskit-aer-0.9.1/src/open_pulse/numeric_integrator.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/ordered_map.hpp` & `qiskit-aer-0.9.1/src/open_pulse/ordered_map.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/pulse_utils.cpp` & `qiskit-aer-0.9.1/src/open_pulse/pulse_utils.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/pulse_utils.hpp` & `qiskit-aer-0.9.1/src/open_pulse/pulse_utils.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/pulse_utils_bindings.cpp` & `qiskit-aer-0.9.1/src/open_pulse/pulse_utils_bindings.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/python_to_cpp.hpp` & `qiskit-aer-0.9.1/src/open_pulse/python_to_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/test_python_to_cpp.cpp` & `qiskit-aer-0.9.1/src/open_pulse/test_python_to_cpp.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/test_python_to_cpp.hpp` & `qiskit-aer-0.9.1/src/open_pulse/test_python_to_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/types.hpp` & `qiskit-aer-0.9.1/src/open_pulse/types.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/zspmv.cpp` & `qiskit-aer-0.9.1/src/open_pulse/zspmv.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/open_pulse/zspmv.hpp` & `qiskit-aer-0.9.1/src/open_pulse/zspmv.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix.hpp` & `qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_state.hpp` & `qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_state_chunk.hpp` & `qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_state_chunk.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/density_matrix/densitymatrix_thrust.hpp` & `qiskit-aer-0.9.1/src/simulators/density_matrix/densitymatrix_thrust.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/extended_stabilizer/ch_runner.hpp` & `qiskit-aer-0.9.1/src/simulators/extended_stabilizer/ch_runner.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/extended_stabilizer/chlib/chstabilizer.hpp` & `qiskit-aer-0.9.1/src/simulators/extended_stabilizer/chlib/chstabilizer.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/extended_stabilizer/chlib/core.hpp` & `qiskit-aer-0.9.1/src/simulators/extended_stabilizer/chlib/core.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/extended_stabilizer/extended_stabilizer_state.hpp` & `qiskit-aer-0.9.1/src/simulators/extended_stabilizer/extended_stabilizer_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/extended_stabilizer/gates.hpp` & `qiskit-aer-0.9.1/src/simulators/extended_stabilizer/gates.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state.hpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_internal.cpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_internal.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_internal.hpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_internal.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/matrix_product_state_tensor.hpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/matrix_product_state_tensor.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/svd.cpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/svd.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -123,22 +123,23 @@
   // that were discarded by approximation
   double discarded_value = 0.0;
 
   if (new_SV_num < SV_num) {
     for (uint_t i=new_SV_num; i<SV_num; i++) {
       discarded_value += std::norm(S[i]);
     }
-    // After approximation, we may need to re-normalize the values of S
-    double new_sum_squares = 0;
-    for (uint_t i=0; i<S.size(); i++) 
-      new_sum_squares +=std::norm(S[i]);
-    
-    double sqrt_sum = std::sqrt(new_sum_squares);
-    for (uint_t i=0; i<S.size(); i++)
-      S[i] /= sqrt_sum;
+  }
+  // Check if we need to re-normalize the values of S
+  double new_sum_squares = 0;
+  for (uint_t i=0; i<S.size(); i++) 
+    new_sum_squares +=std::norm(S[i]);
+  if (!Linalg::almost_equal(1.0 - new_sum_squares, 0., THRESHOLD)) {
+	double sqrt_sum = std::sqrt(new_sum_squares);
+	for (uint_t i=0; i<S.size(); i++)
+	  S[i] /= sqrt_sum;
   }
   return discarded_value;
 }
 
 void validate_SVD_result(const cmatrix_t &A, const cmatrix_t &U, 
 			 const rvector_t &S, const cmatrix_t &V) {
   const uint_t nrows = A.GetRows(), ncols = A.GetColumns();
```

### Comparing `qiskit-aer-0.9.0/src/simulators/matrix_product_state/svd.hpp` & `qiskit-aer-0.9.1/src/simulators/matrix_product_state/svd.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/stabilizer/binary_vector.hpp` & `qiskit-aer-0.9.1/src/simulators/stabilizer/binary_vector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/stabilizer/clifford.hpp` & `qiskit-aer-0.9.1/src/simulators/stabilizer/clifford.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/stabilizer/pauli.hpp` & `qiskit-aer-0.9.1/src/simulators/stabilizer/pauli.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/stabilizer/stabilizer_state.hpp` & `qiskit-aer-0.9.1/src/simulators/stabilizer/stabilizer_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/state.hpp` & `qiskit-aer-0.9.1/src/simulators/state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/state_chunk.hpp` & `qiskit-aer-0.9.1/src/simulators/state_chunk.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk_container.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk_container.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/chunk/chunk_manager.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/chunk/chunk_manager.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/chunk/device_chunk_container.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/chunk/device_chunk_container.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/chunk/host_chunk_container.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/chunk/host_chunk_container.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/indexes.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/indexes.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/qubitvector.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/qubitvector.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/qubitvector_thrust.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/qubitvector_thrust.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/qv_avx2.cpp` & `qiskit-aer-0.9.1/src/simulators/statevector/qv_avx2.cpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/qv_avx2.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/qv_avx2.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/statevector_state.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/statevector_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/statevector_state_chunk.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/statevector_state_chunk.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/transformer.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/transformer.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/statevector/transformer_avx2.hpp` & `qiskit-aer-0.9.1/src/simulators/statevector/transformer_avx2.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/superoperator/superoperator.hpp` & `qiskit-aer-0.9.1/src/simulators/superoperator/superoperator.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/superoperator/superoperator_state.hpp` & `qiskit-aer-0.9.1/src/simulators/superoperator/superoperator_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/superoperator/superoperator_thrust.hpp` & `qiskit-aer-0.9.1/src/simulators/superoperator/superoperator_thrust.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/unitary/unitary_state.hpp` & `qiskit-aer-0.9.1/src/simulators/unitary/unitary_state.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/unitary/unitary_state_chunk.hpp` & `qiskit-aer-0.9.1/src/simulators/unitary/unitary_state_chunk.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/unitary/unitarymatrix.hpp` & `qiskit-aer-0.9.1/src/simulators/unitary/unitarymatrix.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/simulators/unitary/unitarymatrix_thrust.hpp` & `qiskit-aer-0.9.1/src/simulators/unitary/unitarymatrix_thrust.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/third-party/win32/lib/openblas.7z` & `qiskit-aer-0.9.1/src/third-party/win32/lib/openblas.7z`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/third-party/win64/lib/openblas.7z` & `qiskit-aer-0.9.1/src/third-party/win64/lib/openblas.7z`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/transpile/basic_opts.hpp` & `qiskit-aer-0.9.1/src/transpile/basic_opts.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/transpile/cacheblocking.hpp` & `qiskit-aer-0.9.1/src/transpile/cacheblocking.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/transpile/circuitopt.hpp` & `qiskit-aer-0.9.1/src/transpile/circuitopt.hpp`

 * *Files identical despite different names*

### Comparing `qiskit-aer-0.9.0/src/transpile/fusion.hpp` & `qiskit-aer-0.9.1/src/transpile/fusion.hpp`

 * *Files identical despite different names*

