# Comparing `tmp/FinaleTools-0.4.2.tar.gz` & `tmp/FinaleTools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinaleTools-0.4.2.tar", last modified: Fri Mar 29 02:11:51 2024, max compression
+gzip compressed data, was "FinaleTools-0.4.3.tar", last modified: Mon Apr  1 20:44:27 2024, max compression
```

## Comparing `FinaleTools-0.4.2.tar` & `FinaleTools-0.4.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.2/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5686 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3514 2024-03-29 02:06:16.000000 FinaleTools-0.4.2/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-03-29 02:11:45.000000 FinaleTools-0.4.2/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5686 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/FinaleTools.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.2/src/finaletools/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    23075 2024-03-29 01:49:46.000000 FinaleTools-0.4.2/src/finaletools/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/agg_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.2/src/finaletools/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8273 2024-03-29 02:06:16.000000 FinaleTools-0.4.2/src/finaletools/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14487 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2012 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14184 2024-03-29 01:22:38.000000 FinaleTools-0.4.2/src/finaletools/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.2/src/finaletools/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.2/src/finaletools/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.2/src/finaletools/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 02:11:51.000000 FinaleTools-0.4.2/src/finaletools/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.2/src/finaletools/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18313 2024-03-29 01:49:46.000000 FinaleTools-0.4.2/src/finaletools/utils/utils.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 FinaleTools-0.4.3/LICENSE
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3739 2024-04-01 20:34:46.000000 FinaleTools-0.4.3/README.md
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1058 2024-04-01 20:28:58.000000 FinaleTools-0.4.3/pyproject.toml
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/setup.cfg
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     5911 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/PKG-INFO
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1083 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/SOURCES.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/dependency_links.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       57 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/entry_points.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/requires.txt
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       12 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/FinaleTools.egg-info/top_level.txt
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2023-06-21 12:51:49.000000 FinaleTools-0.4.3/src/finaletools/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/cli/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/cli/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    24643 2024-04-01 20:31:34.000000 FinaleTools-0.4.3/src/finaletools/cli/main_cli.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/frag/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)      509 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9664 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/adjust_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4402 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/agg_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9329 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/frag/cleavage_profile.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8349 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/coverage.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14488 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi_gc_correct.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2080 2024-04-01 20:23:25.000000 FinaleTools-0.4.3/src/finaletools/frag/delfi_merge_bins.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14184 2024-03-29 01:22:38.000000 FinaleTools-0.4.3/src/finaletools/frag/end_motifs.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14865 2024-03-29 02:06:16.000000 FinaleTools-0.4.3/src/finaletools/frag/frag_length.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8466 2024-03-29 02:06:16.000000 FinaleTools-0.4.3/src/finaletools/frag/multi_wps.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6797 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/frag/wps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/genome/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       37 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/genome/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14339 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/genome/gaps.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/methylation/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/methylation/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/qc/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/qc/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/too/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/too/__init__.py
+drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-04-01 20:44:27.000000 FinaleTools-0.4.3/src/finaletools/utils/
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)       90 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/__init__.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/cli_hist.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-03-29 01:22:39.000000 FinaleTools-0.4.3/src/finaletools/utils/filter_bam.py
+-rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18313 2024-03-29 01:49:46.000000 FinaleTools-0.4.3/src/finaletools/utils/utils.py
```

### Comparing `FinaleTools-0.4.2/LICENSE` & `FinaleTools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/PKG-INFO` & `FinaleTools-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,17 +46,17 @@
 Requires-Dist: statsmodels
 Requires-Dist: sphinx<7.0.0
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: sphinx-argparse
 Requires-Dist: loess
 
 # FinaleTools
-Lightweight Python library and standalone program to extract features from
-cfDNA paired-end reads. FinaleTools refers to FragmentatIoN AnaLysis of
-cEll-free DNA Tools.
+A package and standalone program to extract fragmentation patterns of cell-free
+DNA from paired-end sequencing data. FinaleTools refers to FragmentatIoN
+AnaLysis of cEll-free DNA Tools.
 
 FinaleTools is in active development, and all API is subject to change and
 should be considered unstable.
 
 ## Installation
 Instructions:
 - (Optional) create a conda or venv environment to use FinaleTools in.
@@ -124,7 +124,13 @@
 03.79%                       ▃██████████                        
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
 ```
+
+## FAQ
+Q: When running on an ARM64 Mac, I can install FinaleTools without errors.
+However, I get an `ImportError` when I run it.
+
+A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `FinaleTools-0.4.2/README.md` & `FinaleTools-0.4.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # FinaleTools
-Lightweight Python library and standalone program to extract features from
-cfDNA paired-end reads. FinaleTools refers to FragmentatIoN AnaLysis of
-cEll-free DNA Tools.
+A package and standalone program to extract fragmentation patterns of cell-free
+DNA from paired-end sequencing data. FinaleTools refers to FragmentatIoN
+AnaLysis of cEll-free DNA Tools.
 
 FinaleTools is in active development, and all API is subject to change and
 should be considered unstable.
 
 ## Installation
 Instructions:
 - (Optional) create a conda or venv environment to use FinaleTools in.
