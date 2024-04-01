# Comparing `tmp/pytorch-sidu-1.0.6.tar.gz` & `tmp/pytorch-sidu-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-sidu-1.0.6.tar", last modified: Wed Mar 27 14:46:14 2024, max compression
+gzip compressed data, was "pytorch-sidu-1.0.7.tar", last modified: Mon Apr  1 14:29:16 2024, max compression
```

## Comparing `pytorch-sidu-1.0.6.tar` & `pytorch-sidu-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:46:14.776528 pytorch-sidu-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-27 14:46:14.776528 pytorch-sidu-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:46:14.772528 pytorch-sidu-1.0.6/pytorch_sidu/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/pytorch_sidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/pytorch_sidu/sidu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:46:14.776528 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-27 14:46:14.000000 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-27 14:46:14.000000 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:46:14.000000 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-27 14:46:14.000000 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-27 14:46:14.000000 pytorch-sidu-1.0.6/pytorch_sidu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-27 14:46:14.776528 pytorch-sidu-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-27 14:44:45.000000 pytorch-sidu-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/pytorch_sidu/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/pytorch_sidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/pytorch_sidu/sidu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:29:16.000000 pytorch-sidu-1.0.7/pytorch_sidu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 14:29:16.693052 pytorch-sidu-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-01 14:15:25.000000 pytorch-sidu-1.0.7/setup.py
```

### Comparing `pytorch-sidu-1.0.6/LICENSE` & `pytorch-sidu-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.6/PKG-INFO` & `pytorch-sidu-1.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.0.6
+Version: 1.0.7
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: numpy
 
 # **pytorch-sidu**
+
+![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
+[![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
+
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
 - Pytorch implementation of the SIDU method. 
 - Simple interface for loading pretrained models by specifying one of the following [string name](https://pytorch.org/vision/stable/models.html#table-of-all-available-classification-weights)
 - Clear interface for generating saliency maps
 
 Some examples made with VGG19 on [Caltech-101 dataset](https://paperswithcode.com/dataset/caltech-101):
```

### Comparing `pytorch-sidu-1.0.6/README.md` & `pytorch-sidu-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # **pytorch-sidu**
+
+![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
+[![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
+
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
 - Pytorch implementation of the SIDU method. 
 - Simple interface for loading pretrained models by specifying one of the following [string name](https://pytorch.org/vision/stable/models.html#table-of-all-available-classification-weights)
 - Clear interface for generating saliency maps
 
 Some examples made with VGG19 on [Caltech-101 dataset](https://paperswithcode.com/dataset/caltech-101):
```

### Comparing `pytorch-sidu-1.0.6/pytorch_sidu/sidu.py` & `pytorch-sidu-1.0.7/pytorch_sidu/sidu.py`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.6/pytorch_sidu.egg-info/PKG-INFO` & `pytorch-sidu-1.0.7/pytorch_sidu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.0.6
+Version: 1.0.7
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: numpy
 
 # **pytorch-sidu**
+
+![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
+[![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
+
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
 - Pytorch implementation of the SIDU method. 
 - Simple interface for loading pretrained models by specifying one of the following [string name](https://pytorch.org/vision/stable/models.html#table-of-all-available-classification-weights)
 - Clear interface for generating saliency maps
 
 Some examples made with VGG19 on [Caltech-101 dataset](https://paperswithcode.com/dataset/caltech-101):
```

### Comparing `pytorch-sidu-1.0.6/setup.cfg` & `pytorch-sidu-1.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.6/setup.py` & `pytorch-sidu-1.0.7/setup.py`

 * *Files identical despite different names*

