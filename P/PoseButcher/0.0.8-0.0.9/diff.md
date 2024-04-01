# Comparing `tmp/posebutcher-0.0.8.tar.gz` & `tmp/posebutcher-0.0.9.tar.gz`

## Comparing `posebutcher-0.0.8.tar` & `posebutcher-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 posebutcher-0.0.8/posebutcher/__init__.py
--rw-r--r--   0        0        0    17622 2020-02-02 00:00:00.000000 posebutcher-0.0.8/posebutcher/butcher.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 posebutcher-0.0.8/posebutcher/log.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 posebutcher-0.0.8/posebutcher/o3d.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 posebutcher-0.0.8/.gitignore
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 posebutcher-0.0.8/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 posebutcher-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 posebutcher-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 posebutcher-0.0.9/posebutcher/__init__.py
+-rw-r--r--   0        0        0    25772 2020-02-02 00:00:00.000000 posebutcher-0.0.9/posebutcher/butcher.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 posebutcher-0.0.9/posebutcher/log.py
+-rw-r--r--   0        0        0    10536 2020-02-02 00:00:00.000000 posebutcher-0.0.9/posebutcher/o3d.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 posebutcher-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 posebutcher-0.0.9/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 posebutcher-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 posebutcher-0.0.9/PKG-INFO
```

### Comparing `posebutcher-0.0.8/posebutcher/log.py` & `posebutcher-0.0.9/posebutcher/log.py`

 * *Files identical despite different names*

### Comparing `posebutcher-0.0.8/README.md` & `posebutcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `posebutcher-0.0.8/pyproject.toml` & `posebutcher-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "PoseButcher"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Max Winokan", email="max@winokan.com"},
 ]
 description = "A tool for categorising and segmenting virtual hits with reference to experimental protein structures and (fragment) hits."
 readme = "README.md"
 requires-python = ">=3.9"
 requires = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "MPyTools >= 0.0.9",
-    "MolParse >= 0.0.6",
+    "MolParse >= 0.0.8",
     "ase",
     "rdkit",
     "py3Dmol",
     "IPython",
     "open3d >= 0.18",
     "numpy",
     "jupyterlab",
```

### Comparing `posebutcher-0.0.8/PKG-INFO` & `posebutcher-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: PoseButcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool for categorising and segmenting virtual hits with reference to experimental protein structures and (fragment) hits.
 Project-URL: Homepage, https://github.com/mwinokan/PoseButcher
 Project-URL: Bug Tracker, https://github.com/mwinokan/PoseButcher/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: ase
 Requires-Dist: ipython
 Requires-Dist: jupyterlab
-Requires-Dist: molparse>=0.0.6
+Requires-Dist: molparse>=0.0.8
 Requires-Dist: mpytools>=0.0.9
 Requires-Dist: numpy
 Requires-Dist: open3d>=0.18
 Requires-Dist: pandas
 Requires-Dist: py3dmol
 Requires-Dist: pygamer
 Requires-Dist: rdkit
```