@@ -72,8 +72,14 @@
 04.55%                        ▄████████▁                        
 03.79%                       ▃██████████                        
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
-```
+```
+
+## FAQ
+Q: When running on an ARM64 Mac, I can install FinaleTools without errors.
+However, I get an `ImportError` when I run it.
+
+A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `FinaleTools-0.4.2/pyproject.toml` & `FinaleTools-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleTools"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `FinaleTools-0.4.2/src/FinaleTools.egg-info/PKG-INFO` & `FinaleTools-0.4.3/src/FinaleTools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleTools
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package and standalone program to process paired-end reads of cfDNA fragment WGS.
 Author-email: James Li <lijw21@wfu.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,17 +46,17 @@
 Requires-Dist: statsmodels
 Requires-Dist: sphinx<7.0.0
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: sphinx-argparse
 Requires-Dist: loess
 
 # FinaleTools
-Lightweight Python library and standalone program to extract features from
-cfDNA paired-end reads. FinaleTools refers to FragmentatIoN AnaLysis of
-cEll-free DNA Tools.
+A package and standalone program to extract fragmentation patterns of cell-free
+DNA from paired-end sequencing data. FinaleTools refers to FragmentatIoN
+AnaLysis of cEll-free DNA Tools.
 
 FinaleTools is in active development, and all API is subject to change and
 should be considered unstable.
 
 ## Installation
 Instructions:
 - (Optional) create a conda or venv environment to use FinaleTools in.
@@ -124,7 +124,13 @@
 03.79%                       ▃██████████                        
 03.03%                     ▂████████████▆                       
 02.27%                     ██████████████▇▃                     
 01.52%                   ▇█████████████████▅▂                   
 00.76%     ▂▂▂▂▂▂▃▃▄▅▄████████████████████████▆▅▄▃▂▂▂▂▂▂▂▁▁▂▂▂▁▁
 len (nt)067   091   115   139   163   187   211   235   259   283
 ```
+
+## FAQ
+Q: When running on an ARM64 Mac, I can install FinaleTools without errors.
+However, I get an `ImportError` when I run it.
+
+A: Try `brew install curl`. Otherwise, email me and I will try to help you.
```

### Comparing `FinaleTools-0.4.2/src/FinaleTools.egg-info/SOURCES.txt` & `FinaleTools-0.4.3/src/FinaleTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/cli/main_cli.py` & `FinaleTools-0.4.3/src/finaletools/cli/main_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,28 +348,68 @@
         default=0)
     parser_command4.set_defaults(func=multi_wps)
 
     # Subcommand 5: delfi
     parser_command5 = subparsers.add_parser(
         'delfi',
         prog='finaletools-delfi',
-        description='Calculates DELFI score over genome'
+        description='Calculates DELFI score over genome.'
+        '\nNOTE: due to some '
+        'ad hoc implementation details, currently the only accepted reference '
+        "genome is hg19."
         )
