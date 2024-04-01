# Comparing `tmp/upc_pymotion-0.1.1.tar.gz` & `tmp/upc_pymotion-0.1.2.tar.gz`

## Comparing `upc_pymotion-0.1.1.tar` & `upc_pymotion-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/io/__init__.py
--rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/io/bvh.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/forward_kinematics.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/forward_kinematics_torch.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/skeleton.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/skeleton_torch.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/time.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/ops/time_torch.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/blender.py
--rw-r--r--   0        0        0    19612 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/render/viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/__init__.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/dual_quat.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/dual_quat_torch.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/ortho6d.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/ortho6d_torch.py
--rw-r--r--   0        0        0    14636 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/quat.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pymotion/rotations/quat_torch.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/LICENSE
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/io/__init__.py
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/io/bvh.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/forward_kinematics.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/forward_kinematics_torch.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/skeleton.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/skeleton_torch.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/time.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/ops/time_torch.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/render/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/render/blender.py
+-rw-r--r--   0        0        0    19612 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/render/viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/__init__.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/dual_quat.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/dual_quat_torch.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/ortho6d.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/ortho6d_torch.py
+-rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/quat.py
+-rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pymotion/rotations/quat_torch.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.2/PKG-INFO
```

### Comparing `upc_pymotion-0.1.1/pymotion/io/bvh.py` & `upc_pymotion-0.1.2/pymotion/io/bvh.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/forward_kinematics.py` & `upc_pymotion-0.1.2/pymotion/ops/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/forward_kinematics_torch.py` & `upc_pymotion-0.1.2/pymotion/ops/forward_kinematics_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/skeleton.py` & `upc_pymotion-0.1.2/pymotion/ops/skeleton.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/skeleton_torch.py` & `upc_pymotion-0.1.2/pymotion/ops/skeleton_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/time.py` & `upc_pymotion-0.1.2/pymotion/ops/time.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/ops/time_torch.py` & `upc_pymotion-0.1.2/pymotion/ops/time_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/render/__init__.py` & `upc_pymotion-0.1.2/pymotion/render/__init__.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/render/blender.py` & `upc_pymotion-0.1.2/pymotion/render/blender.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/render/viewer.py` & `upc_pymotion-0.1.2/pymotion/render/viewer.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/dual_quat.py` & `upc_pymotion-0.1.2/pymotion/rotations/dual_quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/dual_quat_torch.py` & `upc_pymotion-0.1.2/pymotion/rotations/dual_quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/ortho6d.py` & `upc_pymotion-0.1.2/pymotion/rotations/ortho6d.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/ortho6d_torch.py` & `upc_pymotion-0.1.2/pymotion/rotations/ortho6d_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/quat.py` & `upc_pymotion-0.1.2/pymotion/rotations/quat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 
 
 def from_scaled_angle_axis(scaledaxis: np.array) -> np.array:
     """
     Create a quaternion from an scaled angle-axis representation.
```

### Comparing `upc_pymotion-0.1.1/pymotion/rotations/quat_torch.py` & `upc_pymotion-0.1.2/pymotion/rotations/quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/.gitignore` & `upc_pymotion-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/LICENSE` & `upc_pymotion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/README.md` & `upc_pymotion-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.1/pyproject.toml` & `upc_pymotion-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.hatch.build]
 include = ["pymotion/*"]
 exclude = ["*test*"]
 
 [project]
 name = "upc-pymotion"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python library for working with motion data in NumPy or PyTorch."
 readme = "README.md"
 authors = [{ name = "Jose Luis Ponton", email = "jose.luis.ponton@upc.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `upc_pymotion-0.1.1/PKG-INFO` & `upc_pymotion-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: upc-pymotion
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for working with motion data in NumPy or PyTorch.
 Project-URL: Homepage, https://github.com/UPC-ViRVIG/pymotion
 Author-email: Jose Luis Ponton <jose.luis.ponton@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 Jose Luis Ponton
```

