# Comparing `tmp/hartufo-0.6.4.tar.gz` & `tmp/hartufo-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hartufo-0.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hartufo-0.6.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hartufo-0.6.4.tar` & `hartufo-0.6.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-03-03 22:25:55.563287 hartufo-0.6.4/LICENSE
--rw-r--r--   0        0        0     1032 2024-03-03 22:25:55.563287 hartufo-0.6.4/README.md
--rw-r--r--   0        0        0      815 2024-03-03 22:25:55.563287 hartufo-0.6.4/hartufo/__init__.py
--rw-r--r--   0        0        0  1534774 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/checksums.py
--rw-r--r--   0        0        0    29016 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/datareader.py
--rw-r--r--   0        0        0     2915 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/display.py
--rw-r--r--   0        0        0    31378 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/full.py
--rw-r--r--   0        0        0    25284 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/planar.py
--rw-r--r--   0        0        0    49754 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/query.py
--rw-r--r--   0        0        0     2621 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/sklearn/__init__.py
--rw-r--r--   0        0        0     6228 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/specifications.py
--rw-r--r--   0        0        0      258 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/torch/__init__.py
--rw-r--r--   0        0        0      474 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/transforms/__init__.py
--rw-r--r--   0        0        0    25231 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/transforms/hrir.py
--rw-r--r--   0        0        0     1644 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/transforms/image.py
--rw-r--r--   0        0        0     5386 2024-03-03 22:25:55.571287 hartufo-0.6.4/hartufo/util.py
--rw-r--r--   0        0        0     1037 2024-03-03 22:25:55.571287 hartufo-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 hartufo-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 15:25:20.837610 hartufo-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1032 2024-04-01 15:25:20.837610 hartufo-0.6.5/README.md
+-rw-r--r--   0        0        0      815 2024-04-01 15:25:20.837610 hartufo-0.6.5/hartufo/__init__.py
+-rw-r--r--   0        0        0  1534774 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/checksums.py
+-rw-r--r--   0        0        0    29016 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/datareader.py
+-rw-r--r--   0        0        0     2915 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/display.py
+-rw-r--r--   0        0        0    31378 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/full.py
+-rw-r--r--   0        0        0    25284 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/planar.py
+-rw-r--r--   0        0        0    49753 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/query.py
+-rw-r--r--   0        0        0     2621 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/sklearn/__init__.py
+-rw-r--r--   0        0        0     6228 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/specifications.py
+-rw-r--r--   0        0        0      258 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/torch/__init__.py
+-rw-r--r--   0        0        0      474 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/transforms/__init__.py
+-rw-r--r--   0        0        0    26061 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/transforms/hrir.py
+-rw-r--r--   0        0        0     1644 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/transforms/image.py
+-rw-r--r--   0        0        0     5386 2024-04-01 15:25:20.845610 hartufo-0.6.5/hartufo/util.py
+-rw-r--r--   0        0        0     1037 2024-04-01 15:25:20.845610 hartufo-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 hartufo-0.6.5/PKG-INFO
```

### Comparing `hartufo-0.6.4/LICENSE` & `hartufo-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/README.md` & `hartufo-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/__init__.py` & `hartufo-0.6.5/hartufo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A Python toolkit for data-driven HRTF research"""
 
-__version__ = '0.6.4'
+__version__ = '0.6.5'
 
 from .full import (
     Dataset,
     Cipic,
     Ari,
     Listen,
     CrossMod,
```

### Comparing `hartufo-0.6.4/hartufo/checksums.py` & `hartufo-0.6.5/hartufo/checksums.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/datareader.py` & `hartufo-0.6.5/hartufo/datareader.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/display.py` & `hartufo-0.6.5/hartufo/display.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/full.py` & `hartufo-0.6.5/hartufo/full.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/planar.py` & `hartufo-0.6.5/hartufo/planar.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/query.py` & `hartufo-0.6.5/hartufo/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
         super().__init__(collection_id='hutubs', sofa_directory_path=sofa_directory_path, anthropometry_path=anthropometry_csvfile_path, checksum_key=hrir_method, download=download, verify=verify)
         self._default_hrirs_exclude = (1, 96) # FABIAN dummy
         self._default_anthropometry_exclude = (1, 96) # FABIAN dummy
         self._default_mesh_exclude = (1, 96) # FABIAN dummy
 
 
     def _all_hrir_ids(self, side):
-        return sorted([int(x.stem.split('_')[0].split('pp')[1]) for x in self.sofa_directory_path.glob(f'pp??_HRIRs_{self._method_str}.sofa')])
+        return sorted([int(x.stem.split('_')[0].split('pp')[1]) for x in self.sofa_directory_path.glob(f'pp*_HRIRs_{self._method_str}.sofa')])
 
 
     def _load_anthropometry(self, anthropometry_path):
         # cm & deg
         self._anthropometry = {'head-torso': [], 'pinna-size': {'left': [], 'right': []}, 'pinna-angle': {'left': [], 'right': []}}
         anthropometry_ids = []
         with open(anthropometry_path, 'r') as f:
```

### Comparing `hartufo-0.6.4/hartufo/sklearn/__init__.py` & `hartufo-0.6.5/hartufo/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/specifications.py` & `hartufo-0.6.5/hartufo/specifications.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/transforms/hrir.py` & `hartufo-0.6.5/hartufo/transforms/hrir.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 def _to_dense2d(multidim_array: np.ndarray) -> np.ndarray:
     ''' Converts an N-D np.ndarray to a 2-D dense array which flattens all dimensions except the last into one while keeping the last 
         dimension intact.'''
     dense_array = multidim_array.compressed() if np.ma.isMaskedArray(multidim_array) else multidim_array
     return dense_array.reshape(-1, multidim_array.shape[-1])
 
 
+def _to_dense3d(multidim_array: np.ndarray) -> np.ndarray:
+    ''' Converts an N-D np.ndarray to a 3-D dense array which flattens the middle dimensions while keeping the first and last 
+        dimension intact.'''
+    dense_array = multidim_array.compressed() if np.ma.isMaskedArray(multidim_array) else multidim_array
+    return dense_array.reshape(len(multidim_array), -1, multidim_array.shape[-1])
+
+
 def _to_multidim(dense2d_array: np.ndarray, prototype: np.ndarray) -> np.ndarray:
     ''' Converts a 2-D dense np.ndarray into a N-D np.ndarray whose dimensions and sparsity mask is taken from the given prototypical 
         sparse array, except for the final dimension which is taken from the dense array itself.'''
     if np.ma.isMaskedArray(prototype):
         sparse_mask = np.tile(np.ma.getmaskarray(prototype)[..., :1], (*np.ones(prototype.ndim-1, dtype=int), dense2d_array.shape[-1]))
         sparse_array = np.ma.array(np.empty((*prototype.shape[:-1], dense2d_array.shape[-1])), dtype=dense2d_array.dtype, mask=sparse_mask)
         sparse_array[~sparse_mask] = dense2d_array.ravel()
@@ -39,14 +46,29 @@
         return _to_dense2d(hrirs)
 
 
     def inverse(self, hrirs_list: np.ndarray) -> np.ndarray:
         return _to_multidim(hrirs_list, self._prototype)
 
 
+class Hrir3dTransform(BatchTransform):
+    def __init__(self, prototype: Optional[np.ndarray] = None):
+        self._prototype = prototype
+
+
+    def __call__(self, hrirs: np.ndarray) -> np.ndarray:
+        if self._prototype is None:
+            self._prototype = hrirs
+        return _to_dense3d(hrirs)
+
+
+    def inverse(self, hrirs_list: np.ndarray) -> np.ndarray:
+        return _to_multidim(hrirs_list, self._prototype)
+
+
 class ScaleTransform(BatchTransform):
     def __init__(self, additive_factor: float = 0, multiplicative_factor = 1):
         self.additive_factor = additive_factor
         self.multiplicative_factor = multiplicative_factor
 
 
     def __call__(self, values: np.ndarray) -> np.ndarray:
```

### Comparing `hartufo-0.6.4/hartufo/transforms/image.py` & `hartufo-0.6.5/hartufo/transforms/image.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/hartufo/util.py` & `hartufo-0.6.5/hartufo/util.py`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/pyproject.toml` & `hartufo-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hartufo-0.6.4/PKG-INFO` & `hartufo-0.6.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hartufo
-Version: 0.6.4
+Version: 0.6.5
 Summary: A Python toolkit for data-driven HRTF research
 Author-email: Johan Pauwels <johan.pauwels@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: matplotlib >=3.5
 Requires-Dist: netCDF4 >=1.5
```

