# Comparing `tmp/scib-1.1.4.tar.gz` & `tmp/scib-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scib-1.1.4.tar", last modified: Tue Jul 25 09:58:53 2023, max compression
+gzip compressed data, was "scib-1.1.5.tar", last modified: Mon Apr  1 15:53:49 2024, max compression
```

## Comparing `scib-1.1.4.tar` & `scib-1.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 09:58:29.000000 scib-1.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-25 09:58:29.000000 scib-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-25 09:58:53.915817 scib-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-25 09:58:29.000000 scib-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 09:58:29.000000 scib-1.1.4/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 09:58:29.000000 scib-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 09:58:29.000000 scib-1.1.4/scib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 09:58:29.000000 scib-1.1.4/scib/_package_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 09:58:29.000000 scib-1.1.4/scib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-25 09:58:29.000000 scib-1.1.4/scib/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib/knn_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/knn_graph.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    48528 2023-07-25 09:58:53.000000 scib-1.1.4/scib/knn_graph/knn_graph.o
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 09:58:29.000000 scib-1.1.4/scib/knn_graph/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/scib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/ari.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/cell_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/graph_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/isolated_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/kbet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28990 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/lisi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15409 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/nmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/pcr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/silhouette.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 09:58:29.000000 scib-1.1.4/scib/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-07-25 09:58:29.000000 scib-1.1.4/scib/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.915817 scib-1.1.4/scib/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/g2m_genes_tirosh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/g2m_genes_tirosh_hm.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/s_genes_tirosh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 09:58:29.000000 scib-1.1.4/scib/resources/s_genes_tirosh_hm.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-25 09:58:29.000000 scib-1.1.4/scib/trajectory_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-25 09:58:29.000000 scib-1.1.4/scib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:58:53.911817 scib-1.1.4/scib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:58:52.000000 scib-1.1.4/scib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-25 09:58:53.000000 scib-1.1.4/scib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-25 09:58:53.919817 scib-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-25 09:58:29.000000 scib-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.774650 scib-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 15:53:32.000000 scib-1.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 15:53:32.000000 scib-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-01 15:53:49.774650 scib-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-01 15:53:32.000000 scib-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:53:32.000000 scib-1.1.5/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 15:53:32.000000 scib-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.766650 scib-1.1.5/scib/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-01 15:53:32.000000 scib-1.1.5/scib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-01 15:53:32.000000 scib-1.1.5/scib/_package_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 15:53:32.000000 scib-1.1.5/scib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-04-01 15:53:32.000000 scib-1.1.5/scib/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.770650 scib-1.1.5/scib/knn_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-01 15:53:32.000000 scib-1.1.5/scib/knn_graph/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-01 15:53:32.000000 scib-1.1.5/scib/knn_graph/knn_graph.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48528 2024-04-01 15:53:49.000000 scib-1.1.5/scib/knn_graph/knn_graph.o
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 15:53:32.000000 scib-1.1.5/scib/knn_graph/makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.770650 scib-1.1.5/scib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/ari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/cell_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/graph_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/isolated_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/kbet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28990 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/lisi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15409 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/nmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/pcr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/silhouette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-01 15:53:32.000000 scib-1.1.5/scib/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28563 2024-04-01 15:53:32.000000 scib-1.1.5/scib/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.770650 scib-1.1.5/scib/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 15:53:32.000000 scib-1.1.5/scib/resources/g2m_genes_tirosh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 15:53:32.000000 scib-1.1.5/scib/resources/g2m_genes_tirosh_hm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 15:53:32.000000 scib-1.1.5/scib/resources/s_genes_tirosh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 15:53:32.000000 scib-1.1.5/scib/resources/s_genes_tirosh_hm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-01 15:53:32.000000 scib-1.1.5/scib/trajectory_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-01 15:53:32.000000 scib-1.1.5/scib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:53:49.770650 scib-1.1.5/scib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-01 15:53:49.000000 scib-1.1.5/scib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-01 15:53:49.000000 scib-1.1.5/scib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:53:49.000000 scib-1.1.5/scib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:53:48.000000 scib-1.1.5/scib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-01 15:53:49.000000 scib-1.1.5/scib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 15:53:49.000000 scib-1.1.5/scib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-01 15:53:49.774650 scib-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-01 15:53:32.000000 scib-1.1.5/setup.py
```

### Comparing `scib-1.1.4/LICENSE.txt` & `scib-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/PKG-INFO` & `scib-1.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,513 +1,423 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7363 6962  : 2.1.Name: scib
-00000020: 0a56 6572 7369 6f6e 3a20 312e 312e 340a  .Version: 1.1.4.
-00000030: 5375 6d6d 6172 793a 2045 7661 6c75 6174  Summary: Evaluat
-00000040: 696e 6720 7369 6e67 6c65 2d63 656c 6c20  ing single-cell 
-00000050: 6461 7461 2069 6e74 6567 7261 7469 6f6e  data integration
-00000060: 206d 6574 686f 6473 0a48 6f6d 652d 7061   methods.Home-pa
-00000070: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000080: 7562 2e63 6f6d 2f74 6865 6973 6c61 622f  ub.com/theislab/
-00000090: 7363 6962 0a41 7574 686f 723a 204d 616c  scib.Author: Mal
-000000a0: 7465 2044 2e20 4c75 6563 6b65 6e2c 204d  te D. Luecken, M
-000000b0: 6172 656e 2042 7565 7474 6e65 722c 2044  aren Buettner, D
-000000c0: 616e 6965 6c20 432e 2053 7472 6f62 6c2c  aniel C. Strobl,
-000000d0: 204d 6963 6861 656c 6120 462e 204d 7565   Michaela F. Mue
-000000e0: 6c6c 6572 0a41 7574 686f 722d 656d 6169  ller.Author-emai
-000000f0: 6c3a 206d 616c 7465 2e6c 7565 636b 656e  l: malte.luecken
-00000100: 4068 656c 6d68 6f6c 747a 2d6d 7565 6e63  @helmholtz-muenc
-00000110: 6865 6e2e 6465 2c20 6d69 6368 6165 6c61  hen.de, michaela
-00000120: 2e6d 7565 6c6c 6572 4068 656c 6d68 6f6c  .mueller@helmhol
-00000130: 747a 2d6d 7565 6e63 6865 6e2e 6465 0a4c  tz-muenchen.de.L
-00000140: 6963 656e 7365 3a20 4d49 540a 5072 6f6a  icense: MIT.Proj
-00000150: 6563 742d 5552 4c3a 2050 6970 656c 696e  ect-URL: Pipelin
-00000160: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
-00000170: 622e 636f 6d2f 7468 6569 736c 6162 2f73  b.com/theislab/s
-00000180: 6369 622d 7069 7065 6c69 6e65 0a50 726f  cib-pipeline.Pro
-00000190: 6a65 6374 2d55 524c 3a20 5265 7072 6f64  ject-URL: Reprod
-000001a0: 7563 6962 696c 6974 792c 2068 7474 7073  ucibility, https
-000001b0: 3a2f 2f74 6865 6973 6c61 622e 6769 7468  ://theislab.gith
-000001c0: 7562 2e69 6f2f 7363 6962 2d72 6570 726f  ub.io/scib-repro
-000001d0: 6475 6369 6269 6c69 7479 0a50 726f 6a65  ducibility.Proje
-000001e0: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
-000001f0: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
-00000200: 6875 622e 636f 6d2f 7468 6569 736c 6162  hub.com/theislab
-00000210: 2f73 6369 622f 6973 7375 6573 0a4b 6579  /scib/issues.Key
-00000220: 776f 7264 733a 2062 656e 6368 6d61 726b  words: benchmark
-00000230: 696e 672c 7369 6e67 6c65 2063 656c 6c2c  ing,single cell,
-00000240: 6461 7461 2069 6e74 6567 7261 7469 6f6e  data integration
-00000250: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000260: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000270: 3a3a 2033 202d 2041 6c70 6861 0a43 6c61  :: 3 - Alpha.Cla
-00000280: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000290: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000002a0: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
-000002b0: 6965 723a 2049 6e74 656e 6465 6420 4175  ier: Intended Au
-000002c0: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-000002d0: 652f 5265 7365 6172 6368 0a43 6c61 7373  e/Research.Class
-000002e0: 6966 6965 723a 2054 6f70 6963 203a 3a20  ifier: Topic :: 
-000002f0: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
-00000300: 6d65 6e74 203a 3a20 4275 696c 6420 546f  ment :: Build To
-00000310: 6f6c 730a 436c 6173 7369 6669 6572 3a20  ols.Classifier: 
-00000320: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000330: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-00000340: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-00000350: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000360: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000370: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000380: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000390: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003a0: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
-000003b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000003c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000003d0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-000003e0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000003f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000400: 7974 686f 6e20 3a3a 2033 2e39 0a52 6571  ython :: 3.9.Req
-00000410: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-00000420: 332e 370a 4465 7363 7269 7074 696f 6e2d  3.7.Description-
-00000430: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000440: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
-00000450: 6964 6573 2d45 7874 7261 3a20 7270 7932  ides-Extra: rpy2
-00000460: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000470: 2074 6573 740a 5072 6f76 6964 6573 2d45   test.Provides-E
-00000480: 7874 7261 3a20 6465 760a 5072 6f76 6964  xtra: dev.Provid
-00000490: 6573 2d45 7874 7261 3a20 646f 6373 0a50  es-Extra: docs.P
-000004a0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
-000004b0: 6f75 7661 696e 0a50 726f 7669 6465 732d  ouvain.Provides-
-000004c0: 4578 7472 613a 2062 626b 6e6e 0a50 726f  Extra: bbknn.Pro
-000004d0: 7669 6465 732d 4578 7472 613a 2073 6361  vides-Extra: sca
-000004e0: 6e6f 7261 6d61 0a50 726f 7669 6465 732d  norama.Provides-
-000004f0: 4578 7472 613a 206d 6e6e 0a50 726f 7669  Extra: mnn.Provi
-00000500: 6465 732d 4578 7472 613a 2073 6367 656e  des-Extra: scgen
-00000510: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000520: 2073 6376 690a 5072 6f76 6964 6573 2d45   scvi.Provides-E
-00000530: 7874 7261 3a20 7472 7661 650a 5072 6f76  xtra: trvae.Prov
-00000540: 6964 6573 2d45 7874 7261 3a20 7472 7661  ides-Extra: trva
-00000550: 6570 0a50 726f 7669 6465 732d 4578 7472  ep.Provides-Extr
-00000560: 613a 2064 6573 630a 5072 6f76 6964 6573  a: desc.Provides
-00000570: 2d45 7874 7261 3a20 6861 726d 6f6e 790a  -Extra: harmony.
-00000580: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-00000590: 4345 4e53 452e 7478 740a 0a5b 215b 5374  CENSE.txt..[![St
-000005a0: 6172 735d 2868 7474 7073 3a2f 2f69 6d67  ars](https://img
-000005b0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000005c0: 7562 2f73 7461 7273 2f74 6865 6973 6c61  ub/stars/theisla
-000005d0: 622f 7363 6962 3f6c 6f67 6f3d 4769 7448  b/scib?logo=GitH
-000005e0: 7562 2663 6f6c 6f72 3d79 656c 6c6f 7729  ub&color=yellow)
-000005f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000600: 2e63 6f6d 2f74 6865 6973 6c61 622f 7363  .com/theislab/sc
-00000610: 6962 2f73 7461 7267 617a 6572 7329 0a5b  ib/stargazers).[
-00000620: 215b 5079 5049 5d28 6874 7470 733a 2f2f  ![PyPI](https://
-00000630: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000640: 7970 692f 762f 7363 6962 3f6c 6f67 6f3d  ypi/v/scib?logo=
-00000650: 5079 5049 295d 2868 7474 7073 3a2f 2f70  PyPI)](https://p
-00000660: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000670: 7363 6962 290a 5b21 5b50 7950 4944 6f77  scib).[![PyPIDow
-00000680: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
-00000690: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
-000006a0: 7363 6962 295d 2868 7474 7073 3a2f 2f70  scib)](https://p
-000006b0: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-000006c0: 2f73 6369 6229 0a5b 215b 4275 696c 6420  /scib).[![Build 
-000006d0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
-000006e0: 6769 7468 7562 2e63 6f6d 2f74 6865 6973  github.com/theis
-000006f0: 6c61 622f 7363 6962 2f61 6374 696f 6e73  lab/scib/actions
-00000700: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
-00000710: 796d 6c2f 6261 6467 652e 7376 6729 5d28  yml/badge.svg)](
-00000720: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000730: 6f6d 2f74 6865 6973 6c61 622f 7363 6962  om/theislab/scib
-00000740: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000750: 7773 2f74 6573 742e 796d 6c29 0a5b 215b  ws/test.yml).[![
-00000760: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
-00000770: 7474 7073 3a2f 2f72 6561 6474 6865 646f  ttps://readthedo
-00000780: 6373 2e6f 7267 2f70 726f 6a65 6374 732f  cs.org/projects/
-00000790: 7363 6962 2f62 6164 6765 2f3f 7665 7273  scib/badge/?vers
-000007a0: 696f 6e3d 6c61 7465 7374 295d 2868 7474  ion=latest)](htt
-000007b0: 7073 3a2f 2f73 6369 622e 7265 6164 7468  ps://scib.readth
-000007c0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-000007d0: 7374 2f3f 6261 6467 653d 6c61 7465 7374  st/?badge=latest
-000007e0: 290a 5b21 5b63 6f64 6563 6f76 5d28 6874  ).[![codecov](ht
-000007f0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000800: 2f67 682f 7468 6569 736c 6162 2f73 6369  /gh/theislab/sci
-00000810: 622f 6272 616e 6368 2f6d 6169 6e2f 6772  b/branch/main/gr
-00000820: 6170 682f 6261 6467 652e 7376 673f 746f  aph/badge.svg?to
-00000830: 6b65 6e3d 4d31 6e75 5470 4178 7953 295d  ken=M1nuTpAxyS)]
-00000840: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
-00000850: 2e69 6f2f 6768 2f74 6865 6973 6c61 622f  .io/gh/theislab/
-00000860: 7363 6962 290a 5b21 5b70 7265 2d63 6f6d  scib).[![pre-com
-00000870: 6d69 745d 2868 7474 7073 3a2f 2f69 6d67  mit](https://img
-00000880: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000890: 652f 7072 652d 2d63 6f6d 6d69 742d 656e  e/pre--commit-en
-000008a0: 6162 6c65 642d 6272 6967 6874 6772 6565  abled-brightgree
-000008b0: 6e3f 6c6f 676f 3d70 7265 2d63 6f6d 6d69  n?logo=pre-commi
-000008c0: 7426 6c6f 676f 436f 6c6f 723d 7768 6974  t&logoColor=whit
-000008d0: 6529 5d28 6874 7470 733a 2f2f 6769 7468  e)](https://gith
-000008e0: 7562 2e63 6f6d 2f70 7265 2d63 6f6d 6d69  ub.com/pre-commi
-000008f0: 742f 7072 652d 636f 6d6d 6974 290a 0a23  t/pre-commit)..#
-00000900: 2042 656e 6368 6d61 726b 696e 6720 6174   Benchmarking at
-00000910: 6c61 732d 6c65 7665 6c20 6461 7461 2069  las-level data i
-00000920: 6e74 6567 7261 7469 6f6e 2069 6e20 7369  ntegration in si
-00000930: 6e67 6c65 2d63 656c 6c20 6765 6e6f 6d69  ngle-cell genomi
-00000940: 6373 0a0a 5468 6973 2072 6570 6f73 6974  cs..This reposit
-00000950: 6f72 7920 636f 6e74 6169 6e73 2074 6865  ory contains the
-00000960: 2063 6f64 6520 666f 7220 7468 6520 6073   code for the `s
-00000970: 6369 6260 2070 6163 6b61 6765 2075 7365  cib` package use
-00000980: 6420 696e 206f 7572 2062 656e 6368 6d61  d in our benchma
-00000990: 726b 696e 6720 7374 7564 7920 666f 7220  rking study for 
-000009a0: 6461 7461 2069 6e74 6567 7261 7469 6f6e  data integration
-000009b0: 2074 6f6f 6c73 2e0a 496e 205b 6f75 7220   tools..In [our 
-000009c0: 7374 7564 795d 2868 7474 7073 3a2f 2f64  study](https://d
-000009d0: 6f69 2e6f 7267 2f31 302e 3130 3338 2f73  oi.org/10.1038/s
-000009e0: 3431 3539 322d 3032 312d 3031 3333 362d  41592-021-01336-
-000009f0: 3829 2c20 7765 2062 656e 6368 6d61 726b  8), we benchmark
-00000a00: 2031 3620 6d65 7468 6f64 7320 2873 6565   16 methods (see
-00000a10: 2054 6f6f 6c73 2920 7769 7468 2034 2063   Tools) with 4 c
-00000a20: 6f6d 6269 6e61 7469 6f6e 7320 6f66 0a70  ombinations of.p
-00000a30: 7265 7072 6f63 6573 7369 6e67 2073 7465  reprocessing ste
-00000a40: 7073 206c 6561 6469 6e67 2074 6f20 3638  ps leading to 68
-00000a50: 206d 6574 686f 6473 2063 6f6d 6269 6e61   methods combina
-00000a60: 7469 6f6e 7320 6f6e 2038 3520 6261 7463  tions on 85 batc
-00000a70: 6865 7320 6f66 2067 656e 6520 6578 7072  hes of gene expr
-00000a80: 6573 7369 6f6e 2061 6e64 2063 6872 6f6d  ession and chrom
-00000a90: 6174 696e 2061 6363 6573 7369 6269 6c69  atin accessibili
-00000aa0: 7479 0a64 6174 612e 0a0a 215b 576f 726b  ty.data...![Work
-00000ab0: 666c 6f77 5d28 6874 7470 733a 2f2f 7261  flow](https://ra
-00000ac0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000ad0: 656e 742e 636f 6d2f 7468 6569 736c 6162  ent.com/theislab
-00000ae0: 2f73 6369 622f 6d61 696e 2f64 6f63 732f  /scib/main/docs/
-00000af0: 736f 7572 6365 2f5f 7374 6174 6963 2f66  source/_static/f
-00000b00: 6967 7572 652e 706e 6729 0a0a 2323 2052  igure.png)..## R
-00000b10: 6573 6f75 7263 6573 0a0a 2d20 5468 6520  esources..- The 
-00000b20: 6769 7420 7265 706f 7369 746f 7279 206f  git repository o
-00000b30: 6620 7468 6520 5b60 7363 6962 6020 7061  f the [`scib` pa
-00000b40: 636b 6167 655d 2868 7474 7073 3a2f 2f67  ckage](https://g
-00000b50: 6974 6875 622e 636f 6d2f 7468 6569 736c  ithub.com/theisl
-00000b60: 6162 2f73 6369 6229 2061 6e64 0a20 2069  ab/scib) and.  i
-00000b70: 7473 205b 646f 6375 6d65 6e74 6174 696f  ts [documentatio
-00000b80: 6e5d 2868 7474 7073 3a2f 2f73 6369 622e  n](https://scib.
-00000b90: 7265 6164 7468 6564 6f63 732e 696f 2f29  readthedocs.io/)
-00000ba0: 2e0a 2d20 5468 6520 7265 7573 6162 6c65  ..- The reusable
-00000bb0: 2070 6970 656c 696e 6520 7765 2075 7365   pipeline we use
-00000bc0: 6420 696e 2074 6865 2073 7475 6479 2063  d in the study c
-00000bd0: 616e 2062 6520 666f 756e 6420 696e 2074  an be found in t
-00000be0: 6865 0a20 2073 6570 6172 6174 6520 5b73  he.  separate [s
-00000bf0: 6369 6220 7069 7065 6c69 6e65 5d28 6874  cib pipeline](ht
-00000c00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c10: 2f74 6865 6973 6c61 622f 7363 6962 2d70  /theislab/scib-p
-00000c20: 6970 656c 696e 652e 6769 7429 2072 6570  ipeline.git) rep
-00000c30: 6f73 6974 6f72 792e 2049 7420 6973 2072  ository. It is r
-00000c40: 6570 726f 6475 6369 626c 6520 616e 6420  eproducible and 
-00000c50: 6175 746f 6d61 7465 730a 2020 7468 6520  automates.  the 
-00000c60: 636f 6d70 7574 6174 696f 6e20 6f66 2070  computation of p
-00000c70: 7265 7072 6f63 6573 7373 696e 6720 636f  reprocesssing co
-00000c80: 6d62 696e 6174 696f 6e73 2c20 696e 7465  mbinations, inte
-00000c90: 6772 6174 696f 6e20 6d65 7468 6f64 7320  gration methods 
-00000ca0: 616e 6420 6265 6e63 686d 6172 6b69 6e67  and benchmarking
-00000cb0: 206d 6574 7269 6373 2e0a 2d20 4f6e 206f   metrics..- On o
-00000cc0: 7572 205b 7765 6273 6974 655d 2868 7474  ur [website](htt
-00000cd0: 7073 3a2f 2f74 6865 6973 6c61 622e 6769  ps://theislab.gi
-00000ce0: 7468 7562 2e69 6f2f 7363 6962 2d72 6570  thub.io/scib-rep
-00000cf0: 726f 6475 6369 6269 6c69 7479 2920 7765  roducibility) we
-00000d00: 2076 6973 7561 6c69 7365 2074 6865 2072   visualise the r
-00000d10: 6573 756c 7473 206f 6620 7468 6520 7374  esults of the st
-00000d20: 7564 792e 0a2d 2046 6f72 2072 6570 726f  udy..- For repro
-00000d30: 6475 6369 6269 6c69 7479 2061 6e64 2076  ducibility and v
-00000d40: 6973 7561 6c69 7361 7469 6f6e 2077 6520  isualisation we 
-00000d50: 6861 7665 2061 2064 6564 6963 6174 6564  have a dedicated
-00000d60: 0a20 2072 6570 6f73 6974 6f72 793a 205b  .  repository: [
-00000d70: 7363 6962 2d72 6570 726f 6475 6369 6269  scib-reproducibi
-00000d80: 6c69 7479 5d28 6874 7470 733a 2f2f 6769  lity](https://gi
-00000d90: 7468 7562 2e63 6f6d 2f74 6865 6973 6c61  thub.com/theisla
-00000da0: 622f 7363 6962 2d72 6570 726f 6475 6369  b/scib-reproduci
-00000db0: 6269 6c69 7479 292e 0a0a 2323 2320 506c  bility)...### Pl
-00000dc0: 6561 7365 2063 6974 653a 0a0a 4c75 6563  ease cite:..Luec
-00000dd0: 6b65 6e2c 204d 2e44 2e2c 2042 c3bc 7474  ken, M.D., B..tt
-00000de0: 6e65 722c 204d 2e2c 2043 6861 6963 686f  ner, M., Chaicho
-00000df0: 6f6d 7075 2c20 4b2e 2065 7420 616c 2e20  ompu, K. et al. 
-00000e00: 4265 6e63 686d 6172 6b69 6e67 2061 746c  Benchmarking atl
-00000e10: 6173 2d6c 6576 656c 2064 6174 6120 696e  as-level data in
-00000e20: 7465 6772 6174 696f 6e20 696e 2073 696e  tegration in sin
-00000e30: 676c 652d 6365 6c6c 2067 656e 6f6d 6963  gle-cell genomic
-00000e40: 732e 0a4e 6174 204d 6574 686f 6473 2031  s..Nat Methods 1
-00000e50: 392c 2034 31e2 8093 3530 2028 3230 3232  9, 41...50 (2022
-00000e60: 292e 205b 6874 7470 733a 2f2f 646f 692e  ). [https://doi.
-00000e70: 6f72 672f 3130 2e31 3033 382f 7334 3135  org/10.1038/s415
-00000e80: 3932 2d30 3231 2d30 3133 3336 2d38 5d28  92-021-01336-8](
-00000e90: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00000ea0: 3130 2e31 3033 382f 7334 3135 3932 2d30  10.1038/s41592-0
-00000eb0: 3231 2d30 3133 3336 2d38 290a 0a23 2320  21-01336-8)..## 
-00000ec0: 5061 636b 6167 653a 2073 6369 620a 0a57  Package: scib..W
-00000ed0: 6520 6372 6561 7465 6420 7468 6520 7079  e created the py
-00000ee0: 7468 6f6e 2070 6163 6b61 6765 2063 616c  thon package cal
-00000ef0: 6c65 6420 6073 6369 6260 2074 6861 7420  led `scib` that 
-00000f00: 7573 6573 2060 7363 616e 7079 6020 746f  uses `scanpy` to
-00000f10: 2073 7472 6561 6d6c 696e 6520 7468 6520   streamline the 
-00000f20: 696e 7465 6772 6174 696f 6e20 6f66 2073  integration of s
-00000f30: 696e 676c 652d 6365 6c6c 2064 6174 6173  ingle-cell datas
-00000f40: 6574 7320 616e 640a 6576 616c 7561 7465  ets and.evaluate
-00000f50: 2074 6865 2072 6573 756c 7473 2e20 5468   the results. Th
-00000f60: 6520 7061 636b 6167 6520 636f 6e74 6169  e package contai
-00000f70: 6e73 2073 6576 6572 616c 206d 6f64 756c  ns several modul
-00000f80: 6573 2066 6f72 2070 7265 7072 6f63 6573  es for preproces
-00000f90: 7369 6e67 2061 6e20 6061 6e6e 6461 7461  sing an `anndata
-00000fa0: 6020 6f62 6a65 6374 2c20 7275 6e6e 696e  ` object, runnin
-00000fb0: 6720 696e 7465 6772 6174 696f 6e0a 6d65  g integration.me
-00000fc0: 7468 6f64 7320 616e 6420 6576 616c 7561  thods and evalua
-00000fd0: 7469 6e67 2074 6865 2072 6573 756c 7469  ting the resulti
-00000fe0: 6e67 2075 7369 6e67 2061 206e 756d 6265  ng using a numbe
-00000ff0: 7220 6f66 206d 6574 7269 6373 2e20 466f  r of metrics. Fo
-00001000: 7220 7072 6570 726f 6365 7373 696e 672c  r preprocessing,
-00001010: 2060 7363 6962 2e70 7265 7072 6f63 6573   `scib.preproces
-00001020: 7369 6e67 6020 286f 7220 6073 6369 622e  sing` (or `scib.
-00001030: 7070 6029 0a63 6f6e 7461 696e 7320 6675  pp`).contains fu
-00001040: 6e63 7469 6f6e 7320 666f 7220 6e6f 726d  nctions for norm
-00001050: 616c 6973 696e 672c 2073 6361 6c69 6e67  alising, scaling
-00001060: 206f 7220 6261 7463 682d 6177 6172 6520   or batch-aware 
-00001070: 7365 6c65 6374 696f 6e20 6f66 2068 6967  selection of hig
-00001080: 686c 7920 7661 7269 6162 6c65 2067 656e  hly variable gen
-00001090: 6573 2e20 4675 6e63 7469 6f6e 7320 666f  es. Functions fo
-000010a0: 7220 7468 650a 696e 7465 6772 6174 696f  r the.integratio
-000010b0: 6e20 6d65 7468 6f64 7320 6172 6520 696e  n methods are in
-000010c0: 2060 7363 6962 2e69 6e74 6567 7261 7469   `scib.integrati
-000010d0: 6f6e 6020 6f72 2066 6f72 2073 686f 7274  on` or for short
-000010e0: 2060 7363 6962 2e69 6760 2061 6e64 206d   `scib.ig` and m
-000010f0: 6574 7269 6373 2061 7265 2075 6e64 6572  etrics are under
-00001100: 0a60 7363 6962 2e6d 6574 7269 6373 6020  .`scib.metrics` 
-00001110: 286f 7220 6073 6369 622e 6d65 6029 2e0a  (or `scib.me`)..
-00001120: 0a54 6865 2060 7363 6962 6020 7079 7468  .The `scib` pyth
-00001130: 6f6e 2070 6163 6b61 6765 2069 7320 6176  on package is av
-00001140: 6169 6c61 626c 6520 6f6e 205b 5079 5049  ailable on [PyPI
-00001150: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-00001160: 7267 2f29 2061 6e64 2063 616e 2062 6520  rg/) and can be 
-00001170: 696e 7374 616c 6c65 6420 7468 726f 7567  installed throug
-00001180: 680a 0a60 6060 636f 6d6d 616e 646c 696e  h..```commandlin
-00001190: 650a 7069 7020 696e 7374 616c 6c20 7363  e.pip install sc
-000011a0: 6962 0a60 6060 0a0a 496d 706f 7274 2060  ib.```..Import `
-000011b0: 7363 6962 6020 696e 2070 7974 686f 6e3a  scib` in python:
-000011c0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-000011d0: 7274 2073 6369 620a 6060 600a 0a23 2323  rt scib.```..###
-000011e0: 204f 7074 696f 6e61 6c20 4465 7065 6e64   Optional Depend
-000011f0: 656e 6369 6573 0a0a 5468 6520 7061 636b  encies..The pack
-00001200: 6167 6520 636f 6e74 6169 6e73 206f 7074  age contains opt
-00001210: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
-00001220: 6573 2074 6861 7420 6e65 6564 2074 6f20  es that need to 
-00001230: 6265 2069 6e73 7461 6c6c 6564 206d 616e  be installed man
-00001240: 7561 6c6c 7920 6966 206e 6565 6465 642e  ually if needed.
-00001250: 0a54 6865 7365 2069 6e63 6c75 6465 2052  .These include R
-00001260: 2064 6570 656e 6465 6e63 6965 7320 2860   dependencies (`
-00001270: 7270 7932 602c 2060 616e 6e64 6174 6132  rpy2`, `anndata2
-00001280: 7269 6029 2077 6869 6368 2072 6571 7569  ri`) which requi
-00001290: 7265 2061 6e20 696e 7374 616c 6c61 7469  re an installati
-000012a0: 6f6e 206f 6620 5220 696e 7465 6772 6174  on of R integrat
-000012b0: 696f 6e20 6d65 7468 6f64 2070 6163 6b61  ion method packa
-000012c0: 6765 732e 0a41 6c6c 206f 7074 696f 6e61  ges..All optiona
-000012d0: 6c20 6465 7065 6e64 656e 6369 6573 2061  l dependencies a
-000012e0: 7265 206c 6973 7465 6420 756e 6465 7220  re listed under 
-000012f0: 6073 6574 7570 2e63 6667 6020 756e 6465  `setup.cfg` unde
-00001300: 7220 605b 6f70 7469 6f6e 732e 6578 7472  r `[options.extr
-00001310: 6173 5f72 6571 7569 7265 5d60 2061 6e64  as_require]` and
-00001320: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
-00001330: 6420 7468 726f 7567 6820 7069 702e 0a0a  d through pip...
-00001340: 652e 672e 2066 6f72 2069 6e73 7461 6c6c  e.g. for install
-00001350: 696e 6720 6072 7079 3260 2061 6e64 2060  ing `rpy2` and `
-00001360: 6262 6b6e 6e60 2064 6570 656e 6465 6e63  bbknn` dependenc
-00001370: 6965 733a 0a60 6060 636f 6d6d 616e 646c  ies:.```commandl
-00001380: 696e 650a 7069 7020 696e 7374 616c 6c20  ine.pip install 
-00001390: 2773 6369 625b 7270 7932 2c62 626b 6e6e  'scib[rpy2,bbknn
-000013a0: 5d27 0a60 6060 0a0a 4f70 7469 6f6e 616c  ]'.```..Optional
-000013b0: 2064 6570 656e 6465 6e63 6965 7320 6f75   dependencies ou
-000013c0: 7473 6964 6520 6f66 2070 7974 686f 6e20  tside of python 
-000013d0: 6e65 6564 2074 6f20 6265 2069 6e73 7461  need to be insta
-000013e0: 6c6c 6564 2073 6570 6172 6174 656c 792e  lled separately.
-000013f0: 0a46 6f72 2069 6e73 7461 6e63 652c 2069  .For instance, i
-00001400: 6e20 6f72 6465 7220 746f 2072 756e 206b  n order to run k
-00001410: 4245 542c 2069 6e73 7461 6c6c 2069 7420  BET, install it 
-00001420: 7669 6120 7468 6520 666f 6c6c 6f77 696e  via the followin
-00001430: 6720 636f 6d6d 616e 6420 696e 2052 3a0a  g command in R:.
-00001440: 0a60 6060 520a 696e 7374 616c 6c2e 7061  .```R.install.pa
-00001450: 636b 6167 6573 2827 7265 6d6f 7465 7327  ckages('remotes'
-00001460: 290a 7265 6d6f 7465 733a 3a69 6e73 7461  ).remotes::insta
-00001470: 6c6c 5f67 6974 6875 6228 2774 6865 6973  ll_github('theis
-00001480: 6c61 622f 6b42 4554 2729 0a60 6060 0a0a  lab/kBET').```..
-00001490: 2323 204d 6574 7269 6373 0a0a 5765 2069  ## Metrics..We i
-000014a0: 6d70 6c65 6d65 6e74 6564 2064 6966 6665  mplemented diffe
-000014b0: 7265 6e74 206d 6574 7269 6373 2066 6f72  rent metrics for
-000014c0: 2065 7661 6c75 6174 696e 6720 6261 7463   evaluating batc
-000014d0: 6820 636f 7272 6563 7469 6f6e 2061 6e64  h correction and
-000014e0: 2062 696f 6c6f 6769 6361 6c20 636f 6e73   biological cons
-000014f0: 6572 7661 7469 6f6e 2069 6e20 7468 6520  ervation in the 
-00001500: 6073 6369 622e 6d65 7472 6963 7360 0a6d  `scib.metrics`.m
-00001510: 6f64 756c 652e 0a0a 3c74 6162 6c65 2063  odule...<table c
-00001520: 6c61 7373 3d22 646f 6375 7469 6c73 2061  lass="docutils a
-00001530: 6c69 676e 2d64 6566 6175 6c74 223e 0a20  lign-default">. 
-00001540: 203c 636f 6c67 726f 7570 3e0a 2020 2020   <colgroup>.    
-00001550: 3c63 6f6c 2073 7479 6c65 3d22 7769 6474  <col style="widt
-00001560: 683a 2035 3025 2220 2f3e 0a20 2020 203c  h: 50%" />.    <
-00001570: 636f 6c20 7374 796c 653d 2277 6964 7468  col style="width
-00001580: 3a20 3530 2522 202f 3e0a 2020 3c2f 636f  : 50%" />.  </co
-00001590: 6c67 726f 7570 3e0a 2020 3c74 6865 6164  lgroup>.  <thead
-000015a0: 3e0a 2020 2020 3c74 7220 636c 6173 733d  >.    <tr class=
-000015b0: 2272 6f77 2d6f 6464 223e 3c74 6820 636c  "row-odd"><th cl
-000015c0: 6173 733d 2268 6561 6422 3e3c 703e 4269  ass="head"><p>Bi
-000015d0: 6f6c 6f67 6963 616c 2043 6f6e 7365 7276  ological Conserv
-000015e0: 6174 696f 6e3c 2f70 3e3c 2f74 683e 0a20  ation</p></th>. 
-000015f0: 2020 2020 203c 7468 2063 6c61 7373 3d22       <th class="
-00001600: 6865 6164 223e 3c70 3e42 6174 6368 2043  head"><p>Batch C
-00001610: 6f72 7265 6374 696f 6e3c 2f70 3e3c 2f74  orrection</p></t
-00001620: 683e 0a20 2020 203c 2f74 723e 0a20 203c  h>.    </tr>.  <
-00001630: 2f74 6865 6164 3e0a 2020 3c74 626f 6479  /thead>.  <tbody
-00001640: 3e0a 2020 2020 3c74 7220 636c 6173 733d  >.    <tr class=
-00001650: 2272 6f77 2d65 7665 6e22 203e 0a20 2020  "row-even" >.   
-00001660: 2020 203c 7464 3e3c 756c 2063 6c61 7373     <td><ul class
-00001670: 3d22 7369 6d70 6c65 223e 0a20 2020 2020  ="simple">.     
-00001680: 2020 203c 6c69 3e3c 703e 4365 6c6c 2074     <li><p>Cell t
-00001690: 7970 6520 4153 573c 2f70 3e3c 2f6c 693e  ype ASW</p></li>
-000016a0: 0a20 2020 2020 2020 203c 6c69 3e3c 703e  .        <li><p>
-000016b0: 4365 6c6c 2063 7963 6c65 2063 6f6e 7365  Cell cycle conse
-000016c0: 7276 6174 696f 6e3c 2f70 3e3c 2f6c 693e  rvation</p></li>
-000016d0: 0a20 2020 2020 2020 203c 6c69 3e3c 703e  .        <li><p>
-000016e0: 4772 6170 6820 634c 4953 493c 2f70 3e3c  Graph cLISI</p><
-000016f0: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
-00001700: 3e3c 703e 4164 6a75 7374 6564 2072 616e  ><p>Adjusted ran
-00001710: 6420 696e 6465 7820 2841 5249 2920 666f  d index (ARI) fo
-00001720: 7220 6365 6c6c 206c 6162 656c 3c2f 703e  r cell label</p>
-00001730: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
-00001740: 693e 3c70 3e4e 6f72 6d61 6c69 7365 6420  i><p>Normalised 
-00001750: 6d75 7475 616c 2069 6e66 6f72 6d61 7469  mutual informati
-00001760: 6f6e 2028 4e4d 4929 2066 6f72 2063 656c  on (NMI) for cel
-00001770: 6c20 6c61 6265 6c3c 2f70 3e3c 2f6c 693e  l label</p></li>
-00001780: 0a20 2020 2020 2020 203c 6c69 3e3c 703e  .        <li><p>
-00001790: 4869 6768 6c79 2076 6172 6961 626c 6520  Highly variable 
-000017a0: 6765 6e65 2063 6f6e 7365 7276 6174 696f  gene conservatio
-000017b0: 6e3c 2f70 3e3c 2f6c 693e 0a20 2020 2020  n</p></li>.     
-000017c0: 2020 203c 6c69 3e3c 703e 4973 6f6c 6174     <li><p>Isolat
-000017d0: 6564 206c 6162 656c 2041 5357 3c2f 703e  ed label ASW</p>
-000017e0: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
-000017f0: 693e 3c70 3e49 736f 6c61 7465 6420 6c61  i><p>Isolated la
-00001800: 6265 6c20 4631 3c2f 703e 3c2f 6c69 3e0a  bel F1</p></li>.
-00001810: 2020 2020 2020 2020 3c6c 693e 3c70 3e54          <li><p>T
-00001820: 7261 6a65 6374 6f72 7920 636f 6e73 6572  rajectory conser
-00001830: 7661 7469 6f6e 3c2f 703e 3c2f 6c69 3e0a  vation</p></li>.
-00001840: 2020 2020 2020 3c2f 756c 3e3c 2f74 643e        </ul></td>
-00001850: 0a20 2020 2020 203c 7464 3e3c 756c 2063  .      <td><ul c
-00001860: 6c61 7373 3d22 7369 6d70 6c65 223e 0a20  lass="simple">. 
-00001870: 2020 2020 2020 203c 6c69 3e3c 703e 4261         <li><p>Ba
-00001880: 7463 6820 4153 573c 2f70 3e3c 2f6c 693e  tch ASW</p></li>
-00001890: 0a20 2020 2020 2020 203c 6c69 3e3c 703e  .        <li><p>
-000018a0: 5072 696e 6369 7061 6c20 636f 6d70 6f6e  Principal compon
-000018b0: 656e 7420 7265 6772 6573 7369 6f6e 3c2f  ent regression</
-000018c0: 703e 3c2f 6c69 3e0a 2020 2020 2020 2020  p></li>.        
-000018d0: 3c6c 693e 3c70 3e47 7261 7068 2069 4c49  <li><p>Graph iLI
-000018e0: 5349 3c2f 703e 3c2f 6c69 3e0a 2020 2020  SI</p></li>.    
-000018f0: 2020 2020 3c6c 693e 3c70 3e47 7261 7068      <li><p>Graph
-00001900: 2063 6f6e 6e65 6374 6976 6974 793c 2f70   connectivity</p
-00001910: 3e3c 2f6c 693e 0a20 2020 2020 2020 203c  ></li>.        <
-00001920: 6c69 3e3c 703e 6b42 4554 2028 4b2d 6e65  li><p>kBET (K-ne
-00001930: 6172 6573 7420 6e65 6967 6862 6f75 7220  arest neighbour 
-00001940: 6261 7463 6820 6566 6665 6374 293c 2f70  batch effect)</p
-00001950: 3e3c 2f6c 693e 0a20 2020 2020 203c 2f75  ></li>.      </u
-00001960: 6c3e 3c2f 7464 3e0a 2020 2020 3c2f 7472  l></td>.    </tr
-00001970: 3e0a 2020 3c2f 7462 6f64 793e 0a3c 2f74  >.  </tbody>.</t
-00001980: 6162 6c65 3e0a 0a46 6f72 2061 2064 6574  able>..For a det
-00001990: 6169 6c65 6420 6465 7363 7269 7074 696f  ailed descriptio
-000019a0: 6e20 6f66 2074 6865 206d 6574 7269 6373  n of the metrics
-000019b0: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
-000019c0: 7468 6973 2070 6163 6b61 6765 2c20 706c  this package, pl
-000019d0: 6561 7365 2073 6565 206f 7572 0a5b 7075  ease see our.[pu
-000019e0: 626c 6963 6174 696f 6e5d 2868 7474 7073  blication](https
-000019f0: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3130  ://doi.org/10.10
-00001a00: 3338 2f73 3431 3539 322d 3032 312d 3031  38/s41592-021-01
-00001a10: 3333 362d 3829 2061 6e64 2074 6865 2070  336-8) and the p
-00001a20: 6163 6b61 6765 205b 646f 6375 6d65 6e74  ackage [document
-00001a30: 6174 696f 6e5d 2868 7474 7073 3a2f 2f73  ation](https://s
-00001a40: 6369 622e 7265 6164 7468 6564 6f63 732e  cib.readthedocs.
-00001a50: 696f 2f29 2e0a 0a23 2320 496e 7465 6772  io/)...## Integr
-00001a60: 6174 696f 6e20 546f 6f6c 730a 0a54 6f6f  ation Tools..Too
-00001a70: 6c73 2074 6861 7420 6172 6520 636f 6d70  ls that are comp
-00001a80: 6172 6564 2069 6e63 6c75 6465 3a0a 0a2d  ared include:..-
-00001a90: 205b 4242 4b4e 4e5d 2868 7474 7073 3a2f   [BBKNN](https:/
-00001aa0: 2f67 6974 6875 622e 636f 6d2f 5465 6963  /github.com/Teic
-00001ab0: 686c 6162 2f62 626b 6e6e 2920 312e 332e  hlab/bbknn) 1.3.
-00001ac0: 390a 2d20 5b43 6f6d 6261 745d 2868 7474  9.- [Combat](htt
-00001ad0: 7073 3a2f 2f73 6361 6e70 792e 7265 6164  ps://scanpy.read
-00001ae0: 7468 6564 6f63 732e 696f 2f65 6e2f 7374  thedocs.io/en/st
-00001af0: 6162 6c65 2f61 7069 2f73 6361 6e70 792e  able/api/scanpy.
-00001b00: 7070 2e63 6f6d 6261 742e 6874 6d6c 2920  pp.combat.html) 
-00001b10: 5b70 6170 6572 5d28 6874 7470 733a 2f2f  [paper](https://
-00001b20: 6163 6164 656d 6963 2e6f 7570 2e63 6f6d  academic.oup.com
-00001b30: 2f62 696f 7374 6174 6973 7469 6373 2f61  /biostatistics/a
-00001b40: 7274 6963 6c65 2f38 2f31 2f31 3138 2f32  rticle/8/1/118/2
-00001b50: 3532 3037 3329 0a2d 205b 436f 6e6f 735d  52073).- [Conos]
-00001b60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001b70: 636f 6d2f 686d 732d 6462 6d69 2f63 6f6e  com/hms-dbmi/con
-00001b80: 6f73 2920 312e 332e 300a 2d20 5b44 4553  os) 1.3.0.- [DES
-00001b90: 435d 2868 7474 7073 3a2f 2f67 6974 6875  C](https://githu
-00001ba0: 622e 636f 6d2f 656c 656f 7a7a 722f 6465  b.com/eleozzr/de
-00001bb0: 7363 2920 322e 302e 330a 2d20 5b46 6173  sc) 2.0.3.- [Fas
-00001bc0: 744d 4e4e 5d28 6874 7470 733a 2f2f 6269  tMNN](https://bi
-00001bd0: 6f63 6f6e 6475 6374 6f72 2e6f 7267 2f70  oconductor.org/p
-00001be0: 6163 6b61 6765 732f 6261 7463 6865 6c6f  ackages/batchelo
-00001bf0: 722f 2920 2862 6174 6368 656c 6f72 2031  r/) (batchelor 1
-00001c00: 2e34 2e30 290a 2d20 5b48 6172 6d6f 6e79  .4.0).- [Harmony
-00001c10: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001c20: 2e63 6f6d 2f69 6d6d 756e 6f67 656e 6f6d  .com/immunogenom
-00001c30: 6963 732f 6861 726d 6f6e 7929 2031 2e30  ics/harmony) 1.0
-00001c40: 0a2d 205b 4c49 4745 525d 2868 7474 7073  .- [LIGER](https
-00001c50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
-00001c60: 636f 736b 6f4c 6162 2f6c 6967 6572 2920  coskoLab/liger) 
-00001c70: 302e 352e 300a 2d20 5b4d 4e4e 5d28 6874  0.5.0.- [MNN](ht
-00001c80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c90: 2f63 6872 6973 6361 696e 782f 6d6e 6e70  /chriscainx/mnnp
-00001ca0: 7929 2030 2e31 2e39 2e35 0a2d 205b 5341  y) 0.1.9.5.- [SA
-00001cb0: 5543 4945 5d28 6874 7470 733a 2f2f 6769  UCIE](https://gi
-00001cc0: 7468 7562 2e63 6f6d 2f4b 7269 7368 6e61  thub.com/Krishna
-00001cd0: 7377 616d 794c 6162 2f53 4155 4349 4529  swamyLab/SAUCIE)
-00001ce0: 0a2d 205b 5363 616e 6f72 616d 615d 2868  .- [Scanorama](h
-00001cf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001d00: 6d2f 6272 6961 6e68 6965 2f73 6361 6e6f  m/brianhie/scano
-00001d10: 7261 6d61 2920 312e 372e 300a 2d20 5b73  rama) 1.7.0.- [s
-00001d20: 6341 4e56 495d 2868 7474 7073 3a2f 2f67  cANVI](https://g
-00001d30: 6974 6875 622e 636f 6d2f 6368 656e 6c69  ithub.com/chenli
-00001d40: 6e67 616e 7465 6c6f 7065 2f48 6172 6d6f  ngantelope/Harmo
-00001d50: 6e69 7a61 7469 6f6e 5343 414e 5649 2920  nizationSCANVI) 
-00001d60: 2873 6356 4920 302e 362e 3729 0a2d 205b  (scVI 0.6.7).- [
-00001d70: 7363 4765 6e5d 2868 7474 7073 3a2f 2f67  scGen](https://g
-00001d80: 6974 6875 622e 636f 6d2f 7468 6569 736c  ithub.com/theisl
-00001d90: 6162 2f73 6367 656e 2920 312e 312e 350a  ab/scgen) 1.1.5.
-00001da0: 2d20 5b73 6356 495d 2868 7474 7073 3a2f  - [scVI](https:/
-00001db0: 2f67 6974 6875 622e 636f 6d2f 596f 7365  /github.com/Yose
-00001dc0: 664c 6162 2f73 6356 4929 2030 2e36 2e37  fLab/scVI) 0.6.7
-00001dd0: 0a2d 205b 5365 7572 6174 2076 335d 2868  .- [Seurat v3](h
-00001de0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001df0: 6d2f 7361 7469 6a61 6c61 622f 7365 7572  m/satijalab/seur
-00001e00: 6174 2920 332e 322e 3020 4343 4120 2864  at) 3.2.0 CCA (d
-00001e10: 6566 6175 6c74 2920 616e 6420 5250 4341  efault) and RPCA
-00001e20: 0a2d 205b 5472 5661 655d 2868 7474 7073  .- [TrVae](https
-00001e30: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-00001e40: 6569 736c 6162 2f74 7276 6165 2920 302e  eislab/trvae) 0.
-00001e50: 302e 310a 2d20 5b54 7256 6165 705d 2868  0.1.- [TrVaep](h
-00001e60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001e70: 6d2f 7468 6569 736c 6162 2f74 7276 6165  m/theislab/trvae
-00001e80: 7029 2030 2e31 2e30 0a0a 2323 2044 6576  p) 0.1.0..## Dev
-00001e90: 656c 6f70 6d65 6e74 0a0a 466f 7220 6465  elopment..For de
-00001ea0: 7665 6c6f 7069 6e67 2074 6869 7320 7061  veloping this pa
-00001eb0: 636b 6167 652c 2070 6c65 6173 6520 6d61  ckage, please ma
-00001ec0: 6b65 2073 7572 6520 746f 2069 6e73 7461  ke sure to insta
-00001ed0: 6c6c 2061 6464 6974 696f 6e61 6c20 6465  ll additional de
-00001ee0: 7065 6e64 656e 6369 6573 2073 6f20 7468  pendencies so th
-00001ef0: 6174 2079 6f75 2063 616e 2075 7365 2060  at you can use `
-00001f00: 7079 7465 7374 6020 616e 640a 6070 7265  pytest` and.`pre
-00001f10: 2d63 6f6d 6d69 7460 2e0a 0a60 6060 7368  -commit`...```sh
-00001f20: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
-00001f30: 2d65 2027 2e5b 7465 7374 2c64 6576 5d27  -e '.[test,dev]'
-00001f40: 0a60 6060 0a0a 506c 6561 7365 2072 6566  .```..Please ref
-00001f50: 6572 2074 6f20 7468 6520 6073 6574 7570  er to the `setup
-00001f60: 2e63 6667 6020 666f 7220 6d6f 7265 206f  .cfg` for more o
-00001f70: 7074 696f 6e61 6c20 6465 7065 6e64 656e  ptional dependen
-00001f80: 6369 6573 2e0a 0a49 6e73 7461 6c6c 2060  cies...Install `
-00001f90: 7072 652d 636f 6d6d 6974 6020 746f 2074  pre-commit` to t
-00001fa0: 6865 2072 6570 6f73 6974 6f72 7920 666f  he repository fo
-00001fb0: 7220 7275 6e6e 696e 6720 6974 2061 7574  r running it aut
-00001fc0: 6f6d 6174 6963 616c 6c79 2065 7665 7279  omatically every
-00001fd0: 2074 696d 6520 796f 7520 636f 6d6d 6974   time you commit
-00001fe0: 2069 6e20 6769 742e 0a0a 6060 6073 6865   in git...```she
-00001ff0: 6c6c 0a70 7265 2d63 6f6d 6d69 7420 696e  ll.pre-commit in
-00002000: 7374 616c 6c0a 6060 600a                 stall.```.
+00000000: 5b21 5b53 7461 7273 5d28 6874 7470 733a  [![Stars](https:
+00000010: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000020: 2f67 6974 6875 622f 7374 6172 732f 7468  /github/stars/th
+00000030: 6569 736c 6162 2f73 6369 623f 6c6f 676f  eislab/scib?logo
+00000040: 3d47 6974 4875 6226 636f 6c6f 723d 7965  =GitHub&color=ye
+00000050: 6c6c 6f77 295d 2868 7474 7073 3a2f 2f67  llow)](https://g
+00000060: 6974 6875 622e 636f 6d2f 7468 6569 736c  ithub.com/theisl
+00000070: 6162 2f73 6369 622f 7374 6172 6761 7a65  ab/scib/stargaze
+00000080: 7273 290a 5b21 5b50 7950 495d 2868 7474  rs).[![PyPI](htt
+00000090: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000000a0: 2e69 6f2f 7079 7069 2f76 2f73 6369 623f  .io/pypi/v/scib?
+000000b0: 6c6f 676f 3d50 7950 4929 5d28 6874 7470  logo=PyPI)](http
+000000c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000000d0: 6a65 6374 2f73 6369 6229 0a5b 215b 5079  ject/scib).[![Py
+000000e0: 5049 446f 776e 6c6f 6164 735d 2868 7474  PIDownloads](htt
+000000f0: 7073 3a2f 2f70 6570 792e 7465 6368 2f62  ps://pepy.tech/b
+00000100: 6164 6765 2f73 6369 6229 5d28 6874 7470  adge/scib)](http
+00000110: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+00000120: 6f6a 6563 742f 7363 6962 290a 5b21 5b42  oject/scib).[![B
+00000130: 7569 6c64 2053 7461 7475 735d 2868 7474  uild Status](htt
+00000140: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000150: 7468 6569 736c 6162 2f73 6369 622f 6163  theislab/scib/ac
+00000160: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000170: 7465 7374 2e79 6d6c 2f62 6164 6765 2e73  test.yml/badge.s
+00000180: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000190: 6875 622e 636f 6d2f 7468 6569 736c 6162  hub.com/theislab
+000001a0: 2f73 6369 622f 6163 7469 6f6e 732f 776f  /scib/actions/wo
+000001b0: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
+000001c0: 290a 5b21 5b44 6f63 756d 656e 7461 7469  ).[![Documentati
+000001d0: 6f6e 5d28 6874 7470 733a 2f2f 7265 6164  on](https://read
+000001e0: 7468 6564 6f63 732e 6f72 672f 7072 6f6a  thedocs.org/proj
+000001f0: 6563 7473 2f73 6369 622f 6261 6467 652f  ects/scib/badge/
+00000200: 3f76 6572 7369 6f6e 3d6c 6174 6573 7429  ?version=latest)
+00000210: 5d28 6874 7470 733a 2f2f 7363 6962 2e72  ](https://scib.r
+00000220: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000230: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
+00000240: 6174 6573 7429 0a5b 215b 636f 6465 636f  atest).[![codeco
+00000250: 765d 2868 7474 7073 3a2f 2f63 6f64 6563  v](https://codec
+00000260: 6f76 2e69 6f2f 6768 2f74 6865 6973 6c61  ov.io/gh/theisla
+00000270: 622f 7363 6962 2f62 7261 6e63 682f 6d61  b/scib/branch/ma
+00000280: 696e 2f67 7261 7068 2f62 6164 6765 2e73  in/graph/badge.s
+00000290: 7667 3f74 6f6b 656e 3d4d 316e 7554 7041  vg?token=M1nuTpA
+000002a0: 7879 5329 5d28 6874 7470 733a 2f2f 636f  xyS)](https://co
+000002b0: 6465 636f 762e 696f 2f67 682f 7468 6569  decov.io/gh/thei
+000002c0: 736c 6162 2f73 6369 6229 0a5b 215b 7072  slab/scib).[![pr
+000002d0: 652d 636f 6d6d 6974 5d28 6874 7470 733a  e-commit](https:
+000002e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000002f0: 2f62 6164 6765 2f70 7265 2d2d 636f 6d6d  /badge/pre--comm
+00000300: 6974 2d65 6e61 626c 6564 2d62 7269 6768  it-enabled-brigh
+00000310: 7467 7265 656e 3f6c 6f67 6f3d 7072 652d  tgreen?logo=pre-
+00000320: 636f 6d6d 6974 266c 6f67 6f43 6f6c 6f72  commit&logoColor
+00000330: 3d77 6869 7465 295d 2868 7474 7073 3a2f  =white)](https:/
+00000340: 2f67 6974 6875 622e 636f 6d2f 7072 652d  /github.com/pre-
+00000350: 636f 6d6d 6974 2f70 7265 2d63 6f6d 6d69  commit/pre-commi
+00000360: 7429 0a0a 2320 4265 6e63 686d 6172 6b69  t)..# Benchmarki
+00000370: 6e67 2061 746c 6173 2d6c 6576 656c 2064  ng atlas-level d
+00000380: 6174 6120 696e 7465 6772 6174 696f 6e20  ata integration 
+00000390: 696e 2073 696e 676c 652d 6365 6c6c 2067  in single-cell g
+000003a0: 656e 6f6d 6963 730a 0a54 6869 7320 7265  enomics..This re
+000003b0: 706f 7369 746f 7279 2063 6f6e 7461 696e  pository contain
+000003c0: 7320 7468 6520 636f 6465 2066 6f72 2074  s the code for t
+000003d0: 6865 2060 7363 6962 6020 7061 636b 6167  he `scib` packag
+000003e0: 6520 7573 6564 2069 6e20 6f75 7220 6265  e used in our be
+000003f0: 6e63 686d 6172 6b69 6e67 2073 7475 6479  nchmarking study
+00000400: 2066 6f72 2064 6174 6120 696e 7465 6772   for data integr
+00000410: 6174 696f 6e20 746f 6f6c 732e 0a49 6e20  ation tools..In 
+00000420: 5b6f 7572 2073 7475 6479 5d28 6874 7470  [our study](http
+00000430: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+00000440: 3033 382f 7334 3135 3932 2d30 3231 2d30  038/s41592-021-0
+00000450: 3133 3336 2d38 292c 2077 6520 6265 6e63  1336-8), we benc
+00000460: 686d 6172 6b20 3136 206d 6574 686f 6473  hmark 16 methods
+00000470: 2028 7365 6520 546f 6f6c 7329 2077 6974   (see Tools) wit
+00000480: 6820 3420 636f 6d62 696e 6174 696f 6e73  h 4 combinations
+00000490: 206f 660a 7072 6570 726f 6365 7373 696e   of.preprocessin
+000004a0: 6720 7374 6570 7320 6c65 6164 696e 6720  g steps leading 
+000004b0: 746f 2036 3820 6d65 7468 6f64 7320 636f  to 68 methods co
+000004c0: 6d62 696e 6174 696f 6e73 206f 6e20 3835  mbinations on 85
+000004d0: 2062 6174 6368 6573 206f 6620 6765 6e65   batches of gene
+000004e0: 2065 7870 7265 7373 696f 6e20 616e 6420   expression and 
+000004f0: 6368 726f 6d61 7469 6e20 6163 6365 7373  chromatin access
+00000500: 6962 696c 6974 790a 6461 7461 2e0a 0a21  ibility.data...!
+00000510: 5b57 6f72 6b66 6c6f 775d 2868 7474 7073  [Workflow](https
+00000520: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000530: 7263 6f6e 7465 6e74 2e63 6f6d 2f74 6865  rcontent.com/the
+00000540: 6973 6c61 622f 7363 6962 2f6d 6169 6e2f  islab/scib/main/
+00000550: 646f 6373 2f73 6f75 7263 652f 5f73 7461  docs/source/_sta
+00000560: 7469 632f 6669 6775 7265 2e70 6e67 290a  tic/figure.png).
+00000570: 0a23 2320 5265 736f 7572 6365 730a 0a2d  .## Resources..-
+00000580: 2054 6865 2067 6974 2072 6570 6f73 6974   The git reposit
+00000590: 6f72 7920 6f66 2074 6865 205b 6073 6369  ory of the [`sci
+000005a0: 6260 2070 6163 6b61 6765 5d28 6874 7470  b` package](http
+000005b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000005c0: 6865 6973 6c61 622f 7363 6962 2920 616e  heislab/scib) an
+000005d0: 640a 2020 6974 7320 5b64 6f63 756d 656e  d.  its [documen
+000005e0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+000005f0: 7363 6962 2e72 6561 6474 6865 646f 6373  scib.readthedocs
+00000600: 2e69 6f2f 292e 0a2d 2054 6865 2072 6575  .io/)..- The reu
+00000610: 7361 626c 6520 7069 7065 6c69 6e65 2077  sable pipeline w
+00000620: 6520 7573 6564 2069 6e20 7468 6520 7374  e used in the st
+00000630: 7564 7920 6361 6e20 6265 2066 6f75 6e64  udy can be found
+00000640: 2069 6e20 7468 650a 2020 7365 7061 7261   in the.  separa
+00000650: 7465 205b 7363 6962 2070 6970 656c 696e  te [scib pipelin
+00000660: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000670: 622e 636f 6d2f 7468 6569 736c 6162 2f73  b.com/theislab/s
+00000680: 6369 622d 7069 7065 6c69 6e65 2e67 6974  cib-pipeline.git
+00000690: 2920 7265 706f 7369 746f 7279 2e20 4974  ) repository. It
+000006a0: 2069 7320 7265 7072 6f64 7563 6962 6c65   is reproducible
+000006b0: 2061 6e64 2061 7574 6f6d 6174 6573 0a20   and automates. 
+000006c0: 2074 6865 2063 6f6d 7075 7461 7469 6f6e   the computation
+000006d0: 206f 6620 7072 6570 726f 6365 7373 7369   of preprocesssi
+000006e0: 6e67 2063 6f6d 6269 6e61 7469 6f6e 732c  ng combinations,
+000006f0: 2069 6e74 6567 7261 7469 6f6e 206d 6574   integration met
+00000700: 686f 6473 2061 6e64 2062 656e 6368 6d61  hods and benchma
+00000710: 726b 696e 6720 6d65 7472 6963 732e 0a2d  rking metrics..-
+00000720: 204f 6e20 6f75 7220 5b77 6562 7369 7465   On our [website
+00000730: 5d28 6874 7470 733a 2f2f 7468 6569 736c  ](https://theisl
+00000740: 6162 2e67 6974 6875 622e 696f 2f73 6369  ab.github.io/sci
+00000750: 622d 7265 7072 6f64 7563 6962 696c 6974  b-reproducibilit
+00000760: 7929 2077 6520 7669 7375 616c 6973 6520  y) we visualise 
+00000770: 7468 6520 7265 7375 6c74 7320 6f66 2074  the results of t
+00000780: 6865 2073 7475 6479 2e0a 2d20 466f 7220  he study..- For 
+00000790: 7265 7072 6f64 7563 6962 696c 6974 7920  reproducibility 
+000007a0: 616e 6420 7669 7375 616c 6973 6174 696f  and visualisatio
+000007b0: 6e20 7765 2068 6176 6520 6120 6465 6469  n we have a dedi
+000007c0: 6361 7465 640a 2020 7265 706f 7369 746f  cated.  reposito
+000007d0: 7279 3a20 5b73 6369 622d 7265 7072 6f64  ry: [scib-reprod
+000007e0: 7563 6962 696c 6974 795d 2868 7474 7073  ucibility](https
+000007f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
+00000800: 6569 736c 6162 2f73 6369 622d 7265 7072  eislab/scib-repr
+00000810: 6f64 7563 6962 696c 6974 7929 2e0a 0a23  oducibility)...#
+00000820: 2323 2050 6c65 6173 6520 6369 7465 3a0a  ## Please cite:.
+00000830: 0a4c 7565 636b 656e 2c20 4d2e 442e 2c20  .Luecken, M.D., 
+00000840: 42c3 bc74 746e 6572 2c20 4d2e 2c20 4368  B..ttner, M., Ch
+00000850: 6169 6368 6f6f 6d70 752c 204b 2e20 6574  aichoompu, K. et
+00000860: 2061 6c2e 2042 656e 6368 6d61 726b 696e   al. Benchmarkin
+00000870: 6720 6174 6c61 732d 6c65 7665 6c20 6461  g atlas-level da
+00000880: 7461 2069 6e74 6567 7261 7469 6f6e 2069  ta integration i
+00000890: 6e20 7369 6e67 6c65 2d63 656c 6c20 6765  n single-cell ge
+000008a0: 6e6f 6d69 6373 2e0a 4e61 7420 4d65 7468  nomics..Nat Meth
+000008b0: 6f64 7320 3139 2c20 3431 e280 9335 3020  ods 19, 41...50 
+000008c0: 2832 3032 3229 2e20 5b68 7474 7073 3a2f  (2022). [https:/
+000008d0: 2f64 6f69 2e6f 7267 2f31 302e 3130 3338  /doi.org/10.1038
+000008e0: 2f73 3431 3539 322d 3032 312d 3031 3333  /s41592-021-0133
+000008f0: 362d 385d 2868 7474 7073 3a2f 2f64 6f69  6-8](https://doi
+00000900: 2e6f 7267 2f31 302e 3130 3338 2f73 3431  .org/10.1038/s41
+00000910: 3539 322d 3032 312d 3031 3333 362d 3829  592-021-01336-8)
+00000920: 0a0a 2323 2050 6163 6b61 6765 3a20 7363  ..## Package: sc
+00000930: 6962 0a0a 5765 2063 7265 6174 6564 2074  ib..We created t
+00000940: 6865 2070 7974 686f 6e20 7061 636b 6167  he python packag
+00000950: 6520 6361 6c6c 6564 2060 7363 6962 6020  e called `scib` 
+00000960: 7468 6174 2075 7365 7320 6073 6361 6e70  that uses `scanp
+00000970: 7960 2074 6f20 7374 7265 616d 6c69 6e65  y` to streamline
+00000980: 2074 6865 2069 6e74 6567 7261 7469 6f6e   the integration
+00000990: 206f 6620 7369 6e67 6c65 2d63 656c 6c20   of single-cell 
+000009a0: 6461 7461 7365 7473 2061 6e64 0a65 7661  datasets and.eva
+000009b0: 6c75 6174 6520 7468 6520 7265 7375 6c74  luate the result
+000009c0: 732e 2054 6865 2070 6163 6b61 6765 2063  s. The package c
+000009d0: 6f6e 7461 696e 7320 7365 7665 7261 6c20  ontains several 
+000009e0: 6d6f 6475 6c65 7320 666f 7220 7072 6570  modules for prep
+000009f0: 726f 6365 7373 696e 6720 616e 2060 616e  rocessing an `an
+00000a00: 6e64 6174 6160 206f 626a 6563 742c 2072  ndata` object, r
+00000a10: 756e 6e69 6e67 2069 6e74 6567 7261 7469  unning integrati
+00000a20: 6f6e 0a6d 6574 686f 6473 2061 6e64 2065  on.methods and e
+00000a30: 7661 6c75 6174 696e 6720 7468 6520 7265  valuating the re
+00000a40: 7375 6c74 696e 6720 7573 696e 6720 6120  sulting using a 
+00000a50: 6e75 6d62 6572 206f 6620 6d65 7472 6963  number of metric
+00000a60: 732e 2046 6f72 2070 7265 7072 6f63 6573  s. For preproces
+00000a70: 7369 6e67 2c20 6073 6369 622e 7072 6570  sing, `scib.prep
+00000a80: 726f 6365 7373 696e 6760 2028 6f72 2060  rocessing` (or `
+00000a90: 7363 6962 2e70 7060 290a 636f 6e74 6169  scib.pp`).contai
+00000aa0: 6e73 2066 756e 6374 696f 6e73 2066 6f72  ns functions for
+00000ab0: 206e 6f72 6d61 6c69 7369 6e67 2c20 7363   normalising, sc
+00000ac0: 616c 696e 6720 6f72 2062 6174 6368 2d61  aling or batch-a
+00000ad0: 7761 7265 2073 656c 6563 7469 6f6e 206f  ware selection o
+00000ae0: 6620 6869 6768 6c79 2076 6172 6961 626c  f highly variabl
+00000af0: 6520 6765 6e65 732e 2046 756e 6374 696f  e genes. Functio
+00000b00: 6e73 2066 6f72 2074 6865 0a69 6e74 6567  ns for the.integ
+00000b10: 7261 7469 6f6e 206d 6574 686f 6473 2061  ration methods a
+00000b20: 7265 2069 6e20 6073 6369 622e 696e 7465  re in `scib.inte
+00000b30: 6772 6174 696f 6e60 206f 7220 666f 7220  gration` or for 
+00000b40: 7368 6f72 7420 6073 6369 622e 6967 6020  short `scib.ig` 
+00000b50: 616e 6420 6d65 7472 6963 7320 6172 6520  and metrics are 
+00000b60: 756e 6465 720a 6073 6369 622e 6d65 7472  under.`scib.metr
+00000b70: 6963 7360 2028 6f72 2060 7363 6962 2e6d  ics` (or `scib.m
+00000b80: 6560 292e 0a0a 5468 6520 6073 6369 6260  e`)...The `scib`
+00000b90: 2070 7974 686f 6e20 7061 636b 6167 6520   python package 
+00000ba0: 6973 2061 7661 696c 6162 6c65 206f 6e20  is available on 
+00000bb0: 5b50 7950 495d 2868 7474 7073 3a2f 2f70  [PyPI](https://p
+00000bc0: 7970 692e 6f72 672f 2920 616e 6420 6361  ypi.org/) and ca
+00000bd0: 6e20 6265 2069 6e73 7461 6c6c 6564 2074  n be installed t
+00000be0: 6872 6f75 6768 0a0a 6060 6063 6f6d 6d61  hrough..```comma
+00000bf0: 6e64 6c69 6e65 0a70 6970 2069 6e73 7461  ndline.pip insta
+00000c00: 6c6c 2073 6369 620a 6060 600a 0a49 6d70  ll scib.```..Imp
+00000c10: 6f72 7420 6073 6369 6260 2069 6e20 7079  ort `scib` in py
+00000c20: 7468 6f6e 3a0a 0a60 6060 7079 7468 6f6e  thon:..```python
+00000c30: 0a69 6d70 6f72 7420 7363 6962 0a60 6060  .import scib.```
+00000c40: 0a0a 2323 2320 4f70 7469 6f6e 616c 2044  ..### Optional D
+00000c50: 6570 656e 6465 6e63 6965 730a 0a54 6865  ependencies..The
+00000c60: 2070 6163 6b61 6765 2063 6f6e 7461 696e   package contain
+00000c70: 7320 6f70 7469 6f6e 616c 2064 6570 656e  s optional depen
+00000c80: 6465 6e63 6965 7320 7468 6174 206e 6565  dencies that nee
+00000c90: 6420 746f 2062 6520 696e 7374 616c 6c65  d to be installe
+00000ca0: 6420 6d61 6e75 616c 6c79 2069 6620 6e65  d manually if ne
+00000cb0: 6564 6564 2e0a 5468 6573 6520 696e 636c  eded..These incl
+00000cc0: 7564 6520 5220 6465 7065 6e64 656e 6369  ude R dependenci
+00000cd0: 6573 2028 6072 7079 3260 2c20 6061 6e6e  es (`rpy2`, `ann
+00000ce0: 6461 7461 3272 6960 2920 7768 6963 6820  data2ri`) which 
+00000cf0: 7265 7175 6972 6520 616e 2069 6e73 7461  require an insta
+00000d00: 6c6c 6174 696f 6e20 6f66 2052 2069 6e74  llation of R int
+00000d10: 6567 7261 7469 6f6e 206d 6574 686f 6420  egration method 
+00000d20: 7061 636b 6167 6573 2e0a 416c 6c20 6f70  packages..All op
+00000d30: 7469 6f6e 616c 2064 6570 656e 6465 6e63  tional dependenc
+00000d40: 6965 7320 6172 6520 6c69 7374 6564 2075  ies are listed u
+00000d50: 6e64 6572 2060 7365 7475 702e 6366 6760  nder `setup.cfg`
+00000d60: 2075 6e64 6572 2060 5b6f 7074 696f 6e73   under `[options
+00000d70: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+00000d80: 6020 616e 6420 6361 6e20 6265 2069 6e73  ` and can be ins
+00000d90: 7461 6c6c 6564 2074 6872 6f75 6768 2070  talled through p
+00000da0: 6970 2e0a 0a65 2e67 2e20 666f 7220 696e  ip...e.g. for in
+00000db0: 7374 616c 6c69 6e67 2060 7270 7932 6020  stalling `rpy2` 
+00000dc0: 616e 6420 6062 626b 6e6e 6020 6465 7065  and `bbknn` depe
+00000dd0: 6e64 656e 6369 6573 3a0a 6060 6063 6f6d  ndencies:.```com
+00000de0: 6d61 6e64 6c69 6e65 0a70 6970 2069 6e73  mandline.pip ins
+00000df0: 7461 6c6c 2027 7363 6962 5b72 7079 322c  tall 'scib[rpy2,
+00000e00: 6262 6b6e 6e5d 270a 6060 600a 0a4f 7074  bbknn]'.```..Opt
+00000e10: 696f 6e61 6c20 6465 7065 6e64 656e 6369  ional dependenci
+00000e20: 6573 206f 7574 7369 6465 206f 6620 7079  es outside of py
+00000e30: 7468 6f6e 206e 6565 6420 746f 2062 6520  thon need to be 
+00000e40: 696e 7374 616c 6c65 6420 7365 7061 7261  installed separa
+00000e50: 7465 6c79 2e0a 466f 7220 696e 7374 616e  tely..For instan
+00000e60: 6365 2c20 696e 206f 7264 6572 2074 6f20  ce, in order to 
+00000e70: 7275 6e20 6b42 4554 2c20 696e 7374 616c  run kBET, instal
+00000e80: 6c20 6974 2076 6961 2074 6865 2066 6f6c  l it via the fol
+00000e90: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2069  lowing command i
+00000ea0: 6e20 523a 0a0a 6060 6052 0a69 6e73 7461  n R:..```R.insta
+00000eb0: 6c6c 2e70 6163 6b61 6765 7328 2772 656d  ll.packages('rem
+00000ec0: 6f74 6573 2729 0a72 656d 6f74 6573 3a3a  otes').remotes::
+00000ed0: 696e 7374 616c 6c5f 6769 7468 7562 2827  install_github('
+00000ee0: 7468 6569 736c 6162 2f6b 4245 5427 290a  theislab/kBET').
+00000ef0: 6060 600a 0a23 2320 4d65 7472 6963 730a  ```..## Metrics.
+00000f00: 0a57 6520 696d 706c 656d 656e 7465 6420  .We implemented 
+00000f10: 6469 6666 6572 656e 7420 6d65 7472 6963  different metric
+00000f20: 7320 666f 7220 6576 616c 7561 7469 6e67  s for evaluating
+00000f30: 2062 6174 6368 2063 6f72 7265 6374 696f   batch correctio
+00000f40: 6e20 616e 6420 6269 6f6c 6f67 6963 616c  n and biological
+00000f50: 2063 6f6e 7365 7276 6174 696f 6e20 696e   conservation in
+00000f60: 2074 6865 2060 7363 6962 2e6d 6574 7269   the `scib.metri
+00000f70: 6373 600a 6d6f 6475 6c65 2e0a 0a3c 7461  cs`.module...<ta
+00000f80: 626c 6520 636c 6173 733d 2264 6f63 7574  ble class="docut
+00000f90: 696c 7320 616c 6967 6e2d 6465 6661 756c  ils align-defaul
+00000fa0: 7422 3e0a 2020 3c63 6f6c 6772 6f75 703e  t">.  <colgroup>
+00000fb0: 0a20 2020 203c 636f 6c20 7374 796c 653d  .    <col style=
+00000fc0: 2277 6964 7468 3a20 3530 2522 202f 3e0a  "width: 50%" />.
+00000fd0: 2020 2020 3c63 6f6c 2073 7479 6c65 3d22      <col style="
+00000fe0: 7769 6474 683a 2035 3025 2220 2f3e 0a20  width: 50%" />. 
+00000ff0: 203c 2f63 6f6c 6772 6f75 703e 0a20 203c   </colgroup>.  <
+00001000: 7468 6561 643e 0a20 2020 203c 7472 2063  thead>.    <tr c
+00001010: 6c61 7373 3d22 726f 772d 6f64 6422 3e3c  lass="row-odd"><
+00001020: 7468 2063 6c61 7373 3d22 6865 6164 223e  th class="head">
+00001030: 3c70 3e42 696f 6c6f 6769 6361 6c20 436f  <p>Biological Co
+00001040: 6e73 6572 7661 7469 6f6e 3c2f 703e 3c2f  nservation</p></
+00001050: 7468 3e0a 2020 2020 2020 3c74 6820 636c  th>.      <th cl
+00001060: 6173 733d 2268 6561 6422 3e3c 703e 4261  ass="head"><p>Ba
+00001070: 7463 6820 436f 7272 6563 7469 6f6e 3c2f  tch Correction</
+00001080: 703e 3c2f 7468 3e0a 2020 2020 3c2f 7472  p></th>.    </tr
+00001090: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
+000010a0: 7462 6f64 793e 0a20 2020 203c 7472 2063  tbody>.    <tr c
+000010b0: 6c61 7373 3d22 726f 772d 6576 656e 2220  lass="row-even" 
+000010c0: 3e0a 2020 2020 2020 3c74 643e 3c75 6c20  >.      <td><ul 
+000010d0: 636c 6173 733d 2273 696d 706c 6522 3e0a  class="simple">.
+000010e0: 2020 2020 2020 2020 3c6c 693e 3c70 3e43          <li><p>C
+000010f0: 656c 6c20 7479 7065 2041 5357 3c2f 703e  ell type ASW</p>
+00001100: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
+00001110: 693e 3c70 3e43 656c 6c20 6379 636c 6520  i><p>Cell cycle 
+00001120: 636f 6e73 6572 7661 7469 6f6e 3c2f 703e  conservation</p>
+00001130: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
+00001140: 693e 3c70 3e47 7261 7068 2063 4c49 5349  i><p>Graph cLISI
+00001150: 3c2f 703e 3c2f 6c69 3e0a 2020 2020 2020  </p></li>.      
+00001160: 2020 3c6c 693e 3c70 3e41 646a 7573 7465    <li><p>Adjuste
+00001170: 6420 7261 6e64 2069 6e64 6578 2028 4152  d rand index (AR
+00001180: 4929 2066 6f72 2063 656c 6c20 6c61 6265  I) for cell labe
+00001190: 6c3c 2f70 3e3c 2f6c 693e 0a20 2020 2020  l</p></li>.     
+000011a0: 2020 203c 6c69 3e3c 703e 4e6f 726d 616c     <li><p>Normal
+000011b0: 6973 6564 206d 7574 7561 6c20 696e 666f  ised mutual info
+000011c0: 726d 6174 696f 6e20 284e 4d49 2920 666f  rmation (NMI) fo
+000011d0: 7220 6365 6c6c 206c 6162 656c 3c2f 703e  r cell label</p>
+000011e0: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
+000011f0: 693e 3c70 3e48 6967 686c 7920 7661 7269  i><p>Highly vari
+00001200: 6162 6c65 2067 656e 6520 636f 6e73 6572  able gene conser
+00001210: 7661 7469 6f6e 3c2f 703e 3c2f 6c69 3e0a  vation</p></li>.
+00001220: 2020 2020 2020 2020 3c6c 693e 3c70 3e49          <li><p>I
+00001230: 736f 6c61 7465 6420 6c61 6265 6c20 4153  solated label AS
+00001240: 573c 2f70 3e3c 2f6c 693e 0a20 2020 2020  W</p></li>.     
+00001250: 2020 203c 6c69 3e3c 703e 4973 6f6c 6174     <li><p>Isolat
+00001260: 6564 206c 6162 656c 2046 313c 2f70 3e3c  ed label F1</p><
+00001270: 2f6c 693e 0a20 2020 2020 2020 203c 6c69  /li>.        <li
+00001280: 3e3c 703e 5472 616a 6563 746f 7279 2063  ><p>Trajectory c
+00001290: 6f6e 7365 7276 6174 696f 6e3c 2f70 3e3c  onservation</p><
+000012a0: 2f6c 693e 0a20 2020 2020 203c 2f75 6c3e  /li>.      </ul>
+000012b0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000012c0: 3c75 6c20 636c 6173 733d 2273 696d 706c  <ul class="simpl
+000012d0: 6522 3e0a 2020 2020 2020 2020 3c6c 693e  e">.        <li>
+000012e0: 3c70 3e42 6174 6368 2041 5357 3c2f 703e  <p>Batch ASW</p>
+000012f0: 3c2f 6c69 3e0a 2020 2020 2020 2020 3c6c  </li>.        <l
+00001300: 693e 3c70 3e50 7269 6e63 6970 616c 2063  i><p>Principal c
+00001310: 6f6d 706f 6e65 6e74 2072 6567 7265 7373  omponent regress
+00001320: 696f 6e3c 2f70 3e3c 2f6c 693e 0a20 2020  ion</p></li>.   
+00001330: 2020 2020 203c 6c69 3e3c 703e 4772 6170       <li><p>Grap
+00001340: 6820 694c 4953 493c 2f70 3e3c 2f6c 693e  h iLISI</p></li>
+00001350: 0a20 2020 2020 2020 203c 6c69 3e3c 703e  .        <li><p>
+00001360: 4772 6170 6820 636f 6e6e 6563 7469 7669  Graph connectivi
+00001370: 7479 3c2f 703e 3c2f 6c69 3e0a 2020 2020  ty</p></li>.    
+00001380: 2020 2020 3c6c 693e 3c70 3e6b 4245 5420      <li><p>kBET 
+00001390: 284b 2d6e 6561 7265 7374 206e 6569 6768  (K-nearest neigh
+000013a0: 626f 7572 2062 6174 6368 2065 6666 6563  bour batch effec
+000013b0: 7429 3c2f 703e 3c2f 6c69 3e0a 2020 2020  t)</p></li>.    
+000013c0: 2020 3c2f 756c 3e3c 2f74 643e 0a20 2020    </ul></td>.   
+000013d0: 203c 2f74 723e 0a20 203c 2f74 626f 6479   </tr>.  </tbody
+000013e0: 3e0a 3c2f 7461 626c 653e 0a0a 466f 7220  >.</table>..For 
+000013f0: 6120 6465 7461 696c 6564 2064 6573 6372  a detailed descr
+00001400: 6970 7469 6f6e 206f 6620 7468 6520 6d65  iption of the me
+00001410: 7472 6963 7320 696d 706c 656d 656e 7465  trics implemente
+00001420: 6420 696e 2074 6869 7320 7061 636b 6167  d in this packag
+00001430: 652c 2070 6c65 6173 6520 7365 6520 6f75  e, please see ou
+00001440: 720a 5b70 7562 6c69 6361 7469 6f6e 5d28  r.[publication](
+00001450: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
+00001460: 3130 2e31 3033 382f 7334 3135 3932 2d30  10.1038/s41592-0
+00001470: 3231 2d30 3133 3336 2d38 2920 616e 6420  21-01336-8) and 
+00001480: 7468 6520 7061 636b 6167 6520 5b64 6f63  the package [doc
+00001490: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+000014a0: 733a 2f2f 7363 6962 2e72 6561 6474 6865  s://scib.readthe
+000014b0: 646f 6373 2e69 6f2f 292e 0a0a 2323 2049  docs.io/)...## I
+000014c0: 6e74 6567 7261 7469 6f6e 2054 6f6f 6c73  ntegration Tools
+000014d0: 0a0a 546f 6f6c 7320 7468 6174 2061 7265  ..Tools that are
+000014e0: 2063 6f6d 7061 7265 6420 696e 636c 7564   compared includ
+000014f0: 653a 0a0a 2d20 5b42 424b 4e4e 5d28 6874  e:..- [BBKNN](ht
+00001500: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001510: 2f54 6569 6368 6c61 622f 6262 6b6e 6e29  /Teichlab/bbknn)
+00001520: 2031 2e33 2e39 0a2d 205b 436f 6d62 6174   1.3.9.- [Combat
+00001530: 5d28 6874 7470 733a 2f2f 7363 616e 7079  ](https://scanpy
+00001540: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001550: 656e 2f73 7461 626c 652f 6170 692f 7363  en/stable/api/sc
+00001560: 616e 7079 2e70 702e 636f 6d62 6174 2e68  anpy.pp.combat.h
+00001570: 746d 6c29 205b 7061 7065 725d 2868 7474  tml) [paper](htt
+00001580: 7073 3a2f 2f61 6361 6465 6d69 632e 6f75  ps://academic.ou
+00001590: 702e 636f 6d2f 6269 6f73 7461 7469 7374  p.com/biostatist
+000015a0: 6963 732f 6172 7469 636c 652f 382f 312f  ics/article/8/1/
+000015b0: 3131 382f 3235 3230 3733 290a 2d20 5b43  118/252073).- [C
+000015c0: 6f6e 6f73 5d28 6874 7470 733a 2f2f 6769  onos](https://gi
+000015d0: 7468 7562 2e63 6f6d 2f68 6d73 2d64 626d  thub.com/hms-dbm
+000015e0: 692f 636f 6e6f 7329 2031 2e33 2e30 0a2d  i/conos) 1.3.0.-
+000015f0: 205b 4445 5343 5d28 6874 7470 733a 2f2f   [DESC](https://
+00001600: 6769 7468 7562 2e63 6f6d 2f65 6c65 6f7a  github.com/eleoz
+00001610: 7a72 2f64 6573 6329 2032 2e30 2e33 0a2d  zr/desc) 2.0.3.-
+00001620: 205b 4661 7374 4d4e 4e5d 2868 7474 7073   [FastMNN](https
+00001630: 3a2f 2f62 696f 636f 6e64 7563 746f 722e  ://bioconductor.
+00001640: 6f72 672f 7061 636b 6167 6573 2f62 6174  org/packages/bat
+00001650: 6368 656c 6f72 2f29 2028 6261 7463 6865  chelor/) (batche
+00001660: 6c6f 7220 312e 342e 3029 0a2d 205b 4861  lor 1.4.0).- [Ha
+00001670: 726d 6f6e 795d 2868 7474 7073 3a2f 2f67  rmony](https://g
+00001680: 6974 6875 622e 636f 6d2f 696d 6d75 6e6f  ithub.com/immuno
+00001690: 6765 6e6f 6d69 6373 2f68 6172 6d6f 6e79  genomics/harmony
+000016a0: 2920 312e 300a 2d20 5b4c 4947 4552 5d28  ) 1.0.- [LIGER](
+000016b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000016c0: 6f6d 2f4d 6163 6f73 6b6f 4c61 622f 6c69  om/MacoskoLab/li
+000016d0: 6765 7229 2030 2e35 2e30 0a2d 205b 4d4e  ger) 0.5.0.- [MN
+000016e0: 4e5d 2868 7474 7073 3a2f 2f67 6974 6875  N](https://githu
+000016f0: 622e 636f 6d2f 6368 7269 7363 6169 6e78  b.com/chriscainx
+00001700: 2f6d 6e6e 7079 2920 302e 312e 392e 350a  /mnnpy) 0.1.9.5.
+00001710: 2d20 5b53 4155 4349 455d 2868 7474 7073  - [SAUCIE](https
+00001720: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b72  ://github.com/Kr
+00001730: 6973 686e 6173 7761 6d79 4c61 622f 5341  ishnaswamyLab/SA
+00001740: 5543 4945 290a 2d20 5b53 6361 6e6f 7261  UCIE).- [Scanora
+00001750: 6d61 5d28 6874 7470 733a 2f2f 6769 7468  ma](https://gith
+00001760: 7562 2e63 6f6d 2f62 7269 616e 6869 652f  ub.com/brianhie/
+00001770: 7363 616e 6f72 616d 6129 2031 2e37 2e30  scanorama) 1.7.0
+00001780: 0a2d 205b 7363 414e 5649 5d28 6874 7470  .- [scANVI](http
+00001790: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+000017a0: 6865 6e6c 696e 6761 6e74 656c 6f70 652f  henlingantelope/
+000017b0: 4861 726d 6f6e 697a 6174 696f 6e53 4341  HarmonizationSCA
+000017c0: 4e56 4929 2028 7363 5649 2030 2e36 2e37  NVI) (scVI 0.6.7
+000017d0: 290a 2d20 5b73 6347 656e 5d28 6874 7470  ).- [scGen](http
+000017e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000017f0: 6865 6973 6c61 622f 7363 6765 6e29 2031  heislab/scgen) 1
+00001800: 2e31 2e35 0a2d 205b 7363 5649 5d28 6874  .1.5.- [scVI](ht
+00001810: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001820: 2f59 6f73 6566 4c61 622f 7363 5649 2920  /YosefLab/scVI) 
+00001830: 302e 362e 370a 2d20 5b53 6575 7261 7420  0.6.7.- [Seurat 
+00001840: 7633 5d28 6874 7470 733a 2f2f 6769 7468  v3](https://gith
+00001850: 7562 2e63 6f6d 2f73 6174 696a 616c 6162  ub.com/satijalab
+00001860: 2f73 6575 7261 7429 2033 2e32 2e30 2043  /seurat) 3.2.0 C
+00001870: 4341 2028 6465 6661 756c 7429 2061 6e64  CA (default) and
+00001880: 2052 5043 410a 2d20 5b54 7256 6165 5d28   RPCA.- [TrVae](
+00001890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000018a0: 6f6d 2f74 6865 6973 6c61 622f 7472 7661  om/theislab/trva
+000018b0: 6529 2030 2e30 2e31 0a2d 205b 5472 5661  e) 0.0.1.- [TrVa
+000018c0: 6570 5d28 6874 7470 733a 2f2f 6769 7468  ep](https://gith
+000018d0: 7562 2e63 6f6d 2f74 6865 6973 6c61 622f  ub.com/theislab/
+000018e0: 7472 7661 6570 2920 302e 312e 300a 0a23  trvaep) 0.1.0..#
+000018f0: 2320 4465 7665 6c6f 706d 656e 740a 0a46  # Development..F
+00001900: 6f72 2064 6576 656c 6f70 696e 6720 7468  or developing th
+00001910: 6973 2070 6163 6b61 6765 2c20 706c 6561  is package, plea
+00001920: 7365 206d 616b 6520 7375 7265 2074 6f20  se make sure to 
+00001930: 696e 7374 616c 6c20 6164 6469 7469 6f6e  install addition
+00001940: 616c 2064 6570 656e 6465 6e63 6965 7320  al dependencies 
+00001950: 736f 2074 6861 7420 796f 7520 6361 6e20  so that you can 
+00001960: 7573 6520 6070 7974 6573 7460 2061 6e64  use `pytest` and
+00001970: 0a60 7072 652d 636f 6d6d 6974 602e 0a0a  .`pre-commit`...
+00001980: 6060 6073 6865 6c6c 0a70 6970 2069 6e73  ```shell.pip ins
+00001990: 7461 6c6c 202d 6520 272e 5b74 6573 742c  tall -e '.[test,
+000019a0: 6465 765d 270a 6060 600a 0a50 6c65 6173  dev]'.```..Pleas
+000019b0: 6520 7265 6665 7220 746f 2074 6865 2060  e refer to the `
+000019c0: 7365 7475 702e 6366 6760 2066 6f72 206d  setup.cfg` for m
+000019d0: 6f72 6520 6f70 7469 6f6e 616c 2064 6570  ore optional dep
+000019e0: 656e 6465 6e63 6965 732e 0a0a 496e 7374  endencies...Inst
+000019f0: 616c 6c20 6070 7265 2d63 6f6d 6d69 7460  all `pre-commit`
+00001a00: 2074 6f20 7468 6520 7265 706f 7369 746f   to the reposito
+00001a10: 7279 2066 6f72 2072 756e 6e69 6e67 2069  ry for running i
+00001a20: 7420 6175 746f 6d61 7469 6361 6c6c 7920  t automatically 
+00001a30: 6576 6572 7920 7469 6d65 2079 6f75 2063  every time you c
+00001a40: 6f6d 6d69 7420 696e 2067 6974 2e0a 0a60  ommit in git...`
+00001a50: 6060 7368 656c 6c0a 7072 652d 636f 6d6d  ``shell.pre-comm
+00001a60: 6974 2069 6e73 7461 6c6c 0a60 6060 0a    it install.```.
```

### Comparing `scib-1.1.4/scib/__init__.py` & `scib-1.1.5/scib/__init__.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/exceptions.py` & `scib-1.1.5/scib/exceptions.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/integration.py` & `scib-1.1.5/scib/integration.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/knn_graph/knn_graph.cpp` & `scib-1.1.5/scib/knn_graph/knn_graph.cpp`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/knn_graph/knn_graph.o` & `scib-1.1.5/scib/knn_graph/knn_graph.o`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -27,15 +27,15 @@
   [22] .init_array       INIT_ARRAY      00000000000099c8 0089c8 000010 08  WA  0   0  8
   [23] .fini_array       FINI_ARRAY      00000000000099d8 0089d8 000008 08  WA  0   0  8
   [24] .data.rel.ro      PROGBITS        00000000000099e0 0089e0 000200 00  WA  0   0 32
   [25] .dynamic          DYNAMIC         0000000000009be0 008be0 000210 10  WA  7   0  8
   [26] .got              PROGBITS        0000000000009df0 008df0 000210 08  WA  0   0  8
   [27] .data             PROGBITS        000000000000a000 009000 000018 00  WA  0   0  8
   [28] .bss              NOBITS          000000000000a040 009018 000238 00  WA  0   0 64
-  [29] .comment          PROGBITS        0000000000000000 009018 00002d 01  MS  0   0  1
+  [29] .comment          PROGBITS        0000000000000000 009018 00002b 01  MS  0   0  1
   [30] .symtab           SYMTAB          0000000000000000 009048 000c30 18     31  39  8
   [31] .strtab           STRTAB          0000000000000000 009c78 00179b 00      0   0  1
   [32] .shstrtab         STRTAB          0000000000000000 00b413 000139 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000020	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK, x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7fac9fd744cb5f50c84d64510c934390dea8a63b
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: cf9e1d46c375fcf4b4bde0d07d6fc8b82f38fa5b
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -108,15 +108,15 @@
  matrixfile, output_prefix, k, n_chunks, percent_subsample
 matrix must be symmetric and non-empty
 malformed matrix format, cell offset out of bounds 
 malformed matrix format, row number decreased 
 malformed matrix format, column number decreased 
 vector::_M_fill_insert
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
+GCC: (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
 __abi_tag
 knn_graph.cpp
 _ZN12_GLOBAL__N_16MatrixD2Ev
 _ZN12_GLOBAL__N_16MatrixD1Ev
 _ZNSt6vectorIN12_GLOBAL__N_16Matrix5EntryESaIS2_EE7reserveEm
 _ZNSt10_HashtableIjSt4pairIKjjESaIS2_ENSt8__detail10_Select1stESt8equal_toIjESt4hashIjENS4_18_Mod_range_hashingENS4_20_Default_ranged_hashENS4_20_Prime_rehash_policyENS4_17_Hashtable_traitsILb0ELb0ELb1EEEE8_M_eraseESt17integral_constantIbLb1EERS1_.isra.0
 _ZSt4endlIcSt11char_traitsIcEERSt13basic_ostreamIT_T0_ES6_.isra.0
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
+  [     0]  GCC: (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0
```

### Comparing `scib-1.1.4/scib/metrics/__init__.py` & `scib-1.1.5/scib/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/ari.py` & `scib-1.1.5/scib/metrics/ari.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import numpy as np
 import pandas as pd
 import scipy.special
-from scanpy._utils import deprecated_arg_names
 from sklearn.metrics.cluster import adjusted_rand_score
 
+try:
+    from scanpy._utils import renamed_arg
+except ImportError:
+    from .._package_tools import renamed_arg
+
 from ..utils import check_adata, check_batch
 
 
-@deprecated_arg_names({"group1": "cluster_key", "group2": "label_key"})
+@renamed_arg("group1", "cluster_key")
+@renamed_arg("group2", "label_key")
 def ari(adata, cluster_key, label_key, implementation=None):
     """Adjusted Rand Index
 
     The adjusted rand index is a chance-adjusted rand index, which evaluates the pair-wise accuracy of clustering vs.
     ground truth label assignments.
     The score ranges between 0 and 1 with larger values indicating better conservation of the data-driven cell identity
     discovery after integration compared to annotated labels.
```

### Comparing `scib-1.1.4/scib/metrics/cell_cycle.py` & `scib-1.1.5/scib/metrics/cell_cycle.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,20 @@
 
         scores_before.append(before)
         scores_after.append(after)
         scores_final.append(score)
 
     if agg_func is None:
         return pd.DataFrame(
-            [batches, scores_before, scores_after, scores_final],
-            columns=["batch", "before", "after", "score"],
+            {
+                "batch": pd.Series(batches, dtype=str),
+                "before": pd.Series(scores_before, dtype=float),
+                "after": pd.Series(scores_after, dtype=float),
+                "score": pd.Series(scores_final, dtype=float),
+            }
         )
     else:
         return agg_func(scores_final)
 
 
 def get_pcr_before_after(
     adata_pre,
```

### Comparing `scib-1.1.4/scib/metrics/clustering.py` & `scib-1.1.5/scib/metrics/clustering.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/graph_connectivity.py` & `scib-1.1.5/scib/metrics/graph_connectivity.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/highly_variable_genes.py` & `scib-1.1.5/scib/metrics/highly_variable_genes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import numpy as np
 import scanpy as sc
-from scanpy._utils import deprecated_arg_names
+
+try:
+    from scanpy._utils import renamed_arg
+except ImportError:
+    from .._package_tools import renamed_arg
 
 from ..utils import split_batches
 
 
 def precompute_hvg_batch(adata, batch, features, n_hvg=500, save_hvg=False):
     """
     Compute HVGs per batch
@@ -32,15 +36,15 @@
 
     if save_hvg:
         adata.uns["hvg_before"] = hvg_dir
     else:
         return hvg_dir
 
 
-@deprecated_arg_names({"batch": "batch_key"})
+@renamed_arg("batch", "batch_key")
 def hvg_overlap(adata_pre, adata_post, batch_key, n_hvg=500, verbose=False):
     """Highly variable gene overlap
 
     Metric that computes the average percentage of overlapping highly variable genes per batch pre post integration.
 
     :param adata_pre: Unintegrated anndata object
     :param adata_post: Integrated anndata object
```

### Comparing `scib-1.1.4/scib/metrics/isolated_labels.py` & `scib-1.1.5/scib/metrics/isolated_labels.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/kbet.py` & `scib-1.1.5/scib/metrics/kbet.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/lisi.py` & `scib-1.1.5/scib/metrics/lisi.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/metrics.py` & `scib-1.1.5/scib/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/metrics/nmi.py` & `scib-1.1.5/scib/metrics/nmi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import os
 import subprocess
 
-from scanpy._utils import deprecated_arg_names
 from sklearn.metrics.cluster import normalized_mutual_info_score
 
+try:
+    from scanpy._utils import renamed_arg
+except ImportError:
+    from .._package_tools import renamed_arg
+
 from ..utils import check_adata, check_batch
 
 
-@deprecated_arg_names(
-    {"group1": "cluster_key", "group2": "label_key", "method": "implementation"}
-)
+@renamed_arg("group1", "cluster_key")
+@renamed_arg("group2", "label_key")
+@renamed_arg("method", "implementation")
 def nmi(adata, cluster_key, label_key, implementation="arithmetic", nmi_dir=None):
     """Normalized mutual information
 
     The normalized mutual information is a version of the mutual information corrected by the entropy of clustering and
     ground truth labels (e.g. cell type).
     The score ranges between 0 and 1, with 0 representing no sharing and 1 representing perfect sharing of information
     between clustering and annotated cell labels.
```

### Comparing `scib-1.1.4/scib/metrics/pcr.py` & `scib-1.1.5/scib/metrics/pcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         if n_comps is None or n_comps > min(matrix.shape):
             n_comps = min(matrix.shape)
 
         if n_comps == min(matrix.shape):
             svd_solver = "full"
             # convert to dense bc 'full' is not available for sparse matrices
             if sparse.issparse(matrix):
-                matrix = matrix.todense()
+                matrix = matrix.toarray()
 
         if verbose:
             print("compute PCA")
         X_pca, _, _, pca_var = sc.tl.pca(
             matrix,
             n_comps=n_comps,
             use_highly_variable=False,
```

### Comparing `scib-1.1.4/scib/metrics/silhouette.py` & `scib-1.1.5/scib/metrics/silhouette.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import numpy as np
 import pandas as pd
-from scanpy._utils import deprecated_arg_names
 from sklearn.metrics.cluster import silhouette_samples, silhouette_score
 
+try:
+    from scanpy._utils import renamed_arg
+except ImportError:
+    from .._package_tools import renamed_arg
 
-@deprecated_arg_names({"group_key": "label_key"})
+
+@renamed_arg("group_key", "label_key")
 def silhouette(adata, label_key, embed, metric="euclidean", scale=True):
     """Average silhouette width (ASW)
 
     Wrapper for sklearn silhouette function values range from [-1, 1] with
 
         * 1 indicates distinct, compact clusters
         * 0 indicates overlapping clusters
@@ -46,15 +50,15 @@
         X=adata.obsm[embed], labels=adata.obs[label_key], metric=metric
     )
     if scale:
         asw = (asw + 1) / 2
     return asw
 
 
-@deprecated_arg_names({"group_key": "label_key"})
+@renamed_arg("group_key", "label_key")
 def silhouette_batch(
     adata,
     batch_key,
     label_key,
     embed,
     metric="euclidean",
     return_all=False,
```

### Comparing `scib-1.1.4/scib/metrics/trajectory.py` & `scib-1.1.5/scib/metrics/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         Column can contain empty entries, the dataset will be subset to the cells with scores.
     :param dpt_dim: number of diffmap dimensions used to determine root
     """
     n_components, adata_post.obs["neighborhood"] = connected_components(
         csgraph=adata_post.obsp["connectivities"], directed=False, return_labels=True
     )
 
-    start_clust = adata_pre.obs.groupby([ct_key]).mean()[pseudotime_key].idxmin()
+    start_clust = adata_pre.obs.groupby(ct_key)[pseudotime_key].mean().idxmin()
     min_dpt = adata_pre.obs[adata_pre.obs[ct_key] == start_clust].index
     which_max_neigh = (
         adata_post.obs["neighborhood"]
         == adata_post.obs["neighborhood"].value_counts().idxmax()
     )
     min_dpt = [
         value for value in min_dpt if value in adata_post.obs[which_max_neigh].index
```

### Comparing `scib-1.1.4/scib/metrics/utils.py` & `scib-1.1.5/scib/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/preprocessing.py` & `scib-1.1.5/scib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/trajectory_inference.py` & `scib-1.1.5/scib/trajectory_inference.py`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib/utils.py` & `scib-1.1.5/scib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,8 +72,8 @@
     return anndata.AnnData.concatenate(*adata_list, **kwargs)
 
 
 def todense(adata):
     import scipy
 
     if isinstance(adata.X, scipy.sparse.csr_matrix):
-        adata.X = adata.X.todense()
+        adata.X = adata.X.toarray()
```

### Comparing `scib-1.1.4/scib.egg-info/PKG-INFO` & `scib-1.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scib
-Version: 1.1.4
+Version: 1.1.5
 Summary: Evaluating single-cell data integration methods
 Home-page: https://github.com/theislab/scib
 Author: Malte D. Luecken, Maren Buettner, Daniel C. Strobl, Michaela F. Mueller
 Author-email: malte.luecken@helmholtz-muenchen.de, michaela.mueller@helmholtz-muenchen.de
 License: MIT
 Project-URL: Pipeline, https://github.com/theislab/scib-pipeline
 Project-URL: Reproducibility, https://theislab.github.io/scib-reproducibility
@@ -12,34 +12,77 @@
 Keywords: benchmarking,single cell,data integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: pandas>=2
+Requires-Dist: seaborn
+Requires-Dist: matplotlib
+Requires-Dist: numba
+Requires-Dist: scanpy>=1.5
+Requires-Dist: anndata>=0.7.2
+Requires-Dist: h5py
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: scikit-misc
+Requires-Dist: leidenalg
+Requires-Dist: umap-learn
+Requires-Dist: pydot
+Requires-Dist: igraph>=0.10
+Requires-Dist: llvmlite
+Requires-Dist: deprecated
 Provides-Extra: rpy2
+Requires-Dist: rpy2>=3; extra == "rpy2"
+Requires-Dist: anndata2ri; extra == "rpy2"
 Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-icdiff; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: codecov; extra == "test"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: bump2version; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: myst_parser; extra == "docs"
+Requires-Dist: sphinx-automodapi; extra == "docs"
 Provides-Extra: louvain
+Requires-Dist: python-igraph; extra == "louvain"
+Requires-Dist: louvain>=0.8; extra == "louvain"
 Provides-Extra: bbknn
+Requires-Dist: bbknn==1.3.9; extra == "bbknn"
 Provides-Extra: scanorama
+Requires-Dist: scanorama>=1.7.4; extra == "scanorama"
 Provides-Extra: mnn
+Requires-Dist: mnnpy==0.1.9.5; extra == "mnn"
 Provides-Extra: scgen
+Requires-Dist: scgen>=2.1.0; extra == "scgen"
 Provides-Extra: scvi
+Requires-Dist: scvi-tools>=0.16; extra == "scvi"
 Provides-Extra: trvae
+Requires-Dist: trvae==1.1.2; extra == "trvae"
 Provides-Extra: trvaep
+Requires-Dist: trvaep==0.1.0; extra == "trvaep"
 Provides-Extra: desc
+Requires-Dist: desc==2.0.3; extra == "desc"
 Provides-Extra: harmony
-License-File: LICENSE.txt
+Requires-Dist: harmony-pytorch; extra == "harmony"
 
 [![Stars](https://img.shields.io/github/stars/theislab/scib?logo=GitHub&color=yellow)](https://github.com/theislab/scib/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/scib?logo=PyPI)](https://pypi.org/project/scib)
 [![PyPIDownloads](https://pepy.tech/badge/scib)](https://pepy.tech/project/scib)
 [![Build Status](https://github.com/theislab/scib/actions/workflows/test.yml/badge.svg)](https://github.com/theislab/scib/actions/workflows/test.yml)
 [![Documentation](https://readthedocs.org/projects/scib/badge/?version=latest)](https://scib.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/theislab/scib/branch/main/graph/badge.svg?token=M1nuTpAxyS)](https://codecov.io/gh/theislab/scib)
```

### Comparing `scib-1.1.4/scib.egg-info/SOURCES.txt` & `scib-1.1.5/scib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scib-1.1.4/scib.egg-info/requires.txt` & `scib-1.1.5/scib.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 numpy
-pandas<2
+pandas>=2
 seaborn
 matplotlib
 numba
 scanpy>=1.5
 anndata>=0.7.2
 h5py
 scipy
@@ -46,21 +46,21 @@
 mnnpy==0.1.9.5
 
 [rpy2]
 rpy2>=3
 anndata2ri
 
 [scanorama]
-scanorama==1.7.0
+scanorama>=1.7.4
 
 [scgen]
 scgen>=2.1.0
 
 [scvi]
-scvi-tools>=0.16.1
+scvi-tools>=0.16
 
 [test]
 pytest
 pytest-icdiff
 pytest-cov
 codecov
```

### Comparing `scib-1.1.4/setup.cfg` & `scib-1.1.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.4
+current_version = 1.1.5
 commit = True
 tag = True
 
 [bumpversion:file:VERSION.txt]
 search = {current_version}
 replace = {new_version}
 
@@ -28,29 +28,29 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Software Development :: Build Tools
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [bdist_wheel]
 build_number = 1
 
 [options]
 packages = 
 	scib
 	scib.metrics
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	numpy
-	pandas<2
+	pandas>=2
 	seaborn
 	matplotlib
 	numba
 	scanpy>=1.5
 	anndata>=0.7.2
 	h5py
 	scipy
@@ -72,18 +72,18 @@
 [options.extras_require]
 rpy2 = rpy2>=3; anndata2ri
 test = pytest; pytest-icdiff; pytest-cov; codecov
 dev = build; twine; isort; bump2version; pre-commit
 docs = sphinx; sphinx_rtd_theme; myst_parser; sphinx-automodapi
 louvain = python-igraph; louvain>=0.8
 bbknn = bbknn ==1.3.9
-scanorama = scanorama ==1.7.0
+scanorama = scanorama >=1.7.4
 mnn = mnnpy ==0.1.9.5
 scgen = scgen  >=2.1.0
-scvi = scvi-tools  >=0.16.1
+scvi = scvi-tools  >=0.16
 trvae = trvae  ==1.1.2
 trvaep = trvaep  ==0.1.0
 desc = desc  ==2.0.3
 harmony = harmony-pytorch
 
 [tool.isort]
 include_trailing_comma = true
```

### Comparing `scib-1.1.4/setup.py` & `scib-1.1.5/setup.py`

 * *Files identical despite different names*

