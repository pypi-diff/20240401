# Comparing `tmp/seedhelper-0.1.1.tar.gz` & `tmp/seedhelper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedhelper-0.1.1.tar", last modified: Sat Mar 30 14:13:19 2024, max compression
+gzip compressed data, was "seedhelper-0.1.2.tar", last modified: Mon Apr  1 17:50:30 2024, max compression
```

## Comparing `seedhelper-0.1.1.tar` & `seedhelper-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.097576 seedhelper-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-30 14:13:15.000000 seedhelper-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-30 14:13:19.097576 seedhelper-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-30 14:13:15.000000 seedhelper-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-30 14:13:15.000000 seedhelper-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 14:13:19.097576 seedhelper-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-30 14:13:15.000000 seedhelper-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.093577 seedhelper-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.093577 seedhelper-0.1.1/src/c_seedhelper/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/c_seedhelper/structures_helper.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.097576 seedhelper-0.1.1/src/cubiomes/
--rw-r--r--   0 runner    (1001) docker     (127)    62188 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/biomenoise.c
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/biometree.c
--rw-r--r--   0 runner    (1001) docker     (127)   169817 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/finders.c
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/generator.c
--rw-r--r--   0 runner    (1001) docker     (127)    71800 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/layers.c
--rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/noise.c
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/quadbase.c
--rw-r--r--   0 runner    (1001) docker     (127)    22009 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/cubiomes/util.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.097576 seedhelper-0.1.1/src/seedhelper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/seedhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-30 14:13:15.000000 seedhelper-0.1.1/src/seedhelper/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 14:13:19.097576 seedhelper-0.1.1/src/seedhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-30 14:13:19.000000 seedhelper-0.1.1/src/seedhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-30 14:13:19.000000 seedhelper-0.1.1/src/seedhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 14:13:19.000000 seedhelper-0.1.1/src/seedhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 14:13:19.000000 seedhelper-0.1.1/src/seedhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 17:50:26.000000 seedhelper-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 17:50:30.421130 seedhelper-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-01 17:50:26.000000 seedhelper-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 17:50:26.000000 seedhelper-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:50:30.421130 seedhelper-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 17:50:26.000000 seedhelper-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.417130 seedhelper-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/c_seedhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/c_seedhelper/structures_helper.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/cubiomes/
+-rw-r--r--   0 runner    (1001) docker     (127)    62188 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/biomenoise.c
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/biometree.c
+-rw-r--r--   0 runner    (1001) docker     (127)   169817 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/finders.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/generator.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71800 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/layers.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/noise.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/quadbase.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22009 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/util.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/seedhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/seedhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/seedhelper/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/seedhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/top_level.txt
```

### Comparing `seedhelper-0.1.1/LICENSE` & `seedhelper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/PKG-INFO` & `seedhelper-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedhelper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library that help to find specific Minecraft structures or biomes for a given seed.
 Author: Louis Pagnier
 License: MIT
 Keywords: minecraft,seed,biome,structure,elytra
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `seedhelper-0.1.1/README.md` & `seedhelper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/pyproject.toml` & `seedhelper-0.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "seedhelper"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python library that help to find specific Minecraft structures or biomes for a given seed."
 authors = [{ name = "Louis Pagnier" }]
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ["minecraft", "seed", "biome", "structure", "elytra"]
 classifiers = [
```

### Comparing `seedhelper-0.1.1/setup.py` & `seedhelper-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/c_seedhelper/structures_helper.c` & `seedhelper-0.1.2/src/c_seedhelper/structures_helper.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/biomenoise.c` & `seedhelper-0.1.2/src/cubiomes/biomenoise.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/biometree.c` & `seedhelper-0.1.2/src/cubiomes/biometree.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/finders.c` & `seedhelper-0.1.2/src/cubiomes/finders.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/generator.c` & `seedhelper-0.1.2/src/cubiomes/generator.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/layers.c` & `seedhelper-0.1.2/src/cubiomes/layers.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/noise.c` & `seedhelper-0.1.2/src/cubiomes/noise.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/quadbase.c` & `seedhelper-0.1.2/src/cubiomes/quadbase.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/cubiomes/util.c` & `seedhelper-0.1.2/src/cubiomes/util.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.1/src/seedhelper/structures.py` & `seedhelper-0.1.2/src/seedhelper/structures.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import ctypes
 import pathlib
+import platform
 
-lib_file = pathlib.Path(__file__).parent / "libstructureshelper.so"
+lib_file = pathlib.Path(__file__).parent / (
+            "libstructureshelper." + ("dll" if platform.system() == "Windows" else "so"))
 _structures_helper = ctypes.CDLL(str(lib_file))
 
 
 class Pos(ctypes.Structure):
     _fields_ = [('x', ctypes.c_int),
                 ('z', ctypes.c_int)]
```

### Comparing `seedhelper-0.1.1/src/seedhelper.egg-info/PKG-INFO` & `seedhelper-0.1.2/src/seedhelper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedhelper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library that help to find specific Minecraft structures or biomes for a given seed.
 Author: Louis Pagnier
 License: MIT
 Keywords: minecraft,seed,biome,structure,elytra
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

