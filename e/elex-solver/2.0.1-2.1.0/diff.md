# Comparing `tmp/elex-solver-2.0.1.tar.gz` & `tmp/elex-solver-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elex-solver-2.0.1.tar", last modified: Fri Oct 20 17:34:25 2023, max compression
+gzip compressed data, was "elex-solver-2.1.0.tar", last modified: Fri Mar 29 20:31:55 2024, max compression
```

## Comparing `elex-solver-2.0.1.tar` & `elex-solver-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2023-10-20 17:34:25.545369 elex-solver-2.0.1/
--rw-r--r--   0 napolitanod   (503) staff       (20)     2140 2023-10-20 17:34:25.545292 elex-solver-2.0.1/PKG-INFO
--rw-r--r--   0 napolitanod   (503) staff       (20)     1718 2023-10-06 18:36:01.000000 elex-solver-2.0.1/README.md
--rw-r--r--   0 napolitanod   (503) staff       (20)      104 2023-10-20 17:34:25.545613 elex-solver-2.0.1/setup.cfg
--rw-r--r--   0 napolitanod   (503) staff       (20)     1448 2023-10-20 17:31:49.000000 elex-solver-2.0.1/setup.py
-drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2023-10-20 17:34:25.541508 elex-solver-2.0.1/src/
-drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2023-10-20 17:34:25.543256 elex-solver-2.0.1/src/elex_solver.egg-info/
--rw-r--r--   0 napolitanod   (503) staff       (20)     2140 2023-10-20 17:34:25.000000 elex-solver-2.0.1/src/elex_solver.egg-info/PKG-INFO
--rw-r--r--   0 napolitanod   (503) staff       (20)      535 2023-10-20 17:34:25.000000 elex-solver-2.0.1/src/elex_solver.egg-info/SOURCES.txt
--rw-r--r--   0 napolitanod   (503) staff       (20)        1 2023-10-20 17:34:25.000000 elex-solver-2.0.1/src/elex_solver.egg-info/dependency_links.txt
--rw-r--r--   0 napolitanod   (503) staff       (20)        1 2023-10-18 20:59:26.000000 elex-solver-2.0.1/src/elex_solver.egg-info/not-zip-safe
--rw-r--r--   0 napolitanod   (503) staff       (20)       35 2023-10-20 17:34:25.000000 elex-solver-2.0.1/src/elex_solver.egg-info/requires.txt
--rw-r--r--   0 napolitanod   (503) staff       (20)       11 2023-10-20 17:34:25.000000 elex-solver-2.0.1/src/elex_solver.egg-info/top_level.txt
-drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2023-10-20 17:34:25.544483 elex-solver-2.0.1/src/elexsolver/
--rw-r--r--   0 napolitanod   (503) staff       (20)     2359 2023-10-06 18:36:01.000000 elex-solver-2.0.1/src/elexsolver/LinearSolver.py
--rw-r--r--   0 napolitanod   (503) staff       (20)     5354 2023-10-06 18:36:01.000000 elex-solver-2.0.1/src/elexsolver/OLSRegressionSolver.py
--rw-r--r--   0 napolitanod   (503) staff       (20)     4693 2023-10-06 18:36:01.000000 elex-solver-2.0.1/src/elexsolver/QuantileRegressionSolver.py
--rw-r--r--   0 napolitanod   (503) staff       (20)      935 2023-10-20 17:31:44.000000 elex-solver-2.0.1/src/elexsolver/TransitionMatrixSolver.py
--rw-r--r--   0 napolitanod   (503) staff       (20)        0 2023-10-06 18:36:01.000000 elex-solver-2.0.1/src/elexsolver/__init__.py
--rw-r--r--   0 napolitanod   (503) staff       (20)      920 2023-10-06 18:36:01.000000 elex-solver-2.0.1/src/elexsolver/logging.py
-drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2023-10-20 17:34:25.545004 elex-solver-2.0.1/tests/
--rw-r--r--   0 napolitanod   (503) staff       (20)      233 2023-10-06 18:36:01.000000 elex-solver-2.0.1/tests/test_linear_solver.py
--rw-r--r--   0 napolitanod   (503) staff       (20)     9540 2023-10-06 18:36:01.000000 elex-solver-2.0.1/tests/test_ols.py
--rw-r--r--   0 napolitanod   (503) staff       (20)    10446 2023-10-06 18:36:01.000000 elex-solver-2.0.1/tests/test_quantile.py
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.138951 elex-solver-2.1.0/
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.129886 elex-solver-2.1.0/.github/
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1303 2023-10-06 18:36:01.000000 elex-solver-2.1.0/.github/CODEOWNERS
+-rw-r--r--   0 napolitanod   (503) staff       (20)       45 2023-10-06 18:36:01.000000 elex-solver-2.1.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.130193 elex-solver-2.1.0/.github/workflows/
+-rw-r--r--   0 napolitanod   (503) staff       (20)      276 2023-10-06 18:36:01.000000 elex-solver-2.1.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 napolitanod   (503) staff       (20)      610 2024-03-29 20:00:16.000000 elex-solver-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 napolitanod   (503) staff       (20)      149 2023-10-06 18:36:01.000000 elex-solver-2.1.0/.gitignore
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1068 2023-10-06 18:36:01.000000 elex-solver-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1551 2024-03-29 20:31:25.000000 elex-solver-2.1.0/CHANGELOG.md
+-rw-r--r--   0 napolitanod   (503) staff       (20)     2137 2024-03-29 20:31:55.138834 elex-solver-2.1.0/PKG-INFO
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1715 2024-03-29 20:00:16.000000 elex-solver-2.1.0/README.md
+-rw-r--r--   0 napolitanod   (503) staff       (20)       26 2023-10-06 18:36:01.000000 elex-solver-2.1.0/pytest.ini
+-rw-r--r--   0 napolitanod   (503) staff       (20)       92 2023-10-20 17:37:11.000000 elex-solver-2.1.0/requirements-dev.txt
+-rw-r--r--   0 napolitanod   (503) staff       (20)        4 2023-10-06 18:36:01.000000 elex-solver-2.1.0/requirements.txt
+-rw-r--r--   0 napolitanod   (503) staff       (20)      296 2024-03-29 20:31:55.139311 elex-solver-2.1.0/setup.cfg
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1448 2024-03-29 20:31:22.000000 elex-solver-2.1.0/setup.py
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.127860 elex-solver-2.1.0/src/
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.138325 elex-solver-2.1.0/src/elex_solver.egg-info/
+-rw-r--r--   0 napolitanod   (503) staff       (20)     2137 2024-03-29 20:31:55.000000 elex-solver-2.1.0/src/elex_solver.egg-info/PKG-INFO
+-rw-r--r--   0 napolitanod   (503) staff       (20)      974 2024-03-29 20:31:55.000000 elex-solver-2.1.0/src/elex_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 napolitanod   (503) staff       (20)        1 2024-03-29 20:31:55.000000 elex-solver-2.1.0/src/elex_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 napolitanod   (503) staff       (20)        1 2023-10-18 20:59:26.000000 elex-solver-2.1.0/src/elex_solver.egg-info/not-zip-safe
+-rw-r--r--   0 napolitanod   (503) staff       (20)       35 2024-03-29 20:31:55.000000 elex-solver-2.1.0/src/elex_solver.egg-info/requires.txt
+-rw-r--r--   0 napolitanod   (503) staff       (20)       11 2024-03-29 20:31:55.000000 elex-solver-2.1.0/src/elex_solver.egg-info/top_level.txt
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.132141 elex-solver-2.1.0/src/elexsolver/
+-rw-r--r--   0 napolitanod   (503) staff       (20)     2359 2023-10-06 18:36:01.000000 elex-solver-2.1.0/src/elexsolver/LinearSolver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     5354 2023-10-06 18:36:01.000000 elex-solver-2.1.0/src/elexsolver/OLSRegressionSolver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     4693 2023-10-06 18:36:01.000000 elex-solver-2.1.0/src/elexsolver/QuantileRegressionSolver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     3303 2024-03-29 20:00:16.000000 elex-solver-2.1.0/src/elexsolver/TransitionMatrixSolver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     3854 2024-03-29 20:00:16.000000 elex-solver-2.1.0/src/elexsolver/TransitionSolver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)        0 2023-10-06 18:36:01.000000 elex-solver-2.1.0/src/elexsolver/__init__.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)      920 2023-10-06 18:36:01.000000 elex-solver-2.1.0/src/elexsolver/logging.py
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.133226 elex-solver-2.1.0/tests/
+-rw-r--r--   0 napolitanod   (503) staff       (20)     1126 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/conftest.py
+drwxr-xr-x   0 napolitanod   (503) staff       (20)        0 2024-03-29 20:31:55.133578 elex-solver-2.1.0/tests/fixtures/
+-rw-r--r--   0 napolitanod   (503) staff       (20)     5606 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/fixtures/random_data_n100_p5_12549_weights.csv
+-rw-r--r--   0 napolitanod   (503) staff       (20)    11504 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/fixtures/random_data_n100_p5_17554.csv
+-rw-r--r--   0 napolitanod   (503) staff       (20)      233 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/test_linear_solver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     9540 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/test_ols.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)    10446 2023-10-06 18:36:01.000000 elex-solver-2.1.0/tests/test_quantile.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     7542 2024-03-29 20:00:16.000000 elex-solver-2.1.0/tests/test_transition_matrix_solver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)     4319 2024-03-29 20:00:16.000000 elex-solver-2.1.0/tests/test_transition_solver.py
+-rw-r--r--   0 napolitanod   (503) staff       (20)      296 2024-01-23 20:15:13.000000 elex-solver-2.1.0/tox.ini
```

### Comparing `elex-solver-2.0.1/PKG-INFO` & `elex-solver-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: elex-solver
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package for optimization solvers
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cvxpy~=1.4
 Requires-Dist: numpy~=1.26
