# Comparing `tmp/DEHB-0.1.0.tar.gz` & `tmp/DEHB-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DEHB-0.1.0.tar", last modified: Sat Feb 17 15:01:34 2024, max compression
+gzip compressed data, was "DEHB-0.1.1.tar", last modified: Mon Apr  1 16:54:15 2024, max compression
```

## Comparing `DEHB-0.1.0.tar` & `DEHB-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.315001 DEHB-0.1.0/
--rw-r--r--   0 fixja     (1000) fixja     (1000)    11355 2023-09-04 15:38:32.000000 DEHB-0.1.0/LICENSE.txt
--rw-r--r--   0 fixja     (1000) fixja     (1000)      302 2023-09-29 08:33:50.000000 DEHB-0.1.0/MANIFEST.in
--rw-r--r--   0 fixja     (1000) fixja     (1000)    23117 2024-02-17 15:01:34.315001 DEHB-0.1.0/PKG-INFO
--rw-r--r--   0 fixja     (1000) fixja     (1000)     8434 2024-02-17 15:01:29.000000 DEHB-0.1.0/README.md
--rw-r--r--   0 fixja     (1000) fixja     (1000)     5560 2024-02-17 15:01:29.000000 DEHB-0.1.0/pyproject.toml
--rw-r--r--   0 fixja     (1000) fixja     (1000)       38 2024-02-17 15:01:34.315001 DEHB-0.1.0/setup.cfg
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.305001 DEHB-0.1.0/src/
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.305001 DEHB-0.1.0/src/DEHB.egg-info/
--rw-r--r--   0 fixja     (1000) fixja     (1000)    23117 2024-02-17 15:01:34.000000 DEHB-0.1.0/src/DEHB.egg-info/PKG-INFO
--rw-r--r--   0 fixja     (1000) fixja     (1000)      411 2024-02-17 15:01:34.000000 DEHB-0.1.0/src/DEHB.egg-info/SOURCES.txt
--rw-r--r--   0 fixja     (1000) fixja     (1000)        1 2024-02-17 15:01:34.000000 DEHB-0.1.0/src/DEHB.egg-info/dependency_links.txt
--rw-r--r--   0 fixja     (1000) fixja     (1000)      245 2024-02-17 15:01:34.000000 DEHB-0.1.0/src/DEHB.egg-info/requires.txt
--rw-r--r--   0 fixja     (1000) fixja     (1000)        5 2024-02-17 15:01:34.000000 DEHB-0.1.0/src/DEHB.egg-info/top_level.txt
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.305001 DEHB-0.1.0/src/dehb/
--rw-r--r--   0 fixja     (1000) fixja     (1000)      116 2023-10-01 18:26:48.000000 DEHB-0.1.0/src/dehb/__init__.py
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.305001 DEHB-0.1.0/src/dehb/optimizers/
--rw-r--r--   0 fixja     (1000) fixja     (1000)       61 2023-09-04 15:38:32.000000 DEHB-0.1.0/src/dehb/optimizers/__init__.py
--rw-r--r--   0 fixja     (1000) fixja     (1000)    38274 2024-02-17 14:45:49.000000 DEHB-0.1.0/src/dehb/optimizers/de.py
--rw-r--r--   0 fixja     (1000) fixja     (1000)    42643 2024-02-17 15:01:29.000000 DEHB-0.1.0/src/dehb/optimizers/dehb.py
-drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-02-17 15:01:34.305001 DEHB-0.1.0/src/dehb/utils/
--rw-r--r--   0 fixja     (1000) fixja     (1000)       93 2024-02-17 14:45:34.000000 DEHB-0.1.0/src/dehb/utils/__init__.py
--rw-r--r--   0 fixja     (1000) fixja     (1000)     7254 2024-02-17 14:45:49.000000 DEHB-0.1.0/src/dehb/utils/bracket_manager.py
--rw-r--r--   0 fixja     (1000) fixja     (1000)     5398 2024-02-17 14:45:49.000000 DEHB-0.1.0/src/dehb/utils/config_repository.py
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    11355 2024-03-05 10:47:42.000000 DEHB-0.1.1/LICENSE.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      302 2024-03-05 10:47:42.000000 DEHB-0.1.1/MANIFEST.in
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    20631 2024-04-01 16:54:15.632463 DEHB-0.1.1/PKG-INFO
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     5874 2024-04-01 16:43:39.000000 DEHB-0.1.1/README.md
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     5592 2024-04-01 16:44:07.000000 DEHB-0.1.1/pyproject.toml
+-rw-r--r--   0 fixja     (1000) fixja     (1000)       38 2024-04-01 16:54:15.632463 DEHB-0.1.1/setup.cfg
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/src/
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/src/DEHB.egg-info/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    20631 2024-04-01 16:54:15.000000 DEHB-0.1.1/src/DEHB.egg-info/PKG-INFO
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      411 2024-04-01 16:54:15.000000 DEHB-0.1.1/src/DEHB.egg-info/SOURCES.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)        1 2024-04-01 16:54:15.000000 DEHB-0.1.1/src/DEHB.egg-info/dependency_links.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      270 2024-04-01 16:54:15.000000 DEHB-0.1.1/src/DEHB.egg-info/requires.txt
+-rw-r--r--   0 fixja     (1000) fixja     (1000)        5 2024-04-01 16:54:15.000000 DEHB-0.1.1/src/DEHB.egg-info/top_level.txt
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/src/dehb/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)      116 2024-03-05 10:47:42.000000 DEHB-0.1.1/src/dehb/__init__.py
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/src/dehb/optimizers/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)       61 2024-03-05 10:47:42.000000 DEHB-0.1.1/src/dehb/optimizers/__init__.py
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    38559 2024-04-01 16:29:57.000000 DEHB-0.1.1/src/dehb/optimizers/de.py
+-rw-r--r--   0 fixja     (1000) fixja     (1000)    52070 2024-04-01 16:43:39.000000 DEHB-0.1.1/src/dehb/optimizers/dehb.py
+drwxr-xr-x   0 fixja     (1000) fixja     (1000)        0 2024-04-01 16:54:15.632463 DEHB-0.1.1/src/dehb/utils/
+-rw-r--r--   0 fixja     (1000) fixja     (1000)       93 2024-03-05 10:47:42.000000 DEHB-0.1.1/src/dehb/utils/__init__.py
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     7254 2024-03-05 10:47:42.000000 DEHB-0.1.1/src/dehb/utils/bracket_manager.py
+-rw-r--r--   0 fixja     (1000) fixja     (1000)     6000 2024-04-01 16:29:57.000000 DEHB-0.1.1/src/dehb/utils/config_repository.py
```

### Comparing `DEHB-0.1.0/LICENSE.txt` & `DEHB-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DEHB-0.1.0/PKG-INFO` & `DEHB-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DEHB
-Version: 0.1.0
+Version: 0.1.1
 Summary: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
 Author: Noor Awad, Frank Hutter
 Author-email: Neeratyoy Mallik <mallik@cs.uni-freiburg.de>, Janis Fix <fixj@cs.uni-freiburg.de>
 License:                               Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -237,142 +237,84 @@
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: markdown-exec[ansi]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: mike; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: examples
+Requires-Dist: scikit-learn; extra == "examples"
 
 # DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Tests](https://github.com/automl/DEHB/actions/workflows/pytest.yml/badge.svg)](https://github.com/automl/DEHB/actions/workflows/pytest.yml)
 [![docs](https://github.com/automl/DEHB/actions/workflows/docs.yml/badge.svg)](https://automl.github.io/DEHB/)
 [![Coverage Status](https://coveralls.io/repos/github/automl/DEHB/badge.svg)](https://coveralls.io/github/automl/DEHB)
 [![PyPI](https://img.shields.io/pypi/v/dehb)](https://pypi.org/project/dehb/)
 [![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)](https://pypi.org/project/dehb/)
 [![arXiv](https://img.shields.io/badge/arXiv-2105.09821-b31b1b.svg)](https://arxiv.org/abs/2105.09821)
-### Installation
-```bash
-# from pypi
-pip install dehb
 
-# to run examples, install from github
-git clone https://github.com/automl/DEHB.git
-pip install -e DEHB  # -e stands for editable, lets you modify the code and rerun things
-```
-
-### Tutorials/Example notebooks
+Welcome to DEHB, an algorithm for Hyperparameter Optimization (HPO). DEHB uses Differential Evolution (DE) under-the-hood as an Evolutionary Algorithm to power the black-box optimization that HPO problems pose.
 
-* [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
-* [01.1 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01.1_Optimizing_RandomForest_using_DEHB.ipynb)
-* [01.2 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset using Ask & Tell interface](examples/01.2_Optimizing_RandomForest_using_Ask_Tell.ipynb)
-* [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
-* [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
+`dehb` is a python package implementing the [DEHB](https://arxiv.org/abs/2105.09821) algorithm. It offers an intuitive interface to optimize user-defined problems using DEHB.
 
-To run PyTorch example: (*note additional requirements*) 
+### Getting Started
+#### Installation
 ```bash
-python examples/03_pytorch_mnist_hpo.py \
-    --min_fidelity 1 \
-    --max_fidelity 3 \
-    --runtime 60 \
-    --verbose
+pip install dehb
 ```
-
-#### Ask & Tell interface
-DEHB allows users to either utilize the Ask & Tell interface for manual task distribution or leverage the built-in functionality (`run`) to set up a Dask cluster autonomously.
-The Ask & Tell functionality can be utilized as follows:
+#### Using DEHB
+DEHB allows users to either utilize the Ask & Tell interface for manual task distribution or leverage the built-in functionality (`run`) to set up a Dask cluster autonomously. The following snippet offers a small look in to how to use DEHB. For further information, please refer to our [getting started examples](https://automl.github.io/DEHB/latest/getting_started/single_worker/) in our documentation.
 ```python
 optimizer = DEHB(
-    f=your_target_function, # Here we do not need to necessarily specify the target function, but it can still be useful to call 'run' later.
+    f=your_target_function,
     cs=config_space, 
     dimensions=dimensions, 
     min_fidelity=min_fidelity, 
     max_fidelity=max_fidelity)
 
+##### Using Ask & Tell
 # Ask for next configuration to run
 job_info = optimizer.ask()
 
 # Run the configuration for the given fidelity. Here you can freely distribute the computation to any worker you'd like.
 result = your_target_function(config=job_info["config"], fidelity=job_info["fidelity"])
 
 # When you received the result, feed them back to the optimizer
 optimizer.tell(job_info, result)
-```
-
-### Running DEHB in a parallel setting
-
-DEHB has been designed to interface a [Dask client](https://distributed.dask.org/en/latest/api.html#distributed.Client).
-DEHB can either create a Dask client during instantiation and close/kill the client during garbage collection. 
-Or a client can be passed as an argument during instantiation.
-
-* Setting `n_workers` during instantiation \
-    If set to `1` (default) then the entire process is a sequential run without invoking Dask. \
-    If set to `>1` then a Dask Client is initialized with as many workers as `n_workers`. \
-    This parameter is ignored if `client` is not None.
-* Setting `client` during instantiation \
-    When `None` (default), a Dask client is created using `n_workers` specified. \
-    Else, any custom-configured Dask Client can be created and passed as the `client` argument to DEHB.
-  
-#### Using GPUs in a parallel run
-
-Certain target function evaluations (especially for Deep Learning) require computations to be 
-carried out on GPUs. The GPU devices are often ordered by device ID and if not configured, all 
-spawned worker processes access these devices in the same order and can either run out of memory or
-not exhibit parallelism.
-
-For `n_workers>1` and when running on a single node (or local), the `single_node_with_gpus` can be 
-passed to the `run()` call to DEHB. Setting it to `False` (default) has no effect on the default setup 
-of the machine. Setting it to `True` will reorder the GPU device IDs dynamically by setting the environment 
-variable `CUDA_VISIBLE_DEVICES` for each worker process executing a target function evaluation. The re-ordering 
-is done in a manner that the first priority device is the one with the least number of active jobs assigned 
-to it by that DEHB run.
 
-To run the PyTorch MNIST example on a single node using 2 workers:  
-```bash
-python examples/03_pytorch_mnist_hpo.py \
-    --min_fidelity 1 \
-    --max_fidelity 3 \
-    --runtime 60 \
-    --n_workers 2 \
-    --single_node_with_gpus \
-    --verbose
+##### Using run()
+# Run optimization for 1 bracket. Output files will be saved to ./logs
+traj, runtime, history = optimizer.run(brackets=1, verbose=True)
 ```
 
-#### Multi-node runs
+#### Running DEHB in a parallel setting
+For a more in-depth look in how-to run DEHB in a parallel setting, please have a look at our [documentation](https://automl.github.io/DEHB/latest/getting_started/parallel/).
 
-Multi-node parallelism is often contingent on the cluster setup to be deployed on. Dask provides useful 
-frameworks to interface various cluster designs. As long as the `client` passed to DEHB during 
-instantiation is of type `dask.distributed.Client`, DEHB can interact with this client and 
-distribute its optimization process in a parallel manner. 
-
-For instance, `Dask-CLI` can be used to create a `dask-scheduler` which can dump its connection 
-details to a file on a cluster node accessible to all processes. Multiple `dask-worker` can then be
-created to interface the `dask-scheduler` by connecting to the details read from the file dumped. Each
-dask-worker can be triggered on any remote machine. Each worker can be configured as required, 
-including mapping to specific GPU devices. 
+### Tutorials/Example notebooks
 
-Some helper scripts can be found [here](utils/), that can be used as a reference to run DEHB in a multi-node 
-manner on clusters managed by SLURM. (*not expected to work off-the-shelf*)
+* [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
+* [01.1 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01.1_Optimizing_RandomForest_using_DEHB.ipynb)
+* [01.2 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset using Ask & Tell interface](examples/01.2_Optimizing_RandomForest_using_Ask_Tell.ipynb)
+* [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
+* [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
 
-To run the PyTorch MNIST example on a multi-node setup using 4 workers:
+To run PyTorch example: (*note additional requirements*) 
 ```bash
-bash utils/run_dask_setup.sh \
-    -f dask_dump/scheduler.json \  # This is how the workers will be discovered by DEHB
-    -e env_name \
-    -n 4
-
-# Make sure to sleep to allow the workers to setup properly
-sleep 5
 python examples/03_pytorch_mnist_hpo.py \
     --min_fidelity 1 \
     --max_fidelity 3 \
     --runtime 60 \
-    --scheduler_file dask_dump/scheduler.json \
     --verbose
 ```
+### Documentation
+For more details and features, please have a look at our [documentation](https://automl.github.io/DEHB/latest/).
+
+### Contributing
+Any contribution is greaty appreciated! Please take the time to check out our [contributing guidelines](./CONTRIBUTING.md)
 
 ### DEHB Hyperparameters
 
 *We recommend the default settings*.
 The default settings were chosen based on ablation studies over a collection of diverse problems 
 and were found to be *generally* useful across all cases tested. 
 However, the parameters are still available for tuning to a specific problem.
```

### Comparing `DEHB-0.1.0/pyproject.toml` & `DEHB-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # For TOML reference
 # https://learnxinyminutes.com/docs/toml/
 [project]
 urls = { Documentation = "https://automl.github.io/DEHB/", Github = "https://github.com/automl/DEHB" }
 
 name = "DEHB"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
   "numpy>=1.18.2",
   "loguru>=0.5.3",
   "dask>=2.27.0",
   "distributed>=2.27.0",
   "ConfigSpace>=0.4.16",
 ]
@@ -49,14 +49,17 @@
   "mkdocs-jupyter",
   "mike",
   # Others
   "ruff",
   "black",
   "pre-commit",
 ]
+examples = [
+  "scikit-learn"
+]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]                   # path to the test directory
 minversion = "3.8"
 addopts = "--cov=src --cov-report=lcov" # Should be package name
 pythonpath = ["."]
```

### Comparing `DEHB-0.1.0/src/DEHB.egg-info/PKG-INFO` & `DEHB-0.1.1/src/DEHB.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DEHB
-Version: 0.1.0
+Version: 0.1.1
 Summary: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
 Author: Noor Awad, Frank Hutter
 Author-email: Neeratyoy Mallik <mallik@cs.uni-freiburg.de>, Janis Fix <fixj@cs.uni-freiburg.de>
 License:                               Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -237,142 +237,84 @@
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: markdown-exec[ansi]; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
 Requires-Dist: mike; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: examples
+Requires-Dist: scikit-learn; extra == "examples"
 
 # DEHB: Evolutionary Hyperband for Scalable, Robust and Efficient Hyperparameter Optimization
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Tests](https://github.com/automl/DEHB/actions/workflows/pytest.yml/badge.svg)](https://github.com/automl/DEHB/actions/workflows/pytest.yml)
 [![docs](https://github.com/automl/DEHB/actions/workflows/docs.yml/badge.svg)](https://automl.github.io/DEHB/)
 [![Coverage Status](https://coveralls.io/repos/github/automl/DEHB/badge.svg)](https://coveralls.io/github/automl/DEHB)
 [![PyPI](https://img.shields.io/pypi/v/dehb)](https://pypi.org/project/dehb/)
 [![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue)](https://pypi.org/project/dehb/)
 [![arXiv](https://img.shields.io/badge/arXiv-2105.09821-b31b1b.svg)](https://arxiv.org/abs/2105.09821)
-### Installation
-```bash
-# from pypi
-pip install dehb
 
-# to run examples, install from github
-git clone https://github.com/automl/DEHB.git
-pip install -e DEHB  # -e stands for editable, lets you modify the code and rerun things
-```
-
-### Tutorials/Example notebooks
+Welcome to DEHB, an algorithm for Hyperparameter Optimization (HPO). DEHB uses Differential Evolution (DE) under-the-hood as an Evolutionary Algorithm to power the black-box optimization that HPO problems pose.
 
-* [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
-* [01.1 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01.1_Optimizing_RandomForest_using_DEHB.ipynb)
-* [01.2 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset using Ask & Tell interface](examples/01.2_Optimizing_RandomForest_using_Ask_Tell.ipynb)
-* [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
-* [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
+`dehb` is a python package implementing the [DEHB](https://arxiv.org/abs/2105.09821) algorithm. It offers an intuitive interface to optimize user-defined problems using DEHB.
 
-To run PyTorch example: (*note additional requirements*) 
+### Getting Started
+#### Installation
 ```bash
-python examples/03_pytorch_mnist_hpo.py \
-    --min_fidelity 1 \
-    --max_fidelity 3 \
-    --runtime 60 \
-    --verbose
+pip install dehb
 ```
-
-#### Ask & Tell interface
-DEHB allows users to either utilize the Ask & Tell interface for manual task distribution or leverage the built-in functionality (`run`) to set up a Dask cluster autonomously.
-The Ask & Tell functionality can be utilized as follows:
+#### Using DEHB
+DEHB allows users to either utilize the Ask & Tell interface for manual task distribution or leverage the built-in functionality (`run`) to set up a Dask cluster autonomously. The following snippet offers a small look in to how to use DEHB. For further information, please refer to our [getting started examples](https://automl.github.io/DEHB/latest/getting_started/single_worker/) in our documentation.
 ```python
 optimizer = DEHB(
-    f=your_target_function, # Here we do not need to necessarily specify the target function, but it can still be useful to call 'run' later.
+    f=your_target_function,
     cs=config_space, 
     dimensions=dimensions, 
     min_fidelity=min_fidelity, 
     max_fidelity=max_fidelity)
 
+##### Using Ask & Tell
 # Ask for next configuration to run
 job_info = optimizer.ask()
 
 # Run the configuration for the given fidelity. Here you can freely distribute the computation to any worker you'd like.
 result = your_target_function(config=job_info["config"], fidelity=job_info["fidelity"])
 
 # When you received the result, feed them back to the optimizer
 optimizer.tell(job_info, result)
-```
-
-### Running DEHB in a parallel setting
-
-DEHB has been designed to interface a [Dask client](https://distributed.dask.org/en/latest/api.html#distributed.Client).
-DEHB can either create a Dask client during instantiation and close/kill the client during garbage collection. 
-Or a client can be passed as an argument during instantiation.
-
-* Setting `n_workers` during instantiation \
-    If set to `1` (default) then the entire process is a sequential run without invoking Dask. \
-    If set to `>1` then a Dask Client is initialized with as many workers as `n_workers`. \
-    This parameter is ignored if `client` is not None.
-* Setting `client` during instantiation \
-    When `None` (default), a Dask client is created using `n_workers` specified. \
-    Else, any custom-configured Dask Client can be created and passed as the `client` argument to DEHB.
-  
-#### Using GPUs in a parallel run
-
-Certain target function evaluations (especially for Deep Learning) require computations to be 
-carried out on GPUs. The GPU devices are often ordered by device ID and if not configured, all 
-spawned worker processes access these devices in the same order and can either run out of memory or
-not exhibit parallelism.
-
-For `n_workers>1` and when running on a single node (or local), the `single_node_with_gpus` can be 
-passed to the `run()` call to DEHB. Setting it to `False` (default) has no effect on the default setup 
-of the machine. Setting it to `True` will reorder the GPU device IDs dynamically by setting the environment 
-variable `CUDA_VISIBLE_DEVICES` for each worker process executing a target function evaluation. The re-ordering 
-is done in a manner that the first priority device is the one with the least number of active jobs assigned 
-to it by that DEHB run.
 
-To run the PyTorch MNIST example on a single node using 2 workers:  
-```bash
-python examples/03_pytorch_mnist_hpo.py \
-    --min_fidelity 1 \
-    --max_fidelity 3 \
-    --runtime 60 \
-    --n_workers 2 \
-    --single_node_with_gpus \
-    --verbose
+##### Using run()
+# Run optimization for 1 bracket. Output files will be saved to ./logs
+traj, runtime, history = optimizer.run(brackets=1, verbose=True)
 ```
 
-#### Multi-node runs
+#### Running DEHB in a parallel setting
+For a more in-depth look in how-to run DEHB in a parallel setting, please have a look at our [documentation](https://automl.github.io/DEHB/latest/getting_started/parallel/).
 
-Multi-node parallelism is often contingent on the cluster setup to be deployed on. Dask provides useful 
-frameworks to interface various cluster designs. As long as the `client` passed to DEHB during 
-instantiation is of type `dask.distributed.Client`, DEHB can interact with this client and 
-distribute its optimization process in a parallel manner. 
-
-For instance, `Dask-CLI` can be used to create a `dask-scheduler` which can dump its connection 
-details to a file on a cluster node accessible to all processes. Multiple `dask-worker` can then be
-created to interface the `dask-scheduler` by connecting to the details read from the file dumped. Each
-dask-worker can be triggered on any remote machine. Each worker can be configured as required, 
-including mapping to specific GPU devices. 
+### Tutorials/Example notebooks
 
-Some helper scripts can be found [here](utils/), that can be used as a reference to run DEHB in a multi-node 
-manner on clusters managed by SLURM. (*not expected to work off-the-shelf*)
+* [00 - A generic template to use DEHB for multi-fidelity Hyperparameter Optimization](examples/00_interfacing_DEHB.ipynb)
+* [01.1 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset](examples/01.1_Optimizing_RandomForest_using_DEHB.ipynb)
+* [01.2 - Using DEHB to optimize 4 hyperparameters of a Scikit-learn's Random Forest on a classification dataset using Ask & Tell interface](examples/01.2_Optimizing_RandomForest_using_Ask_Tell.ipynb)
+* [02 - Optimizing Scikit-learn's Random Forest without using ConfigSpace to represent the hyperparameter space](examples/02_using%20DEHB_without_ConfigSpace.ipynb)
+* [03 - Hyperparameter Optimization for MNIST in PyTorch](examples/03_pytorch_mnist_hpo.py)
 
-To run the PyTorch MNIST example on a multi-node setup using 4 workers:
+To run PyTorch example: (*note additional requirements*) 
 ```bash
-bash utils/run_dask_setup.sh \
-    -f dask_dump/scheduler.json \  # This is how the workers will be discovered by DEHB
-    -e env_name \
-    -n 4
-
-# Make sure to sleep to allow the workers to setup properly
-sleep 5
 python examples/03_pytorch_mnist_hpo.py \
     --min_fidelity 1 \
     --max_fidelity 3 \
     --runtime 60 \
-    --scheduler_file dask_dump/scheduler.json \
     --verbose
 ```
+### Documentation
+For more details and features, please have a look at our [documentation](https://automl.github.io/DEHB/latest/).
+
+### Contributing
+Any contribution is greaty appreciated! Please take the time to check out our [contributing guidelines](./CONTRIBUTING.md)
 
 ### DEHB Hyperparameters
 
 *We recommend the default settings*.
 The default settings were chosen based on ablation studies over a collection of diverse problems 
 and were found to be *generally* useful across all cases tested. 
 However, the parameters are still available for tuning to a specific problem.
```

### Comparing `DEHB-0.1.0/src/dehb/optimizers/de.py` & `DEHB-0.1.1/src/dehb/optimizers/de.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from typing import List
 
 import ConfigSpace
 import ConfigSpace.util
 import numpy as np
 from distributed import Client
 
@@ -10,15 +11,18 @@
 
 
 class DEBase():
     '''Base class for Differential Evolution
     '''
     def __init__(self, cs=None, f=None, dimensions=None, pop_size=None, max_age=None,
                  mutation_factor=None, crossover_prob=None, strategy=None,
-                 boundary_fix_type='random', config_repository=None, **kwargs):
+                 boundary_fix_type='random', config_repository=None, seed=None, rng=None, **kwargs):
+        # Rng, either uses the rng passed by user/DEHB or creates its own
+        self.rng = rng if rng is not None else np.random.default_rng(seed)
+
         # Benchmark related variables
         self.cs = cs
         self.f = f
         if dimensions is None and self.cs is not None:
             self.dimensions = len(self.cs.get_hyperparameters())
         else:
             self.dimensions = dimensions
@@ -34,16 +38,16 @@
         # Miscellaneous
         self.configspace = True if isinstance(self.cs, ConfigSpace.ConfigurationSpace) else False
         self.hps = dict()
         if self.configspace:
             for i, hp in enumerate(cs.get_hyperparameters()):
                 # maps hyperparameter name to positional index in vector form
                 self.hps[hp.name] = i
-        self.output_path = kwargs['output_path'] if 'output_path' in kwargs else './'
-        os.makedirs(self.output_path, exist_ok=True)
+        self.output_path = Path(kwargs["output_path"]) if "output_path" in kwargs else Path("./")
+        self.output_path.mkdir(parents=True, exist_ok=True)
 
         if config_repository:
             self.config_repository = config_repository
         else:
             self.config_repository = ConfigRepository()
 
         # Global trackers
@@ -65,22 +69,22 @@
         self.population_ids = None
         self.fitness = None
         self.age = None
         self.history = []
 
     def _shuffle_pop(self):
         pop_order = np.arange(len(self.population))
-        np.random.shuffle(pop_order)
+        self.rng.shuffle(pop_order)
         self.population = self.population[pop_order]
         self.fitness = self.fitness[pop_order]
         self.age = self.age[pop_order]
 
     def _sort_pop(self):
         pop_order = np.argsort(self.fitness)
-        np.random.shuffle(pop_order)
+        self.rng.shuffle(pop_order)
         self.population = self.population[pop_order]
         self.fitness = self.fitness[pop_order]
         self.age = self.age[pop_order]
 
     def _set_min_pop_size(self):
         if self.mutation_strategy in ['rand1', 'rand2dir', 'randtobest1']:
             self._min_pop_size = 3
@@ -102,37 +106,37 @@
             if not isinstance(population, List):
                 population = [population]
             # the population is maintained in a list-of-vector form where each ConfigSpace
             # configuration is scaled to a unit hypercube, i.e., all dimensions scaled to [0,1]
             population = [self.configspace_to_vector(individual) for individual in population]
         else:
             # if no ConfigSpace representation available, uniformly sample from [0, 1]
-            population = np.random.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
+            population = self.rng.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
 
         return np.array(population)
 
     def sample_population(self, size: int = 3, alt_pop: List = None) -> List:
         '''Samples 'size' individuals
 
         If alt_pop is None or a list/array of None, sample from own population
         Else sample from the specified alternate population (alt_pop)
         '''
         if isinstance(alt_pop, list) or isinstance(alt_pop, np.ndarray):
             idx = [indv is None for indv in alt_pop]
             if any(idx):
-                selection = np.random.choice(np.arange(len(self.population)), size, replace=False)
+                selection = self.rng.choice(np.arange(len(self.population)), size, replace=False)
                 return self.population[selection]
             else:
                 if len(alt_pop) < 3:
                     alt_pop = np.vstack((alt_pop, self.population))
-                selection = np.random.choice(np.arange(len(alt_pop)), size, replace=False)
+                selection = self.rng.choice(np.arange(len(alt_pop)), size, replace=False)
                 alt_pop = np.stack(alt_pop)
                 return alt_pop[selection]
         else:
-            selection = np.random.choice(np.arange(len(self.population)), size, replace=False)
+            selection = self.rng.choice(np.arange(len(self.population)), size, replace=False)
             return self.population[selection]
 
     def boundary_check(self, vector: np.ndarray) -> np.ndarray:
         '''
         Checks whether each of the dimensions of the input vector are within [0, 1].
         If not, values of those dimensions are replaced with the type of fix selected.
 
@@ -147,15 +151,15 @@
         -------
         array
         '''
         violations = np.where((vector > 1) | (vector < 0))[0]
         if len(violations) == 0:
             return vector
         if self.fix_type == 'random':
-            vector[violations] = np.random.uniform(low=0.0, high=1.0, size=len(violations))
+            vector[violations] = self.rng.uniform(low=0.0, high=1.0, size=len(violations))
         else:
             vector[violations] = np.clip(vector[violations], a_min=0, a_max=1)
         return vector
 
     def vector_to_configspace(self, vector: np.ndarray) -> ConfigSpace.Configuration:
         '''Converts numpy array to ConfigSpace object
 
@@ -239,19 +243,19 @@
 
     def run(self):
         raise NotImplementedError("The function needs to be defined in the sub class.")
 
 
 class DE(DEBase):
     def __init__(self, cs=None, f=None, dimensions=None, pop_size=20, max_age=np.inf,
-                 mutation_factor=None, crossover_prob=None, strategy='rand1_bin',
-                 encoding=False, dim_map=None, config_repository=None, **kwargs):
+                 mutation_factor=None, crossover_prob=None, strategy='rand1_bin', encoding=False,
+                 dim_map=None, seed=None, rng=None, config_repository=None, **kwargs):
         super().__init__(cs=cs, f=f, dimensions=dimensions, pop_size=pop_size, max_age=max_age,
                          mutation_factor=mutation_factor, crossover_prob=crossover_prob,
-                         strategy=strategy, config_repository=config_repository,
+                         strategy=strategy, seed=seed, rng=rng, config_repository=config_repository,
                          **kwargs)
         if self.strategy is not None:
             self.mutation_strategy = self.strategy.split('_')[0]
             self.crossover_strategy = self.strategy.split('_')[1]
         else:
             self.mutation_strategy = self.crossover_strategy = None
         self.encoding = encoding
@@ -290,15 +294,15 @@
         else:
             self._min_pop_size = 1
 
         return self._min_pop_size
 
     def map_to_original(self, vector):
         dimensions = len(self.dim_map.keys())
-        new_vector = np.random.uniform(size=dimensions)
+        new_vector = self.rng.uniform(size=dimensions)
         for i in range(dimensions):
             new_vector[i] = np.max(np.array(vector)[self.dim_map[i]])
         return new_vector
 
     def f_objective(self, x, fidelity=None, **kwargs):
         if self.f is None:
             raise NotImplementedError("An objective function needs to be passed.")
@@ -459,26 +463,26 @@
             mutant = self.mutation_currenttobest1(r1, best, r2, r3)
 
         return mutant
 
     def crossover_bin(self, target, mutant):
         '''Performs the binomial crossover of DE
         '''
-        cross_points = np.random.rand(self.dimensions) < self.crossover_prob
+        cross_points = self.rng.random(self.dimensions) < self.crossover_prob
         if not np.any(cross_points):
-            cross_points[np.random.randint(0, self.dimensions)] = True
+            cross_points[self.rng.integers(0, self.dimensions)] = True
         offspring = np.where(cross_points, mutant, target)
         return offspring
 
     def crossover_exp(self, target, mutant):
         '''Performs the exponential crossover of DE
         '''
-        n = np.random.randint(0, self.dimensions)
+        n = self.rng.integers(0, self.dimensions)
         L = 0
-        while ((np.random.rand() < self.crossover_prob) and L < self.dimensions):
+        while ((self.rng.random() < self.crossover_prob) and L < self.dimensions):
             idx = (n+L) % self.dimensions
             target[idx] = mutant[idx]
             L = L + 1
         return target
 
     def crossover(self, target, mutant):
         '''Performs DE crossover
@@ -547,15 +551,15 @@
         if population is None:
             population = self.population
         elif len(population) < 3:
             population = np.vstack((self.population, population))
 
         old_strategy = self.mutation_strategy
         self.mutation_strategy = 'rand1'
-        mutants = np.random.uniform(low=0.0, high=1.0, size=(size, self.dimensions))
+        mutants = self.rng.uniform(low=0.0, high=1.0, size=(size, self.dimensions))
         for i in range(size):
             mutant = self.mutation(current=None, best=None, alt_pop=population)
             mutants[i] = self.boundary_check(mutant)
         self.mutation_strategy = old_strategy
 
         return mutants
 
@@ -582,15 +586,15 @@
 
         return np.array(self.traj), np.array(self.runtime), np.array(self.history, dtype=object)
 
 
 class AsyncDE(DE):
     def __init__(self, cs=None, f=None, dimensions=None, pop_size=None, max_age=np.inf,
                  mutation_factor=None, crossover_prob=None, strategy='rand1_bin',
-                 async_strategy='immediate', config_repository=None, **kwargs):
+                 async_strategy='immediate', seed=None, rng=None, config_repository=None, **kwargs):
         '''Extends DE to be Asynchronous with variations
 
         Parameters
         ----------
         async_strategy : str
             'deferred' - target will be chosen sequentially from the population
                 the winner of the selection step will be included in the population only after
@@ -601,15 +605,15 @@
                 the winner of the selection step is included in the population right away
             'worst' - the worst individual will be chosen as the target
                 the winner of the selection step is included in the population right away
             {immediate, worst, random} implement Asynchronous-DE
         '''
         super().__init__(cs=cs, f=f, dimensions=dimensions, pop_size=pop_size, max_age=max_age,
                          mutation_factor=mutation_factor, crossover_prob=crossover_prob,
-                         strategy=strategy, config_repository=config_repository,
+                         strategy=strategy, seed=seed, rng=rng, config_repository=config_repository,
                          **kwargs)
         if self.strategy is not None:
             self.mutation_strategy = self.strategy.split('_')[0]
             self.crossover_strategy = self.strategy.split('_')[1]
         else:
             self.mutation_strategy = self.crossover_strategy = None
         self.async_strategy = async_strategy
@@ -633,15 +637,15 @@
         age = np.concatenate((age, new_age))
 
         return population, fitness, age
 
     def _init_mutant_population(self, pop_size, population, target=None, best=None):
         '''Generates pop_size mutants from the passed population
         '''
-        mutants = np.random.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
+        mutants = self.rng.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
         for i in range(pop_size):
             mutants[i] = self.mutation(current=target, best=best, alt_pop=population)
         return mutants
 
     def _sample_population(self, size=3, alt_pop=None, target=None):
         '''Samples 'size' individuals for mutation step
 
@@ -670,15 +674,15 @@
                     break
         if len(population) < self._min_pop_size:
             # compensate if target was part of the population and deleted earlier
             filler = self._min_pop_size - len(population)
             new_pop = self.init_population(pop_size=filler)  # chosen in a uniformly random manner
             population = np.concatenate((population, new_pop))
 
-        selection = np.random.choice(np.arange(len(population)), size, replace=False)
+        selection = self.rng.choice(np.arange(len(population)), size, replace=False)
         return population[selection]
 
     def eval_pop(self, population=None, population_ids=None, fidelity=None, **kwargs):
         pop = self.population if population is None else population
         pop_ids = self.population_ids if population_ids is None else population_ids
         pop_size = self.pop_size if population is None else len(pop)
         traj = []
@@ -749,17 +753,17 @@
 
     def sample_mutants(self, size, population=None):
         '''Samples 'size' mutants from the population
         '''
         if population is None:
             population = self.population
 
-        mutants = np.random.uniform(low=0.0, high=1.0, size=(size, self.dimensions))
+        mutants = self.rng.uniform(low=0.0, high=1.0, size=(size, self.dimensions))
         for i in range(size):
-            j = np.random.choice(np.arange(len(population)))
+            j = self.rng.choice(np.arange(len(population)))
             mutant = self.mutation(current=population[j], best=self.inc_config, alt_pop=population)
             mutants[i] = self.boundary_check(mutant)
 
         return mutants
 
     def evolve_generation(self, fidelity=None, best=None, alt_pop=None, **kwargs):
         '''Performs a complete DE evolution, mutation -> crossover -> selection
@@ -807,15 +811,15 @@
                 history.extend(de_history)
             return traj, runtime, history
 
         else:  # async_strategy == 'random' or async_strategy == 'worst':
             for count in range(self.pop_size):
                 # choosing target individual
                 if self.async_strategy == "random":
-                    i = np.random.choice(np.arange(self.pop_size))
+                    i = self.rng.choice(np.arange(self.pop_size))
                 else:  # async_strategy == 'worst'
                     i = np.argsort(-self.fitness)[0]
                 target = self.population[i]
                 mutant = self.mutation(current=target, best=best, alt_pop=alt_pop)
                 trial = self.crossover(target, mutant)
                 trial = self.boundary_check(trial)
                 trial_id = self.config_repository.announce_config(trial, float(fidelity or 0))
```

### Comparing `DEHB-0.1.0/src/dehb/optimizers/dehb.py` & `DEHB-0.1.1/src/dehb/optimizers/dehb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,48 @@
+import json
 import os
+import pickle
 import sys
-import json
 import time
-import pickle
-import numpy as np
-import ConfigSpace
-from typing import List
 from copy import deepcopy
-from loguru import logger
-from distributed import Client
+from pathlib import Path
+from typing import List
 
-from .de import DE, AsyncDE
-from ..utils import SHBracketManager
-from ..utils import ConfigRepository
+import ConfigSpace
+import numpy as np
+from distributed import Client
+from loguru import logger
 
+from ..utils import ConfigRepository, SHBracketManager
+from .de import AsyncDE
 
 logger.configure(handlers=[{"sink": sys.stdout, "level": "INFO"}])
 _logger_props = {
     "format": "{time} {level} {message}",
     "enqueue": True,
     "rotation": "500 MB"
 }
 
 
 class DEHBBase:
     def __init__(self, cs=None, f=None, dimensions=None, mutation_factor=None,
                  crossover_prob=None, strategy=None, min_fidelity=None,
-                 max_fidelity=None, eta=None, min_clip=None, max_clip=None,
+                 max_fidelity=None, eta=None, min_clip=None, max_clip=None, seed=None,
                  boundary_fix_type='random', max_age=np.inf, **kwargs):
+        # Rng
+        self.rng = np.random.default_rng(seed)
+
         # Miscellaneous
         self._setup_logger(kwargs)
         self.config_repository = ConfigRepository()
 
         # Benchmark related variables
         self.cs = cs
-        self.configspace = True if isinstance(self.cs, ConfigSpace.ConfigurationSpace) else False
-        if self.configspace:
+        self.use_configspace = True if isinstance(self.cs, ConfigSpace.ConfigurationSpace) else False
+        if self.use_configspace:
             self.dimensions = len(self.cs.get_hyperparameters())
         elif dimensions is None or not isinstance(dimensions, (int, np.integer)):
             assert "Need to specify `dimensions` as an int when `cs` is not available/specified!"
         else:
             self.dimensions = dimensions
         self.f = f
 
@@ -49,20 +52,21 @@
         self.strategy = strategy
         self.fix_type = boundary_fix_type
         self.max_age = max_age
         self.de_params = {
             "mutation_factor": self.mutation_factor,
             "crossover_prob": self.crossover_prob,
             "strategy": self.strategy,
-            "configspace": self.configspace,
+            "configspace": self.use_configspace,
             "boundary_fix_type": self.fix_type,
             "max_age": self.max_age,
             "cs": self.cs,
             "dimensions": self.dimensions,
-            "f": f
+            "rng": self.rng,
+            "f": f,
         }
 
         # Hyperband related variables
         self.min_fidelity = min_fidelity
         self.max_fidelity = max_fidelity
         if self.max_fidelity <= self.min_fidelity:
             self.logger.error("Only (Max Fidelity > Min Fidelity) is supported for DEHB.")
@@ -73,46 +77,49 @@
                     "https://automl.github.io/DEHB/references/de")
             raise AssertionError()
         self.eta = eta
         self.min_clip = min_clip
         self.max_clip = max_clip
 
         # Precomputing fidelity spacing and number of configurations for HB iterations
-        self.max_SH_iter = None
-        self.fidelities = None
-        if self.min_fidelity is not None and \
-           self.max_fidelity is not None and \
-           self.eta is not None:
-            self.max_SH_iter = -int(np.log(self.min_fidelity / self.max_fidelity) / np.log(self.eta)) + 1
-            self.fidelities = self.max_fidelity * np.power(self.eta,
-                                                     -np.linspace(start=self.max_SH_iter - 1,
-                                                                  stop=0, num=self.max_SH_iter))
+        self._pre_compute_fidelity_spacing()
 
         # Updating DE parameter list
         self.de_params.update({"output_path": self.output_path})
 
         # Global trackers
         self.population = None
         self.fitness = None
         self.inc_score = np.inf
         self.inc_config = None
         self.history = []
 
     def _setup_logger(self, kwargs):
         """Sets up the logger."""
-        self.output_path = kwargs['output_path'] if 'output_path' in kwargs else './'
-        os.makedirs(self.output_path, exist_ok=True)
+        self.output_path = Path(kwargs["output_path"]) if "output_path" in kwargs else Path("./")
+        self.output_path.mkdir(parents=True, exist_ok=True)
         self.logger = logger
         log_suffix = time.strftime("%x %X %Z")
-        log_suffix = log_suffix.replace("/", '-').replace(":", '-').replace(" ", '_')
+        log_suffix = log_suffix.replace("/", "-").replace(":", "-").replace(" ", "_")
         self.logger.add(
-            "{}/dehb_{}.log".format(self.output_path, log_suffix),
-            **_logger_props
+            f"{self.output_path}/dehb_{log_suffix}.log",
+            **_logger_props,
         )
-        self.log_filename = "{}/dehb_{}.log".format(self.output_path, log_suffix)
+        self.log_filename = f"{self.output_path}/dehb_{log_suffix}.log"
+
+    def _pre_compute_fidelity_spacing(self):
+        self.max_SH_iter = None
+        self.fidelities = None
+        if self.min_fidelity is not None and \
+           self.max_fidelity is not None and \
+           self.eta is not None:
+            self.max_SH_iter = -int(np.log(self.min_fidelity / self.max_fidelity) / np.log(self.eta)) + 1
+            self.fidelities = self.max_fidelity * np.power(self.eta,
+                                                     -np.linspace(start=self.max_SH_iter - 1,
+                                                                  stop=0, num=self.max_SH_iter))
 
     def reset(self):
         self.inc_score = np.inf
         self.inc_config = None
         self.population = None
         self.fitness = None
         self.traj = []
@@ -120,31 +127,31 @@
         self.history = []
         self.logger.info("\n\nRESET at {}\n\n".format(time.strftime("%x %X %Z")))
 
     def init_population(self):
         raise NotImplementedError("Redefine!")
 
     def get_next_iteration(self, iteration):
-        '''Computes the Successive Halving spacing
+        """Computes the Successive Halving spacing.
 
         Given the iteration index, computes the fidelity spacing to be used and
         the number of configurations to be used for the SH iterations.
 
         Parameters
         ----------
         iteration : int
             Iteration index
         clip : int, {1, 2, 3, ..., None}
             If not None, clips the minimum number of configurations to 'clip'
 
-        Returns
+        Returns:
         -------
         ns : array
         fidelities : array
-        '''
+        """
         # number of 'SH runs'
         s = self.max_SH_iter - 1 - (iteration % self.max_SH_iter)
         # fidelity spacing for this iteration
         fidelities = self.fidelities[(-s-1):]
         # number of configurations in that bracket
         n0 = int(np.floor((self.max_SH_iter)/(s+1)) * self.eta**s)
         ns = [max(int(n0*(self.eta**(-i))), 1) for i in range(s+1)]
@@ -152,46 +159,53 @@
             ns = np.clip(ns, a_min=self.min_clip, a_max=self.max_clip)
         elif self.min_clip is not None:
             ns = np.clip(ns, a_min=self.min_clip, a_max=np.max(ns))
 
         return ns, fidelities
 
     def get_incumbents(self):
-        """ Returns a tuple of the (incumbent configuration, incumbent score/fitness). """
-        if self.configspace:
+        """Returns a tuple of the (incumbent configuration, incumbent score/fitness)."""
+        if self.use_configspace:
             return self.vector_to_configspace(self.inc_config), self.inc_score
         return self.inc_config, self.inc_score
 
     def f_objective(self):
         raise NotImplementedError("The function needs to be defined in the sub class.")
 
     def run(self):
         raise NotImplementedError("The function needs to be defined in the sub class.")
 
 
 class DEHB(DEHBBase):
     def __init__(self, cs=None, f=None, dimensions=None, mutation_factor=0.5,
-                 crossover_prob=0.5, strategy='rand1_bin', min_fidelity=None,
-                 max_fidelity=None, eta=3, min_clip=None, max_clip=None, configspace=True,
-                 boundary_fix_type='random', max_age=np.inf, n_workers=None, client=None,
-                 async_strategy="immediate", **kwargs):
+                 crossover_prob=0.5, strategy="rand1_bin", min_fidelity=None,
+                 max_fidelity=None, eta=3, min_clip=None, max_clip=None, seed=None,
+                 configspace=True, boundary_fix_type="random", max_age=np.inf, n_workers=None,
+                 client=None, async_strategy="immediate", save_freq="incumbent", resume=False,
+                 **kwargs):
         super().__init__(cs=cs, f=f, dimensions=dimensions, mutation_factor=mutation_factor,
                          crossover_prob=crossover_prob, strategy=strategy, min_fidelity=min_fidelity,
-                         max_fidelity=max_fidelity, eta=eta, min_clip=min_clip, max_clip=max_clip,
-                         configspace=configspace, boundary_fix_type=boundary_fix_type,
+                         max_fidelity=max_fidelity, eta=eta, min_clip=min_clip, max_clip=max_clip, 
+                         seed=seed, configspace=configspace, boundary_fix_type=boundary_fix_type,
                          max_age=max_age, **kwargs)
         self.de_params.update({"async_strategy": async_strategy})
         self.iteration_counter = -1
         self.de = {}
         self._max_pop_size = None
         self.active_brackets = []  # list of SHBracketManager objects
         self.traj = []
         self.runtime = []
         self.history = []
+        self._ask_counter = 0
+        self._tell_counter = 0
         self.start = None
+        if save_freq not in ["incumbent", "step", "end"] and save_freq is not None:
+            self.logger.warning(f"Save frequency {save_freq} unknown. Resorting to using 'end'.")
+            save_freq = "end"
+        self.save_freq = "end" if save_freq is None else save_freq
 
         # Dask variables
         if n_workers is None and client is None:
             raise ValueError("Need to specify either 'n_workers'(>0) or 'client' (a Dask client)!")
         if client is not None and isinstance(client, Client):
             self.client = client
             self.n_workers = len(client.ncores())
@@ -211,31 +225,47 @@
         self._init_subpop()
 
         # Misc.
         self.available_gpus = None
         self.gpu_usage = None
         self.single_node_with_gpus = None
 
+        # Setup logging and potentially reload state
+        if resume:
+            self.logger.info("Loading checkpoint...")
+            success = self._load_checkpoint(self.output_path)
+            if not success:
+                self.logger.error("Checkpoint could not be loaded. " \
+                                  "Please refer to the prior warning in order to " \
+                                  "identifiy the problem.")
+                raise AttributeError("Checkpoint could not be loaded. Check the logs" \
+                                     "for more information")
+        elif (self.output_path / "dehb_state.json").exists():
+            self.logger.warning("A checkpoint already exists, " \
+                                "results could potentially be overwritten.")
+
+        # Save initial random state
+        self.random_state = self.rng.bit_generator.state
+        if self.use_configspace:
+            self.cs_random_state = self.cs.random.get_state()
+
     def __getstate__(self):
-        """ Allows the object to picklable while having Dask client as a class attribute.
-        """
+        """Allows the object to picklable while having Dask client as a class attribute."""
         d = dict(self.__dict__)
         d["client"] = None  # hack to allow Dask client to be a class attribute
         d["logger"] = None  # hack to allow logger object to be a class attribute
         return d
 
     def __del__(self):
-        """ Ensures a clean kill of the Dask client and frees up a port.
-        """
+        """Ensures a clean kill of the Dask client and frees up a port."""
         if hasattr(self, "client") and isinstance(self, Client):
             self.client.close()
 
     def _f_objective(self, job_info):
-        """ Wrapper to call DE's objective function.
-        """
+        """Wrapper to call DE's objective function."""
         # check if job_info appended during job submission self.submit_job() includes "gpu_devices"
         if "gpu_devices" in job_info and self.single_node_with_gpus:
             # should set the environment variable for the spawned worker process
             # reprioritising a CUDA device order specific to this worker process
             os.environ.update({"CUDA_VISIBLE_DEVICES": job_info["gpu_devices"]})
 
         config, config_id = job_info["config"], job_info["config_id"]
@@ -262,44 +292,44 @@
         if "gpu_devices" in job_info:
             # important for GPU usage tracking if single_node_with_gpus=True
             device_id = int(job_info["gpu_devices"].strip().split(",")[0])
             run_info.update({"device_id": device_id})
         return run_info
 
     def _create_cuda_visible_devices(self, available_gpus: List[int], start_id: int) -> str:
-        """ Generates a string to set the CUDA_VISIBLE_DEVICES environment variable.
+        """Generates a string to set the CUDA_VISIBLE_DEVICES environment variable.
 
         Given a list of available GPU device IDs and a preferred ID (start_id), the environment
         variable is created by putting the start_id device first, followed by the remaining devices
         arranged randomly. The worker that uses this string to set the environment variable uses
         the start_id GPU device primarily now.
         """
         assert start_id in available_gpus
         available_gpus = deepcopy(available_gpus)
         available_gpus.remove(start_id)
-        np.random.shuffle(available_gpus)
+        self.rng.shuffle(available_gpus)
         final_variable = [str(start_id)] + [str(_id) for _id in available_gpus]
         final_variable = ",".join(final_variable)
         return final_variable
 
     def distribute_gpus(self):
-        """ Function to create a GPU usage tracker dict.
+        """Function to create a GPU usage tracker dict.
 
         The idea is to extract the exact GPU device IDs available. During job submission, each
         submitted job is given a preference of a GPU device ID based on the GPU device with the
         least number of active running jobs. On retrieval of the result, this gpu usage dict is
         updated for the device ID that the finished job was mapped to.
         """
         try:
             available_gpus = os.environ["CUDA_VISIBLE_DEVICES"]
             available_gpus = available_gpus.strip().split(",")
             self.available_gpus = [int(_id) for _id in available_gpus]
         except KeyError as e:
             print("Unable to find valid GPU devices. "
-                  "Environment variable {} not visible!".format(str(e)))
+                  f"Environment variable {str(e)} not visible!")
             self.available_gpus = []
         self.gpu_usage = dict()
         for _id in self.available_gpus:
             self.gpu_usage[_id] = 0
 
     def vector_to_configspace(self, config):
         assert hasattr(self, "de")
@@ -323,30 +353,33 @@
         self.de = {}
         self._max_pop_size = None
         self.start = None
         self.active_brackets = []
         self.traj = []
         self.runtime = []
         self.history = []
+        self._ask_counter = 0
+        self._tell_counter = 0
+        self.config_repository.reset()
         self._get_pop_sizes()
         self._init_subpop()
         self.available_gpus = None
         self.gpu_usage = None
+        self.saving_scheduler = None
 
     def init_population(self, pop_size):
-        if self.configspace:
+        if self.use_configspace:
             population = self.cs.sample_configuration(size=pop_size)
             population = [self.configspace_to_vector(individual) for individual in population]
         else:
-            population = np.random.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
+            population = self.rng.uniform(low=0.0, high=1.0, size=(pop_size, self.dimensions))
         return population
 
     def clean_inactive_brackets(self):
-        """ Removes brackets from the active list if it is done as communicated by Bracket Manager
-        """
+        """Removes brackets from the active list if it is done as communicated by Bracket Manager."""
         if len(self.active_brackets) == 0:
             return
         self.active_brackets = [
             bracket for bracket in self.active_brackets if ~bracket.is_bracket_done()
         ]
         return
 
@@ -357,54 +390,50 @@
 
     def _update_incumbents(self, config, score, info):
         self.inc_config = config
         self.inc_score = score
         self.inc_info = info
 
     def _get_pop_sizes(self):
-        """Determines maximum pop size for each fidelity
-        """
+        """Determines maximum pop size for each fidelity."""
         self._max_pop_size = {}
         for i in range(self.max_SH_iter):
             n, r = self.get_next_iteration(i)
             for j, r_j in enumerate(r):
                 self._max_pop_size[r_j] = max(
                     n[j], self._max_pop_size[r_j]
                 ) if r_j in self._max_pop_size.keys() else n[j]
 
     def _init_subpop(self):
-        """ List of DE objects corresponding to the fidelities
-        """
+        """List of DE objects corresponding to the fidelities."""
         self.de = {}
         for i, f in enumerate(self._max_pop_size.keys()):
             self.de[f] = AsyncDE(**self.de_params, pop_size=self._max_pop_size[f],
                                  config_repository=self.config_repository)
             self.de[f].population = self.de[f].init_population(pop_size=self._max_pop_size[f])
             self.de[f].population_ids = self.config_repository.announce_population(self.de[f].population, f)
             self.de[f].fitness = np.array([np.inf] * self._max_pop_size[f])
             # adding attributes to DEHB objects to allow communication across subpopulations
             self.de[f].parent_counter = 0
             self.de[f].promotion_pop = None
             self.de[f].promotion_pop_ids = None
             self.de[f].promotion_fitness = None
 
     def _concat_pops(self, exclude_fidelity=None):
-        """ Concatenates all subpopulations
-        """
+        """Concatenates all subpopulations."""
         fidelities = list(self.fidelities)
         if exclude_fidelity is not None:
             fidelities.remove(exclude_fidelity)
         pop = []
         for fidelity in fidelities:
             pop.extend(self.de[fidelity].population.tolist())
         return np.array(pop)
 
     def _start_new_bracket(self):
-        """ Starts a new bracket based on Hyperband
-        """
+        """Starts a new bracket based on Hyperband."""
         # start new bracket
         self.iteration_counter += 1  # iteration counter gives the bracket count or bracket ID
         n_configs, fidelities = self.get_next_iteration(self.iteration_counter)
         bracket = SHBracketManager(
             n_configs=n_configs, fidelities=fidelities, bracket_id=self.iteration_counter
         )
         self.active_brackets.append(bracket)
@@ -413,30 +442,29 @@
     def _get_worker_count(self):
         if isinstance(self.client, Client):
             return len(self.client.ncores())
         else:
             return 1
 
     def is_worker_available(self, verbose=False):
-        """ Checks if at least one worker is available to run a job
-        """
+        """Checks if at least one worker is available to run a job."""
         if self.n_workers == 1 or self.client is None or not isinstance(self.client, Client):
             # in the synchronous case, one worker is always available
             return True
         # checks the absolute number of workers mapped to the client scheduler
         # client.ncores() should return a dict with the keys as unique addresses to these workers
         # treating the number of available workers in this manner
         workers = self._get_worker_count()  # len(self.client.ncores())
         if len(self.futures) >= workers:
             # pause/wait if active worker count greater allocated workers
             return False
         return True
 
     def _get_promotion_candidate(self, low_fidelity, high_fidelity, n_configs):
-        """ Manages the population to be promoted from the lower to the higher fidelity.
+        """Manages the population to be promoted from the lower to the higher fidelity.
 
         This is triggered or in action only during the first full HB bracket, which is equivalent
         to the number of brackets <= max_SH_iter.
         """
         # finding the individuals that have been evaluated (fitness < np.inf)
         evaluated_configs = np.where(self.de[low_fidelity].fitness != np.inf)[0]
         promotion_candidate_pop = self.de[low_fidelity].population[evaluated_configs]
@@ -488,24 +516,22 @@
             # in case of an edge failure case where all high fidelity individuals are same
             # just choose the best performing individual from the lower fidelity (again)
             config = self.de[low_fidelity].population[pop_idx[0]]
             config_id = self.de[low_fidelity].population_ids[pop_idx[0]]
         return config, config_id
 
     def _get_next_parent_for_subpop(self, fidelity):
-        """ Maintains a looping counter over a subpopulation, to iteratively select a parent
-        """
+        """Maintains a looping counter over a subpopulation, to iteratively select a parent."""
         parent_id = self.de[fidelity].parent_counter
         self.de[fidelity].parent_counter += 1
         self.de[fidelity].parent_counter = self.de[fidelity].parent_counter % self._max_pop_size[fidelity]
         return parent_id
 
     def _acquire_config(self, bracket, fidelity):
-        """ Generates/chooses a configuration based on the fidelity and iteration number
-        """
+        """Generates/chooses a configuration based on the fidelity and iteration number."""
         # select a parent/target
         parent_id = self._get_next_parent_for_subpop(fidelity)
         target = self.de[fidelity].population[parent_id]
         # identify lower fidelity to transfer information from
         lower_fidelity, num_configs = bracket.get_lower_fidelity_promotions(fidelity)
 
         if self.iteration_counter < self.max_SH_iter:
@@ -541,60 +567,80 @@
         config = self.de[fidelity].crossover(target=target, mutant=mutant)
         config = self.de[fidelity].boundary_check(config)
 
         # announce new config
         config_id = self.config_repository.announce_config(config, fidelity)
         return config, config_id, parent_id
 
-    def _get_next_job(self):
-        """Loads a configuration and fidelity to be evaluated next.
+    def _get_next_bracket(self, only_id=False):
+        """Used to retrieve what bracket the bracket for the next job.
+
+        Optionally, a new bracket is started, if there are no more pending jobs or
+        when all active brackets are waiting.
+
+        Args:
+            only_id (bool): Only returns the id of the next bracket
 
         Returns:
-            dict: Dicitonary containing all necessary information of the next job.
+            SHBracketmanager or int: bracket or bracket ID of next job
         """
         bracket = None
+        start_new_bracket = False
         if len(self.active_brackets) == 0 or \
                 np.all([bracket.is_bracket_done() for bracket in self.active_brackets]):
             # start new bracket when no pending jobs from existing brackets or empty bracket list
-            bracket = self._start_new_bracket()
+            start_new_bracket = True
         else:
             for _bracket in self.active_brackets:
                 # check if _bracket is not waiting for previous rung results of same bracket
                 # _bracket is not waiting on the last rung results
                 # these 2 checks allow DEHB to have a "synchronous" Successive Halving
                 if not _bracket.previous_rung_waits() and _bracket.is_pending():
                     # bracket eligible for job scheduling
                     bracket = _bracket
                     break
             if bracket is None:
                 # start new bracket when existing list has all waiting brackets
-                bracket = self._start_new_bracket()
+                start_new_bracket = True
+
+        if only_id:
+            return self.iteration_counter + 1 if start_new_bracket else bracket.bracket_id
+
+        return self._start_new_bracket() if start_new_bracket else bracket
+
+    def _get_next_job(self):
+        """Loads a configuration and fidelity to be evaluated next.
+
+        Returns:
+            dict: Dicitonary containing all necessary information of the next job.
+        """
+        bracket = self._get_next_bracket()
         # fidelity that the SH bracket allots
         fidelity = bracket.get_next_job_fidelity()
         config, config_id, parent_id = self._acquire_config(bracket, fidelity)
 
         # transform config to proper representation
-        if self.configspace:
+        if self.use_configspace:
             # converts [0, 1] vector to a ConfigSpace object
             config = self.de[fidelity].vector_to_configspace(config)
 
         # notifies the Bracket Manager that a single config is to run for the fidelity chosen
         job_info = {
             "config": config,
             "config_id": config_id,
             "fidelity": fidelity,
             "parent_id": parent_id,
             "bracket_id": bracket.bracket_id,
         }
 
         # pass information of job submission to Bracket Manager
         for bracket in self.active_brackets:
-            if bracket.bracket_id == job_info['bracket_id']:
+            if bracket.bracket_id == job_info["bracket_id"]:
                 # registering is IMPORTANT for Bracket Manager to perform SH
-                bracket.register_job(job_info['fidelity'])
+                bracket.register_job(job_info["fidelity"])
                 break
         return job_info
 
     def ask(self, n_configs: int=1):
         """Get the next configuration to run from the optimizer.
 
         The retrieved configuration can then be evaluated by the user.
@@ -603,65 +649,69 @@
 
         Args:
             n_configs (int, optional): Number of configs to ask for. Defaults to 1.
 
         Returns:
             dict or list of dict: Job info(s) of next configuration to evaluate.
         """
-        if n_configs == 1:
-            return self._get_next_job()
-
         jobs = []
-        for _ in range(n_configs):
-            jobs.append(self._get_next_job())
+        if n_configs == 1:
+            jobs = self._get_next_job()
+            self._ask_counter += 1
+        else:
+            for _ in range(n_configs):
+                jobs.append(self._get_next_job())
+                self._ask_counter += 1
+        # Save random state after ask
+        self.random_state = self.rng.bit_generator.state
+        if self.use_configspace:
+            self.cs_random_state = self.cs.random.get_state()
         return jobs
 
     def _get_gpu_id_with_low_load(self):
         candidates = []
         for k, v in self.gpu_usage.items():
             if v == min(self.gpu_usage.values()):
                 candidates.append(k)
-        device_id = np.random.choice(candidates)
+        device_id = self.rng.choice(candidates)
         # creating string for setting environment variable CUDA_VISIBLE_DEVICES
         gpu_ids = self._create_cuda_visible_devices(
-            self.available_gpus, device_id
+            self.available_gpus, device_id,
         )
         # updating GPU usage
         self.gpu_usage[device_id] += 1
-        self.logger.debug("GPU device selected: {}".format(device_id))
-        self.logger.debug("GPU device usage: {}".format(self.gpu_usage))
+        self.logger.debug(f"GPU device selected: {device_id}")
+        self.logger.debug(f"GPU device usage: {self.gpu_usage}")
         return gpu_ids
 
     def submit_job(self, job_info, **kwargs):
-        """ Asks a free worker to run the objective function on config and fidelity
-        """
+        """Asks a free worker to run the objective function on config and fidelity."""
         job_info["kwargs"] = self.shared_data if self.shared_data is not None else kwargs
         # submit to Dask client
         if self.n_workers > 1 or isinstance(self.client, Client):
             if self.single_node_with_gpus:
                 # managing GPU allocation for the job to be submitted
                 job_info.update({"gpu_devices": self._get_gpu_id_with_low_load()})
             self.futures.append(
                 self.client.submit(self._f_objective, job_info)
             )
         else:
             # skipping scheduling to Dask worker to avoid added overheads in the synchronous case
             self.futures.append(self._f_objective(job_info))
 
     def _fetch_results_from_workers(self):
-        """ Iterate over futures and collect results from finished workers
-        """
+        """Iterate over futures and collect results from finished workers."""
         if self.n_workers > 1 or isinstance(self.client, Client):
             done_list = [(i, future) for i, future in enumerate(self.futures) if future.done()]
         else:
             # Dask not invoked in the synchronous case
             done_list = [(i, future) for i, future in enumerate(self.futures)]
         if len(done_list) > 0:
             self.logger.debug(
-                "Collecting {} of the {} job(s) active.".format(len(done_list), len(self.futures))
+                f"Collecting {len(done_list)} of the {len(self.futures)} job(s) active.",
             )
         for _, future in done_list:
             if self.n_workers > 1 or isinstance(self.client, Client):
                 run_info = future.result()
                 if "device_id" in run_info:
                     # updating GPU usage
                     self.gpu_usage[run_info["device_id"]] -= 1
@@ -676,145 +726,320 @@
         self.futures = np.delete(self.futures, [i for i, _ in done_list]).tolist()
 
     def _adjust_budgets(self, fevals=None, brackets=None):
         # only update budgets if it is not the first run
         if fevals is not None and len(self.traj) > 0:
             fevals = len(self.traj) + fevals
         elif brackets is not None and self.iteration_counter > -1:
-            brackets = self.iteration_counter + brackets
+            brackets = self.iteration_counter + brackets + 1
 
         return fevals, brackets
 
+    def _get_state(self):
+        state = {}
+        # DE parameters
+        serializable_de_params = self.de_params.copy()
+        serializable_de_params.pop("cs")
+        serializable_de_params.pop("rng")
+        serializable_de_params.pop("f")
+        serializable_de_params["output_path"] = str(serializable_de_params["output_path"])
+        state["DE_params"] = serializable_de_params
+        # Hyperband variables
+        hb_dict = {}
+        hb_dict["min_fidelity"] = self.min_fidelity
+        hb_dict["max_fidelity"] = self.max_fidelity
+        hb_dict["min_clip"] = self.min_clip
+        hb_dict["max_clip"] = self.max_clip
+        hb_dict["eta"] = self.eta
+        state["HB_params"] = hb_dict
+        # Save DEHB interals
+        dehb_internals = {}
+        if self.inc_config is not None:
+            dehb_internals["inc_score"] = self.inc_score
+            dehb_internals["inc_config"] = self.inc_config.tolist()
+            dehb_internals["inc_info"] = self.inc_info
+        state["internals"] = dehb_internals
+        return state
+
+    def _save_state(self):
+        # Save ConfigRepository
+        config_repo_path = self.output_path / "config_repository.json"
+        self.config_repository.save_state(config_repo_path)
+
+        # Get state
+        state = self._get_state()
+        # Write state to disk
+        state_path = self.output_path / "dehb_state.json"
+        with state_path.open("w") as f:
+            json.dump(state, f, indent=2)
+
+        # Write random state to disk
+        rnd_state_path = self.output_path / "random_state.pkl"
+        with rnd_state_path.open("wb") as f:
+            pickle.dump(self.random_state, f)
+
+        if self.use_configspace:
+            cs_rnd_path = self.output_path / "cs_random_state.pkl"
+            with cs_rnd_path.open("wb") as f:
+                pickle.dump(self.cs_random_state, f)
+
+
     def _is_run_budget_exhausted(self, fevals=None, brackets=None, total_cost=None):
-        """ Checks if the DEHB run should be terminated or continued
-        """
+        """Checks if the DEHB run should be terminated or continued."""
         delimiters = [fevals, brackets, total_cost]
         delim_sum = sum(x is not None for x in delimiters)
         if delim_sum == 0:
             raise ValueError(
                 "Need one of 'fevals', 'brackets' or 'total_cost' as budget for DEHB to run."
             )
         if fevals is not None:
             if len(self.traj) >= fevals:
                 return True
         elif brackets is not None:
-            if self.iteration_counter >= brackets:
+            future_iteration_counter = self._get_next_bracket(only_id=True)
+            if future_iteration_counter >= brackets:
                 for bracket in self.active_brackets:
                     # waits for all brackets < iteration_counter to finish by collecting results
-                    if bracket.bracket_id < self.iteration_counter and \
+                    if bracket.bracket_id < future_iteration_counter and \
                             not bracket.is_bracket_done():
                         return False
                 return True
         else:
             if time.time() - self.start >= total_cost:
                 return True
             if len(self.runtime) > 0 and self.runtime[-1] - self.start >= total_cost:
                 return True
         return False
 
-    def _save_incumbent(self, name=None):
-        if name is None:
-            name = time.strftime("%x %X %Z", time.localtime(self.start))
-            name = name.replace("/", '-').replace(":", '-').replace(" ", '_')
+    def _save_incumbent(self):
+        # Return early if there is no incumbent yet
+        if self.inc_config is None:
+            return
         try:
-            res = dict()
-            if self.configspace:
+            res = {}
+            if self.use_configspace:
                 config = self.vector_to_configspace(self.inc_config)
                 res["config"] = config.get_dictionary()
             else:
                 res["config"] = self.inc_config.tolist()
             res["score"] = self.inc_score
             res["info"] = self.inc_info
-            with open(os.path.join(self.output_path, "incumbent_{}.json".format(name)), 'w') as f:
+            incumbent_path = self.output_path / "incumbent.json"
+            with incumbent_path.open("w") as f:
                 json.dump(res, f)
         except Exception as e:
-            self.logger.warning("Incumbent not saved: {}".format(repr(e)))
+            self.logger.warning(f"Incumbent not saved: {e!r}")
 
-    def _save_history(self, name=None):
-        if name is None:
-            name = time.strftime("%x %X %Z", time.localtime(self.start))
-            name = name.replace("/", '-').replace(":", '-').replace(" ", '_')
+    def _save_history(self):
+        # Return early if there is no history yet
+        if self.history is None:
+            return
         try:
-            with open(os.path.join(self.output_path, "history_{}.pkl".format(name)), 'wb') as f:
+            history_path = self.output_path / "history.pkl"
+            with history_path.open("wb") as f:
                 pickle.dump(self.history, f)
         except Exception as e:
-            self.logger.warning("History not saved: {}".format(repr(e)))
+            self.logger.warning(f"History not saved: {e!r}")
 
     def _verbosity_debug(self):
         for bracket in self.active_brackets:
-            self.logger.debug("Bracket ID {}:\n{}".format(
-                bracket.bracket_id,
-                str(bracket)
-            ))
+            self.logger.debug(f"Bracket ID {bracket.bracket_id}:\n{bracket!s}")
 
     def _verbosity_runtime(self, fevals, brackets, total_cost):
         if fevals is not None:
             remaining = (len(self.traj), fevals, "function evaluation(s) done")
         elif brackets is not None:
-            _suffix = "bracket(s) started; # active brackets: {}".format(len(self.active_brackets))
+            _suffix = f"bracket(s) started; # active brackets: {len(self.active_brackets)}"
             remaining = (self.iteration_counter + 1, brackets, _suffix)
         else:
             elapsed = np.format_float_positional(time.time() - self.start, precision=2)
             remaining = (elapsed, total_cost, "seconds elapsed")
         self.logger.info(
-            "{}/{} {}".format(remaining[0], remaining[1], remaining[2])
+            f"{remaining[0]}/{remaining[1]} {remaining[2]}",
         )
 
-    def tell(self, job_info: dict, result: dict):
+    def _load_checkpoint(self, run_dir: str):
+        # Check if path exists, otherwise give warning
+        run_dir = Path(run_dir)
+        if not Path.exists(run_dir):
+            self.logger.warning("Path to run directory does not exist.")
+            return False
+        # Load dehb state
+        dehb_state_path = run_dir / "dehb_state.json"
+        with dehb_state_path.open() as f:
+            dehb_state = json.load(f)
+        # Convert output_path of checkpoint to Path
+        dehb_state["DE_params"]["output_path"] = Path(dehb_state["DE_params"]["output_path"])
+        if not all(dehb_state["DE_params"][key] == self.de_params[key]
+                   for key in dehb_state["DE_params"]):
+            self.logger.warning("Initialized DE parameters do not match saved parameters.")
+            return False
+        self.de_params.update(dehb_state["DE_params"])
+
+        hb_vars = dehb_state["HB_params"]
+        if self.min_fidelity != hb_vars["min_fidelity"]:
+            self.logger.warning("Initialized min_fidelity does not match saved parameters.")
+            return False
+        self.min_fidelity = hb_vars["min_fidelity"]
+
+        if self.max_fidelity != hb_vars["max_fidelity"]:
+            self.logger.warning("Initialized max_fidelity does not match saved parameters.")
+            return False
+        self.max_fidelity = hb_vars["max_fidelity"]
+
+        if self.min_clip != hb_vars["min_clip"]:
+            self.logger.warning("Initialized min_clip does not match saved parameters.")
+            return False
+        self.min_clip = hb_vars["min_clip"]
+
+        if self.max_clip != hb_vars["max_clip"]:
+            self.logger.warning("Initialized max_clip does not match saved parameters.")
+            return False
+        self.max_clip = hb_vars["max_clip"]
+
+        if self.eta != hb_vars["eta"]:
+            self.logger.warning("Initialized eta does not match saved parameters.")
+            return False
+        self.eta = hb_vars["eta"]
+
+        self._pre_compute_fidelity_spacing()
+        self._get_pop_sizes()
+        self._init_subpop()
+        # Reset ConfigRepo after initializing DE
+        self.config_repository.reset()
+        # Load initial configurations from config repository
+        config_repo_path = run_dir / "config_repository.json"
+        with config_repo_path.open() as f:
+            config_repo_list = json.load(f)
+        # Get initial configs
+        num_initial_configs = sum(self._max_pop_size.values())
+        initial_config_entries = config_repo_list[:num_initial_configs]
+        # Filter initial configs by fidelity
+        initial_configs_by_fidelity = {fidelity: [np.array(item["config"]) for item in initial_config_entries
+                                                  if str(fidelity) in item["results"]]
+                                                  for fidelity in self.fidelities}
+        # Add initial configs to DE and announce them to ConfigRepo
+        for fidelity, sub_pop in initial_configs_by_fidelity.items():
+            self.de[fidelity].population = np.array(sub_pop)
+            self.de[fidelity].population_ids = self.config_repository.announce_population(sub_pop,
+                                                                                          fidelity)
+
+        # Load history
+        history_path = run_dir / "history.pkl"
+        with history_path.open("rb") as f:
+            history = pickle.load(f)
+
+        # Replay history
+        for config_id, config, fitness, cost, fidelity, info in history:
+            job_info = {
+                "fidelity": fidelity,
+                "config_id": config_id,
+                "config": np.array(config),
+            }
+            result = {
+                "fitness": fitness,
+                "cost": cost,
+                "info": info,
+            }
+
+            self.tell(job_info, result, replay=True)
+        # Clean inactive brackets
+        self.clean_inactive_brackets()
+
+        # Load and set random state
+        rnd_state_path = run_dir / "random_state.pkl"
+        with rnd_state_path.open("rb") as f:
+            self.rng.bit_generator.state = pickle.load(f)
+
+        if self.use_configspace:
+            cs_rnd_state_path = run_dir / "cs_random_state.pkl"
+            with cs_rnd_state_path.open("rb") as f:
+                self.cs.random.set_state(pickle.load(f))
+        return True
+
+    def save(self):
+        self.logger.info("Saving state to disk...")
+        self._save_incumbent()
+        self._save_history()
+        self._save_state()
+
+    def tell(self, job_info: dict, result: dict, replay: bool=False):
         """Feed a result back to the optimizer.
 
         In order to correctly interpret the results, the `job_info` dict, retrieved by `ask`,
         has to be given. Moreover, the `result` dict has to contain the keys `fitness` and `cost`.
         It is also possible to add the field `info` to the `result` in order to store additional,
         user-specific information.
 
         Args:
             job_info (dict): Job info returned by ask().
             result (dict): Result dictionary with mandatory keys `fitness` and `cost`.
         """
-        # update bracket information
+        if replay:
+            # Get job_info container from ask and update fields
+            job_info_container = self.ask()
+            # Update according to given history
+            job_info_container["fidelity"] = job_info["fidelity"]
+            job_info_container["config"] = job_info["config"]
+            job_info_container["config_id"] = job_info["config_id"]
+
+            # Update entry in ConfigRepository
+            self.config_repository.configs[job_info["config_id"]].config = job_info["config"]
+            # Replace job_info with container to make sure all fields are given
+            job_info = job_info_container
+
+        if self._tell_counter >= self._ask_counter:
+            raise NotImplementedError("Called tell() more often than ask(). \
+                                      Warmstarting with tell is not supported. ")
+        self._tell_counter += 1
+        # Update bracket information
         fitness, cost = result["fitness"], result["cost"]
         info = result["info"] if "info" in result else dict()
         fidelity, parent_id = job_info["fidelity"], job_info["parent_id"]
         config, config_id = job_info["config"], job_info["config_id"]
         bracket_id = job_info["bracket_id"]
         for bracket in self.active_brackets:
             if bracket.bracket_id == bracket_id:
                 # bracket job complete
                 bracket.complete_job(fidelity)  # IMPORTANT to perform synchronous SH
 
         self.config_repository.tell_result(config_id, fidelity, fitness, cost, info)
 
         # get hypercube representation from config repo
-        if self.configspace:
+        if self.use_configspace:
             config = self.config_repository.get(config_id)
 
         # carry out DE selection
         if fitness <= self.de[fidelity].fitness[parent_id]:
             self.de[fidelity].population[parent_id] = config
             self.de[fidelity].population_ids[parent_id] = config_id
             self.de[fidelity].fitness[parent_id] = fitness
         # updating incumbents
         if self.de[fidelity].fitness[parent_id] < self.inc_score:
             self._update_incumbents(
                 config=self.de[fidelity].population[parent_id],
                 score=self.de[fidelity].fitness[parent_id],
-                info=info
+                info=info,
             )
+            if self.save_freq == "incumbent" and not replay:
+                self.save()
         # book-keeping
         self._update_trackers(
             traj=self.inc_score, runtime=cost, history=(
-                config.tolist(), float(fitness), float(cost), float(fidelity), info
-            )
+                config_id, config.tolist(), float(fitness), float(cost), float(fidelity), info,
+            ),
         )
 
+        if self.save_freq == "step" and not replay:
+            self.save()
+
     @logger.catch
     def run(self, fevals=None, brackets=None, total_cost=None, single_node_with_gpus=False,
-            verbose=False, debug=False, save_intermediate=True, save_history=True, name=None, **kwargs):
-        """ Main interface to run optimization by DEHB
+            verbose=False, debug=False, **kwargs):
+        """Main interface to run optimization by DEHB.
 
         This function waits on workers and if a worker is free, asks for a configuration and a
         fidelity to evaluate on and submits it to the worker. In each loop, it checks if a job
         is complete, fetches the results, carries the necessary processing of it asynchronously
         to the worker computations.
 
         The duration of the DEHB run can be controlled by specifying one of 3 parameters. If more
@@ -842,85 +1067,79 @@
         if self.single_node_with_gpus:
             self.distribute_gpus()
 
         self.start = self.start = time.time()
         fevals, brackets = self._adjust_budgets(fevals, brackets)
         if verbose:
             print("\nLogging at {} for optimization starting at {}\n".format(
-                os.path.join(os.getcwd(), self.log_filename),
-                time.strftime("%x %X %Z", time.localtime(self.start))
+                Path.cwd() / self.log_filename,
+                time.strftime("%x %X %Z", time.localtime(self.start)),
             ))
         if debug:
             logger.configure(handlers=[{"sink": sys.stdout}])
         while True:
             if self._is_run_budget_exhausted(fevals, brackets, total_cost):
                 break
             if self.is_worker_available():
-                job_info = self.ask()
-                if brackets is not None and job_info["bracket_id"] >= brackets:
+                next_bracket_id = self._get_next_bracket(only_id=True)
+                if brackets is not None and next_bracket_id >= brackets:
                     # ignore submission and only collect results
                     # when brackets are chosen as run budget, an extra bracket is created
                     # since iteration_counter is incremented in ask() and then checked
                     # in _is_run_budget_exhausted(), therefore, need to skip suggestions
                     # coming from the extra allocated bracket
                     # _is_run_budget_exhausted() will not return True until all the lower brackets
                     # have finished computation and returned its results
                     pass
                 else:
                     if self.n_workers > 1 or isinstance(self.client, Client):
                         self.logger.debug("{}/{} worker(s) available.".format(
-                            self._get_worker_count() - len(self.futures), self._get_worker_count()
+                            self._get_worker_count() - len(self.futures), self._get_worker_count(),
                         ))
-                    # submits job_info to a worker for execution
+                    # Ask for new job_info
+                    job_info = self.ask()
+                    # Submit job_info to a worker for execution
                     self.submit_job(job_info, **kwargs)
                     if verbose:
                         fidelity = job_info["fidelity"]
                         config_id = job_info["config_id"]
                         self._verbosity_runtime(fevals, brackets, total_cost)
                         self.logger.info(
                             "Evaluating configuration {} with fidelity {} under "
-                            "bracket ID {}".format(config_id, fidelity, job_info["bracket_id"])
+                            "bracket ID {}".format(config_id, fidelity, job_info["bracket_id"]),
                         )
                         self.logger.info(
-                            "Best score seen/Incumbent score: {}".format(self.inc_score)
+                            f"Best score seen/Incumbent score: {self.inc_score}",
                         )
                     self._verbosity_debug()
             self._fetch_results_from_workers()
-            if save_intermediate and self.inc_config is not None:
-                self._save_incumbent(name)
-            if save_history and self.history is not None:
-                self._save_history(name)
             self.clean_inactive_brackets()
         # end of while
 
         if verbose and len(self.futures) > 0:
             self.logger.info(
                 "DEHB optimisation over! Waiting to collect results from workers running..."
             )
         while len(self.futures) > 0:
             self._fetch_results_from_workers()
-            if save_intermediate and self.inc_config is not None:
-                self._save_incumbent(name)
-            if save_history and self.history is not None:
-                self._save_history(name)
             time.sleep(0.05)  # waiting 50ms
 
         if verbose:
             time_taken = time.time() - self.start
             self.logger.info("End of optimisation! Total duration: {}; Total fevals: {}\n".format(
-                time_taken, len(self.traj)
+                time_taken, len(self.traj),
             ))
-            self.logger.info("Incumbent score: {}".format(self.inc_score))
+            self.logger.info(f"Incumbent score: {self.inc_score}")
             self.logger.info("Incumbent config: ")
-            if self.configspace:
+            if self.use_configspace:
                 config = self.vector_to_configspace(self.inc_config)
                 for k, v in config.get_dictionary().items():
-                    self.logger.info("{}: {}".format(k, v))
+                    self.logger.info(f"{k}: {v}")
             else:
-                self.logger.info("{}".format(self.inc_config))
-        self._save_incumbent(name)
-        self._save_history(name)
+                self.logger.info(f"{self.inc_config}")
+        self.save()
         # reset waiting jobs of active bracket to allow for continuation
+        self.active_brackets = []
         if len(self.active_brackets) > 0:
             for active_bracket in self.active_brackets:
                 active_bracket.reset_waiting_jobs()
         return np.array(self.traj), np.array(self.runtime), np.array(self.history, dtype=object)
```

### Comparing `DEHB-0.1.0/src/dehb/utils/bracket_manager.py` & `DEHB-0.1.1/src/dehb/utils/bracket_manager.py`

 * *Files identical despite different names*

### Comparing `DEHB-0.1.0/src/dehb/utils/config_repository.py` & `DEHB-0.1.1/src/dehb/utils/config_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+import json
+from dataclasses import asdict, dataclass
+from pathlib import Path
 from typing import Any
 
 import numpy as np
 
 
 @dataclass
 class ConfigItem:
@@ -57,15 +59,15 @@
             int: ID of configuration
         """
         config_id = len(self.configs)
         fidelity = float(fidelity or 0)
         result_dict = {
                 fidelity: ResultItem(np.inf, -1, {}),
             }
-        config_item = ConfigItem(config_id, config, result_dict)
+        config_item = ConfigItem(config_id, config.copy(), result_dict)
         self.configs.append(config_item)
         return config_id
 
     def announce_population(self, population: np.ndarray, fidelity=None) -> np.ndarray:
         """Announce population, retrieving ids for the population.
 
         Args:
@@ -136,8 +138,22 @@
         Returns:
             np.ndarray: Config in hypercube representation
         """
         try:
             config_item = self.configs[config_id]
         except IndexError as e:
             raise IndexError("Config with the given ID can not be found.") from e
-        return config_item.config
+        return config_item.config
+
+    def save_state(self, save_path: Path):
+        """Saves the current state to `save_path`.
+
+        Args:
+            save_path (Path): Path where the state should be saved to.
+        """
+        with save_path.open("w") as f:
+            serialized_data = []
+            for config in self.configs:
+                serialized_config = asdict(config)
+                serialized_config["config"] = serialized_config["config"].tolist()
+                serialized_data.append(serialized_config)
+            json.dump(serialized_data, f, indent=2)
```

