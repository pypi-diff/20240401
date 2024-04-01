# Comparing `tmp/cvpack-0.8.0.tar.gz` & `tmp/cvpack-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvpack-0.8.0.tar", last modified: Wed Jan 31 20:09:36 2024, max compression
+gzip compressed data, was "cvpack-0.9.0.tar", last modified: Mon Feb 26 15:33:20 2024, max compression
```

## Comparing `cvpack-0.8.0.tar` & `cvpack-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-01-31 20:06:18.000000 cvpack-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-31 20:06:18.000000 cvpack-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-31 20:06:18.000000 cvpack-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-01-31 20:09:36.577996 cvpack-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-01-31 20:06:18.000000 cvpack-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/atomic_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/attraction_strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/base_radius_of_gyration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/base_rmsd_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/centroid_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/composite_rmsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12685 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/cvpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack/data/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/data/ideal_alpha_helix.csv
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/data/ideal_antiparallel_beta_sheet.csv
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/data/ideal_parallel_beta_sheet.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/helix_angle_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/helix_hbond_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/helix_rmsd_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/helix_torsion_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/number_of_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/radius_of_gyration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/radius_of_gyration_sq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/residue_coordination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/rmsd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack/serializer/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/serializer/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/sheet_rmsd_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29688 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/tests/test_cvpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/torsion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/torsion_similarity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack/unit/
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-01-31 20:06:18.000000 cvpack-0.8.0/cvpack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 20:09:36.577996 cvpack-0.8.0/cvpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 20:06:52.000000 cvpack-0.8.0/cvpack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-31 20:09:36.000000 cvpack-0.8.0/cvpack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-01-31 20:06:18.000000 cvpack-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-31 20:09:36.577996 cvpack-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-26 15:30:15.000000 cvpack-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-26 15:30:15.000000 cvpack-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-26 15:30:15.000000 cvpack-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-02-26 15:33:20.298384 cvpack-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-02-26 15:30:15.000000 cvpack-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.294384 cvpack-0.9.0/cvpack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14441 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/atomic_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/attraction_strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/base_custom_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/base_radius_of_gyration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/base_rmsd_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/centroid_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/composite_rmsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/cvpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/cvpack/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/data/ideal_alpha_helix.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/data/ideal_antiparallel_beta_sheet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/data/ideal_parallel_beta_sheet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/helix_angle_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/helix_hbond_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/helix_rmsd_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/helix_torsion_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/number_of_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/path_in_cv_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/radius_of_gyration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/radius_of_gyration_sq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/residue_coordination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/rmsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/cvpack/serializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/serializer/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/sheet_rmsd_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/cvpack/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31832 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/tests/test_cvpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/torsion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/torsion_similarity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/cvpack/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)    28195 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-02-26 15:30:15.000000 cvpack-0.9.0/cvpack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:33:20.298384 cvpack-0.9.0/cvpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 15:30:50.000000 cvpack-0.9.0/cvpack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-26 15:33:20.000000 cvpack-0.9.0/cvpack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-02-26 15:30:15.000000 cvpack-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-26 15:33:20.298384 cvpack-0.9.0/setup.cfg
```

### Comparing `cvpack-0.8.0/CODE_OF_CONDUCT.md` & `cvpack-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/LICENSE` & `cvpack-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/PKG-INFO` & `cvpack-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpack
-Version: 0.8.0
+Version: 0.9.0
 Summary: Useful Collective Variables for OpenMM
 Author-email: Charlles Abreu <craabreu@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -61,22 +61,30 @@
 | [Composite RMSD]        | multibody RMSD with concerted-rotation alignment                 |
 | [Distance]              | distance between two atoms                                       |
 | [Helix angle content]   | alpha-helix angle content of a sequence of residues              |
 | [Helix H-bond content]  | alpha-helix hydrogen-bond content of a sequence of residues      |
 | [Helix RMSD content]    | alpha-helix RMSD content of a sequence of residues               |
 | [Helix torsion content] | alpha-helix Ramachandran content of a sequence of residues       |
 | [Number of contacts]    | number of contacts between two groups of atoms                   |
+| [PathInCVSpace]         | progress along (deviation from) a predefined path in CV space    |
 | [Radius of gyration]    | radius of gyration of a group of atoms                           |
 | [(Radius of gyration)^2]| square of the radius of gyration of a group of atoms             |
 | [Residue coordination]  | number of contacts between two disjoint groups of residues       |
 | [RMSD]                  | root-mean-square deviation with respect to a reference structure |
 | [Sheet RMSD content]    | beta-sheet RMSD content of a sequence of residues                |
 | [Torsion]               | torsion angle formed by four atoms                               |
 | [Torsion similarity]    | degree of similarity between pairs of torsion angles             |
 
