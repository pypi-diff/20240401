# Comparing `tmp/tga_data_analysis-1.0.1.tar.gz` & `tmp/tga_data_analysis-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-1.0.1.tar", last modified: Thu Feb  1 20:43:38 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.0.1.tar", last modified: Mon Apr  1 20:55:00 2024, max compression
```

## Comparing `tga_data_analysis-1.0.1.tar` & `tga_data_analysis-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 20:43:38.124446 tga_data_analysis-1.0.1/
--rw-rw-rw-   0        0        0     1401 2024-02-01 20:43:38.122455 tga_data_analysis-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      953 2024-02-01 19:55:16.000000 tga_data_analysis-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-02-01 20:43:38.125442 tga_data_analysis-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1400 2024-02-01 20:41:28.000000 tga_data_analysis-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-01 20:43:38.098532 tga_data_analysis-1.0.1/tga_data_analysis/
--rw-rw-rw-   0        0        0      259 2024-01-31 20:52:22.000000 tga_data_analysis-1.0.1/tga_data_analysis/__init__.py
--rw-rw-rw-   0        0        0   100946 2024-02-01 20:24:55.000000 tga_data_analysis-1.0.1/tga_data_analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-02-01 20:43:38.117474 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/
--rw-rw-rw-   0        0        0     1401 2024-02-01 20:43:37.000000 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-02-01 20:43:37.000000 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 20:43:37.000000 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-02-01 20:43:37.000000 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-01 20:43:37.000000 tga_data_analysis-1.0.1/tga_data_analysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:55:00.562552 tga_data_analysis-2.0.1/
+-rw-rw-rw-   0        0        0     2012 2024-04-01 20:55:00.559561 tga_data_analysis-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/README.md
+-rw-rw-rw-   0        0        0      783 2024-04-01 20:54:50.000000 tga_data_analysis-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:55:00.563550 tga_data_analysis-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-01 20:55:00.503657 tga_data_analysis-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-01 20:55:00.521487 tga_data_analysis-2.0.1/src/tga_data_analysis/
+-rw-rw-rw-   0        0        0        2 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/src/tga_data_analysis/__init__.py
+-rw-rw-rw-   0        0        0    11375 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/src/tga_data_analysis/kas_kinetics.py
+-rw-rw-rw-   0        0        0    22168 2024-04-01 20:51:14.000000 tga_data_analysis-2.0.1/src/tga_data_analysis/myfigure.py
+-rw-rw-rw-   0        0        0    62513 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/src/tga_data_analysis/tga.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:55:00.556565 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2012 2024-04-01 20:55:00.000000 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2024-04-01 20:55:00.000000 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:55:00.000000 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-01 20:55:00.000000 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-01 20:55:00.000000 tga_data_analysis-2.0.1/src/tga_data_analysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 20:55:00.552581 tga_data_analysis-2.0.1/tests/
+-rw-rw-rw-   0        0        0     1855 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/tests/test_measure.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/tests/test_sample.py
+-rw-rw-rw-   0        0        0      911 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.1/tests/test_tga.py
```

### Comparing `tga_data_analysis-1.0.1/PKG-INFO` & `tga_data_analysis-2.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,17 @@
-Metadata-Version: 2.1
-Name: tga_data_analysis
-Version: 1.0.1
-Summary: Tool for automatic analysis of multiple TGA results
-Home-page: https://github.com/mpecchi/PyTGA
-Author: Matteo Pecchi
-Author-email: your.email@example.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# Thermogravimetric Analysis in Python
 
-# PyTGA - Thermogravimetric Analysis in Python
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ## Overview
 PyTGA is a Python module designed for conducting and analyzing Thermogravimetric Analysis (TGA) experiments. It offers tools for loading, processing, and analyzing TGA data, focusing on proximate and oxidation analysis, solid distillation analysis, and deconvolution analysis.
 
 ## Features
 - **Data Loading**: Supports loading TGA data from files.
 - **Proximate Analysis**: Calculates moisture, ash, and volatile matter.
 - **Oxidation Analysis**: Computes Ti, Tp, Tb, etc.
 - **Solid Distillation Analysis**: Analyzes solid distillation over time.
 - **Deconvolution Analysis**: Deconvolutes TGA curves for peak analysis.
 - **Plotting and Visualization**: Functions for TGA data visualization.
 
 ## Example
-The example is available in the example folder (with necessary data) and demonstrates how to use the tga_data_analysis package for basic TGA data analysis and visualization.
+The example is available in the example folder that can be found using the project link homepage. Necessary data are provided. The example demonstrates how to use the tga_data_analysis package for basic TGA data analysis and visualization, the example requires downloading the data, installing the package, and setting the folder path to the example data folder.
```

