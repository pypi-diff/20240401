# Comparing `tmp/ions-0.2.7.tar.gz` & `tmp/ions-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ions-0.2.7.tar", last modified: Wed Mar  6 14:55:58 2024, max compression
+gzip compressed data, was "ions-0.2.8.tar", last modified: Mon Apr  1 15:30:21 2024, max compression
```

## Comparing `ions-0.2.7.tar` & `ions-0.2.8.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-03-06 14:55:58.683129 ions-0.2.7/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.2.7/LICENSE
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.2.7/MANIFEST.in
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-03-06 14:55:58.682927 ions-0.2.7/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10819 2024-03-05 07:10:45.000000 ions-0.2.7/README.md
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-03-06 14:55:58.670704 ions-0.2.7/ions/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.2.7/ions/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7322 2023-12-29 14:18:01.000000 ions-0.2.7/ions/calculators.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-03-06 14:55:58.681446 ions-0.2.7/ions/data/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.2.7/ions/data/Li2O_mp-1960.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.2.7/ions/data/bvparam_1991.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/bvparams2020-average.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/bvparams2020-average.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/bvparams_averaged2020.csv
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.2.7/ions/data/bvparm2020.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.2.7/ions/data/bvparm2020_edit.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/bvse_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/bvse_data.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.2.7/ions/data/elneg_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.2.7/ions/data/icsd_bv.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.2.7/ions/data/icsd_bv_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.2.7/ions/data/quantum_n.pkl
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/shannon-data-crystal.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/shannon-data-crystal.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/shannon-data-ionic.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/shannon-data-ionic.pickle
--rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.2.7/ions/data/shannon-radii.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.2.7/ions/data/shannon-radii.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.2.7/ions/data.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2023-12-28 12:26:57.000000 ions-0.2.7/ions/decorator.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.2.7/ions/potential.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-03-06 14:55:58.682527 ions-0.2.7/ions/tools/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       83 2024-01-10 09:49:05.000000 ions-0.2.7/ions/tools/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19386 2024-03-06 14:39:21.000000 ions-0.2.7/ions/tools/perconeb.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7061 2024-03-04 19:36:00.000000 ions-0.2.7/ions/tools/saddle_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4244 2023-12-28 12:19:50.000000 ions-0.2.7/ions/utils.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-03-06 14:55:58.671553 ions-0.2.7/ions.egg-info/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-03-06 14:55:58.000000 ions-0.2.7/ions.egg-info/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      928 2024-03-06 14:55:58.000000 ions-0.2.7/ions.egg-info/SOURCES.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-03-06 14:55:58.000000 ions-0.2.7/ions.egg-info/dependency_links.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       40 2024-03-06 14:55:58.000000 ions-0.2.7/ions.egg-info/requires.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-03-06 14:55:58.000000 ions-0.2.7/ions.egg-info/top_level.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-03-06 14:55:58.683218 ions-0.2.7/setup.cfg
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1500 2024-03-06 14:55:47.000000 ions-0.2.7/setup.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.690105 ions-0.2.8/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.2.8/LICENSE
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.2.8/MANIFEST.in
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 15:30:21.689814 ions-0.2.8/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10819 2024-03-05 07:10:45.000000 ions-0.2.8/README.md
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.676555 ions-0.2.8/ions/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.2.8/ions/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7322 2023-12-29 14:18:01.000000 ions-0.2.8/ions/calculators.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688188 ions-0.2.8/ions/data/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.2.8/ions/data/Li2O_mp-1960.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.2.8/ions/data/bvparam_1991.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams2020-average.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams2020-average.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvparams_averaged2020.csv
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.2.8/ions/data/bvparm2020.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.2.8/ions/data/bvparm2020_edit.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvse_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/bvse_data.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.2.8/ions/data/elneg_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.2.8/ions/data/icsd_bv.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.2.8/ions/data/icsd_bv_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.2.8/ions/data/quantum_n.pkl
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-crystal.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-crystal.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-ionic.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-data-ionic.pickle
+-rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.2.8/ions/data/shannon-radii.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.2.8/ions/data/shannon-radii.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.2.8/ions/data.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2023-12-28 12:26:57.000000 ions-0.2.8/ions/decorator.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688544 ions-0.2.8/ions/featurizers/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.2.8/ions/featurizers/__init__.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.688909 ions-0.2.8/ions/geom/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       22 2024-04-01 10:11:35.000000 ions-0.2.8/ions/geom/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     8649 2024-04-01 15:27:28.000000 ions-0.2.8/ions/geom/edge.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2023-12-29 18:07:12.000000 ions-0.2.8/ions/potential.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.689432 ions-0.2.8/ions/tools/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       86 2024-04-01 14:11:28.000000 ions-0.2.8/ions/tools/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    19592 2024-04-01 14:15:22.000000 ions-0.2.8/ions/tools/path_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     7061 2024-03-04 19:36:00.000000 ions-0.2.8/ions/tools/saddle_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4230 2024-04-01 12:24:32.000000 ions-0.2.8/ions/utils.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-01 15:30:21.677497 ions-0.2.8/ions.egg-info/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11535 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1000 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/SOURCES.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/dependency_links.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/requires.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-01 15:30:21.000000 ions-0.2.8/ions.egg-info/top_level.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-01 15:30:21.690331 ions-0.2.8/setup.cfg
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-01 09:47:25.000000 ions-0.2.8/setup.py
```

### Comparing `ions-0.2.7/LICENSE` & `ions-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/PKG-INFO` & `ions-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.2.7/README.md` & `ions-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/calculators.py` & `ions-0.2.8/ions/calculators.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/Li2O_mp-1960.cif` & `ions-0.2.8/ions/data/Li2O_mp-1960.cif`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparam_1991.yaml` & `ions-0.2.8/ions/data/bvparam_1991.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparams2020-average.json` & `ions-0.2.8/ions/data/bvparams2020-average.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparams2020-average.pickle` & `ions-0.2.8/ions/data/bvparams2020-average.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparams_averaged2020.csv` & `ions-0.2.8/ions/data/bvparams_averaged2020.csv`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparm2020.cif` & `ions-0.2.8/ions/data/bvparm2020.cif`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvparm2020_edit.txt` & `ions-0.2.8/ions/data/bvparm2020_edit.txt`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvse_data.json` & `ions-0.2.8/ions/data/bvse_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/bvse_data.pickle` & `ions-0.2.8/ions/data/bvse_data.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/elneg_data.json` & `ions-0.2.8/ions/data/elneg_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/icsd_bv.yaml` & `ions-0.2.8/ions/data/icsd_bv.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/quantum_n.pkl` & `ions-0.2.8/ions/data/quantum_n.pkl`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-data-crystal.json` & `ions-0.2.8/ions/data/shannon-data-crystal.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-data-crystal.pickle` & `ions-0.2.8/ions/data/shannon-data-crystal.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-data-ionic.json` & `ions-0.2.8/ions/data/shannon-data-ionic.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-data-ionic.pickle` & `ions-0.2.8/ions/data/shannon-data-ionic.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-radii.json` & `ions-0.2.8/ions/data/shannon-radii.json`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data/shannon-radii.pickle` & `ions-0.2.8/ions/data/shannon-radii.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/data.py` & `ions-0.2.8/ions/data.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/decorator.py` & `ions-0.2.8/ions/decorator.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/potential.py` & `ions-0.2.8/ions/potential.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/tools/perconeb.py` & `ions-0.2.8/ions/tools/path_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ase.neb import NEB
 from ase.spacegroup import get_spacegroup
 from ase.neighborlist import neighbor_list
 from ase.build import make_supercell
 from ase.data import covalent_radii
 from spglib import get_symmetry_dataset
 from spglib import standardize_cell
