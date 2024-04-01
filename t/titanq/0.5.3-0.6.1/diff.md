# Comparing `tmp/titanq-0.5.3.tar.gz` & `tmp/titanq-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.5.3.tar", last modified: Tue Mar 12 14:42:55 2024, max compression
+gzip compressed data, was "titanq-0.6.1.tar", last modified: Mon Apr  1 12:55:56 2024, max compression
```

## Comparing `titanq-0.5.3.tar` & `titanq-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.288395 titanq-0.5.3/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      549 2024-02-14 15:46:31.000000 titanq-0.5.3/LICENSE.txt
--rw-r--r--   0 hubert    (1000) hubert    (1000)     5697 2024-03-12 14:42:55.288395 titanq-0.5.3/PKG-INFO
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     4725 2024-03-12 14:37:24.000000 titanq-0.5.3/README.md
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     1179 2024-03-12 14:42:21.000000 titanq-0.5.3/pyproject.toml
--rw-rw-r--   0 hubert    (1000) hubert    (1000)       61 2024-03-12 14:37:24.000000 titanq-0.5.3/requirements.txt
--rw-rw-r--   0 hubert    (1000) hubert    (1000)       38 2024-03-12 14:42:55.288395 titanq-0.5.3/setup.cfg
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.284395 titanq-0.5.3/tests/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     6098 2024-02-28 20:26:10.000000 titanq-0.5.3/tests/test_client.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)    11525 2024-02-28 20:26:10.000000 titanq-0.5.3/tests/test_model.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      730 2024-02-24 14:38:26.000000 titanq-0.5.3/tests/test_optimize_response.py
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.284395 titanq-0.5.3/titanq/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      757 2024-03-12 13:00:59.000000 titanq-0.5.3/titanq/__init__.py
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.284395 titanq-0.5.3/titanq/_client/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      117 2024-01-31 16:09:04.000000 titanq-0.5.3/titanq/_client/__init__.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     3771 2024-03-12 13:00:59.000000 titanq-0.5.3/titanq/_client/client.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     3380 2024-02-28 20:26:10.000000 titanq-0.5.3/titanq/_client/model.py
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.288395 titanq-0.5.3/titanq/_model/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      151 2023-12-20 14:40:12.000000 titanq-0.5.3/titanq/_model/__init__.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     2072 2024-02-28 20:26:10.000000 titanq-0.5.3/titanq/_model/constraints.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      775 2024-03-05 15:31:12.000000 titanq-0.5.3/titanq/_model/errors.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)    12058 2024-03-12 14:37:24.000000 titanq-0.5.3/titanq/_model/model.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     1986 2023-12-20 14:40:12.000000 titanq-0.5.3/titanq/_model/objective.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     3942 2024-03-12 13:00:59.000000 titanq-0.5.3/titanq/_model/optimize_response.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      871 2024-02-16 15:44:09.000000 titanq-0.5.3/titanq/_model/variable.py
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.288395 titanq-0.5.3/titanq/_storage/
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      119 2024-01-31 16:09:04.000000 titanq-0.5.3/titanq/_storage/__init__.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     3813 2024-03-12 14:37:24.000000 titanq-0.5.3/titanq/_storage/managed_storage.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     5682 2024-02-28 20:26:10.000000 titanq-0.5.3/titanq/_storage/s3_storage.py
--rw-rw-r--   0 hubert    (1000) hubert    (1000)     3746 2024-02-28 20:26:10.000000 titanq-0.5.3/titanq/_storage/storage_client.py
-drwxrwxr-x   0 hubert    (1000) hubert    (1000)        0 2024-03-12 14:42:55.288395 titanq-0.5.3/titanq.egg-info/
--rw-r--r--   0 hubert    (1000) hubert    (1000)     5697 2024-03-12 14:42:55.000000 titanq-0.5.3/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 hubert    (1000) hubert    (1000)      687 2024-03-12 14:42:55.000000 titanq-0.5.3/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 hubert    (1000) hubert    (1000)        1 2024-03-12 14:42:55.000000 titanq-0.5.3/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 hubert    (1000) hubert    (1000)       62 2024-03-12 14:42:55.000000 titanq-0.5.3/titanq.egg-info/requires.txt
--rw-rw-r--   0 hubert    (1000) hubert    (1000)        7 2024-03-12 14:42:55.000000 titanq-0.5.3/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-03-15 13:28:09.000000 titanq-0.6.1/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-01 12:55:56.798160 titanq-0.6.1/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-03-26 16:14:37.000000 titanq-0.6.1/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-01 12:53:14.000000 titanq-0.6.1/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-03-26 16:14:37.000000 titanq-0.6.1/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-01 12:55:56.798160 titanq-0.6.1/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6098 2024-03-15 13:45:14.000000 titanq-0.6.1/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    16855 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1492 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      736 2024-03-26 16:14:37.000000 titanq-0.6.1/tests/test_optimize_response.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      117 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3380 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     8880 2024-03-28 20:55:17.000000 titanq-0.6.1/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      985 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    18311 2024-03-28 18:48:10.000000 titanq-0.6.1/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      993 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3942 2024-03-22 12:53:12.000000 titanq-0.6.1/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      871 2024-03-25 14:26:36.000000 titanq-0.6.1/titanq/_model/variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-03-07 17:48:15.000000 titanq-0.6.1/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3813 2024-03-26 16:14:37.000000 titanq-0.6.1/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5682 2024-03-15 13:45:14.000000 titanq-0.6.1/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3746 2024-03-22 14:53:41.000000 titanq-0.6.1/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-01 12:55:56.798160 titanq-0.6.1/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      740 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-01 12:55:56.000000 titanq-0.6.1/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.5.3/LICENSE.txt` & `titanq-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/PKG-INFO` & `titanq-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.5.3
+Version: 0.6.1
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
+Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +25,15 @@
 Requires-Dist: pydantic>=2.5.3
 
 # The TitanQ SDK for Python
 
 ![Python](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue) ![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
 
 TitanQ is the InfinityQ Software Development Kit (SDK) for Python. The SDK facilitates and opens the way for faster implementation
-of the TitanQ solver without having to deal directly with the API.
+of the TitanQ solver without having to deal directly with the [TitanQ API](https://docs.titanq.infinityq.io).
 
 This TitanQ package is maintained and published by [InfinityQ](https://www.infinityq.tech/)
 
 
 ## API Key
 
 In order to use the TitanQ service, a user needs an API key.
@@ -91,11 +92,21 @@
 
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
+
+Additional parameters are avialble to tune the problem:
+- beta
+- coupling_mult
+- num_chains
+- num_engines
+
+For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
+
+
 ## Getting support or help
 
 
-Further help can be obtained by contacting [InfinityQ support](support@infinityq.tech)
+Further help can be obtained by contacting [InfinityQ support](mailto:support@infinityq.tech)
```

### Comparing `titanq-0.5.3/README.md` & `titanq-0.6.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # The TitanQ SDK for Python
 
 ![Python](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue) ![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
 
 TitanQ is the InfinityQ Software Development Kit (SDK) for Python. The SDK facilitates and opens the way for faster implementation
-of the TitanQ solver without having to deal directly with the API.
+of the TitanQ solver without having to deal directly with the [TitanQ API](https://docs.titanq.infinityq.io).
 
 This TitanQ package is maintained and published by [InfinityQ](https://www.infinityq.tech/)
 
 
 ## API Key
 
 In order to use the TitanQ service, a user needs an API key.
@@ -66,11 +66,21 @@
 
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
+
+Additional parameters are avialble to tune the problem:
+- beta
+- coupling_mult
+- num_chains
+- num_engines
+
+For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
+
+
 ## Getting support or help
 
 
-Further help can be obtained by contacting [InfinityQ support](support@infinityq.tech)
+Further help can be obtained by contacting [InfinityQ support](mailto:support@infinityq.tech)
```

### Comparing `titanq-0.5.3/pyproject.toml` & `titanq-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.5.3"
+version = "0.6.1"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
@@ -27,13 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 Homepage = "https://www.infinityq.tech"
 Documentation = "https://docs.titanq.infinityq.io/quickstart/category/python-sdk"
+Examples = "https://github.com/infinityq-tech/titanq-examples"
+
 #Repository = "https://example.com"
 #Issues = "https://example.com"
 #Changelog = "https://example.com"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `titanq-0.5.3/tests/test_client.py` & `titanq-0.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/tests/test_model.py` & `titanq-0.6.1/tests/test_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 from titanq import Model, Vtype, errors, Target
 from titanq._storage.s3_storage import S3Storage
 from titanq._storage.managed_storage import ManagedStorage
 from titanq._client.model import SolveResponse
 
 from .mock import TitanQClientMock, MockS3StorageClient
 
-from collections import namedtuple
-
 
 def file_in_filename_list(filename: str, filename_list: List[str]) -> bool:
     return any(filename in s for s in filename_list)
 
 def np_array_to_bytes(arr: np.ndarray) -> bytes:
     buf = io.BytesIO()
     np.save(buf, arr)
     return buf.getvalue()
 
 @pytest.fixture
 def mock_metrics() -> Dict[str, Any]:
-    return {"metrics1": 1, "metrics2": "value2"}
+    return {
+        "computation_metrics": {
+            "metrics1": 1,
+            "metrics2": "value2"
+        }
+    }
 
 @pytest.fixture
 def mock_result() -> Dict[str, Any]:
     return [np.random.rand(10).astype(np.float32) for _ in range(10)]
 
 @pytest.fixture
 def mock_s3_storage(mock_metrics, mock_result) -> MockS3StorageClient:
@@ -195,65 +198,49 @@
     weights = np.random.rand(10, 10).astype(np.float32)
     bias = np.random.rand(10).astype(np.float32)
 
     model.add_variable_vector('x', 10, Vtype.BINARY)
     model.set_objective_matrices(weights, bias)
     response = model.optimize()
 
-    assert response.metrics() == mock_metrics
+    assert response.computation_metrics() == mock_metrics["computation_metrics"]
     assert (response.result_vector() == mock_result).all()
 
     assert mock_s3_storage.array_uploaded['bias'] == np_array_to_bytes(bias)
     assert mock_s3_storage.array_uploaded['weights'] == np_array_to_bytes(weights)
     assert mock_s3_storage.array_uploaded['constraint_weights'] == None
     assert mock_s3_storage.array_uploaded['constraint_bounds'] == None
 
     assert mock_s3_storage.file_removed
 
-def test_optimize_with_constraints(model_s3_client, mock_s3_storage, mock_metrics, mock_result):
+
+def test_optimize_with_set_constraints_matrices(model_s3_client, mock_s3_storage, mock_metrics, mock_result):
     model = model_s3_client
 
     # optimize using sdk
     weights = np.random.rand(10, 10).astype(np.float32)
     constraint_weights = np.random.rand(4, 10).astype(np.float32)
     bias = np.random.rand(10).astype(np.float32)
     constraint_bounds = np.random.rand(4, 2).astype(np.float32)
 
     model.add_variable_vector('x', 10, Vtype.BINARY)
     model.set_objective_matrices(weights, bias)
     model.set_constraints_matrices(constraint_weights, constraint_bounds)
     response = model.optimize()
 
-    assert response.metrics() == mock_metrics
+    assert response.computation_metrics() == mock_metrics["computation_metrics"]
     assert (response.result_vector() == mock_result).all()
 
     assert mock_s3_storage.array_uploaded['bias'] == np_array_to_bytes(bias)
     assert mock_s3_storage.array_uploaded['weights'] == np_array_to_bytes(weights)
     assert mock_s3_storage.array_uploaded['constraint_weights'] == np_array_to_bytes(constraint_weights)
     assert mock_s3_storage.array_uploaded['constraint_bounds'] == np_array_to_bytes(constraint_bounds)
 
     assert mock_s3_storage.file_removed
 
-@pytest.mark.parametrize("vtype", [
-    Vtype.BINARY, Vtype.BIPOLAR,
-])
-def test_vtype_sent(model_s3_client, mock_titanq_client, vtype):
-    model = model_s3_client
-    mock_client = mock_titanq_client
-
-    # optimize using sdk
-    weights = np.random.rand(10, 10).astype(np.float32)
-    bias = np.random.rand(10).astype(np.float32)
-
-    model.add_variable_vector('x', 10, vtype)
-    model.set_objective_matrices(weights, bias)
-
-    model.optimize()
-
-    assert mock_client.request_sent.parameters.variables_format == str(vtype)
 
 @pytest.mark.parametrize("constraint_weights_shape, constraint_bounds_shape, error", [
     ((2, 10), (2,2), None),
     ((10, 10), (10,2), None),
     ((2, 10), (3,2), ValueError),
     ((2, 10), (2,), ValueError),
     ((2, 10), (10,2), ValueError),
@@ -271,14 +258,34 @@
 
     if error:
         with pytest.raises(error):
             model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
     else:
         model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
 
+
+@pytest.mark.parametrize("vtype", [
+    Vtype.BINARY, Vtype.BIPOLAR,
+])
+def test_vtype_sent(model_s3_client, mock_titanq_client, vtype):
+    model = model_s3_client
+    mock_client = mock_titanq_client
+
+    # optimize using sdk
+    weights = np.random.rand(10, 10).astype(np.float32)
+    bias = np.random.rand(10).astype(np.float32)
+
+    model.add_variable_vector('x', 10, vtype)
+    model.set_objective_matrices(weights, bias)
+
+    model.optimize()
+
+    assert mock_client.request_sent.parameters.variables_format == str(vtype)
+
+
 @pytest.mark.parametrize("constraint_weights_dtype, constraint_bounds_dtype, error", [
     (np.float32, np.float32, None),
     (np.float64, np.float32, ValueError),
     (np.float32, np.float64, ValueError),
     (np.int32, np.int32, ValueError),
 ])
 def test_constraints_dtype(model_s3_client, constraint_weights_dtype, constraint_bounds_dtype, error):
@@ -290,24 +297,118 @@
     if error:
         with pytest.raises(error):
             model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
     else:
         model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
 
 
+
 def test_constraints_without_variable(model_s3_client):
     constraint_weights = np.random.rand(2, 10).astype(np.float32)
     constraint_bounds = np.random.rand(2).astype(np.float32)
 
     with pytest.raises(errors.MissingVariableError):
         model_s3_client.set_constraints_matrices(constraint_weights, constraint_bounds)
 
+    with pytest.raises(errors.MissingVariableError):
+        model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
 
-def test_set_constraints_multiple_time(model_s3_client):
-    model_s3_client.add_variable_vector('x', 10, Vtype.BINARY)
+    with pytest.raises(errors.MissingVariableError):
+        model_s3_client.add_set_partitioning_constraint(np.array([0, 1]))
+
+    with pytest.raises(errors.MissingVariableError):
+        model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 0, 1, 0], [0, 1, 1, 1]]), np.array([2, 3]))
+
+    with pytest.raises(errors.MissingVariableError):
+        model_s3_client.add_cardinality_constraint(np.array([1, 1]), 2)
+
+
+def test_add_set_partitioning_constraints_matrix(model_s3_client):
+    model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
+
+    model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+
+    model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 0, 0, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1], [1, 1]])).all()
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_set_partitioning_constraints_matrix(np.array([[1, 1, 0, 0], [1, 1, 0, 0]]))
+
+
+def test_add_set_partitioning_constraint(model_s3_client):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    model_s3_client.add_set_partitioning_constraint(np.array([0, 1]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 1]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1]])).all()
+
+    model_s3_client.add_set_partitioning_constraint(np.array([1, 0]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 1], [1, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_set_partitioning_constraint(np.array([1, 0]))
+
+
+def test_add_cardinality_constraints_matrix(model_s3_client):
+    model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
+
+    model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 0, 1, 0], [0, 1, 1, 1]]), np.array([2, 3]))
+    assert (model_s3_client._constraints.weights() == np.array([[1, 0, 1, 0], [0, 1, 1, 1]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [3, 3]])).all()
+
+    model_s3_client.add_cardinality_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]), np.array([1, 1]))
+    assert (model_s3_client._constraints.weights() == np.array([[1, 0, 1, 0], [0, 1, 1, 1], [0, 1, 0, 0], [1, 0, 0, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [3, 3], [1, 1], [1, 1]])).all()
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_cardinality_constraints_matrix(np.array([[0, 1, 0, 0], [1, 0, 0, 0]]), np.array([1, 1]))
+
+
+def test_add_cardinality_constraint(model_s3_client):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    model_s3_client.add_cardinality_constraint(np.array([1, 1]), 2)
+    assert (model_s3_client._constraints.weights() == np.array([[1, 1]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[2, 2]])).all()
+
+    model_s3_client.add_cardinality_constraint(np.array([0, 1]), 1)
+    assert (model_s3_client._constraints.weights() == np.array([[1, 1], [0, 1]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[2, 2], [1, 1]])).all()
+
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_cardinality_constraint(np.array([0, 1]), 1)
+
+@pytest.mark.parametrize("constraint_mask, cardinality, error", [
+    (np.array([1, 1]), 1, None),
+    (np.array([1, 1]), 2, None),
+    (np.array([1, 1]), 3, ValueError),
+])
+def test_cardinalities_sum(model_s3_client, constraint_mask, cardinality, error):
+    model_s3_client.add_variable_vector('x', 2, Vtype.BINARY)
+
+    if error:
+        with pytest.raises(ValueError):
+            model_s3_client.add_cardinality_constraint(constraint_mask, cardinality)
+    else:
+        model_s3_client.add_cardinality_constraint(constraint_mask, cardinality)
+
+def test_combination_constraint(model_s3_client):
+    model_s3_client.add_variable_vector('x', 4, Vtype.BINARY)
+
+    model_s3_client.add_set_partitioning_constraints_matrix(np.array([[0, 0, 1, 0], [0, 1, 0, 0]]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1]])).all()
+
+    model_s3_client.add_set_partitioning_constraint(np.array([0, 1, 0, 0]))
+    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1]])).all()
 