-    parser_command5.add_argument('input_file')
-    parser_command5.add_argument('autosomes')
-    parser_command5.add_argument('reference_file')
-    parser_command5.add_argument('bins_file')
-    parser_command5.add_argument('-b', '--blacklist_file')
-    parser_command5.add_argument('-g', '--gap_file')
-    parser_command5.add_argument('-o', '--output_file')
-    parser_command5.add_argument('-W', '--window_size', default=100000, type=int)
-    parser_command5.add_argument('-gc', '--gc_correct', action='store_true')
-    parser_command5.add_argument('-m', '--merge_bins', action='store_true')
-    parser_command5.add_argument('-q', '--quality_threshold', default=30, type=int)
-    parser_command5.add_argument('-w', '--workers', default=1, type=int)
+    parser_command5.add_argument(
+        'input_file',
+        help="SAM, BAM, CRAM, or Frag.gz file containing fragment reads.")
+    parser_command5.add_argument(
+        'autosomes',
+        help="Tab-delimited file where column one is chromosomes and column "
+        "two is the length of said chromosome."
+        )
+    parser_command5.add_argument(
+        'reference_file',
+        help="2bit file for reference sequence used during alignment."
+        )
+    parser_command5.add_argument(
+        'bins_file',
+        help="BED format file containing bins over which to calculate delfi. "
+        "To replicate Cristiano and colleage's methodology, use 100kb bins "
+        "over human autosomes."
+        )
+    parser_command5.add_argument(
+        '-b', '--blacklist_file',
+        help="BED file containing darkregions to ignore when calculating DELFI."
+        )
+    parser_command5.add_argument(
+        '-g', '--gap_file',
+        help='BED4 format file with columns "chrom","start","stop","type". '
+        '"type" should be "centromere", "telomere", or "short arm"; all others'
+        ' are ignored. This information corresponds to "gap" track for hg19 in'
+        ' UCSC Genome Browser.'
+        )
+    parser_command5.add_argument(
+        '-o', '--output_file', default='-',
+        help='BED, bed.gz, tsv, or csv file to write results to. If "-", '
+        'writes tab-deliniated data to stdout. Default is "-".')
+    parser_command5.add_argument(
+        '-W', '--window_size', default=5000000, type=int,
+        help="Currently unused.")
+    parser_command5.add_argument(
+        '-gc', '--gc_correct', action='store_true',
+        help="Indicate whther or not gc correction is applied.")
+    parser_command5.add_argument(
+        '-m', '--merge_bins', action='store_true',
+        help="Indicate whther or not bins are merged to 5Mb bins.")
+    parser_command5.add_argument(
+        '-q', '--quality_threshold', default=30, type=int,
+        help="MAPQ to be filtered.")
+    parser_command5.add_argument(
+        '-w', '--workers', default=1, type=int,
+        help="Maximum number of subprocesses to spawn. Should be close to "
+        "number of cores.")
     parser_command5.add_argument('-v', '--verbose', action='count', default=0)
     parser_command5.set_defaults(func=delfi)
 
     # Subcommand 6: filter_bam
     parser_command6 = subparsers.add_parser(
         'filter-bam',
         prog='finaletools-filter-bam',
```

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/adjust_wps.py` & `FinaleTools-0.4.3/src/finaletools/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/agg_wps.py` & `FinaleTools-0.4.3/src/finaletools/frag/agg_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/cleavage_profile.py` & `FinaleTools-0.4.3/src/finaletools/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/coverage.py` & `FinaleTools-0.4.3/src/finaletools/frag/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,29 +131,31 @@
     fragments of size approaching interval size.
 
     Parameters
     ----------
     input_file : str or pysam.AlignmentFile
         BAM, SAM, or CRAM file containing paired-end fragment reads or
         its path. `AlignmentFile` must be opened in read mode.
-    intervals : str
-        Path for BAM file containing intervals
+    interval_file : str
+        BED4 file containing intervals over which to generate coverage
+        statistics.
     output_file : string, optional
         Path for bed file to print coverages to. If output_file = `_`,
         results will be printed to stdout.
     scale_factor : int, optional
         Amount to multiply coverages by. Default is 10^6.
     quality_threshold : int, optional
     verbose : int or bool, optional
 
     Returns
     -------
     coverage : int
         Fragment coverage over contig and region.
     """
+    #FIXME update docstring
     if (verbose):
         start_time = time.time()
         sys.stderr.write(
             f"""
             input_file: {input_file}
             interval file: {interval_file}
             output_file: {output_file}
```

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/delfi.py` & `FinaleTools-0.4.3/src/finaletools/frag/delfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
           bins_file: str,
           reference_file: str,
           blacklist_file: str=None,
           gap_file: Union(str, GenomeGaps)=None,
           output_file: str=None,
           gc_correct:bool=True,
           merge_bins:bool=True,
-          window_size: int=100000,
+          window_size: int=5000000,
           subsample_coverage: float=2,
           quality_threshold: int=30,
           workers: int=1,
           preprocessing: bool=True,
           verbose: Union[int, bool]=False) -> pandas.DataFrame:
     """
     A function that replicates the methodology of Christiano et al
```

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/delfi_gc_correct.py` & `FinaleTools-0.4.3/src/finaletools/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/delfi_merge_bins.py` & `FinaleTools-0.4.3/src/finaletools/frag/delfi_merge_bins.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 )
 
 def delfi_merge_bins(
         hundred_kb_bins: pd.DataFrame,
         add_chr:bool=False,
         verbose:bool=False
 ):
+    #FIXME: find a way to calculate this that is not dependent on b37 format
     delfi_scripts_5mb_bins = pd.read_csv(BINS_PATH)
 
     if add_chr:
         chr_bins = hundred_kb_bins.copy()
         chr_bins['contig'] = hundred_kb_bins['contig'].apply(
             lambda x: f"chr{x}")
     else:
@@ -56,8 +57,8 @@
         five_mb_bins.iloc[[i],[4]] = subset['short_corrected'].sum()
         five_mb_bins.iloc[[i],[5]] = subset['long_corrected'].sum()
         five_mb_bins.iloc[[i],[6]] = subset['ratio_corrected'].mean()
         five_mb_bins.iloc[[i],[7]] = subset['num_frags_corrected'].sum()
     
     return five_mb_bins
 
-# TODO: add CLI, make binning customizable
+# TODO: make binning customizable
```

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/end_motifs.py` & `FinaleTools-0.4.3/src/finaletools/frag/end_motifs.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/frag_length.py` & `FinaleTools-0.4.3/src/finaletools/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/multi_wps.py` & `FinaleTools-0.4.3/src/finaletools/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/frag/wps.py` & `FinaleTools-0.4.3/src/finaletools/frag/wps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/genome/gaps.py` & `FinaleTools-0.4.3/src/finaletools/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/utils/cli_hist.py` & `FinaleTools-0.4.3/src/finaletools/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/utils/filter_bam.py` & `FinaleTools-0.4.3/src/finaletools/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `FinaleTools-0.4.2/src/finaletools/utils/utils.py` & `FinaleTools-0.4.3/src/finaletools/utils/utils.py`

 * *Files identical despite different names*

