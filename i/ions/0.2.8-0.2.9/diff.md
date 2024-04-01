# Comparing `tmp/ions-0.2.8.tar.gz` & `tmp/ions-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ions-0.2.8.tar", last modified: Mon Apr  1 15:30:21 2024, max compression
+gzip compressed data, was "ions-0.2.9.tar", last modified: Mon Apr  1 16:12:20 2024, max compression
```

## Comparing `ions-0.2.8.tar` & `ions-0.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.690105 ions-0.2.8/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.2.8/LICENSE
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.2.8/MANIFEST.in
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 15:30:21.689814 ions-0.2.8/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10819 2024-03-05 07:10:45.000000 ions-0.2.8/README.md
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.676555 ions-0.2.8/ions/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.2.8/ions/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7322 2023-12-29 14:18:01.000000 ions-0.2.8/ions/calculators.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688188 ions-0.2.8/ions/data/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.2.8/ions/data/Li2O_mp-1960.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.2.8/ions/data/bvparam_1991.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams2020-average.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams2020-average.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams_averaged2020.csv
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.2.8/ions/data/bvparm2020.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.2.8/ions/data/bvparm2020_edit.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvse_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvse_data.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.2.8/ions/data/elneg_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.2.8/ions/data/icsd_bv.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.2.8/ions/data/icsd_bv_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.2.8/ions/data/quantum_n.pkl
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-crystal.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-crystal.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-ionic.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-ionic.pickle
--rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.2.8/ions/data/shannon-radii.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-radii.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.2.8/ions/data.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2023-12-28 12:26:57.000000 ions-0.2.8/ions/decorator.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688544 ions-0.2.8/ions/featurizers/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.2.8/ions/featurizers/__init__.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688909 ions-0.2.8/ions/geom/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       22 2024-04-01 10:11:35.000000 ions-0.2.8/ions/geom/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     8649 2024-04-01 15:27:28.000000 ions-0.2.8/ions/geom/edge.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.2.8/ions/potential.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.689432 ions-0.2.8/ions/tools/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       86 2024-04-01 14:11:28.000000 ions-0.2.8/ions/tools/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19592 2024-04-01 14:15:22.000000 ions-0.2.8/ions/tools/path_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7061 2024-03-04 19:36:00.000000 ions-0.2.8/ions/tools/saddle_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4230 2024-04-01 12:24:32.000000 ions-0.2.8/ions/utils.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.677497 ions-0.2.8/ions.egg-info/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1000 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/SOURCES.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/dependency_links.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/requires.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/top_level.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-01 15:30:21.690331 ions-0.2.8/setup.cfg
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-01 09:47:25.000000 ions-0.2.8/setup.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.339968 ions-0.2.9/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.2.9/LICENSE
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.2.9/MANIFEST.in
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 16:12:20.338857 ions-0.2.9/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10819 2024-03-05 07:10:45.000000 ions-0.2.9/README.md
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.318045 ions-0.2.9/ions/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.2.9/ions/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7322 2023-12-29 14:18:01.000000 ions-0.2.9/ions/calculators.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.335362 ions-0.2.9/ions/data/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.2.9/ions/data/Li2O_mp-1960.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.2.9/ions/data/bvparam_1991.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/bvparams2020-average.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/bvparams2020-average.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/bvparams_averaged2020.csv
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.2.9/ions/data/bvparm2020.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.2.9/ions/data/bvparm2020_edit.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/bvse_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/bvse_data.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.2.9/ions/data/elneg_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.2.9/ions/data/icsd_bv.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.2.9/ions/data/icsd_bv_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.2.9/ions/data/quantum_n.pkl
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/shannon-data-crystal.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/shannon-data-crystal.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/shannon-data-ionic.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/shannon-data-ionic.pickle
+-rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.2.9/ions/data/shannon-radii.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.2.9/ions/data/shannon-radii.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.2.9/ions/data.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2023-12-28 12:26:57.000000 ions-0.2.9/ions/decorator.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.335929 ions-0.2.9/ions/featurizers/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.2.9/ions/featurizers/__init__.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.336531 ions-0.2.9/ions/geom/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       22 2024-04-01 10:11:35.000000 ions-0.2.9/ions/geom/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     8929 2024-04-01 16:10:30.000000 ions-0.2.9/ions/geom/edge.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.2.9/ions/potential.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.338379 ions-0.2.9/ions/tools/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       86 2024-04-01 14:11:28.000000 ions-0.2.9/ions/tools/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19592 2024-04-01 14:15:22.000000 ions-0.2.9/ions/tools/path_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7061 2024-03-04 19:36:00.000000 ions-0.2.9/ions/tools/saddle_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4230 2024-04-01 12:24:32.000000 ions-0.2.9/ions/utils.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 16:12:20.321183 ions-0.2.9/ions.egg-info/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 16:12:20.000000 ions-0.2.9/ions.egg-info/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1000 2024-04-01 16:12:20.000000 ions-0.2.9/ions.egg-info/SOURCES.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-01 16:12:20.000000 ions-0.2.9/ions.egg-info/dependency_links.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-01 16:12:20.000000 ions-0.2.9/ions.egg-info/requires.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-01 16:12:20.000000 ions-0.2.9/ions.egg-info/top_level.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-01 16:12:20.340323 ions-0.2.9/setup.cfg
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-01 16:11:10.000000 ions-0.2.9/setup.py
```

### Comparing `ions-0.2.8/LICENSE` & `ions-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/PKG-INFO` & `ions-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.2.8/README.md` & `ions-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/calculators.py` & `ions-0.2.9/ions/calculators.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/Li2O_mp-1960.cif` & `ions-0.2.9/ions/data/Li2O_mp-1960.cif`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparam_1991.yaml` & `ions-0.2.9/ions/data/bvparam_1991.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparams2020-average.json` & `ions-0.2.9/ions/data/bvparams2020-average.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparams2020-average.pickle` & `ions-0.2.9/ions/data/bvparams2020-average.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparams_averaged2020.csv` & `ions-0.2.9/ions/data/bvparams_averaged2020.csv`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparm2020.cif` & `ions-0.2.9/ions/data/bvparm2020.cif`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvparm2020_edit.txt` & `ions-0.2.9/ions/data/bvparm2020_edit.txt`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvse_data.json` & `ions-0.2.9/ions/data/bvse_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/bvse_data.pickle` & `ions-0.2.9/ions/data/bvse_data.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/elneg_data.json` & `ions-0.2.9/ions/data/elneg_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/icsd_bv.yaml` & `ions-0.2.9/ions/data/icsd_bv.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/quantum_n.pkl` & `ions-0.2.9/ions/data/quantum_n.pkl`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-data-crystal.json` & `ions-0.2.9/ions/data/shannon-data-crystal.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-data-crystal.pickle` & `ions-0.2.9/ions/data/shannon-data-crystal.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-data-ionic.json` & `ions-0.2.9/ions/data/shannon-data-ionic.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-data-ionic.pickle` & `ions-0.2.9/ions/data/shannon-data-ionic.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-radii.json` & `ions-0.2.9/ions/data/shannon-radii.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data/shannon-radii.pickle` & `ions-0.2.9/ions/data/shannon-radii.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/data.py` & `ions-0.2.9/ions/data.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/decorator.py` & `ions-0.2.9/ions/decorator.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/geom/edge.py` & `ions-0.2.9/ions/geom/edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,18 +201,26 @@
             distance, index = tree.query(p2_wrapped)
             assert distance < 1e-10
             source = self.source
             target = int(target_replicas[index])
         images = []
         freezed = np.array([i != source for i in range(len(supercell))])
         supercell.set_array('freezed', freezed)
-        base = supercell.copy()
+        #base = supercell.copy()
         traj = np.linspace(p1, p2, n_images)
         for p in traj:
-            image = base.copy()
+            image = supercell.copy()
             image.positions[source] = p
             image = image[[i for i in range(len(image)) if i != target]]
             images.append(image)
         return images
     
+    def centroid(self, cutoff = 8.0):
+        supercell, source, target = self.unwrap(cutoff=cutoff)
+        supercell.append('X')
+        p = (supercell.positions[source] + supercell.positions[target]) / 2
+        supercell.positions[-1] = p
+        return supercell
+
+    
     def __repr__(self):
         return f"Edge(source={self.source}, target={self.target}, offset={self.offset}), atoms={self.atoms}"
```

### Comparing `ions-0.2.8/ions/potential.py` & `ions-0.2.9/ions/potential.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/tools/path_finder.py` & `ions-0.2.9/ions/tools/path_finder.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/tools/saddle_finder.py` & `ions-0.2.9/ions/tools/saddle_finder.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions/utils.py` & `ions-0.2.9/ions/utils.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/ions.egg-info/PKG-INFO` & `ions-0.2.9/ions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.2.8/ions.egg-info/SOURCES.txt` & `ions-0.2.9/ions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ions-0.2.8/setup.py` & `ions-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='ions',  
-     version='0.2.8',
+     version='0.2.9',
      py_modules = ["ions"],
      install_requires = [
                          "ase>=3.22.1",
                          "numpy",
 			             "spglib",
                          "networkx",
                          "scipy",
```