-    weights = np.random.rand(2, 10).astype(np.float32)
-    bias = np.random.rand(2, 2).astype(np.float32)
-    model_s3_client.set_constraints_matrices(weights, bias)
+    model_s3_client.add_cardinality_constraint(np.array([1, 1, 1, 1]), 2)
+    assert (model_s3_client._constraints.weights() == np.array([[0, 0, 1, 0], [0, 1, 0, 0], [0, 1, 0, 0], [1, 1, 1, 1]])).all()
+    assert (model_s3_client._constraints.bounds() == np.array([[1, 1], [1, 1], [1, 1], [2, 2]])).all()
 
-    with pytest.raises(errors.ConstraintsAlreadySetError):
-        model_s3_client.set_constraints_matrices(weights, bias)
+    with pytest.raises(errors.MaximumConstraintLimitError):
+        model_s3_client.add_cardinality_constraints_matrix(np.array([[1, 1, 0, 0], [1, 1, 0, 0]]), [2, 2])
```

### Comparing `titanq-0.5.3/titanq/__init__.py` & `titanq-0.6.1/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_client/client.py` & `titanq-0.6.1/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_client/model.py` & `titanq-0.6.1/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_model/errors.py` & `titanq-0.6.1/titanq/_model/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 class MissingVariableError(TitanQError):
     """Variable has not already been registered"""
 
 class MissingObjectiveError(TitanQError):
     """Objective has not already been registered"""
 