+
+from ions.geom import Edge
 #from ions.tools import SaddleFinder
 
 __version__ = "0.1"
         
 class PathFinder:
     
     """ 
@@ -357,15 +359,21 @@
         mask = self._filter_edges(tr = tr, cutoff = cutoff)
         #self.accepted_mask = mask
         s = np.vstack(self.mobile_atoms.get_array('sym_label')[self.w[:, :2] - self.w[:, :2].min()][mask]) # ?
         s.sort(axis = 1)
         d = self.distances[mask].round(3)
         j = self.jump_distances[mask].round(3)
         unique_pairs, idx, inverse = np.unique(np.column_stack((s, d, j)), axis = 0, return_index = True, return_inverse = True)
-        return self.w[mask][idx], unique_pairs
+        edges = []
+        for e in self.w[mask][idx]:
+            edge = Edge(self.atoms, e[0], e[1], e[2:])
+            edges.append(edge)
+
+        #return self.w[mask][idx], unique_pairs
+        return edges, unique_pairs
 
 
 
     def create_percotraj(self, cutoff, tr, spacing = 0.5):
 
         """creates a [2, 2, 2] supercell of the mobile sublattice
            and adds linearly interpolated segments for accepted jumps
```

### Comparing `ions-0.2.7/ions/tools/saddle_finder.py` & `ions-0.2.8/ions/tools/saddle_finder.py`

 * *Files identical despite different names*

### Comparing `ions-0.2.7/ions/utils.py` & `ions-0.2.8/ions/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,9 @@
     y = X[:, 1]
     z = X[:, 2]
     x0 = center.copy().positions[source]
     def dist_func(x0):
         return sum(((np.full(len(x),x0[0])-x)**2+(np.full(len(x),x0[1])-y)**2+(np.full(len(x),x0[2])-z)**2)**(1/2))
     
     bounds = ((x0[0] - 0.25, x0[0] + 0.25),(x0[1] - 0.25, x0[1] + 0.25), (x0[2] - 0.25, x0[2] + 0.25))
-    res = minimize(dist_func, x0, method='nelder-mead', options={'xtol': 1e-8, 'disp': False}, bounds=bounds)
+    res = minimize(dist_func, x0, method='nelder-mead', options={'disp': False}, bounds=bounds)
     return res.x, x0
```

### Comparing `ions-0.2.7/ions.egg-info/PKG-INFO` & `ions-0.2.8/ions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.2.7/ions.egg-info/SOURCES.txt` & `ions-0.2.8/ions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,10 +28,13 @@
 ions/data/quantum_n.pkl
 ions/data/shannon-data-crystal.json
 ions/data/shannon-data-crystal.pickle
 ions/data/shannon-data-ionic.json
 ions/data/shannon-data-ionic.pickle
 ions/data/shannon-radii.json
 ions/data/shannon-radii.pickle
+ions/featurizers/__init__.py
+ions/geom/__init__.py
+ions/geom/edge.py
 ions/tools/__init__.py
-ions/tools/perconeb.py
+ions/tools/path_finder.py
 ions/tools/saddle_finder.py
```

### Comparing `ions-0.2.7/setup.py` & `ions-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='ions',  
-     version='0.2.7',
+     version='0.2.8',
      py_modules = ["ions"],
      install_requires = [
                          "ase>=3.22.1",
                          "numpy",
 			             "spglib",
                          "networkx",
-                         "scipy"
+                         "scipy",
+                         "pymatgen"
                         ],
      author="Artem Dembitskiy",
      author_email="art.dembitskiy@gmail.com",
      description="A python library for studying percolation in solids",
      key_words = ['ionic', 'radius', 'bond valence'],
      long_description=long_description,
      long_description_content_type="text/markdown",
```