+Below is a list of new CVs already available in the development version:
+
+| Collective Variable     | Description                                                      |
+|-------------------------|------------------------------------------------------------------|
+| [PathInCVSpace]         | progress along (or deviation from) a predefined path in CV space |
+
+
 ### Installation and Usage
 
 CVPack is available as a conda package on the
 [mdtools](https://anaconda.org/mdtools/cvpack) channel. To install it, run:
 
 ```bash
     conda install -c conda-forge -c mdtools cvpack
@@ -112,25 +120,27 @@
 [CollectiveVariable]: https://ufedmm.readthedocs.io/en/latest/pythonapi/ufedmm.html#ufedmm.ufedmm.CollectiveVariable
 [CustomCVForce]:      https://docs.openmm.org/latest/api-python/generated/openmm.openmm.CustomCVForce.html
 [Force]:              https://docs.openmm.org/latest/api-python/generated/openmm.openmm.Force.html
 [Metadynamics]:       https://docs.openmm.org/latest/api-python/generated/openmm.app.metadynamics.Metadynamics.html
 [OpenMM]:             https://openmm.org
 [UFED]:               https://ufedmm.readthedocs.io/en/latest/index.html
 
-[Angle]:                  https://redesignscience.github.io/cvpack/api/Angle.html
-[Atomic Function]:        https://redesignscience.github.io/cvpack/api/AtomicFunction.html
-[Attraction Strength]:    https://redesignscience.github.io/cvpack/api/AttractionStrength.html
-[Centroid Function]:      https://redesignscience.github.io/cvpack/api/CentroidFunction.html
-[Composite RMSD]:         https://redesignscience.github.io/cvpack/api/CompositeRMSD.html
-[Distance]:               https://redesignscience.github.io/cvpack/api/Distance.html
-[Helix angle content]:    https://redesignscience.github.io/cvpack/api/HelixAngleContent.html
-[Helix H-bond content]:   https://redesignscience.github.io/cvpack/api/HelixHBondContent.html
-[Helix RMSD content]:     https://redesignscience.github.io/cvpack/api/HelixRMSDContent.html
-[Helix torsion content]:  https://redesignscience.github.io/cvpack/api/HelixTorsionContent.html
-[Number of contacts]:     https://redesignscience.github.io/cvpack/api/NumberOfContacts.html
-[Radius of gyration]:     https://redesignscience.github.io/cvpack/api/RadiusOfGyration.html
-[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/api/RadiusOfGyrationSq.html
-[Residue coordination]:   https://redesignscience.github.io/cvpack/api/ResidueCoordination.html
-[RMSD]:                   https://redesignscience.github.io/cvpack/api/RMSD.html
-[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/api/SheetRMSDContent.html
-[Torsion]:                https://redesignscience.github.io/cvpack/api/Torsion.html
-[Torsion similarity]:     https://redesignscience.github.io/cvpack/api/TorsionSimilarity.html
+[Angle]:                  https://redesignscience.github.io/cvpack/latest/api/Angle.html
+[Atomic Function]:        https://redesignscience.github.io/cvpack/latest/api/AtomicFunction.html
+[Attraction Strength]:    https://redesignscience.github.io/cvpack/latest/api/AttractionStrength.html
+[Centroid Function]:      https://redesignscience.github.io/cvpack/latest/api/CentroidFunction.html
+[Composite RMSD]:         https://redesignscience.github.io/cvpack/latest/api/CompositeRMSD.html
+[Distance]:               https://redesignscience.github.io/cvpack/latest/api/Distance.html
+[Helix angle content]:    https://redesignscience.github.io/cvpack/latest/api/HelixAngleContent.html
+[Helix H-bond content]:   https://redesignscience.github.io/cvpack/latest/api/HelixHBondContent.html
+[Helix RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/HelixRMSDContent.html
+[Helix torsion content]:  https://redesignscience.github.io/cvpack/latest/api/HelixTorsionContent.html
+[Number of contacts]:     https://redesignscience.github.io/cvpack/latest/api/NumberOfContacts.html
+[Radius of gyration]:     https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyration.html
+[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyrationSq.html
+[Residue coordination]:   https://redesignscience.github.io/cvpack/latest/api/ResidueCoordination.html
+[RMSD]:                   https://redesignscience.github.io/cvpack/latest/api/RMSD.html
+[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/SheetRMSDContent.html
+[Torsion]:                https://redesignscience.github.io/cvpack/latest/api/Torsion.html
+[Torsion similarity]:     https://redesignscience.github.io/cvpack/latest/api/TorsionSimilarity.html
+
+[PathInCVSpace]:          https://redesignscience.github.io/cvpack/development/api/PathInCVSpace.html
```

### Comparing `cvpack-0.8.0/README.md` & `cvpack-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,30 @@
 | [Composite RMSD]        | multibody RMSD with concerted-rotation alignment                 |
 | [Distance]              | distance between two atoms                                       |
 | [Helix angle content]   | alpha-helix angle content of a sequence of residues              |
 | [Helix H-bond content]  | alpha-helix hydrogen-bond content of a sequence of residues      |
 | [Helix RMSD content]    | alpha-helix RMSD content of a sequence of residues               |
 | [Helix torsion content] | alpha-helix Ramachandran content of a sequence of residues       |
 | [Number of contacts]    | number of contacts between two groups of atoms                   |
+| [PathInCVSpace]         | progress along (deviation from) a predefined path in CV space    |
 | [Radius of gyration]    | radius of gyration of a group of atoms                           |
 | [(Radius of gyration)^2]| square of the radius of gyration of a group of atoms             |
 | [Residue coordination]  | number of contacts between two disjoint groups of residues       |
 | [RMSD]                  | root-mean-square deviation with respect to a reference structure |
 | [Sheet RMSD content]    | beta-sheet RMSD content of a sequence of residues                |
 | [Torsion]               | torsion angle formed by four atoms                               |
 | [Torsion similarity]    | degree of similarity between pairs of torsion angles             |
 
+Below is a list of new CVs already available in the development version:
+
+| Collective Variable     | Description                                                      |
+|-------------------------|------------------------------------------------------------------|
+| [PathInCVSpace]         | progress along (or deviation from) a predefined path in CV space |
+
+
 ### Installation and Usage
 
 CVPack is available as a conda package on the
 [mdtools](https://anaconda.org/mdtools/cvpack) channel. To install it, run:
 
 ```bash
     conda install -c conda-forge -c mdtools cvpack
@@ -93,25 +101,27 @@
 [CollectiveVariable]: https://ufedmm.readthedocs.io/en/latest/pythonapi/ufedmm.html#ufedmm.ufedmm.CollectiveVariable
 [CustomCVForce]:      https://docs.openmm.org/latest/api-python/generated/openmm.openmm.CustomCVForce.html
 [Force]:              https://docs.openmm.org/latest/api-python/generated/openmm.openmm.Force.html
 [Metadynamics]:       https://docs.openmm.org/latest/api-python/generated/openmm.app.metadynamics.Metadynamics.html
 [OpenMM]:             https://openmm.org
 [UFED]:               https://ufedmm.readthedocs.io/en/latest/index.html
 
-[Angle]:                  https://redesignscience.github.io/cvpack/api/Angle.html
-[Atomic Function]:        https://redesignscience.github.io/cvpack/api/AtomicFunction.html
-[Attraction Strength]:    https://redesignscience.github.io/cvpack/api/AttractionStrength.html
-[Centroid Function]:      https://redesignscience.github.io/cvpack/api/CentroidFunction.html
-[Composite RMSD]:         https://redesignscience.github.io/cvpack/api/CompositeRMSD.html
-[Distance]:               https://redesignscience.github.io/cvpack/api/Distance.html
-[Helix angle content]:    https://redesignscience.github.io/cvpack/api/HelixAngleContent.html
-[Helix H-bond content]:   https://redesignscience.github.io/cvpack/api/HelixHBondContent.html
-[Helix RMSD content]:     https://redesignscience.github.io/cvpack/api/HelixRMSDContent.html
-[Helix torsion content]:  https://redesignscience.github.io/cvpack/api/HelixTorsionContent.html
-[Number of contacts]:     https://redesignscience.github.io/cvpack/api/NumberOfContacts.html
-[Radius of gyration]:     https://redesignscience.github.io/cvpack/api/RadiusOfGyration.html
-[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/api/RadiusOfGyrationSq.html
-[Residue coordination]:   https://redesignscience.github.io/cvpack/api/ResidueCoordination.html
-[RMSD]:                   https://redesignscience.github.io/cvpack/api/RMSD.html
-[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/api/SheetRMSDContent.html
-[Torsion]:                https://redesignscience.github.io/cvpack/api/Torsion.html
-[Torsion similarity]:     https://redesignscience.github.io/cvpack/api/TorsionSimilarity.html
+[Angle]:                  https://redesignscience.github.io/cvpack/latest/api/Angle.html
+[Atomic Function]:        https://redesignscience.github.io/cvpack/latest/api/AtomicFunction.html
+[Attraction Strength]:    https://redesignscience.github.io/cvpack/latest/api/AttractionStrength.html
+[Centroid Function]:      https://redesignscience.github.io/cvpack/latest/api/CentroidFunction.html
+[Composite RMSD]:         https://redesignscience.github.io/cvpack/latest/api/CompositeRMSD.html
+[Distance]:               https://redesignscience.github.io/cvpack/latest/api/Distance.html
+[Helix angle content]:    https://redesignscience.github.io/cvpack/latest/api/HelixAngleContent.html
+[Helix H-bond content]:   https://redesignscience.github.io/cvpack/latest/api/HelixHBondContent.html
+[Helix RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/HelixRMSDContent.html
+[Helix torsion content]:  https://redesignscience.github.io/cvpack/latest/api/HelixTorsionContent.html
+[Number of contacts]:     https://redesignscience.github.io/cvpack/latest/api/NumberOfContacts.html
+[Radius of gyration]:     https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyration.html
+[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyrationSq.html
+[Residue coordination]:   https://redesignscience.github.io/cvpack/latest/api/ResidueCoordination.html
+[RMSD]:                   https://redesignscience.github.io/cvpack/latest/api/RMSD.html
+[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/SheetRMSDContent.html
+[Torsion]:                https://redesignscience.github.io/cvpack/latest/api/Torsion.html
+[Torsion similarity]:     https://redesignscience.github.io/cvpack/latest/api/TorsionSimilarity.html
+
+[PathInCVSpace]:          https://redesignscience.github.io/cvpack/development/api/PathInCVSpace.html
```

### Comparing `cvpack-0.8.0/cvpack/__init__.py` & `cvpack-0.9.0/cvpack/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 """Useful Collective Variables for OpenMM"""
 
+import yaml
+
 # Add imports here
 from ._version import __version__  # noqa: F401
 from .angle import Angle  # noqa: F401
 from .atomic_function import AtomicFunction  # noqa: F401
 from .attraction_strength import AttractionStrength  # noqa: F401
 from .centroid_function import CentroidFunction  # noqa: F401
 from .composite_rmsd import CompositeRMSD  # noqa: F401
 from .distance import Distance  # noqa: F401
 from .helix_angle_content import HelixAngleContent  # noqa: F401
 from .helix_hbond_content import HelixHBondContent  # noqa: F401
 from .helix_rmsd_content import HelixRMSDContent  # noqa: F401
 from .helix_torsion_content import HelixTorsionContent  # noqa: F401
 from .number_of_contacts import NumberOfContacts  # noqa: F401
+from .path_in_cv_space import PathInCVSpace  # noqa: F401
 from .radius_of_gyration import RadiusOfGyration  # noqa: F401
 from .radius_of_gyration_sq import RadiusOfGyrationSq  # noqa: F401
 from .residue_coordination import ResidueCoordination  # noqa: F401
 from .rmsd import RMSD  # noqa: F401
 from .sheet_rmsd_content import SheetRMSDContent  # noqa: F401
 from .torsion import Torsion  # noqa: F401
 from .torsion_similarity import TorsionSimilarity  # noqa: F401
+
+for _cv in [
+    Angle,
+    AtomicFunction,
+    AttractionStrength,
+    CentroidFunction,
+    CompositeRMSD,
+    Distance,
+    HelixAngleContent,
+    HelixHBondContent,
+    HelixRMSDContent,
+    HelixTorsionContent,
+    NumberOfContacts,
+    PathInCVSpace,
+    RadiusOfGyration,
+    RadiusOfGyrationSq,
+    ResidueCoordination,
+    RMSD,
+    SheetRMSDContent,
+    Torsion,
+    TorsionSimilarity,
+]:
+    yaml.SafeDumper.add_representer(_cv, _cv.to_yaml)
+    yaml.SafeLoader.add_constructor(_cv.yaml_tag, _cv.from_yaml)
+del _cv
```

### Comparing `cvpack-0.8.0/cvpack/angle.py` & `cvpack-0.9.0/cvpack/angle.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
    :platform: Linux, MacOS, Windows
    :synopsis: The angle formed by three atoms
 
 .. classauthor:: Charlles Abreu <craabreu@gmail.com>
 
 """
 
+import math
+
 import openmm
 
 from cvpack import unit as mmunit
 
 from .cvpack import BaseCollectiveVariable
 
 
@@ -54,12 +56,15 @@
         >>> positions = [[0, 0, 0], [1, 0, 0], [1, 1, 0]]
         >>> context.setPositions([openmm.Vec3(*pos) for pos in positions])
         >>> print(angle.getValue(context, digits=6))
         1.570796 rad
 
     """
 
+    yaml_tag = "!cvpack.Angle"
+
     def __init__(self, atom1: int, atom2: int, atom3: int, pbc: bool = False) -> None:
         super().__init__("theta")
         self.addAngle(atom1, atom2, atom3, [])
         self.setUsesPeriodicBoundaryConditions(pbc)
         self._registerCV(mmunit.radians, atom1, atom2, atom3, pbc)
+        self._registerPeriod(2 * math.pi)
```

### Comparing `cvpack-0.8.0/cvpack/atomic_function.py` & `cvpack-0.9.0/cvpack/atomic_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,39 +13,18 @@
 
 import numpy as np
 import openmm
 from numpy.typing import ArrayLike
 
 from cvpack import unit as mmunit
 
-from .cvpack import BaseCollectiveVariable
+from .base_custom_function import BaseCustomFunction
 
 
-def _add_parameters(
-    force: openmm.Force,
-    size: int,
-    **parameters: t.Union[mmunit.ScalarQuantity, t.Sequence[mmunit.ScalarQuantity]],
-) -> t.List[t.Union[float, t.Sequence[mmunit.ScalarQuantity]]]:
-    perbond_parameters = []
-    for name, data in parameters.items():
-        if isinstance(data, mmunit.Quantity):
-            data = data.value_in_unit_system(mmunit.md_unit_system)
-        if isinstance(data, t.Sequence):
-            if len(data) != size:
-                raise ValueError(
-                    f"The length of parameter {name} is {len(data)}. Should be {size}."
-                )
-            force.addPerBondParameter(name)
-            perbond_parameters.append(data)
-        else:
-            force.addGlobalParameter(name, data)
-    return perbond_parameters
-
-
-class AtomicFunction(openmm.CustomCompoundBondForce, BaseCollectiveVariable):
+class AtomicFunction(openmm.CustomCompoundBondForce, BaseCustomFunction):
     r"""
     A generic function of the coordinates of atoms split into `m` groups of `n`
     atoms each:
 
     .. math::
 
         f({\bf r}) = \sum_{i=1}^m F\left(
@@ -66,23 +45,25 @@
     function
         The function to be evaluated. It must be a valid
         :OpenMM:`CustomCompoundBondForce` expression
     groups
         The indices of the atoms in each group, passed as a 2D array-like object of
         shape `(m, n)`, where `m` is the number of groups and `n` is the number of
         atoms per group. If a 1D object is passed, it is assumed that `m` is 1 and
-        `n` is the length of the object.
+        `n` is the length of the object
     unit
         The unit of measurement of the collective variable. It must be compatible
         with the MD unit system (mass in `daltons`, distance in `nanometers`, time
         in `picoseconds`, temperature in `kelvin`, energy in `kilojoules_per_mol`,
         angle in `radians`). If the collective variables does not have a unit, use
         `unit.dimensionless`
+    period
+        The period of the collective variable if it is periodic, or `None` if it is not
     pbc
-        Whether to use periodic boundary conditions
+        Whether to use periodic boundary conditions when computing atomic distances
 
     Keyword Args
     ------------
     **parameters
         The named parameters of the function. Each parameter can be a scalar
         quantity or a 1D array-like object of length `m`, where `m` is the number of
         groups. In the latter case, each entry of the array is used for the
@@ -122,34 +103,40 @@
         >>> theta2 = angle2.getValue(context).value_in_unit(openmm.unit.radian)
         >>> print(round(500*((theta1 - np.pi/2)**2 + (theta2 - np.pi/3)**2), 3))
         429.479
         >>> print(colvar.getValue(context, digits=6))
         429.479 kJ/mol
     """
 
+    yaml_tag = "!cvpack.AtomicFunction"
+
+    @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         function: str,
         unit: mmunit.Unit,
         groups: ArrayLike,
+        period: t.Optional[mmunit.ScalarQuantity] = None,
         pbc: bool = True,
-        **parameters: t.Union[mmunit.ScalarQuantity, t.Sequence[mmunit.ScalarQuantity]],
+        **parameters: t.Union[mmunit.ScalarQuantity, mmunit.VectorQuantity],
     ) -> None:
         groups = np.atleast_2d(groups)
-        num_groups, atoms_per_group, *others = groups.shape
-        if others:
+        num_groups, atoms_per_group, *other_dimensions = groups.shape
+        if other_dimensions:
             raise ValueError("Array `groups` cannot have more than 2 dimensions")
         super().__init__(atoms_per_group, function)
-        perbond_parameters = _add_parameters(self, num_groups, **parameters)
-        for group, *values in zip(groups, *perbond_parameters):
-            self.addBond(group, values)
-        self.setUsesPeriodicBoundaryConditions(pbc)
-        self._checkUnitCompatibility(unit)
+        overalls, perbonds = self._extractParameters(num_groups, **parameters)
+        self._addParameters(overalls, perbonds, groups, pbc, unit)
         unit = mmunit.SerializableUnit(unit)
-        self._registerCV(unit, function, unit, groups, pbc, **parameters)
+        groups = [list(map(int, group)) for group in groups]
+        self._registerCV(
+            unit, function, unit, groups, period, pbc, **overalls, **perbonds
+        )
+        if period is not None:
+            self._registerPeriod(period)
 
     @classmethod
     def _fromCustomForce(
         cls,
         force: t.Union[
             openmm.CustomAngleForce,
             openmm.CustomBondForce,
```

### Comparing `cvpack-0.8.0/cvpack/attraction_strength.py` & `cvpack-0.9.0/cvpack/attraction_strength.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class AttractionStrength(openmm.CustomNonbondedForce, BaseCollectiveVariable):
     r"""
     The strength of the attraction between two atom groups:
 
     .. math::
 
-        S_{\rm attr}({\bf r}) = &-\frac{1}{E_{\rm ref}} \Bigg[
+        S_{\rm attr}({\bf r}) = S_{1,2}({\bf r}) = &-\frac{1}{E_{\rm ref}} \Bigg[
             \sum_{i \in {\bf g}_1}
                 \sum_{\substack{j \in {\bf g}_2 \\ j \neq i}}
                     \epsilon_{ij} u_{\rm disp}\left(
                         \frac{\|{\bf r}_i - {\bf r}_j\|}{\sigma_{ij}}
                     \right) \\
             &+\sum_{i \in {\bf g}_1}
             \sum_{\substack{j \in {\bf g}_2 \\ q_jq_i < 0}}
@@ -41,14 +41,31 @@
     :math:`r_{\rm c}` is the cutoff distance, :math:`\varepsilon_0` is the
     permittivity of empty space, :math:`q_i` is the charge of atom :math:`i`, and
     :math:`E_{\rm ref}` is a reference value (in energy units per mole).
     The Lennard-Jones parameters are given by the Lorentz-Berthelot mixing rule, i.e.
     :math:`\epsilon_{ij} = \sqrt{\epsilon_i \epsilon_j}`, and
     :math:`\sigma_{ij} = (\sigma_i + \sigma_j)/2`.
 
+    Optionally, one can provide a third atom group :math:`{\bf g}_3` to contrast
+    the attraction strength between :math:`{\bf g}_1` and :math:`{\bf g}_2` with
+    that between :math:`{\bf g}_1` and :math:`{\bf g}_3`. In this case, the
+    collective variable becomes
+
+    .. math::
+
+        S_{\rm attr}({\bf r}) = S_{1,2}({\bf r}) - S_{1,3}({\bf r})
+
+    .. note::
+
+        Groups :math:`{\bf g}_1` and :math:`{\bf g}_2` can overlap or even be the
+        same, in which case the collective variable will measure the strength of
+        the self-attraction of :math:`{\bf g}_1`. On the other hand, the contrast
+        group :math:`{\bf g}_3` cannot overlap with neither :math:`{\bf g}_1` nor
+        :math:`{\bf g}_2`.
+
     The function :math:`u_{\rm disp}(x)` is a Lennard-Jones-like reduced potential with
     a highly softened repulsion part, defined as
 
     .. math::
 
         u_{\rm disp}(x) = 4\left(\frac{1}{y^2} - \frac{1}{y}\right),
         \quad \text{where} \quad
@@ -72,96 +89,97 @@
         adopted reference value.
 
     The Lennard-Jones parameters, atomic charges, cutoff distance, boundary conditions,
     as well as whether to use a switching function and its corresponding switching
     distance, are taken from :openmm:`NonbondedForce` object.
 
     .. note::
-        Any non-exclusion exceptions involving atoms in :math:`{\bf g}_1` and
-        :math:`{\bf g}_2` in the provided :class:`openmm.NonbondedForce` are turned
-        into exclusions in this collective variable.
+        Any non-exclusion exceptions involving an atom in :math:`{\bf g}_1` and an atom
+        in either :math:`{\bf g}_2` or :math:`{\bf g}_3` are turned into exclusions in
+        this collective variable.
 
     Parameters
     ----------
     group1
         The first atom group.
     group2
         The second atom group.
     nonbondedForce
         The :class:`openmm.NonbondedForce` object from which to collect the necessary
         parameters.
+    contrastGroup
+        An optional third atom group to contrast the attraction strength between
+        :math:`{\bf g}_1` and :math:`{\bf g}_2` with that between :math:`{\bf g}_1`
+        and :math:`{\bf g}_3`.
     reference
         A reference value (in energy units per mole) to which the collective variable
         should be normalized. One can also provide an :OpenMM:`Context` object from
-        which to obtain a reference attraction strength.
+        which to extract a reference attraction strength. The extracted value will be
+        :math:`S_{1,2}({\bf r})` for :math:`E_{\rm ref} = 1`, regardless of whether
+        `contrastGroup` is provided or not.
 
     Examples
     --------
     >>> import cvpack
     >>> from openmm import unit
     >>> from openmmtools import testsystems
     >>> model = testsystems.HostGuestExplicit()
-    >>> group1, group2 = [], []
-    >>> for residue in model.topology.residues():
-    ...     if residue.name != "HOH":
-    ...         group = group1 if residue.name == "B2" else group2
-    ...         group.extend(atom.index for atom in residue.atoms())
+    >>> guest = [a.index for a in model.topology.atoms() if a.residue.name == "B2"]
+    >>> host = [a.index for a in model.topology.atoms() if a.residue.name == "CUC"]
     >>> forces = {f.getName(): f for f in model.system.getForces()}
-    >>> cv1 = cvpack.AttractionStrength(group1, group2, forces["NonbondedForce"])
-    >>> cv1.setUnusedForceGroup(0, model.system)
-    1
-    >>> model.system.addForce(cv1)
-    5
-    >>> cv2 = cvpack.AttractionStrength(
-    ...     group1, group2, forces["NonbondedForce"], 100*unit.kilojoules_per_mole,
-    ... )
-    >>> cv2.setUnusedForceGroup(0, model.system)
-    2
-    >>> model.system.addForce(cv2)
-    6
+    >>> cv1 = cvpack.AttractionStrength(guest, host, forces["NonbondedForce"])
+    >>> _ = cv1.setUnusedForceGroup(0, model.system)
+    >>> _ = model.system.addForce(cv1)
     >>> platform = openmm.Platform.getPlatformByName("Reference")
     >>> integrator = openmm.VerletIntegrator(1.0 * mmunit.femtoseconds)
     >>> context = openmm.Context(model.system, integrator, platform)
     >>> context.setPositions(model.positions)
     >>> print(cv1.getValue(context, 4))
     4912.5 dimensionless
-    >>> print(cv1.getEffectiveMass(context, 4))
-    2.1639e-07 nm**2 Da
+
+    >>> water = [a.index for a in model.topology.atoms() if a.residue.name == "HOH"]
+    >>> cv2 = cvpack.AttractionStrength(guest, water, forces["NonbondedForce"])
+    >>> _ = cv2.setUnusedForceGroup(0, model.system)
+    >>> _ = model.system.addForce(cv2)
+    >>> context.reinitialize(preserveState=True)
     >>> print(cv2.getValue(context, 4))
-    49.125 dimensionless
-    >>> print(cv2.getEffectiveMass(context, 4))
-    0.0021639 nm**2 Da
-    >>> cv3 = cvpack.AttractionStrength(
-    ...     group1, group2, forces["NonbondedForce"], context,
-    ... )
-    >>> cv3.setUnusedForceGroup(0, model.system)
-    3
-    >>> model.system.addForce(cv3)
-    7
+    2063.3 dimensionless
+
+    >>> cv3 = cvpack.AttractionStrength(guest, host, forces["NonbondedForce"], water)
+    >>> _ = cv3.setUnusedForceGroup(0, model.system)
+    >>> _ = model.system.addForce(cv3)
     >>> context.reinitialize(preserveState=True)
     >>> print(cv3.getValue(context, 4))
-    1.0 dimensionless
-    >>> print(cv3.getEffectiveMass(context, 4))
-    5.2222 nm**2 Da
+    2849.2 dimensionless
+    >>> print(cv1.getValue(context, 4) - cv2.getValue(context, 4))
+    2849.2 dimensionless
     """
 
+    yaml_tag = "!cvpack.AttractionStrength"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        group1: t.Sequence[int],
-        group2: t.Sequence[int],
+        group1: t.Iterable[int],
+        group2: t.Iterable[int],
         nonbondedForce: openmm.NonbondedForce,
+        contrastGroup: t.Optional[t.Iterable[int]] = None,
         reference: t.Union[mmunit.ScalarQuantity, openmm.Context] = mmunit.Quantity(
             1.0, mmunit.kilojoule_per_mole
         ),
     ) -> None:
+        group1 = list(group1)
+        group2 = list(group2)
+        contrasting = contrastGroup is not None
+        if contrasting:
+            contrastGroup = list(contrastGroup)
         nonbondedForce = NonbondedForceSurrogate(nonbondedForce)
         cutoff = nonbondedForce.getCutoffDistance()
         expression = (
-            "-(lj + coul)/ref"
+            f"-(lj + coul){'*sign1*sign2' if contrasting else ''}/ref"
             "; lj = 4*epsilon*(1/y^2 - 1/y)"
             f"; coul = {ONE_4PI_EPS0}*q1q2*(1/x + (x^2 - 3)/2)"
             f"; x = r/{cutoff}"
             "; y = abs((r/sigma)^6 - 2) + 2"
             "; q1q2 = min(0, charge1*charge2)"
             "; epsilon = sqrt(epsilon1*epsilon2)"
             "; sigma = (sigma1 + sigma2)/2"
@@ -169,24 +187,35 @@
         )
         super().__init__(expression)
         if nonbondedForce.usesPeriodicBoundaryConditions():
             self.setNonbondedMethod(self.CutoffPeriodic)
         else:
             self.setNonbondedMethod(self.CutoffNonPeriodic)
         self.setCutoffDistance(cutoff)
-        for parameter in ("charge", "sigma", "epsilon"):
+        for parameter in ("charge", "sigma", "epsilon") + ("sign",) * contrasting:
             self.addPerParticleParameter(parameter)
         for atom in range(nonbondedForce.getNumParticles()):
-            self.addParticle(nonbondedForce.getParticleParameters(atom))
+            parameters = nonbondedForce.getParticleParameters(atom)
+            if contrasting:
+                parameters += (-1 if atom in contrastGroup else 1,)
+            self.addParticle(parameters)
         for exception in range(nonbondedForce.getNumExceptions()):
             i, j, *_ = nonbondedForce.getExceptionParameters(exception)
             self.addExclusion(i, j)
         self.setUseSwitchingFunction(nonbondedForce.getUseSwitchingFunction())
         self.setSwitchingDistance(nonbondedForce.getSwitchingDistance())
         self.setUseLongRangeCorrection(False)
         self.addInteractionGroup(group1, group2)
         if isinstance(reference, openmm.Context):
             reference = evaluate_in_context(self, reference)
         self.setEnergyFunction(expression.replace("ref = 1", f"ref = {reference}"))
+        if contrasting:
+            self.addInteractionGroup(group1, contrastGroup)
+        # pylint: disable=duplicate-code
         self._registerCV(
-            mmunit.dimensionless, group1, group2, nonbondedForce, reference
+            mmunit.dimensionless,
+            group1,
+            group2,
+            nonbondedForce,
+            contrastGroup,
+            reference,
         )
```

### Comparing `cvpack-0.8.0/cvpack/base_radius_of_gyration.py` & `cvpack-0.9.0/cvpack/base_radius_of_gyration.py`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/cvpack/base_rmsd_content.py` & `cvpack-0.9.0/cvpack/base_rmsd_content.py`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/cvpack/centroid_function.py` & `cvpack-0.9.0/cvpack/centroid_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,18 @@
 
 import numpy as np
 import openmm
 from numpy.typing import ArrayLike
 
 from cvpack import unit as mmunit
 
-from .atomic_function import _add_parameters
-from .cvpack import BaseCollectiveVariable
+from .base_custom_function import BaseCustomFunction
 
 
-class CentroidFunction(openmm.CustomCentroidBondForce, BaseCollectiveVariable):
+class CentroidFunction(openmm.CustomCentroidBondForce, BaseCustomFunction):
     r"""
     A generic function of the centroids of :math:`m \times n` atoms groups split
     into `m` collections of `n` groups each:
 
     .. math::
 
         f({\bf r}) = \sum_{i=1}^m F\Big(
@@ -62,28 +61,30 @@
     the mass of the :math:`k`-th atom in group :math:`j`.
 
     Parameters
     ----------
     function
         The function to be evaluated. It must be a valid
         :OpenMM:`CustomCentroidBondForce` expression
+    unit
+        The unit of measurement of the collective variable. It must be compatible
+        with the MD unit system (mass in `daltons`, distance in `nanometers`, time
+        in `picoseconds`, temperature in `kelvin`, energy in `kilojoules_per_mol`,
+        angle in `radians`). If the collective variables does not have a unit, use
+        `dimensionless`
     groups
         The groups of atoms to be used in the function. Each group must be specified
         as a list of atom indices with arbitrary length
     collections
         The indices of the groups in each collection, passed as a 2D array-like object
         of shape `(m, n)`, where `m` is the number of collections and `n` is the number
         groups per collection. If a 1D object is passed, it is assumed that `m` is 1 and
         `n` is the length of the object.
-    unit
-        The unit of measurement of the collective variable. It must be compatible
-        with the MD unit system (mass in `daltons`, distance in `nanometers`, time
-        in `picoseconds`, temperature in `kelvin`, energy in `kilojoules_per_mol`,
-        angle in `radians`). If the collective variables does not have a unit, use
-        `dimensionless`
+    period
+        The period of the collective variable if it is periodic, or `None` if it is not
     pbc
         Whether to use periodic boundary conditions
     weighByMass
         Whether to define the centroid as the center of mass of the group instead of
         the geometric center
 
     Keyword Args
@@ -146,38 +147,51 @@
         >>> model.system.addForce(colvar)
         7
         >>> context.reinitialize(preserveState=True)
         >>> print(colvar.getValue(context))
         33.0 dimensionless
     """
 
+    yaml_tag = "!cvpack.CentroidFunction"
+
+    @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         function: str,
         unit: mmunit.Unit,
-        groups: t.Sequence[t.Sequence[int]],
+        groups: t.Iterable[t.Iterable[int]],
         collections: t.Optional[ArrayLike] = None,
+        period: t.Optional[mmunit.ScalarQuantity] = None,
         pbc: bool = True,
         weighByMass: bool = True,
-        **parameters: mmunit.ScalarQuantity,
+        **parameters: t.Union[mmunit.ScalarQuantity, mmunit.VectorQuantity],
     ) -> None:
+        groups = [list(map(int, group)) for group in groups]
+        num_groups = len(groups)
         collections = np.atleast_2d(
-            np.arange(len(groups)) if collections is None else collections
+            np.arange(num_groups) if collections is None else collections
         )
         num_collections, groups_per_collection, *others = collections.shape
         if others:
             raise ValueError("Array `collections` cannot have more than 2 dimensions")
-        num_groups = len(groups)
         if np.any(collections < 0) or np.any(collections >= num_groups):
             raise ValueError("Group index out of bounds")
         super().__init__(groups_per_collection, function)
         for group in groups:
             self.addGroup(group, *([] if weighByMass else [[1] * len(group)]))
-        perbond_parameters = _add_parameters(self, num_collections, **parameters)
-        for collection, *values in zip(collections, *perbond_parameters):
-            self.addBond(collection, values)
-        self.setUsesPeriodicBoundaryConditions(pbc)
-        self._checkUnitCompatibility(unit)
+        overalls, perbonds = self._extractParameters(num_collections, **parameters)
+        self._addParameters(overalls, perbonds, collections, pbc, unit)
         unit = mmunit.SerializableUnit(unit)
         self._registerCV(
-            unit, function, unit, groups, collections, pbc, weighByMass, **parameters
+            unit,
+            function,
+            unit,
+            groups,
+            [list(map(int, collection)) for collection in collections],
+            period,
+            pbc,
+            weighByMass,
+            **overalls,
+            **perbonds,
         )
+        if period is not None:
+            self._registerPeriod(period)
```

### Comparing `cvpack-0.8.0/cvpack/composite_rmsd.py` & `cvpack-0.9.0/cvpack/composite_rmsd.py`

 * *Files 9% similar despite different names*

```diff
@@ -121,28 +121,33 @@
     0.0 nm
     >>> model.positions[guest_atoms] += 1.0 * unit.nanometers
     >>> context.setPositions(model.positions)
     >>> print(composite_rmsd.getValue(context))
     0.0 nm
     """
 
+    yaml_tag = "!cvpack.CompositeRMSD"
+
     @mmunit.convert_quantities
     def __init__(
         self,
         referencePositions: t.Union[
             mmunit.MatrixQuantity, t.Dict[int, mmunit.VectorQuantity]
         ],
-        groups: t.Sequence[t.Sequence[int]],
+        groups: t.Iterable[t.Iterable[int]],
         numAtoms: t.Optional[int] = None,
     ) -> None:
         num_atoms = numAtoms or len(referencePositions)
+        groups = [list(map(int, group)) for group in groups]
         all_atoms = sum(groups, [])
         if len(set(all_atoms)) != len(all_atoms):
             raise ValueError("Atom groups must be disjoint")
-        defined_coords = {atom: referencePositions[atom] for atom in all_atoms}
+        defined_coords = {
+            atom: list(map(float, referencePositions[atom])) for atom in all_atoms
+        }
         all_coords = np.zeros((num_atoms, 3))
         for atom, coords in defined_coords.items():
             all_coords[atom, :] = coords
         super().__init__(all_coords)
         for group in groups:
             self.addGroup(group)
         self._registerCV(mmunit.nanometers, defined_coords, groups, num_atoms)
```

### Comparing `cvpack-0.8.0/cvpack/cvpack.py` & `cvpack-0.9.0/cvpack/cvpack.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,51 +10,114 @@
 import collections
 import functools
 import inspect
 import typing as t
 
 import numpy as np
 import openmm
+import yaml
 from openmm import app as mmapp
 
 from cvpack import unit as mmunit
 
 from .unit import value_in_md_units
 
 
-class SerializableResidue(mmapp.topology.Residue):
+class SerializableAtom(yaml.YAMLObject):
     r"""
-    A class that extends OpenMM's Residue class with additional methods for
-    serialization and deserialization.
+    A serializable version of OpenMM's Atom class.
     """
 
-    def __init__(self, residue: mmapp.topology.Residue) -> None:
-        super().__init__(residue.name, residue.index, None, residue.id, None)
-        self._atoms = [
-            mmapp.topology.Atom(atom.name, atom.element, atom.index, None, atom.id)
-            for atom in residue.atoms()
-        ]
+    yaml_tag = "!cvpack.Atom"
 
+    def __init__(  # pylint: disable=super-init-not-called
+        self, atom: t.Union[mmapp.topology.Atom, "SerializableAtom"]
+    ) -> None:
+        self.name = atom.name
+        self.index = atom.index
+        if isinstance(atom, mmapp.topology.Atom):
+            self.element = atom.element.symbol
+            self.residue = atom.residue.index
+        else:
+            self.element = atom.element
+            self.residue = atom.residue
+        self.id = atom.id
 
-class BaseCollectiveVariable(openmm.Force):
+    def __getstate__(self) -> t.Dict[str, t.Any]:
+        return self.__dict__
+
+    def __setstate__(self, keywords: t.Dict[str, t.Any]) -> None:
+        self.__dict__.update(keywords)
+
+
+yaml.SafeDumper.add_representer(SerializableAtom, SerializableAtom.to_yaml)
+yaml.SafeLoader.add_constructor(SerializableAtom.yaml_tag, SerializableAtom.from_yaml)
+
+
+class SerializableResidue(yaml.YAMLObject):
+    r"""
+    A serializable version of OpenMM's Residue class.
+    """
+
+    yaml_tag = "!cvpack.Residue"
+
+    def __init__(  # pylint: disable=super-init-not-called
+        self, residue: t.Union[mmapp.topology.Residue, "SerializableResidue"]
+    ) -> None:
+        self.name = residue.name
+        self.index = residue.index
+        if isinstance(residue, mmapp.topology.Residue):
+            self.chain = residue.chain.index
+        else:
+            self.chain = residue.chain
+        self.id = residue.id
+        self._atoms = list(map(SerializableAtom, residue.atoms()))
+
+    def __getstate__(self) -> t.Dict[str, t.Any]:
+        return self.__dict__
+
+    def __setstate__(self, keywords: t.Dict[str, t.Any]) -> None:
+        self.__dict__.update(keywords)
+
+    def __len__(self) -> int:
+        return len(self._atoms)
+
+    def atoms(self):
+        """Iterate over all Atoms in the Residue."""
+        return iter(self._atoms)
+
+
+yaml.SafeDumper.add_representer(SerializableResidue, SerializableResidue.to_yaml)
+yaml.SafeLoader.add_constructor(
+    SerializableResidue.yaml_tag, SerializableResidue.from_yaml
+)
+
+
+class BaseCollectiveVariable(openmm.Force, yaml.YAMLObject):
     r"""
     An abstract class with common attributes and method for all CVs.
     """
 
     _unit: mmunit.Unit = mmunit.dimensionless
     _mass_unit: mmunit.Unit = mmunit.dalton * mmunit.nanometers**2
     _args: t.Dict[str, t.Any] = {}
+    _period: t.Optional[float] = None
 
     def __getstate__(self) -> t.Dict[str, t.Any]:
         return self._args
 
     def __setstate__(self, keywords: t.Dict[str, t.Any]) -> None:
         self.__init__(**keywords)
 
-    def _registerCV(self, unit: mmunit.Unit, *args: t.Any, **kwargs: t.Any) -> None:
+    def _registerCV(
+        self,
+        unit: mmunit.Unit,
+        *args: t.Any,
+        **kwargs: t.Any,
+    ) -> None:
         """
         Register the newly created BaseCollectiveVariable subclass instance.
 
         This method must always be called from Subclass.__init__.
 
         Parameters
         ----------
@@ -63,21 +126,37 @@
                 in the MD unit system (mass in Da, distance in nm, time in ps,
                 temperature in K, energy in kJ/mol, angle in rad).
             args
                 The arguments needed to construct this collective variable
             kwargs
                 The keyword arguments needed to construct this collective variable
         """
-        self.setName(self.__class__.__name__)
+        cls = self.__class__
+        self.setName(cls.__name__)
         self.setUnit(unit)
         self._mass_unit = mmunit.dalton * (mmunit.nanometers / self.getUnit()) ** 2
+        self._period = kwargs.get("period", None)
         arguments, _ = self.getArguments()
         self._args = dict(zip(arguments, args))
         self._args.update(kwargs)
 
+    def _registerPeriod(self, period: float) -> None:
+        """
+        Register the period of this collective variable.
+
+        This method must called from Subclass.__init__ if the collective variable is
+        periodic.
+
+        Parameters
+        ----------
+            period
+                The period of this collective variable
+        """
+        self._period = period
+
     def _getSingleForceState(
         self, context: openmm.Context, getEnergy: bool = False, getForces: bool = False
     ) -> openmm.State:
         """
         Get an OpenMM State containing the potential energy and/or force values computed
         from this single force object.
 
@@ -136,30 +215,14 @@
             The rounded number
         """
         if digits is None:
             return number
         power = f"{number:e}".split("e")[1]
         return round(number, -(int(power) - digits))
 
-    @staticmethod
-    def _checkUnitCompatibility(unit: mmunit.Unit) -> None:
-        """
-        Check if the given unit is compatible with the MD unit system.
-
-        Parameters
-        ----------
-            unit
-                The unit to check
-        """
-        if not np.isclose(
-            mmunit.Quantity(1.0, unit).value_in_unit_system(mmunit.md_unit_system),
-            1.0,
-        ):
-            raise ValueError(f"Unit {unit} is not compatible with the MD unit system.")
-
     @classmethod
     def getArguments(cls) -> t.Tuple[collections.OrderedDict, collections.OrderedDict]:
         """
         Inspect the arguments needed for constructing an instance of this collective
         variable.
 
         Returns
@@ -170,15 +233,15 @@
 
         Example
         -------
             >>> import cvpack
             >>> args, defaults = cvpack.RadiusOfGyration.getArguments()
             >>> for name, annotation in args.items():
             ...     print(f"{name}: {annotation}")
-            group: typing.Sequence[int]
+            group: typing.Iterable[int]
             pbc: <class 'bool'>
             weighByMass: <class 'bool'>
             >>> print(*defaults.items())
             ('pbc', False) ('weighByMass', False)
         """
         arguments = collections.OrderedDict()
         defaults = collections.OrderedDict()
@@ -201,14 +264,26 @@
 
     def getUnit(self) -> mmunit.Unit:
         """
         Get the unit of measurement of this collective variable.
         """
         return self._unit
 
+    def getPeriod(self) -> t.Optional[mmunit.SerializableQuantity]:
+        """
+        Get the period of this collective variable.
+
+        Returns
+        -------
+            The period of this collective variable or None if it is not periodic
+        """
+        if self._period is None:
+            return None
+        return mmunit.SerializableQuantity(self._period, self.getUnit())
+
     def setUnusedForceGroup(self, position: int, system: openmm.System) -> int:
         """
         Set the force group of this collective variable to the one at a given position
         in the ascending ordered list of unused force groups in an :OpenMM:`System`.
 
         .. note::
```

### Comparing `cvpack-0.8.0/cvpack/data/ideal_alpha_helix.csv` & `cvpack-0.9.0/cvpack/data/ideal_alpha_helix.csv`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/cvpack/data/ideal_antiparallel_beta_sheet.csv` & `cvpack-0.9.0/cvpack/data/ideal_antiparallel_beta_sheet.csv`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/cvpack/data/ideal_parallel_beta_sheet.csv` & `cvpack-0.9.0/cvpack/data/ideal_parallel_beta_sheet.csv`

 * *Files identical despite different names*

### Comparing `cvpack-0.8.0/cvpack/distance.py` & `cvpack-0.9.0/cvpack/distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,12 +45,14 @@
         >>> context =openmm.Context(system, integrator, platform)
         >>> context.setPositions([openmm.Vec3(0, 0, 0),openmm.Vec3(1, 1, 1)])
         >>> print(distance.getValue(context, digits=5))
         1.73205 nm
 
     """
 
+    yaml_tag = "!cvpack.Distance"
+
     def __init__(self, atom1: int, atom2: int, pbc: bool = False) -> None:
         super().__init__("r")
         self.addBond(atom1, atom2, [])
         self.setUsesPeriodicBoundaryConditions(pbc)
         self._registerCV(mmunit.nanometers, atom1, atom2, pbc)
```

### Comparing `cvpack-0.8.0/cvpack/helix_angle_content.py` & `cvpack-0.9.0/cvpack/helix_angle_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         >>> integrator = openmm.VerletIntegrator(0)
         >>> context = openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(helix_content.getValue(context, digits=6))
         18.76058 dimensionless
     """
 
+    yaml_tag = "!cvpack.HelixAngleContent"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         residues: t.Sequence[mmapp.topology.Residue],
         pbc: bool = False,
         thetaReference: mmunit.ScalarQuantity = mmunit.Quantity(88, mmunit.degrees),
         tolerance: mmunit.ScalarQuantity = mmunit.Quantity(15, mmunit.degrees),
```

### Comparing `cvpack-0.8.0/cvpack/helix_hbond_content.py` & `cvpack-0.9.0/cvpack/helix_hbond_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         >>> integrator = openmm.VerletIntegrator(0)
         >>> context = openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(helix_content.getValue(context, digits=6))
         15.88038 dimensionless
     """
 
+    yaml_tag = "!cvpack.HelixHBondContent"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         residues: t.Sequence[mmapp.topology.Residue],
         pbc: bool = False,
         thresholdDistance: mmunit.ScalarQuantity = mmunit.Quantity(
             0.33, mmunit.nanometers
```

### Comparing `cvpack-0.8.0/cvpack/helix_rmsd_content.py` & `cvpack-0.9.0/cvpack/helix_rmsd_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         >>> integrator = openmm.VerletIntegrator(0)
         >>> context = openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(helix_content.getValue(context, digits=4))
         15.981 dimensionless
     """
 
+    yaml_tag = "!cvpack.HelixRMSDContent"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         residues: t.Sequence[mmapp.topology.Residue],
         numAtoms: int,
         thresholdRMSD: mmunit.ScalarQuantity = mmunit.Quantity(0.08, mmunit.nanometers),
         stepFunction: str = "(1+x^4)/(1+x^4+x^8)",
```

### Comparing `cvpack-0.8.0/cvpack/helix_torsion_content.py` & `cvpack-0.9.0/cvpack/helix_torsion_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         >>> integrator = openmm.VerletIntegrator(0)
         >>> context = openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(helix_content.getValue(context, digits=6))
         17.45285 dimensionless
     """
 
+    yaml_tag = "!cvpack.HelixTorsionContent"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         residues: t.Sequence[mmapp.topology.Residue],
         pbc: bool = False,
         phiReference: mmunit.ScalarQuantity = mmunit.Quantity(-63.8, mmunit.degrees),
         psiReference: mmunit.ScalarQuantity = mmunit.Quantity(-41.1, mmunit.degrees),
```

### Comparing `cvpack-0.8.0/cvpack/number_of_contacts.py` & `cvpack-0.9.0/cvpack/number_of_contacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     >>> model.system.addForce(nc_normalized)
     6
     >>> context.reinitialize(preserveState=True)
     >>> print(nc_normalized.getValue(context, 4))
     1.0 dimensionless
     """
 
+    yaml_tag = "!cvpack.NumberOfContacts"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         group1: t.Sequence[int],
         group2: t.Sequence[int],
         nonbondedForce: openmm.NonbondedForce,
         reference: t.Union[mmunit.ScalarQuantity, openmm.Context] = 1.0,
```

### Comparing `cvpack-0.8.0/cvpack/radius_of_gyration.py` & `cvpack-0.9.0/cvpack/radius_of_gyration.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,20 @@
         >>> context =openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(radius_of_gyration.getValue(context, digits=6))
         0.2951431 nm
 
     """
 
+    yaml_tag = "!cvpack.RadiusOfGyration"
+
     def __init__(
-        self, group: t.Sequence[int], pbc: bool = False, weighByMass: bool = False
+        self, group: t.Iterable[int], pbc: bool = False, weighByMass: bool = False
     ) -> None:
+        group = list(group)
         num_atoms = len(group)
         num_groups = num_atoms + 1
         sum_dist_sq = "+".join(
             [f"distance(g{i+1}, g{num_atoms + 1})^2" for i in range(num_atoms)]
         )
         super().__init__(
             num_groups, f"sqrt(({sum_dist_sq})/{num_atoms})", group, pbc, weighByMass
```

### Comparing `cvpack-0.8.0/cvpack/radius_of_gyration_sq.py` & `cvpack-0.9.0/cvpack/radius_of_gyration_sq.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,18 @@
         >>> context =openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(rgsq.getValue(context, digits=6))  # doctest: +ELLIPSIS
         0.0871... nm**2
 
     """
 
+    yaml_tag = "!cvpack.RadiusOfGyrationSq"
+
     def __init__(
-        self, group: t.Sequence[int], pbc: bool = False, weighByMass: bool = False
+        self, group: t.Iterable[int], pbc: bool = False, weighByMass: bool = False
     ) -> None:
+        group = list(group)
         num_atoms = len(group)
         super().__init__(2, f"distance(g1, g2)^2/{num_atoms}", group, pbc, weighByMass)
         for atom in group:
             self.addBond([atom, num_atoms])
         self._registerCV(mmunit.nanometers**2, group, pbc, weighByMass)
```

### Comparing `cvpack-0.8.0/cvpack/residue_coordination.py` & `cvpack-0.9.0/cvpack/residue_coordination.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,14 +56,16 @@
             in contact
         normalize
             Whether the number of contacts should be normalized by the total number of
             possible contacts
         weighByMass
             Whether the centroid of each residue should be weighted by the mass of the
             atoms in the residue
+        includeHydrogens
+            Whether hydrogen atoms should be included in the centroid calculations
 
     Raises
     ------
         ValueError
             If the two groups of residues are not disjoint
 
     Example
@@ -99,54 +101,65 @@
         26.0 dimensionless
         >>> residue_coordination.setReferenceValue(26 * unit.dimensionless)
         >>> context.reinitialize(preserveState=True)
         >>> print(residue_coordination.getValue(context, digits=6))
         1.0 dimensionless
     """
 
+    yaml_tag = "!cvpack.ResidueCoordination"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        residueGroup1: t.Sequence[Residue],
-        residueGroup2: t.Sequence[Residue],
+        residueGroup1: t.Iterable[Residue],
+        residueGroup2: t.Iterable[Residue],
         pbc: bool = True,
         stepFunction: str = "1/(1+x^6)",
         thresholdDistance: mmunit.ScalarQuantity = mmunit.Quantity(
             1.0, mmunit.nanometers
         ),
         normalize: bool = False,
         weighByMass: bool = True,
+        includeHydrogens: bool = True,
     ) -> None:
+        residueGroup1 = list(map(SerializableResidue, residueGroup1))
+        residueGroup2 = list(map(SerializableResidue, residueGroup2))
         nr1 = len(residueGroup1)
         nr2 = len(residueGroup2)
         self._ref_val = nr1 * nr2 if normalize else 1.0
         expression = (
             f"({stepFunction})/refval"
             f"; x=distance(g1,g2)/{thresholdDistance}"
             f"; refval={self._ref_val}"
         )
         super().__init__(2, expression)
         self.setUsesPeriodicBoundaryConditions(pbc)
         for res in residueGroup1 + residueGroup2:
+            atoms = [
+                atom.index
+                for atom in res.atoms()
+                if includeHydrogens or atom.element != "H"
+            ]
             self.addGroup(
-                [atom.index for atom in res.atoms()],
-                *([] if weighByMass else [[1] * len(res)]),
+                atoms,
+                *([] if weighByMass else [[1] * len(atoms)]),
             )
         for idx1 in range(nr1):
             for idx2 in range(nr1, nr1 + nr2):
                 self.addBond([idx1, idx2], [])
         self._registerCV(
             mmunit.dimensionless,
-            list(map(SerializableResidue, residueGroup1)),
-            list(map(SerializableResidue, residueGroup2)),
+            residueGroup1,
+            residueGroup2,
             pbc,
             stepFunction,
             thresholdDistance,
             normalize,
             weighByMass,
+            includeHydrogens,
         )
 
     def getReferenceValue(self) -> mmunit.Quantity:
         """
         Get the reference value used for normalizing the residue coordination.
 
         Returns
```

### Comparing `cvpack-0.8.0/cvpack/rmsd.py` & `cvpack-0.9.0/cvpack/rmsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from cvpack import unit as mmunit
 
 from .cvpack import BaseCollectiveVariable
 
 
 class RMSD(openmm.RMSDForce, BaseCollectiveVariable):
     r"""
-    The minimum root-mean-square deviation (RMSD) between the current and reference
+    The root-mean-square deviation (RMSD) between the current and reference
     coordinates of a group of `n` atoms:
 
     .. math::
 
         d_{\rm rms}({\bf r}) = \sqrt{
             \frac{1}{n} \min_{
                 \bf q \in \mathbb{R}^4 \atop \|{\bf q}\| = 1
@@ -80,25 +80,30 @@
         >>> integrator.step(1000)
         >>> value = rmsd.getValue(context)
         >>> round(value/value.unit, 7)
         0.1231383
 
     """
 
+    yaml_tag = "!cvpack.RMSD"
+
     @mmunit.convert_quantities
     def __init__(
         self,
         referencePositions: t.Union[
             mmunit.MatrixQuantity, t.Dict[int, mmunit.VectorQuantity]
         ],
-        group: t.Sequence[int],
+        group: t.Iterable[int],
         numAtoms: t.Optional[int] = None,
     ) -> None:
+        group = list(map(int, group))
         num_atoms = numAtoms or len(referencePositions)
-        defined_coords = {atom: referencePositions[atom] for atom in group}
+        defined_coords = {
+            atom: list(map(float, referencePositions[atom])) for atom in group
+        }
         all_coords = np.zeros((num_atoms, 3))
         for atom, coords in defined_coords.items():
             all_coords[atom, :] = coords
         super().__init__(all_coords, group)
         self._registerCV(mmunit.nanometers, defined_coords, group, num_atoms)
 
     def getNullBondForce(self) -> openmm.HarmonicBondForce:
```

### Comparing `cvpack-0.8.0/cvpack/serializer/serializer.py` & `cvpack-0.9.0/cvpack/serializer/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,25 @@
         >>> import cvpack
         >>> import io
         >>> from cvpack import serializer
         >>> radius_of_gyration = cvpack.RadiusOfGyration([0, 1, 2])
         >>> iostream = io.StringIO()
         >>> serializer.serialize(radius_of_gyration, iostream)
         >>> print(iostream.getvalue())
-        !!python/object:cvpack.radius_of_gyration.RadiusOfGyration
+        !cvpack.RadiusOfGyration
         group:
         - 0
         - 1
         - 2
         pbc: false
         weighByMass: false
         <BLANKLINE>
 
     """
-    iostream.write(yaml.dump(obj, Dumper=yaml.CDumper))
+    iostream.write(yaml.safe_dump(obj))
 
 
 def deserialize(iostream: t.IO) -> t.Any:
     """
     Deserializes a cvpack object.
 
     Parameters
@@ -70,8 +70,8 @@
         >>> iostream.seek(0)
         0
         >>> new_object = serializer.deserialize(iostream)
         >>> print(type(new_object))
         <class 'cvpack.radius_of_gyration.RadiusOfGyration'>
 
     """
-    return yaml.load(iostream.read(), Loader=yaml.CLoader)
+    return yaml.safe_load(iostream.read())
```

### Comparing `cvpack-0.8.0/cvpack/sheet_rmsd_content.py` & `cvpack-0.9.0/cvpack/sheet_rmsd_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
         >>> model.system.addForce(blockwise_sheet_content)
         7
         >>> context.reinitialize(preserveState=True)
         >>> print(blockwise_sheet_content.getValue(context, digits=4))
         0.98594 dimensionless
     """
 
+    yaml_tag = "!cvpack.SheetRMSDContent"
+
     @mmunit.convert_quantities
     def __init__(  # pylint: disable=too-many-arguments
         self,
         residues: t.Sequence[mmapp.topology.Residue],
         numAtoms: int,
         parallel: bool = False,
         blockSizes: t.Optional[t.Sequence[int]] = None,
```

### Comparing `cvpack-0.8.0/cvpack/tests/test_cvpack.py` & `cvpack-0.9.0/cvpack/tests/test_cvpack.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,18 @@
     assert unity.value_in_unit_system(unit.md_unit_system) == 1
 
     # Class must have full type annotation (except for argument `self`)
     args, _ = collectiveVariable.getArguments()
     for _, annotation in args.items():
         assert annotation is not inspect.Parameter.empty
 
+    # Yaml tag must be defined and start with "!cvpack."
+    assert hasattr(collectiveVariable, "yaml_tag")
+    assert collectiveVariable.yaml_tag.startswith("!cvpack.")
+
     # Test serialization/deserialization
     pipe = io.StringIO()
     serializer.serialize(collectiveVariable, pipe)
     pipe.seek(0)
     new_cv = serializer.deserialize(pipe)
     new_cv.setUnusedForceGroup(0, context.getSystem())
     context.getSystem().addForce(new_cv)
@@ -754,40 +758,85 @@
     integreator = openmm.VerletIntegrator(0)
     context = openmm.Context(system, integreator, platform)
     context.setPositions(positions)
     assert unit.value_in_md_units(colvar.getValue(context)) == pytest.approx(strength)
     perform_common_tests(colvar, context)
 
 
-def test_residue_coordination():
+@pytest.mark.parametrize("includeHs", [False, True])
+def test_residue_coordination(includeHs: bool):
     """
     Test whether a residue coordination CV is computed correctly.
 
     """
     model = testsystems.LysozymeImplicit()
     positions = model.positions.value_in_unit(unit.nanometers)
     groups = [
         list(it.islice(model.topology.residues(), start, end))
         for start, end in [(125, 142), (142, 156)]
     ]
-    centroids = [
-        np.vstack(
-            [np.mean(positions[[a.index for a in r.atoms()]], axis=0) for r in group]
-        )
-        for group in groups
-    ]
+    centroids = []
+    for group in groups:
+        residue_centroids = []
+        for r in group:
+            atoms = [a.index for a in r.atoms() if includeHs or a.element.symbol != "H"]
+            residue_centroids.append(np.mean(positions[atoms], axis=0))
+        centroids.append(np.vstack(residue_centroids))
     distances = np.linalg.norm(centroids[0][:, None, :] - centroids[1], axis=2)
     computed_cv = np.sum(1 / (1 + distances**6))
 
-    res_coord = cvpack.ResidueCoordination(*groups, pbc=False, weighByMass=False)
+    res_coord = cvpack.ResidueCoordination(
+        *groups, pbc=False, weighByMass=False, includeHydrogens=includeHs
+    )
     res_coord.setUnusedForceGroup(0, model.system)
     model.system.addForce(res_coord)
     context = openmm.Context(
         model.system,
         openmm.VerletIntegrator(0),
         openmm.Platform.getPlatformByName("Reference"),
     )
     context.setPositions(positions)
     cv_value = res_coord.getValue(context)
 
     assert cv_value / cv_value.unit == pytest.approx(computed_cv)
     perform_common_tests(res_coord, context)
+
+
+@pytest.mark.parametrize("metric", [cvpack.path.progress, cvpack.path.deviation])
+def test_path_in_cv_space(metric: cvpack.path.Metric):
+    """
+    Test whether a path in CV space is computed correctly.
+
+    """
+    model = testsystems.AlanineDipeptideVacuum()
+    phi_atoms = ["ACE-C", "ALA-N", "ALA-CA", "ALA-C"]
+    psi_atoms = ["ALA-N", "ALA-CA", "ALA-C", "NME-N"]
+    atoms = [f"{a.residue.name}-{a.name}" for a in model.topology.atoms()]
+    milestones = np.array(
+        [[1.3, -0.2], [1.2, 3.1], [-2.7, 2.9], [-1.3, 2.7], [-1.3, -0.4]]
+    )
+    phi = cvpack.Torsion(*[atoms.index(atom) for atom in phi_atoms])
+    psi = cvpack.Torsion(*[atoms.index(atom) for atom in psi_atoms])
+    sigma = np.pi / 6
+    var = cvpack.PathInCVSpace(metric, [phi, psi], milestones, sigma)
+    var.setUnusedForceGroup(0, model.system)
+    model.system.addForce(var)
+    context = openmm.Context(model.system, openmm.VerletIntegrator(1.0))
+    context.setPositions(model.positions)
+    cv_value = var.getValue(context)
+
+    def logsumexp(x, a=None):
+        xmax = np.max(x)
+        if a is None:
+            return xmax + np.log(np.sum(np.exp(x - xmax)))
+        return xmax + np.log(np.sum(a * np.exp(x - xmax)))
+
+    angles = np.array(var.getCollectiveVariableValues(context))
+    deltas = np.abs(milestones - angles)
+    x = -0.5 * np.sum(np.minimum(deltas, 2 * np.pi - deltas) ** 2, axis=1) / sigma**2
+    if metric is cvpack.path.progress:
+        n = len(x)
+        computed_value = np.exp(logsumexp(x, np.arange(n)) - logsumexp(x)) / (n - 1)
+    else:
+        computed_value = -2 * sigma**2 * logsumexp(x)
+    assert cv_value / cv_value.unit == pytest.approx(computed_value)
+    perform_common_tests(var, context)
```

### Comparing `cvpack-0.8.0/cvpack/torsion.py` & `cvpack-0.9.0/cvpack/torsion.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
    :platform: Linux, MacOS, Windows
    :synopsis: The torsion angle formed by four atoms
 
 .. classauthor:: Charlles Abreu <craabreu@gmail.com>
 
 """
 
+import math
+
 import openmm
 
 from cvpack import unit as mmunit
 
 from .cvpack import BaseCollectiveVariable
 
 
@@ -61,14 +63,17 @@
         >>> positions = [[0, 0, 0], [1, 0, 0], [1, 1, 0], [1, 1, 1]]
         >>> context.setPositions([openmm.Vec3(*pos) for pos in positions])
         >>> print(torsion.getValue(context, digits=6))
         1.570796 rad
 
     """
 
+    yaml_tag = "!cvpack.Torsion"
+
     def __init__(  # pylint: disable=too-many-arguments
         self, atom1: int, atom2: int, atom3: int, atom4: int, pbc: bool = False
     ) -> None:
         super().__init__("theta")
         self.addTorsion(atom1, atom2, atom3, atom4, [])
         self.setUsesPeriodicBoundaryConditions(pbc)
         self._registerCV(mmunit.radians, atom1, atom2, atom3, atom4, pbc)
+        self._registerPeriod(2 * math.pi)
```

### Comparing `cvpack-0.8.0/cvpack/torsion_similarity.py` & `cvpack-0.9.0/cvpack/torsion_similarity.py`

 * *Files 12% similar despite different names*

```diff
@@ -75,20 +75,24 @@
         >>> platform =openmm.Platform.getPlatformByName("Reference")
         >>> context =openmm.Context(model.system, integrator, platform)
         >>> context.setPositions(model.positions)
         >>> print(torsion_similarity.getValue(context, digits=6))
         18.65992 dimensionless
     """
 
+    yaml_tag = "!cvpack.TorsionSimilarity"
+
     def __init__(
         self,
-        firstList: t.Sequence[t.Sequence[int]],
-        secondList: t.Sequence[t.Sequence[int]],
+        firstList: t.Iterable[t.Tuple[int, int, int, int]],
+        secondList: t.Iterable[t.Tuple[int, int, int, int]],
         pbc: bool = False,
     ) -> None:
+        firstList = [list(map(int, first)) for first in firstList]
+        secondList = [list(map(int, second)) for second in secondList]
         function = f"0.5*(1 + cos(min(delta, {2*np.pi} - delta)))"
         definition = "delta = dihedral(p1, p2, p3, p4) - dihedral(p5, p6, p7, p8)"
         super().__init__(8, f"{function}; {definition}")
         for first, second in zip(firstList, secondList):
             self.addBond([*first, *second], [])
         self.setUsesPeriodicBoundaryConditions(pbc)
         self._registerCV(mmunit.dimensionless, firstList, secondList)
```

### Comparing `cvpack-0.8.0/cvpack/unit/__init__.py` & `cvpack-0.9.0/cvpack/unit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import inspect
 import typing as t
 from functools import wraps
 from numbers import Real
 
 import numpy as np
 import openmm
+import yaml
 from openmm import unit as _mmunit
 
 ScalarQuantity = t.Union[_mmunit.Quantity, Real]
 VectorQuantity = t.Union[_mmunit.Quantity, np.ndarray, openmm.Vec3]
 MatrixQuantity = t.Union[
     _mmunit.Quantity, np.ndarray, t.Sequence[openmm.Vec3], t.Sequence[np.ndarray]
 ]
@@ -41,15 +42,15 @@
         Replace an instance of ast.Name with an ast.Attribute with the value "unit" and
         the attribute name equal to the original id of the ast.Name.
         """
         mod = ast.Name(id="_mmunit", ctx=ast.Load())
         return ast.Attribute(value=mod, attr=node.id, ctx=ast.Load())
 
 
-class SerializableUnit(_mmunit.Unit):
+class SerializableUnit(_mmunit.Unit, yaml.YAMLObject):
     r"""
     A child class of openmm.unit.Unit that allows for serialization/deserialization.
 
     Parameters
     ----------
         base_or_scaled_units
             The base or scaled units.
@@ -57,24 +58,26 @@
     Examples
     --------
         >>> import yaml
         >>> from cvpack.unit import SerializableUnit
         >>> from openmm.unit import nanometer, picosecond
         >>> SerializableUnit(nanometer)  # doctest: +ELLIPSIS
         Unit(..., name="nanometer", symbol="nm"): 1.0})
-        >>> dump = yaml.dump(SerializableUnit(nanometer/picosecond))
+        >>> dump = yaml.safe_dump(SerializableUnit(nanometer/picosecond))
         >>> print(dump)
-        !!python/object:cvpack.unit.SerializableUnit
+        !cvpack.Unit
         description: nanometer/picosecond
         version: 1
         <BLANKLINE>
-        >>> 2*yaml.load(dump, Loader=yaml.CLoader)
+        >>> 2*yaml.safe_load(dump)
         Quantity(value=2, unit=nanometer/picosecond)
     """
 
+    yaml_tag = "!cvpack.Unit"
+
     def __init__(self, base_or_scaled_units):
         if isinstance(base_or_scaled_units, _mmunit.Unit):
             self.__dict__ = base_or_scaled_units.__dict__
         elif isinstance(base_or_scaled_units, str):
             tree = _NodeTransformer().visit(
                 ast.parse(base_or_scaled_units, mode="eval")
             )
@@ -89,15 +92,19 @@
 
     def __setstate__(self, kwds) -> None:
         if kwds["version"] != 1:
             raise ValueError("Unknown version")
         self.__init__(kwds["description"])
 
 
-class SerializableQuantity(_mmunit.Quantity):
+yaml.SafeDumper.add_representer(SerializableUnit, SerializableUnit.to_yaml)
+yaml.SafeLoader.add_constructor(SerializableUnit.yaml_tag, SerializableUnit.from_yaml)
+
+
+class SerializableQuantity(_mmunit.Quantity, yaml.YAMLObject):
     r"""
     A child class of openmm.unit.Quantity that allows for serialization/deserialization.
 
     Parameters
     ----------
         value
             Another quantity or the numerical value of a quantity.
@@ -107,27 +114,29 @@
     Examples
     --------
         >>> import yaml
         >>> from cvpack.unit import SerializableQuantity
         >>> from openmm.unit import nanometer
         >>> SerializableQuantity(1.0, nanometer)
         Quantity(value=1.0, unit=nanometer)
-        >>> dump = yaml.dump(SerializableQuantity(1.0, nanometer))
+        >>> dump = yaml.safe_dump(SerializableQuantity(1.0, nanometer))
         >>> print(dump)
-        !!python/object:cvpack.unit.SerializableQuantity
-        unit: !!python/object:cvpack.unit.SerializableUnit
+        !cvpack.Quantity
+        unit: !cvpack.Unit
           description: nanometer
           version: 1
         value: 1.0
         version: 1
         <BLANKLINE>
-        >>> yaml.load(dump, Loader=yaml.CLoader)
+        >>> yaml.safe_load(dump)
         Quantity(value=1.0, unit=nanometer)
     """
 
+    yaml_tag = "!cvpack.Quantity"
+
     def __init__(self, value, unit=None):  # pylint: disable=redefined-outer-name
         if unit is None:
             super().__init__(value._value, SerializableUnit(value.unit))
         else:
             super().__init__(value, SerializableUnit(unit))
 
     def __getstate__(self):
@@ -143,14 +152,20 @@
         Return the numerical value of the quantity in the MD unit system (e.g. mass in
         Da, distance in nm, time in ps, temperature in K, energy in kJ/mol, angle in
         rad).
         """
         return value_in_md_units(self)
 
 
+yaml.SafeDumper.add_representer(SerializableQuantity, SerializableQuantity.to_yaml)
+yaml.SafeLoader.add_constructor(
+    SerializableQuantity.yaml_tag, SerializableQuantity.from_yaml
+)
+
+
 def value_in_md_units(  # pylint: disable=redefined-outer-name
     quantity: t.Union[ScalarQuantity, VectorQuantity, MatrixQuantity]
 ) -> t.Union[float, np.ndarray, openmm.Vec3, t.List[openmm.Vec3], t.List[np.ndarray]]:
     """
     Return the numerical value of a quantity in the MD unit system (e.g. mass in Da,
     distance in nm, time in ps, temperature in K, energy in kJ/mol, angle in rad).
```

### Comparing `cvpack-0.8.0/cvpack/utils.py` & `cvpack-0.9.0/cvpack/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,29 @@
 .. classauthor:: Charlles Abreu <craabreu@gmail.com>
 
 """
 
 import typing as t
 from copy import deepcopy
 
+import numpy as np
 import openmm
+import yaml
+from numpy import typing as npt
 
 from cvpack import unit as mmunit
 
 
-class NonbondedForceSurrogate:  # pylint: disable=too-many-instance-attributes
+class NonbondedForceSurrogate(
+    yaml.YAMLObject
+):  # pylint: disable=too-many-instance-attributes
     """A surrogate class for the NonbondedForce class in OpenMM."""
 
+    yaml_tag = "!cvpack.NonbondedForce"
+
     def __init__(self, other: openmm.NonbondedForce) -> None:
         self._cutoff = other.getCutoffDistance()
         self._uses_pbc = other.usesPeriodicBoundaryConditions()
         self._num_particles = other.getNumParticles()
         self._particle_parameters = list(
             map(other.getParticleParameters, range(self._num_particles))
         )
@@ -90,34 +97,77 @@
         return self._use_switching_function
 
     def getSwitchingDistance(self) -> float:
         """Get the switching distance."""
         return mmunit.value_in_md_units(self._switching_distance)
 
 
-def evaluate_in_context(force: openmm.Force, context: openmm.Context) -> float:
-    """Evaluate the potential energy of a force in a given context.
+yaml.SafeDumper.add_representer(
+    NonbondedForceSurrogate, NonbondedForceSurrogate.to_yaml
+)
+yaml.SafeLoader.add_constructor(
+    NonbondedForceSurrogate.yaml_tag, NonbondedForceSurrogate.from_yaml
+)
+
+
+def evaluate_in_context(
+    forces: t.Union[openmm.Force, t.Iterable[openmm.Force]], context: openmm.Context
+) -> t.Union[float, t.List[float]]:
+    """Evaluate the potential energies of OpenMM Forces in a given context.
 
     Parameters
     ----------
-        force : openmm.Force
-            The force to be evaluated.
-        context : openmm.Context
+        forces
+            The forces to be evaluated.
+        context
             The context in which the force will be evaluated.
 
     Returns
     -------
         float
             The potential energy of the force in the given context.
     """
+    is_single = isinstance(forces, openmm.Force)
+    if is_single:
+        forces = [forces]
     system = openmm.System()
     for _ in range(context.getSystem().getNumParticles()):
         system.addParticle(1.0)
-    system.addForce(deepcopy(force))
+    for i, force in enumerate(forces):
+        force_copy = deepcopy(force)
+        force_copy.setForceGroup(i)
+        system.addForce(force_copy)
     state = context.getState(getPositions=True)
     context = openmm.Context(system, openmm.VerletIntegrator(1.0))
     context.setPositions(state.getPositions())
     context.setPeriodicBoxVectors(*state.getPeriodicBoxVectors())
-    # pylint: disable=unexpected-keyword-arg # to avoid false positive
-    state = context.getState(getEnergy=True)
-    # pylint: enable=unexpected-keyword-arg
-    return mmunit.value_in_md_units(state.getPotentialEnergy())
+    energies = []
+    for i in range(len(forces)):
+        state = context.getState(  # pylint: disable=unexpected-keyword-arg
+            getEnergy=True, groups=1 << i
+        )
+        energies.append(mmunit.value_in_md_units(state.getPotentialEnergy()))
+    return energies[0] if is_single else tuple(energies)
+
+
+def convert_to_matrix(array: npt.ArrayLike) -> t.Tuple[np.ndarray, int, int]:
+    """Convert a 1D or 2D array-like object to a 2D numpy array.
+
+    Parameters
+    ----------
+        array : array_like
+            The array to be converted.
+
+    Returns
+    -------
+        numpy.ndarray
+            The 2D numpy array.
+        int
+            The number of rows in the array.
+        int
+            The number of columns in the array.
+    """
+    array = np.atleast_2d(array)
+    numrows, numcols, *other_dimensions = array.shape
+    if other_dimensions:
+        raise ValueError("Array-like object cannot have more than two dimensions.")
+    return array, numrows, numcols
```

### Comparing `cvpack-0.8.0/cvpack.egg-info/PKG-INFO` & `cvpack-0.9.0/cvpack.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvpack
-Version: 0.8.0
+Version: 0.9.0
 Summary: Useful Collective Variables for OpenMM
 Author-email: Charlles Abreu <craabreu@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -61,22 +61,30 @@
 | [Composite RMSD]        | multibody RMSD with concerted-rotation alignment                 |
 | [Distance]              | distance between two atoms                                       |
 | [Helix angle content]   | alpha-helix angle content of a sequence of residues              |
 | [Helix H-bond content]  | alpha-helix hydrogen-bond content of a sequence of residues      |
 | [Helix RMSD content]    | alpha-helix RMSD content of a sequence of residues               |
 | [Helix torsion content] | alpha-helix Ramachandran content of a sequence of residues       |
 | [Number of contacts]    | number of contacts between two groups of atoms                   |
+| [PathInCVSpace]         | progress along (deviation from) a predefined path in CV space    |
 | [Radius of gyration]    | radius of gyration of a group of atoms                           |
 | [(Radius of gyration)^2]| square of the radius of gyration of a group of atoms             |
 | [Residue coordination]  | number of contacts between two disjoint groups of residues       |
 | [RMSD]                  | root-mean-square deviation with respect to a reference structure |
 | [Sheet RMSD content]    | beta-sheet RMSD content of a sequence of residues                |
 | [Torsion]               | torsion angle formed by four atoms                               |
 | [Torsion similarity]    | degree of similarity between pairs of torsion angles             |
 
+Below is a list of new CVs already available in the development version:
+
+| Collective Variable     | Description                                                      |
+|-------------------------|------------------------------------------------------------------|
+| [PathInCVSpace]         | progress along (or deviation from) a predefined path in CV space |
+
+
 ### Installation and Usage
 
 CVPack is available as a conda package on the
 [mdtools](https://anaconda.org/mdtools/cvpack) channel. To install it, run:
 
 ```bash
     conda install -c conda-forge -c mdtools cvpack
@@ -112,25 +120,27 @@
 [CollectiveVariable]: https://ufedmm.readthedocs.io/en/latest/pythonapi/ufedmm.html#ufedmm.ufedmm.CollectiveVariable
 [CustomCVForce]:      https://docs.openmm.org/latest/api-python/generated/openmm.openmm.CustomCVForce.html
 [Force]:              https://docs.openmm.org/latest/api-python/generated/openmm.openmm.Force.html
 [Metadynamics]:       https://docs.openmm.org/latest/api-python/generated/openmm.app.metadynamics.Metadynamics.html
 [OpenMM]:             https://openmm.org
 [UFED]:               https://ufedmm.readthedocs.io/en/latest/index.html
 
-[Angle]:                  https://redesignscience.github.io/cvpack/api/Angle.html
-[Atomic Function]:        https://redesignscience.github.io/cvpack/api/AtomicFunction.html
-[Attraction Strength]:    https://redesignscience.github.io/cvpack/api/AttractionStrength.html
-[Centroid Function]:      https://redesignscience.github.io/cvpack/api/CentroidFunction.html
-[Composite RMSD]:         https://redesignscience.github.io/cvpack/api/CompositeRMSD.html
-[Distance]:               https://redesignscience.github.io/cvpack/api/Distance.html
-[Helix angle content]:    https://redesignscience.github.io/cvpack/api/HelixAngleContent.html
-[Helix H-bond content]:   https://redesignscience.github.io/cvpack/api/HelixHBondContent.html
-[Helix RMSD content]:     https://redesignscience.github.io/cvpack/api/HelixRMSDContent.html
-[Helix torsion content]:  https://redesignscience.github.io/cvpack/api/HelixTorsionContent.html
-[Number of contacts]:     https://redesignscience.github.io/cvpack/api/NumberOfContacts.html
-[Radius of gyration]:     https://redesignscience.github.io/cvpack/api/RadiusOfGyration.html
-[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/api/RadiusOfGyrationSq.html
-[Residue coordination]:   https://redesignscience.github.io/cvpack/api/ResidueCoordination.html
-[RMSD]:                   https://redesignscience.github.io/cvpack/api/RMSD.html
-[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/api/SheetRMSDContent.html
-[Torsion]:                https://redesignscience.github.io/cvpack/api/Torsion.html
-[Torsion similarity]:     https://redesignscience.github.io/cvpack/api/TorsionSimilarity.html
+[Angle]:                  https://redesignscience.github.io/cvpack/latest/api/Angle.html
+[Atomic Function]:        https://redesignscience.github.io/cvpack/latest/api/AtomicFunction.html
+[Attraction Strength]:    https://redesignscience.github.io/cvpack/latest/api/AttractionStrength.html
+[Centroid Function]:      https://redesignscience.github.io/cvpack/latest/api/CentroidFunction.html
+[Composite RMSD]:         https://redesignscience.github.io/cvpack/latest/api/CompositeRMSD.html
+[Distance]:               https://redesignscience.github.io/cvpack/latest/api/Distance.html
+[Helix angle content]:    https://redesignscience.github.io/cvpack/latest/api/HelixAngleContent.html
+[Helix H-bond content]:   https://redesignscience.github.io/cvpack/latest/api/HelixHBondContent.html
+[Helix RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/HelixRMSDContent.html
+[Helix torsion content]:  https://redesignscience.github.io/cvpack/latest/api/HelixTorsionContent.html
+[Number of contacts]:     https://redesignscience.github.io/cvpack/latest/api/NumberOfContacts.html
+[Radius of gyration]:     https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyration.html
+[(Radius of gyration)^2]: https://redesignscience.github.io/cvpack/latest/api/RadiusOfGyrationSq.html
+[Residue coordination]:   https://redesignscience.github.io/cvpack/latest/api/ResidueCoordination.html
+[RMSD]:                   https://redesignscience.github.io/cvpack/latest/api/RMSD.html
+[Sheet RMSD content]:     https://redesignscience.github.io/cvpack/latest/api/SheetRMSDContent.html
+[Torsion]:                https://redesignscience.github.io/cvpack/latest/api/Torsion.html
+[Torsion similarity]:     https://redesignscience.github.io/cvpack/latest/api/TorsionSimilarity.html
+
+[PathInCVSpace]:          https://redesignscience.github.io/cvpack/development/api/PathInCVSpace.html
```

### Comparing `cvpack-0.8.0/cvpack.egg-info/SOURCES.txt` & `cvpack-0.9.0/cvpack.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 pyproject.toml
 setup.cfg
 cvpack/__init__.py
 cvpack/_version.py
 cvpack/angle.py
 cvpack/atomic_function.py
 cvpack/attraction_strength.py
+cvpack/base_custom_function.py
 cvpack/base_radius_of_gyration.py
 cvpack/base_rmsd_content.py
 cvpack/centroid_function.py
 cvpack/composite_rmsd.py
 cvpack/cvpack.py
 cvpack/distance.py
 cvpack/helix_angle_content.py
 cvpack/helix_hbond_content.py
 cvpack/helix_rmsd_content.py
 cvpack/helix_torsion_content.py
 cvpack/number_of_contacts.py
+cvpack/path.py
+cvpack/path_in_cv_space.py
 cvpack/py.typed
 cvpack/radius_of_gyration.py
 cvpack/radius_of_gyration_sq.py
 cvpack/residue_coordination.py
 cvpack/rmsd.py
 cvpack/sheet_rmsd_content.py
 cvpack/torsion.py
```

### Comparing `cvpack-0.8.0/pyproject.toml` & `cvpack-0.9.0/pyproject.toml`

 * *Files identical despite different names*