+class MaximumConstraintLimitError(TitanQError):
+    """The number of constraints is bigger than the number of variables"""
+
+class ConstraintSizeError(TitanQError):
+    """The constraint size does not match"""
+
 class ObjectiveAlreadySetError(TitanQError):
     """An objective has already been set"""
 
 class ConstraintsAlreadySetError(TitanQError):
     """Constraints has already been set"""
 
 class OptimizeError(TitanQError):
```

### Comparing `titanq-0.5.3/titanq/_model/objective.py` & `titanq-0.6.1/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_model/optimize_response.py` & `titanq-0.6.1/titanq/_model/optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_model/variable.py` & `titanq-0.6.1/titanq/_model/variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_storage/managed_storage.py` & `titanq-0.6.1/titanq/_storage/managed_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_storage/s3_storage.py` & `titanq-0.6.1/titanq/_storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq/_storage/storage_client.py` & `titanq-0.6.1/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.5.3/titanq.egg-info/PKG-INFO` & `titanq-0.6.1/titanq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.5.3
+Version: 0.6.1
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
+Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -24,15 +25,15 @@
 Requires-Dist: pydantic>=2.5.3
 
 # The TitanQ SDK for Python
 
 ![Python](https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11-blue) ![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
 
 TitanQ is the InfinityQ Software Development Kit (SDK) for Python. The SDK facilitates and opens the way for faster implementation
-of the TitanQ solver without having to deal directly with the API.
+of the TitanQ solver without having to deal directly with the [TitanQ API](https://docs.titanq.infinityq.io).
 
 This TitanQ package is maintained and published by [InfinityQ](https://www.infinityq.tech/)
 
 
 ## API Key
 
 In order to use the TitanQ service, a user needs an API key.
@@ -91,11 +92,21 @@
 
 [![\\ \mathbf{W}=(W_{i,j})\in \mathbb{R}^{n \times n}, ~ where ~ \mathbf{Q} = \mathbf{W} + \mathbf{b}^{\intercal}\boldsymbol{I}, ~ and ~ \mathbf{b} = (b_i) \in \mathbb{R}^{n}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cmathbf%7BW%7D%3D(W_%7Bi%2Cj%7D)%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%20%5Ctimes%20n%7D%2C%20~%20where%20~%20%5Cmathbf%7BQ%7D%20%3D%20%5Cmathbf%7BW%7D%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cboldsymbol%7BI%7D%2C%20~%20and%20~%20%5Cmathbf%7Bb%7D%20%3D%20(b_i)%20%5Cin%20%5Cmathbb%7BR%7D%5E%7Bn%7D)](#_)
 
 denotes the *biases*, which are used in the final model formulation described below
 
 [![\\ \begin{align} \notag \\ argmin_{\mathbf{x}} \, \, \, \, E(\mathbf{x}) & = \sum_{i=1}^n \sum_{i < j}^n W_{i,j}x_i x_j + \sum_i^n b_i x_i \notag \\ & = \frac{1}{2}\sum_{i=1}^n\sum_{j=1}^n W_{i,j}x_{i}x_{j} + \sum_{i=1}^{n} b_{i}x_{i} \notag \\ & = \frac{1}{2}(\mathbf{x}^{\intercal}\mathbf{W}\mathbf{x}) + \mathbf{b}^{\intercal}\mathbf{x} \notag \end{align}](https://latex.codecogs.com/svg.latex?%5C%5C%20%5Cbegin%7Balign%7D%20%5Cnotag%20%5C%5C%20argmin_%7B%5Cmathbf%7Bx%7D%7D%20%5C%2C%20%5C%2C%20%5C%2C%20%5C%2C%20E(%5Cmathbf%7Bx%7D)%20%26%20%3D%20%5Csum_%7Bi%3D1%7D%5En%20%5Csum_%7Bi%20%3C%20j%7D%5En%20W_%7Bi%2Cj%7Dx_i%20x_j%20%2B%20%5Csum_i%5En%20b_i%20x_i%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D%5Csum_%7Bi%3D1%7D%5En%5Csum_%7Bj%3D1%7D%5En%20W_%7Bi%2Cj%7Dx_%7Bi%7Dx_%7Bj%7D%20%2B%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20b_%7Bi%7Dx_%7Bi%7D%20%5Cnotag%20%5C%5C%20%26%20%3D%20%5Cfrac%7B1%7D%7B2%7D(%5Cmathbf%7Bx%7D%5E%7B%5Cintercal%7D%5Cmathbf%7BW%7D%5Cmathbf%7Bx%7D)%20%2B%20%5Cmathbf%7Bb%7D%5E%7B%5Cintercal%7D%5Cmathbf%7Bx%7D%20%5Cnotag%20%5Cend%7Balign%7D)](#_)
 
+
+Additional parameters are avialble to tune the problem:
+- beta
+- coupling_mult
+- num_chains
+- num_engines
+
+For more informations how to use theses parameters, please refer to the [API documentation](https://docs.titanq.infinityq.io)
+
+
 ## Getting support or help
 
 
-Further help can be obtained by contacting [InfinityQ support](support@infinityq.tech)
+Further help can be obtained by contacting [InfinityQ support](mailto:support@infinityq.tech)
```

### Comparing `titanq-0.5.3/titanq.egg-info/SOURCES.txt` & `titanq-0.6.1/titanq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE.txt
 README.md
 pyproject.toml
 requirements.txt
 tests/test_client.py
 tests/test_model.py
+tests/test_numpy_util.py
 tests/test_optimize_response.py
 titanq/__init__.py
 titanq.egg-info/PKG-INFO
 titanq.egg-info/SOURCES.txt
 titanq.egg-info/dependency_links.txt
 titanq.egg-info/requires.txt
 titanq.egg-info/top_level.txt
 titanq/_client/__init__.py
 titanq/_client/client.py
 titanq/_client/model.py
 titanq/_model/__init__.py
 titanq/_model/constraints.py
 titanq/_model/errors.py
 titanq/_model/model.py
+titanq/_model/numpy_util.py
 titanq/_model/objective.py
 titanq/_model/optimize_response.py
 titanq/_model/variable.py
 titanq/_storage/__init__.py
 titanq/_storage/managed_storage.py
 titanq/_storage/s3_storage.py
 titanq/_storage/storage_client.py
```

