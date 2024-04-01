# Comparing `tmp/tools-jsyoo61-2024.3.4.0.tar.gz` & `tmp/tools-jsyoo61-2024.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.3.4.0.tar", last modified: Mon Mar  4 21:02:05 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.4.1.0.tar", last modified: Mon Apr  1 19:44:57 2024, max compression
```

## Comparing `tools-jsyoo61-2024.3.4.0.tar` & `tools-jsyoo61-2024.4.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.721848 tools-jsyoo61-2024.3.4.0/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1342 2024-03-04 21:02:05.720906 tools-jsyoo61-2024.3.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-04 21:02:05.722847 tools-jsyoo61-2024.3.4.0/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.648682 tools-jsyoo61-2024.3.4.0/tools/
--rw-rw-rw-   0        0        0      292 2024-03-04 21:01:56.000000 tools-jsyoo61-2024.3.4.0/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.649792 tools-jsyoo61-2024.3.4.0/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.3.4.0/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.656342 tools-jsyoo61-2024.3.4.0/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     2219 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.657808 tools-jsyoo61-2024.3.4.0/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.661814 tools-jsyoo61-2024.3.4.0/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.664816 tools-jsyoo61-2024.3.4.0/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.3.4.0/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.666054 tools-jsyoo61-2024.3.4.0/tools/stats/
--rw-rw-rw-   0        0        0      881 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    14960 2024-01-19 21:34:43.000000 tools-jsyoo61-2024.3.4.0/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.682347 tools-jsyoo61-2024.3.4.0/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/layers.py
--rw-rw-rw-   0        0        0    17712 2024-03-04 21:01:36.000000 tools-jsyoo61-2024.3.4.0/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.686346 tools-jsyoo61-2024.3.4.0/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.3.4.0/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.3.4.0/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:02:05.717852 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-03-04 21:02:04.000000 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-03-04 21:02:05.000000 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 21:02:04.000000 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-03-04 21:02:05.000000 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-04 21:02:05.000000 tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.302612 tools-jsyoo61-2024.4.1.0/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1342 2024-04-01 19:44:57.301614 tools-jsyoo61-2024.4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 19:44:57.303615 tools-jsyoo61-2024.4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.188996 tools-jsyoo61-2024.4.1.0/tools/
+-rw-rw-rw-   0        0        0      292 2024-04-01 19:44:34.000000 tools-jsyoo61-2024.4.1.0/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.191995 tools-jsyoo61-2024.4.1.0/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.4.1.0/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.199993 tools-jsyoo61-2024.4.1.0/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2219 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.200994 tools-jsyoo61-2024.4.1.0/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.206994 tools-jsyoo61-2024.4.1.0/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.213516 tools-jsyoo61-2024.4.1.0/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.4.1.0/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.230522 tools-jsyoo61-2024.4.1.0/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.4.1.0/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    14960 2024-01-19 21:34:43.000000 tools-jsyoo61-2024.4.1.0/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.260521 tools-jsyoo61-2024.4.1.0/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.265539 tools-jsyoo61-2024.4.1.0/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.4.1.0/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.4.1.0/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-01 19:44:57.299626 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1342 2024-04-01 19:44:56.000000 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2024-04-01 19:44:56.000000 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 19:44:56.000000 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-01 19:44:56.000000 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-01 19:44:56.000000 tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.3.4.0/LICENSE.txt` & `tools-jsyoo61-2024.4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/PKG-INFO` & `tools-jsyoo61-2024.4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.3.4.0
+Version: 2024.4.1.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.3.4.0/README.md` & `tools-jsyoo61-2024.4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/setup.py` & `tools-jsyoo61-2024.4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/array.py` & `tools-jsyoo61-2024.4.1.0/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/data.py` & `tools-jsyoo61-2024.4.1.0/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/exp.py` & `tools-jsyoo61-2024.4.1.0/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/modules.py` & `tools-jsyoo61-2024.4.1.0/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/numpy/_f.py` & `tools-jsyoo61-2024.4.1.0/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/numpy/_utils.py` & `tools-jsyoo61-2024.4.1.0/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/os.py` & `tools-jsyoo61-2024.4.1.0/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/plot/sklearn.py` & `tools-jsyoo61-2024.4.1.0/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/plot/utils.py` & `tools-jsyoo61-2024.4.1.0/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/random.py` & `tools-jsyoo61-2024.4.1.0/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.4.1.0/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/tools.py` & `tools-jsyoo61-2024.4.1.0/tools/tools.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/torch/estimator.py` & `tools-jsyoo61-2024.4.1.0/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.4.1.0/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/torch/model.py` & `tools-jsyoo61-2024.4.1.0/tools/torch/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,34 +307,42 @@
     Residual module which computes residual connections in forward pass.
     Note that intermediate tensors need to have the same shape.
 
     Parameters
     ----------
     blocks : list of nn.Module objects, or an iterable nn.Module object.
 
+    activation : nn.Module object (default: None)
+        activation function to be applied at each residual connection betwee blocks.
+
     Examples
     --------
     >>> blocks = [nn.Linear(10,10) for i in range(5)]
     >>> model = Residual(blocks)
     >>> model
 
     """
-    # def __init__(self, block, n_repeat, activation = nn.ReLU()):
-    def __init__(self, blocks):
+    def __init__(self, blocks, activation=None):
         super().__init__()
         if issubclass(type(blocks), nn.Module):
             self.blocks = blocks
         elif issubclass(type(blocks), list):
             self.blocks = nn.ModuleList(blocks)
         else:
             raise Exception('')
+        self.activation = activation
 
     def forward(self, x):
-        for block in self.blocks:
-            x = block(x)+x
+        if self.activation is not None:
+            for block in self.blocks:
+                x = self.activation(block(x)+x)
+
+        else: # No activation
+            for block in self.blocks:
+                x = block(x)+x
         return x
 
 class Parallel(nn.Module):
     """
     Similar to nn.Sequential, but parallel connection.
     Note that the shape of each output from each module must be identical,
     since Parallel() sums up all outputs in forward().
```

### Comparing `tools-jsyoo61-2024.3.4.0/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.4.1.0/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools/torch/utils.py` & `tools-jsyoo61-2024.4.1.0/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.3.4.0
+Version: 2024.4.1.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tools-jsyoo61-2024.3.4.0/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.4.1.0/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files identical despite different names*