-Requires-Dist: scipy~=1.11
+Requires-Dist: scipy~=1.12
 
 # elex-solver
 
 This packages includes solvers for:
 * Ordinary least squares regression
 * Quantile regression
 * Transition matrices
@@ -26,16 +26,16 @@
 
 ## Ordinary least squares
 We have our own implementation of ordinary least squares in Python because this let us optimize it towards the bootstrap by storing and re-using the normal equations. This allows for significant speed up.
 
 ## Quantile Regression
 Since we did not find any implementations of quantile regression in Python that fit our needs, we decided to write one ourselves. At the moment this uses two libraries, the version that solves the non-regularized problem uses `numpy`and solves the dual based on [this](https://arxiv.org/pdf/2305.12616.pdf) paper. The version that solves the regularized problem uses [`cvxpy`](https://www.cvxpy.org/#) and sets up the problem as a normal optimization problem. Eventually, we are planning on replacing the regularized version with the dual also.
 
-## Transition matrices
-We also have a solver for transition matrices. While this works arbitrarily, we have used this in the past for our primary election night model. We can still use this to create the sankey diagram coefficients.
+## Transition Matrices
+We also have a matrix regression solver built with `cvxpy`.  We've used this for our primary election model and analysis.  The transitions it generates form the transitions displayed in our sankey diagrams.
 
 ## Development
 We welcome contributions to this repo. Please open a Github issue for any issues or comments you have.
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
```

### Comparing `elex-solver-2.0.1/README.md` & `elex-solver-2.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 ## Ordinary least squares
 We have our own implementation of ordinary least squares in Python because this let us optimize it towards the bootstrap by storing and re-using the normal equations. This allows for significant speed up.
 
 ## Quantile Regression
 Since we did not find any implementations of quantile regression in Python that fit our needs, we decided to write one ourselves. At the moment this uses two libraries, the version that solves the non-regularized problem uses `numpy`and solves the dual based on [this](https://arxiv.org/pdf/2305.12616.pdf) paper. The version that solves the regularized problem uses [`cvxpy`](https://www.cvxpy.org/#) and sets up the problem as a normal optimization problem. Eventually, we are planning on replacing the regularized version with the dual also.
 
-## Transition matrices
-We also have a solver for transition matrices. While this works arbitrarily, we have used this in the past for our primary election night model. We can still use this to create the sankey diagram coefficients.
+## Transition Matrices
+We also have a matrix regression solver built with `cvxpy`.  We've used this for our primary election model and analysis.  The transitions it generates form the transitions displayed in our sankey diagrams.
 
 ## Development
 We welcome contributions to this repo. Please open a Github issue for any issues or comments you have.
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
```

### Comparing `elex-solver-2.0.1/setup.py` & `elex-solver-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 from codecs import open
 
 from setuptools import find_packages, setup
 
-INSTALL_REQUIRES = ["cvxpy~=1.4", "numpy~=1.26", "scipy~=1.11"]
+INSTALL_REQUIRES = ["cvxpy~=1.4", "numpy~=1.26", "scipy~=1.12"]
 
 THIS_FILE_DIR = os.path.dirname(__file__)
 
 LONG_DESCRIPTION = ""
 # Get the long description from the README file
 with open(os.path.join(THIS_FILE_DIR, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # The full version, including alpha/beta/rc tags
-RELEASE = "2.0.1"
+RELEASE = "2.1.0"
 # The short X.Y version
 VERSION = ".".join(RELEASE.split(".")[:2])
 
 PROJECT = "elex-solver"
 AUTHOR = "The Wapo Newsroom Engineering Team"
-COPYRIGHT = "2023, {}".format(AUTHOR)
+COPYRIGHT = "2024, {}".format(AUTHOR)
 
 
 setup(
     name=PROJECT,
     version=RELEASE,
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     description="A package for optimization solvers",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages("src", exclude=["docs", "tests"]),
     package_dir={"": "src"},
```

### Comparing `elex-solver-2.0.1/src/elex_solver.egg-info/PKG-INFO` & `elex-solver-2.1.0/src/elex_solver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: elex-solver
-Version: 2.0.1
+Version: 2.1.0
 Summary: A package for optimization solvers
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cvxpy~=1.4
 Requires-Dist: numpy~=1.26
-Requires-Dist: scipy~=1.11
+Requires-Dist: scipy~=1.12
 
 # elex-solver
 
 This packages includes solvers for:
 * Ordinary least squares regression
 * Quantile regression
 * Transition matrices
@@ -26,16 +26,16 @@
 
 ## Ordinary least squares
 We have our own implementation of ordinary least squares in Python because this let us optimize it towards the bootstrap by storing and re-using the normal equations. This allows for significant speed up.
 
 ## Quantile Regression
 Since we did not find any implementations of quantile regression in Python that fit our needs, we decided to write one ourselves. At the moment this uses two libraries, the version that solves the non-regularized problem uses `numpy`and solves the dual based on [this](https://arxiv.org/pdf/2305.12616.pdf) paper. The version that solves the regularized problem uses [`cvxpy`](https://www.cvxpy.org/#) and sets up the problem as a normal optimization problem. Eventually, we are planning on replacing the regularized version with the dual also.
 
-## Transition matrices
-We also have a solver for transition matrices. While this works arbitrarily, we have used this in the past for our primary election night model. We can still use this to create the sankey diagram coefficients.
+## Transition Matrices
+We also have a matrix regression solver built with `cvxpy`.  We've used this for our primary election model and analysis.  The transitions it generates form the transitions displayed in our sankey diagrams.
 
 ## Development
 We welcome contributions to this repo. Please open a Github issue for any issues or comments you have.
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
```

### Comparing `elex-solver-2.0.1/src/elexsolver/LinearSolver.py` & `elex-solver-2.1.0/src/elexsolver/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `elex-solver-2.0.1/src/elexsolver/OLSRegressionSolver.py` & `elex-solver-2.1.0/src/elexsolver/OLSRegressionSolver.py`

 * *Files identical despite different names*

### Comparing `elex-solver-2.0.1/src/elexsolver/QuantileRegressionSolver.py` & `elex-solver-2.1.0/src/elexsolver/QuantileRegressionSolver.py`

 * *Files identical despite different names*

### Comparing `elex-solver-2.0.1/src/elexsolver/logging.py` & `elex-solver-2.1.0/src/elexsolver/logging.py`

 * *Files identical despite different names*

### Comparing `elex-solver-2.0.1/tests/test_ols.py` & `elex-solver-2.1.0/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `elex-solver-2.0.1/tests/test_quantile.py` & `elex-solver-2.1.0/tests/test_quantile.py`

 * *Files identical despite different names*

