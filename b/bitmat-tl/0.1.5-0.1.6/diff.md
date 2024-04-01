# Comparing `tmp/bitmat-tl-0.1.5.tar.gz` & `tmp/bitmat-tl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.1.5.tar", last modified: Sun Mar 31 19:25:17 2024, max compression
+gzip compressed data, was "bitmat-tl-0.1.6.tar", last modified: Mon Apr  1 18:07:35 2024, max compression
```

## Comparing `bitmat-tl-0.1.5.tar` & `bitmat-tl-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.5/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)       98 2024-03-26 17:02:00.000000 bitmat-tl-0.1.5/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-30 14:45:20.000000 bitmat-tl-0.1.5/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1078 2024-03-31 18:15:33.000000 bitmat-tl-0.1.5/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.5/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12721 2024-03-31 16:41:21.000000 bitmat-tl-0.1.5/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.5/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.5/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.5/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2463 2024-03-31 18:04:18.000000 bitmat-tl-0.1.5/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1750 2024-03-31 19:24:56.000000 bitmat-tl-0.1.5/bitmat/utils/convert_hf.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.5/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.5/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-03-31 19:25:17.000000 bitmat-tl-0.1.5/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      496 2024-03-31 19:25:17.000000 bitmat-tl-0.1.5/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-03-31 19:25:17.000000 bitmat-tl-0.1.5/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-03-31 19:25:17.000000 bitmat-tl-0.1.5/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-03-31 19:25:17.000000 bitmat-tl-0.1.5/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-03-31 19:25:17.644075 bitmat-tl-0.1.5/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-03-31 19:24:56.000000 bitmat-tl-0.1.5/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.6/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)       98 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-30 14:45:20.000000 bitmat-tl-0.1.6/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1077 2024-04-01 18:07:20.000000 bitmat-tl-0.1.6/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12721 2024-03-31 16:41:21.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2463 2024-03-31 18:04:18.000000 bitmat-tl-0.1.6/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1750 2024-03-31 19:24:56.000000 bitmat-tl-0.1.6/bitmat/utils/convert_hf_model.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.6/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.6/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 18:06:22.000000 bitmat-tl-0.1.6/setup.py
```

### Comparing `bitmat-tl-0.1.5/LICENSE` & `bitmat-tl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/PKG-INFO` & `bitmat-tl-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.1.5
+Version: 0.1.6
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.1.5/bitmat/bitlinear.py` & `bitmat-tl-0.1.6/bitmat/bitlinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import torch
 
 from .utils.bitmat import bitmat
 from .utils.rmsnorm import RMSLayerNorm
 
-
 class BitLinear(torch.nn.Module):
     """
     A linear layer that uses packed terniary matrix multiplication.
     """
     def __init__(self, in_features, out_features, eps, bias=None):
         super(BitLinear, self).__init__()
         self.eps = eps
```

### Comparing `bitmat-tl-0.1.5/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.1.6/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.1.6/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.1.6/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat/utils/bitmat.py` & `bitmat-tl-0.1.6/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat/utils/convert_hf.py` & `bitmat-tl-0.1.6/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat/utils/packing.py` & `bitmat-tl-0.1.6/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.5/bitmat_tl.egg-info/PKG-INFO` & `bitmat-tl-0.1.6/bitmat_tl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.1.5
+Version: 0.1.6
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `bitmat-tl-0.1.5/setup.py` & `bitmat-tl-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.1.5',
+    version='0.1.6',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

