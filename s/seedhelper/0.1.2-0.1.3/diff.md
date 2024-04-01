# Comparing `tmp/seedhelper-0.1.2.tar.gz` & `tmp/seedhelper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedhelper-0.1.2.tar", last modified: Mon Apr  1 17:50:30 2024, max compression
+gzip compressed data, was "seedhelper-0.1.3.tar", last modified: Mon Apr  1 19:11:47 2024, max compression
```

## Comparing `seedhelper-0.1.2.tar` & `seedhelper-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 17:50:26.000000 seedhelper-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 17:50:30.421130 seedhelper-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-01 17:50:26.000000 seedhelper-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 17:50:26.000000 seedhelper-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:50:30.421130 seedhelper-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 17:50:26.000000 seedhelper-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.417130 seedhelper-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/c_seedhelper/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/c_seedhelper/structures_helper.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/cubiomes/
--rw-r--r--   0 runner    (1001) docker     (127)    62188 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/biomenoise.c
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/biometree.c
--rw-r--r--   0 runner    (1001) docker     (127)   169817 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/finders.c
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/generator.c
--rw-r--r--   0 runner    (1001) docker     (127)    71800 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/layers.c
--rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/noise.c
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/quadbase.c
--rw-r--r--   0 runner    (1001) docker     (127)    22009 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/cubiomes/util.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/seedhelper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/seedhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-01 17:50:26.000000 seedhelper-0.1.2/src/seedhelper/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:50:30.421130 seedhelper-0.1.2/src/seedhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 17:50:30.000000 seedhelper-0.1.2/src/seedhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.252932 seedhelper-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 19:11:41.000000 seedhelper-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 19:11:47.252932 seedhelper-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-01 19:11:41.000000 seedhelper-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 19:11:41.000000 seedhelper-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:11:47.252932 seedhelper-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 19:11:41.000000 seedhelper-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.248932 seedhelper-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.248932 seedhelper-0.1.3/src/c_seedhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/c_seedhelper/structures_helper.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.252932 seedhelper-0.1.3/src/cubiomes/
+-rw-r--r--   0 runner    (1001) docker     (127)    62188 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/biomenoise.c
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/biometree.c
+-rw-r--r--   0 runner    (1001) docker     (127)   169817 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/finders.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/generator.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71800 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/layers.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/noise.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/quadbase.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22009 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/cubiomes/util.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.252932 seedhelper-0.1.3/src/seedhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/seedhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-01 19:11:41.000000 seedhelper-0.1.3/src/seedhelper/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:11:47.252932 seedhelper-0.1.3/src/seedhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-01 19:11:47.000000 seedhelper-0.1.3/src/seedhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 19:11:47.000000 seedhelper-0.1.3/src/seedhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:11:47.000000 seedhelper-0.1.3/src/seedhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 19:11:47.000000 seedhelper-0.1.3/src/seedhelper.egg-info/top_level.txt
```

### Comparing `seedhelper-0.1.2/LICENSE` & `seedhelper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/PKG-INFO` & `seedhelper-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedhelper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library that help to find specific Minecraft structures or biomes for a given seed.
 Author: Louis Pagnier
 License: MIT
 Keywords: minecraft,seed,biome,structure,elytra
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `seedhelper-0.1.2/README.md` & `seedhelper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/pyproject.toml` & `seedhelper-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "seedhelper"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python library that help to find specific Minecraft structures or biomes for a given seed."
 authors = [{ name = "Louis Pagnier" }]
 readme = "README.md"
 requires-python = ">=3.10"
 license = { text = "MIT" }
 keywords = ["minecraft", "seed", "biome", "structure", "elytra"]
 classifiers = [
```

### Comparing `seedhelper-0.1.2/setup.py` & `seedhelper-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/c_seedhelper/structures_helper.c` & `seedhelper-0.1.3/src/c_seedhelper/structures_helper.c`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 #include "../cubiomes/generator.h"
 #include "../cubiomes/finders.h"
 #include "../cubiomes/util.h"
 #include "structures_helper.h"
 
 
+
 Piece* get_elytras_positions(struct find_elytras_arguments* arguments, int *n_ships)
 {
     const int structType = End_City;
     const int mc = str2mc(arguments->mc_version);
     const uint64_t seed = arguments->seed;
     const int c_x = arguments->x;
     const int c_z = arguments->z;
```

### Comparing `seedhelper-0.1.2/src/cubiomes/biomenoise.c` & `seedhelper-0.1.3/src/cubiomes/biomenoise.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/biometree.c` & `seedhelper-0.1.3/src/cubiomes/biometree.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/finders.c` & `seedhelper-0.1.3/src/cubiomes/finders.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/generator.c` & `seedhelper-0.1.3/src/cubiomes/generator.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/layers.c` & `seedhelper-0.1.3/src/cubiomes/layers.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/noise.c` & `seedhelper-0.1.3/src/cubiomes/noise.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/quadbase.c` & `seedhelper-0.1.3/src/cubiomes/quadbase.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/cubiomes/util.c` & `seedhelper-0.1.3/src/cubiomes/util.c`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/seedhelper/structures.py` & `seedhelper-0.1.3/src/seedhelper/structures.py`

 * *Files identical despite different names*

### Comparing `seedhelper-0.1.2/src/seedhelper.egg-info/PKG-INFO` & `seedhelper-0.1.3/src/seedhelper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedhelper
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library that help to find specific Minecraft structures or biomes for a given seed.
 Author: Louis Pagnier
 License: MIT
 Keywords: minecraft,seed,biome,structure,elytra
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

