# Comparing `tmp/lightcurver-1.0.3.tar.gz` & `tmp/lightcurver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurver-1.0.3.tar", last modified: Sun Mar 24 01:50:57 2024, max compression
+gzip compressed data, was "lightcurver-1.0.4.tar", last modified: Mon Apr  1 18:13:20 2024, max compression
```

## Comparing `lightcurver-1.0.3.tar` & `lightcurver-1.0.4.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.218391 lightcurver-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-24 01:50:47.000000 lightcurver-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-24 01:50:57.218391 lightcurver-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-24 01:50:47.000000 lightcurver-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.210390 lightcurver-1.0.3/lightcurver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.210390 lightcurver-1.0.3/lightcurver/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/pipeline/pipeline_dependency_graph.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/pipeline/state_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/pipeline/task_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/pipeline/workflow_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.210390 lightcurver-1.0.3/lightcurver/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/footprint_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/image_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/normalization_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/psf_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/sources_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/plotting/star_photometry_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.214391 lightcurver-1.0.3/lightcurver/processes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/alternate_plate_solving_with_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/background_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/cutout_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/frame_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/frame_importation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/frame_star_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/normalization_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/plate_solving.py
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/psf_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/roi_deconv_file_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/roi_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/star_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/star_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/processes/star_querying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.214391 lightcurver-1.0.3/lightcurver/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/structure/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/structure/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/structure/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/structure/user_header_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.218391 lightcurver-1.0.3/lightcurver/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/chi2_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/star_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/starred_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-03-24 01:50:47.000000 lightcurver-1.0.3/lightcurver/utilities/zeropoint_from_gaia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:50:57.218391 lightcurver-1.0.3/lightcurver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-24 01:50:57.000000 lightcurver-1.0.3/lightcurver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-24 01:50:57.000000 lightcurver-1.0.3/lightcurver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 01:50:57.000000 lightcurver-1.0.3/lightcurver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-24 01:50:57.000000 lightcurver-1.0.3/lightcurver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-24 01:50:57.000000 lightcurver-1.0.3/lightcurver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-24 01:50:47.000000 lightcurver-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 01:50:57.218391 lightcurver-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 18:13:11.000000 lightcurver-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-01 18:13:20.158257 lightcurver-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-01 18:13:11.000000 lightcurver-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.150257 lightcurver-1.0.4/lightcurver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.150257 lightcurver-1.0.4/lightcurver/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/pipeline_dependency_graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/state_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/task_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/pipeline/workflow_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/footprint_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/image_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/normalization_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/psf_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/sources_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/plotting/star_photometry_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/alternate_plate_solving_with_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/background_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/cutout_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_importation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/frame_star_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/normalization_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/plate_solving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/psf_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/roi_deconv_file_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/roi_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/processes/star_querying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.154257 lightcurver-1.0.4/lightcurver/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/structure/user_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/lightcurver/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/chi2_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/lightcurves_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/star_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/starred_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-01 18:13:11.000000 lightcurver-1.0.4/lightcurver/utilities/zeropoint_from_gaia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:13:20.158257 lightcurver-1.0.4/lightcurver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 18:13:20.000000 lightcurver-1.0.4/lightcurver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-01 18:13:11.000000 lightcurver-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:13:20.158257 lightcurver-1.0.4/setup.cfg
```

### Comparing `lightcurver-1.0.3/LICENSE` & `lightcurver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/PKG-INFO` & `lightcurver-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.3
+Version: 1.0.4
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,68 +35,68 @@
 Requires-Dist: h5py
 Requires-Dist: widefield_plate_solver
 Requires-Dist: photutils
 Requires-Dist: astroalign
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
-<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:30em;"/>
+<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:28em;"/>
 
 [![python](https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/lightcurver)](https://pypi.org/project/lightcurver/)
 ![tests](https://github.com/duxfrederic/lightcurver/actions/workflows/python-app.yml/badge.svg)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Docs](https://img.shields.io/badge/Docs-Available-green)](https://duxfrederic.github.io/lightcurver/)
 
 
-# LightCurver 
-
+# `lightcurver`
 Welcome to `lightcurver`! 
 This is a photometry library leveraging [STARRED](https://gitlab.com/cosmograil/starred), 
 best used with time series of wide-field images. You can read more about it in the [documentation](https://duxfrederic.github.io/lightcurver/).
 
-`lightcurver` essentially prepares a Point Spread Function (PSF) model for each wide-field image, before using it
-to precisely calibrate the relative zero point between each image.
-Finally, `STARRED` models the pixels of the region of interest, 
-yielding of course high quality light curves of the point sources in the region of interest, 
-but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the region of interest itself.
+Essentially, `lightcurver` provides the infrastructure to 
+- prepare a Point Spread Function (PSF) model for each wide-field image, 
+- precisely calibrate the relative zero point between each image.
+
+This enables `STARRED` to model the pixels of the region of interest (ROI), 
+yielding of course high quality light curves of the point sources in the ROI, 
+but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the ROI itself.
 The example below shows a cutout of a wide-field image (one in a set of a hundred), 
 the model/deconvolution, and the Hubble Space Telescope image of the same region.
 
 ![example_deconvolution](docs/mkdocs/contents/example_deconv.png)
 
 ## Features
-* Uses plate solving (https://astrometry.net/) to keep track of the footprint of each frame, allowing for an independent selection of reference stars in each frame.
-* Leverages _Gaia_ information to select the right reference stars in the field of view.
-* Never interpolates: essential to preserve the sub-pixel information that can be reocovered by `STARRED` in a multi-epoch deconvolution.
-* Provides an extremely precise relative flux calibration between epochs and a PSF model for each epoch.
-* Uses `sqlite3` queries to dynamically determine which process needs be executed on which frame. (adding a new frame does not require the reprocessing of everything).
-* Attempts to keep the number of created files to a minimum, this is crucial when working on servers with high lattency storage.
-
+* **Plate solving:** uses [Astrometry.net](https://astrometry.net/) to establish the footprint of each frame.
+* **_Gaia_ reference stars:** leverages _Gaia_ information to select the right reference stars in the field of view of each frame.
+* **Preserves sub-pixel information**: never interpolates, essential to preserve the sub-pixel information that can be recovered by `STARRED` in a multi-epoch deconvolution.
+* **Incremental:** uses `SQL` queries to dynamically determine which process needs be executed on which frame. 
+* **Semi-automatic:** create a `yaml` configuration file once for the first few frames, then run the 
+pipeline whenever a new frame is added, providing auto-updating light curves.
 
 ## Getting Started
-
 1. **Installation**: the short version, install via `pip`:
 
     ```
     pip install lightcurver
     ```
-[The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
-
-2. **Tutorial** follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
-
-## The implemented processing steps
-![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
+   [The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
+2. **Tutorial**: follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
 
+You can also test your installation with a subset of the dataset provided in the tutorial:
+```bash
+cd /clone/of/lightcurver
+pytest .
+```
 
 ## Contributing
-
-Whether you're fixing a bug, implementing a new feature, or improving documentation, your efforts are highly appreciated. 
-If you are using this code and are encountering issues, feel free to contact me or to directly open an issue or pull request.
+If you're encountering problems, then I would like to hear about them and will try to fix them. Feel free to create an issue
+in this repository.
+If you're finding this package useful and want to contribute, please create a pull request after forking the repository.
+If you need general help, feel free to [reach out](mailto:frederic.dux@epfl.ch)!
 
 ## License
+`lightcurver` is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
 
-LightCurver is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
-
-## Contact
-
-Have questions or suggestions? Feel free to open an issue, a pull request, or [reach out](mailto:frederic.dux@epfl.ch)!
+## The implemented processing steps
+This is an overview of the steps taken by the pipeline.
+![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
```

### Comparing `lightcurver-1.0.3/README.md` & `lightcurver-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:30em;"/>
+<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:28em;"/>
 
 [![python](https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/lightcurver)](https://pypi.org/project/lightcurver/)
 ![tests](https://github.com/duxfrederic/lightcurver/actions/workflows/python-app.yml/badge.svg)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Docs](https://img.shields.io/badge/Docs-Available-green)](https://duxfrederic.github.io/lightcurver/)
 
 
-# LightCurver 
-
+# `lightcurver`
 Welcome to `lightcurver`! 
 This is a photometry library leveraging [STARRED](https://gitlab.com/cosmograil/starred), 
 best used with time series of wide-field images. You can read more about it in the [documentation](https://duxfrederic.github.io/lightcurver/).
 
-`lightcurver` essentially prepares a Point Spread Function (PSF) model for each wide-field image, before using it
-to precisely calibrate the relative zero point between each image.
-Finally, `STARRED` models the pixels of the region of interest, 
-yielding of course high quality light curves of the point sources in the region of interest, 
-but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the region of interest itself.
+Essentially, `lightcurver` provides the infrastructure to 
+- prepare a Point Spread Function (PSF) model for each wide-field image, 
+- precisely calibrate the relative zero point between each image.
+
+This enables `STARRED` to model the pixels of the region of interest (ROI), 
+yielding of course high quality light curves of the point sources in the ROI, 
+but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the ROI itself.
 The example below shows a cutout of a wide-field image (one in a set of a hundred), 
 the model/deconvolution, and the Hubble Space Telescope image of the same region.
 
 ![example_deconvolution](docs/mkdocs/contents/example_deconv.png)
 
 ## Features
-* Uses plate solving (https://astrometry.net/) to keep track of the footprint of each frame, allowing for an independent selection of reference stars in each frame.
-* Leverages _Gaia_ information to select the right reference stars in the field of view.
-* Never interpolates: essential to preserve the sub-pixel information that can be reocovered by `STARRED` in a multi-epoch deconvolution.
-* Provides an extremely precise relative flux calibration between epochs and a PSF model for each epoch.
-* Uses `sqlite3` queries to dynamically determine which process needs be executed on which frame. (adding a new frame does not require the reprocessing of everything).
-* Attempts to keep the number of created files to a minimum, this is crucial when working on servers with high lattency storage.
-
+* **Plate solving:** uses [Astrometry.net](https://astrometry.net/) to establish the footprint of each frame.
+* **_Gaia_ reference stars:** leverages _Gaia_ information to select the right reference stars in the field of view of each frame.
+* **Preserves sub-pixel information**: never interpolates, essential to preserve the sub-pixel information that can be recovered by `STARRED` in a multi-epoch deconvolution.
+* **Incremental:** uses `SQL` queries to dynamically determine which process needs be executed on which frame. 
+* **Semi-automatic:** create a `yaml` configuration file once for the first few frames, then run the 
+pipeline whenever a new frame is added, providing auto-updating light curves.
 
 ## Getting Started
-
 1. **Installation**: the short version, install via `pip`:
 
     ```
     pip install lightcurver
     ```
-[The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
-
-2. **Tutorial** follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
-
-## The implemented processing steps
-![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
+   [The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
+2. **Tutorial**: follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
 
+You can also test your installation with a subset of the dataset provided in the tutorial:
+```bash
+cd /clone/of/lightcurver
+pytest .
+```
 
 ## Contributing
-
-Whether you're fixing a bug, implementing a new feature, or improving documentation, your efforts are highly appreciated. 
-If you are using this code and are encountering issues, feel free to contact me or to directly open an issue or pull request.
+If you're encountering problems, then I would like to hear about them and will try to fix them. Feel free to create an issue
+in this repository.
+If you're finding this package useful and want to contribute, please create a pull request after forking the repository.
+If you need general help, feel free to [reach out](mailto:frederic.dux@epfl.ch)!
 
 ## License
+`lightcurver` is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
 
-LightCurver is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
-
-## Contact
-
-Have questions or suggestions? Feel free to open an issue, a pull request, or [reach out](mailto:frederic.dux@epfl.ch)!
+## The implemented processing steps
+This is an overview of the steps taken by the pipeline.
+![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
```

### Comparing `lightcurver-1.0.3/lightcurver/pipeline/pipeline_dependency_graph.yaml` & `lightcurver-1.0.4/lightcurver/pipeline/pipeline_dependency_graph.yaml`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/pipeline/state_checkers.py` & `lightcurver-1.0.4/lightcurver/pipeline/state_checkers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/pipeline/task_wrappers.py` & `lightcurver-1.0.4/lightcurver/pipeline/task_wrappers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/pipeline/workflow_manager.py` & `lightcurver-1.0.4/lightcurver/pipeline/workflow_manager.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/footprint_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/footprint_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/image_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/image_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/normalization_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/normalization_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/psf_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/psf_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/sources_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/sources_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/plotting/star_photometry_plotting.py` & `lightcurver-1.0.4/lightcurver/plotting/star_photometry_plotting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 
-def plot_joint_deconv_diagnostic(datas, noisemaps, residuals, loss_curve, chi2_per_frame,
+def plot_joint_deconv_diagnostic(datas, noisemaps, residuals, loss_curve, chi2_per_frame, starlet_background=None,
                                  save_path=None):
     """
     a diagnostic of how well a joint deconv went. We will plot a stack of the data, and a stack of
     the residuals. We will show how the loss behaved during optimization.
     It is important to avoid systematics, as this is the core of this package: doing precise photometry,
     so convergence when modelling the pixels is essential.
     Args:
         datas: 3d array of shape (N, nx, ny): N stars, one slice per star.
         noisemaps: same as above but for the noisemaps
         residuals: same as above but for the residuals
         loss_curve: 1D array containing the evolution of the loss during optimization
         chi2_per_frame: 1D array, the chi2 value of the fit, one per slice.
+        starlet_background: 2D array, in case we included a regularized pixelated background in the model. default None.
         save_path: optional, string or path, where to save the plot.
 
     Returns: None
 
     """
     plt.style.use('dark_background')
     cmap = 'viridis'
@@ -27,15 +28,17 @@
     text_size = 11
 
     data_stack = np.mean(datas, axis=0)  # mean and not median, we wanna see them outliers
     residuals_stack = np.mean(residuals, axis=0)
     rel_residuals_stack = np.mean(residuals / noisemaps, axis=0)
 
     sub_size = 3
-    fig, ax = plt.subplots(1, 5, figsize=(4.6 * sub_size, sub_size))
+    ncols = 5 if starlet_background is None else 6
+    fig_size_mult = 4.6 if starlet_background is None else 5.6
+    fig, ax = plt.subplots(1, ncols, figsize=(fig_size_mult * sub_size, sub_size))
     ax = ax.flatten()
     # data stack
     ax[0].imshow(data_stack, cmap=cmap, aspect='auto')
     ax[0].axis('off')
     ax[0].text(0.5, 0.01, 'Data stack',
                horizontalalignment='center',
                verticalalignment='bottom',
@@ -76,14 +79,24 @@
     ax[4].hist(chi2_per_frame, color='white', bins=len(chi2_per_frame))
     ax[4].text(0.5, 0.99, 'chi2 per frame',
                horizontalalignment='center',
                verticalalignment='top',
                transform=ax[4].transAxes,
                color='white', fontsize=text_size,
                weight='bold')
+    # and view of the background common to all epochs if we included one, just to make sure it isn't nonsense.
+    if starlet_background is not None:
+        ax[5].imshow(starlet_background)
+        ax[5].axis('off')
+        ax[5].text(0.5, 0.99, 'regularized background',
+                   horizontalalignment='center',
+                   verticalalignment='top',
+                   transform=ax[5].transAxes,
+                   color='white', fontsize=text_size,
+                   weight='bold')
     plt.tight_layout()
 
     if save_path is not None:
         plt.savefig(save_path, pad_inches=0, bbox_inches='tight', dpi=130)
         plt.close()
     else:
         plt.show()
```

### Comparing `lightcurver-1.0.3/lightcurver/processes/alternate_plate_solving_with_gaia.py` & `lightcurver-1.0.4/lightcurver/processes/alternate_plate_solving_with_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/background_estimation.py` & `lightcurver-1.0.4/lightcurver/processes/background_estimation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/cutout_making.py` & `lightcurver-1.0.4/lightcurver/processes/cutout_making.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/frame_characterization.py` & `lightcurver-1.0.4/lightcurver/processes/frame_characterization.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/frame_importation.py` & `lightcurver-1.0.4/lightcurver/processes/frame_importation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/frame_star_assignment.py` & `lightcurver-1.0.4/lightcurver/processes/frame_star_assignment.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/normalization_calculation.py` & `lightcurver-1.0.4/lightcurver/processes/normalization_calculation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/plate_solving.py` & `lightcurver-1.0.4/lightcurver/processes/plate_solving.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/psf_modelling.py` & `lightcurver-1.0.4/lightcurver/processes/psf_modelling.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/roi_deconv_file_preparation.py` & `lightcurver-1.0.4/lightcurver/processes/roi_deconv_file_preparation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/roi_modelling.py` & `lightcurver-1.0.4/lightcurver/processes/roi_modelling.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/star_extraction.py` & `lightcurver-1.0.4/lightcurver/processes/star_extraction.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/processes/star_photometry.py` & `lightcurver-1.0.4/lightcurver/processes/star_photometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 from datetime import datetime
 import logging
 from time import time
 from starred.deconvolution.deconvolution import setup_model
 from starred.deconvolution.loss import Loss
 from starred.deconvolution.parameters import ParametersDeconv
 from starred.optim.optimization import Optimizer
+from starred.utils.noise_utils import propagate_noise
 
 from ..structure.database import execute_sqlite_query, select_stars, select_stars_for_a_frame, get_pandas
 from ..structure.user_config import get_user_config
 from ..utilities.chi2_selector import get_chi2_bounds
 from ..utilities.footprint import get_combined_footprint_hash
 from ..utilities.starred_utilities import get_flux_uncertainties
 from ..plotting.star_photometry_plotting import plot_joint_deconv_diagnostic
 
 
-def do_one_deconvolution(data, noisemap, psf, subsampling_factor, n_iter=2000):
+def do_one_deconvolution(data, noisemap, psf, subsampling_factor,
+                         n_iter=2000, uniform_background_per_epoch=False, starlet_global_background=True):
     """
     Joint 'deconvolution' of N stamps of a star (in data), with noisemap, and associated PSF at each slice.
     the subsampling factor is that used for building the psf model.
     Equivalent to PSF photometry of all slices.
     Args:
         data: numpy array (N, nx, ny) containing the epochs of the star
         noisemap:  numpy array (N, nx, ny) noisemap of the above
         psf: numpy array (N, nxx, nyy) PSF model, one per slice
         subsampling_factor: int, subsampling_factor of the psf model.
         n_iter: int, number of adabelief iterations to do. default 2000
+        uniform_background_per_epoch: bool, whether we allow a constant value added to each epoch (default False, all 0)
+        starlet_global_background: bool, whether we optimize a starlet background common to all epochs (defualt True)
+
 
     Returns: dictionary, containing the fluxes (ready to be used) as a 1D array, the final kwargs of the optimization,
              the chi2, and by how much we rescaled the data before optimizing. (the fluxes are already scaled back
              to the data's actual scale, but not the kwargs.)
 
     """
     # so, rescale
@@ -68,29 +73,48 @@
         'kwargs_background': {
             'h': kwargs_init['kwargs_background']['h'],  # very little chance that starred changes the initial h = 0.
             'mean': np.ravel([0. for _ in range(len(data))])  # we trust our background subtraction. mean = 0.
         },
         'kwargs_sersic': {},
     }
 
+    # ...and unfix if we want the background free.
+    if uniform_background_per_epoch:
+        del kwargs_fixed['kwargs_background']['mean']
+    if starlet_global_background:
+        del kwargs_fixed['kwargs_background']['h']
+
     parameters = ParametersDeconv(kwargs_init=kwargs_init,
                                   kwargs_fixed=kwargs_fixed,
                                   kwargs_up=kwargs_up,
                                   kwargs_down=kwargs_down)
 
-    loss = Loss(data=data, deconv_class=model, param_class=parameters, sigma_2=sigma_2,
-                regularization_terms='l1_starlet',
-                regularization_strength_scales=1,  # not needed since no free background...
-                regularization_strength_hf=1)      # but the starred interface wants us to provide them anyway
+    # ok, let us prepare the parameters passed to loss which differ depending on our choices
+    kwargs_loss = {
+        'data': data,
+        'deconv_class': model,
+        'param_class': parameters,
+        'sigma_2': sigma_2,
+        'regularization_terms': 'l1_starlet',
+        'regularization_strength_scales': 3,
+        'regularization_strength_hf': 3
+    }
+    if starlet_global_background:
+        # passing a ton of arguments, not really necessary, but at least we know what we are doing
+        # in case the API changes. (num_samples are not even used for 'SLIT')
+        kwargs_loss['W'] = propagate_noise(model, noisemap, kwargs_init, wavelet_type_list=['starlet'],
+                                           method='SLIT', num_samples=200, seed=1, likelihood_type='chi2',
+                                           verbose=False, upsampling_factor=subsampling_factor)[0]
+    loss = Loss(**kwargs_loss)
 
     optim = Optimizer(loss, parameters, method='adabelief')
 
     optimiser_optax_option = {
                 'max_iterations': n_iter, 'min_iterations': None,
-                'init_learning_rate': 2e-3, 'schedule_learning_rate': True,
+                'init_learning_rate': 1e-3, 'schedule_learning_rate': True,
                 'restart_from_init': True, 'stop_at_loss_increase': False,
                 'progress_bar': True, 'return_param_history': True
     }
 
     optim.minimize(**optimiser_optax_option)
     kwargs_final = parameters.best_fit_values(as_kwargs=True)
     modelled_pixels = model.model(kwargs_final)
@@ -101,23 +125,28 @@
     fluxes = scale * np.array(kwargs_final['kwargs_analytic']['a'])
 
     # let us calculate the uncertainties ~ equivalent to photon noise / read noise
     flux_uncertainties = get_flux_uncertainties(kwargs=kwargs_final, kwargs_down=kwargs_down, kwargs_up=kwargs_up,
                                                 data=data, noisemap=noisemap, model=model)
     fluxes_uncertainties = scale * flux_uncertainties
 
+    # and in case we included a background, return it:
+    deconv, h = model.getDeconvolved(kwargs_final, 0)
+
     result = {
         'scale': scale,
         'kwargs_final': kwargs_final,
         'fluxes': fluxes,
         'fluxes_uncertainties': fluxes_uncertainties,
         'chi2': float(chi2),
         'chi2_per_frame': np.array(chi2_per_frame),
         'loss_curve': optim.loss_history,
-        'residuals': scale * residuals
+        'residuals': scale * residuals,
+        'deconvolved_image': deconv,
+        'starlet_background': h
     }
     return result
 
 
 def get_frames_for_star(combined_footprint_hash, gaia_id,
                         psf_fit_chi2_min, psf_fit_chi2_max, only_fluxless_frames=False):
     """
@@ -261,27 +290,41 @@
             mask = ~(np.array(mask).astype(bool))  # so we invert it.
             # oh, we invert it again to boost the noisemap where mask is False,
             # but better have the masks loaded the right way for the future.
             noisemap[np.where(~mask)[0]] *= 1000.
             # ok now that everything is ready let's get out of the context manager, also to close the file.
 
         # ready to "deconvolve" using starred!
-        result = do_one_deconvolution(data=data, noisemap=noisemap, psf=psf,
-                                      subsampling_factor=user_config['subsampling_factor'],
-                                      n_iter=user_config['star_deconv_n_iter'])
+        result = do_one_deconvolution(
+            data=data, noisemap=noisemap, psf=psf,
+            subsampling_factor=user_config['subsampling_factor'],
+            n_iter=user_config['star_deconv_n_iter'],
+            uniform_background_per_epoch=user_config['star_photometry_uniform_background_per_epoch'],
+            starlet_global_background=user_config['star_photometry_starlet_global_background']
+        )
         # ok, plot the diagnostic
         plot_deconv_dir = user_config['plots_dir'] / 'deconvolutions' / str(combined_footprint_hash)
         plot_deconv_dir.mkdir(exist_ok=True, parents=True)
         loss_history = result['loss_curve']
 
         plot_file = plot_deconv_dir / f"{time_now}_joint_deconv_star_{star['name']}.jpg"
-        plot_joint_deconv_diagnostic(datas=data, noisemaps=noisemap,
-                                     residuals=result['residuals'],
-                                     chi2_per_frame=result['chi2_per_frame'], loss_curve=loss_history,
-                                     save_path=plot_file)
+
+        kwargs_plot = {
+            'datas': data,
+            'noisemaps': noisemap,
+            'residuals': result['residuals'],
+            'chi2_per_frame': result['chi2_per_frame'],
+            'loss_curve': loss_history,
+            'save_path': plot_file
+        }
+
+        if user_config['star_photometry_starlet_global_background']:
+            logger.info(f"This PSF photometry (star {star['name']}) included a pixelated background.")
+            kwargs_plot['starlet_background'] = np.array(result['starlet_background'])
+        plot_joint_deconv_diagnostic(**kwargs_plot)
 
         # now we can insert our results in our dedicated database table.
         loss_index = int(0.9 * np.array(loss_history).size)
         initial_change = np.nanmax(loss_history[:loss_index]) - np.nanmin(loss_history[:loss_index])
         end_change = np.nanmax(loss_history[loss_index:]) - np.nanmin(loss_history[loss_index:])
         relative_loss_differential = float(end_change / initial_change)
         # flux_data should be a list of tuples, each containing (frame_id, star_gaia_id, flux, flux_uncertainty)
```

### Comparing `lightcurver-1.0.3/lightcurver/processes/star_querying.py` & `lightcurver-1.0.4/lightcurver/processes/star_querying.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/structure/database.py` & `lightcurver-1.0.4/lightcurver/structure/database.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/structure/user_config.py` & `lightcurver-1.0.4/lightcurver/structure/user_config.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/structure/user_header_parser.py` & `lightcurver-1.0.4/lightcurver/structure/user_header_parser.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/chi2_selector.py` & `lightcurver-1.0.4/lightcurver/utilities/chi2_selector.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/footprint.py` & `lightcurver-1.0.4/lightcurver/utilities/footprint.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/gaia.py` & `lightcurver-1.0.4/lightcurver/utilities/gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/star_naming.py` & `lightcurver-1.0.4/lightcurver/utilities/star_naming.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/starred_utilities.py` & `lightcurver-1.0.4/lightcurver/utilities/starred_utilities.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver/utilities/zeropoint_from_gaia.py` & `lightcurver-1.0.4/lightcurver/utilities/zeropoint_from_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.3/lightcurver.egg-info/PKG-INFO` & `lightcurver-1.0.4/lightcurver.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.3
+Version: 1.0.4
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,68 +35,68 @@
 Requires-Dist: h5py
 Requires-Dist: widefield_plate_solver
 Requires-Dist: photutils
 Requires-Dist: astroalign
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
-<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:30em;"/>
+<img src="docs/mkdocs/contents/lightcurver_logo.svg" alt="logo" style="width:28em;"/>
 
 [![python](https://img.shields.io/badge/Python-3.11-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/lightcurver)](https://pypi.org/project/lightcurver/)
 ![tests](https://github.com/duxfrederic/lightcurver/actions/workflows/python-app.yml/badge.svg)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Docs](https://img.shields.io/badge/Docs-Available-green)](https://duxfrederic.github.io/lightcurver/)
 
 
-# LightCurver 
-
+# `lightcurver`
 Welcome to `lightcurver`! 
 This is a photometry library leveraging [STARRED](https://gitlab.com/cosmograil/starred), 
 best used with time series of wide-field images. You can read more about it in the [documentation](https://duxfrederic.github.io/lightcurver/).
 
-`lightcurver` essentially prepares a Point Spread Function (PSF) model for each wide-field image, before using it
-to precisely calibrate the relative zero point between each image.
-Finally, `STARRED` models the pixels of the region of interest, 
-yielding of course high quality light curves of the point sources in the region of interest, 
-but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the region of interest itself.
+Essentially, `lightcurver` provides the infrastructure to 
+- prepare a Point Spread Function (PSF) model for each wide-field image, 
+- precisely calibrate the relative zero point between each image.
+
+This enables `STARRED` to model the pixels of the region of interest (ROI), 
+yielding of course high quality light curves of the point sources in the ROI, 
+but also recovering the subpixel information to provide a high signal-to-noise ratio deconvolution of the ROI itself.
 The example below shows a cutout of a wide-field image (one in a set of a hundred), 
 the model/deconvolution, and the Hubble Space Telescope image of the same region.
 
 ![example_deconvolution](docs/mkdocs/contents/example_deconv.png)
 
 ## Features
-* Uses plate solving (https://astrometry.net/) to keep track of the footprint of each frame, allowing for an independent selection of reference stars in each frame.
-* Leverages _Gaia_ information to select the right reference stars in the field of view.
-* Never interpolates: essential to preserve the sub-pixel information that can be reocovered by `STARRED` in a multi-epoch deconvolution.
-* Provides an extremely precise relative flux calibration between epochs and a PSF model for each epoch.
-* Uses `sqlite3` queries to dynamically determine which process needs be executed on which frame. (adding a new frame does not require the reprocessing of everything).
-* Attempts to keep the number of created files to a minimum, this is crucial when working on servers with high lattency storage.
-
+* **Plate solving:** uses [Astrometry.net](https://astrometry.net/) to establish the footprint of each frame.
+* **_Gaia_ reference stars:** leverages _Gaia_ information to select the right reference stars in the field of view of each frame.
+* **Preserves sub-pixel information**: never interpolates, essential to preserve the sub-pixel information that can be recovered by `STARRED` in a multi-epoch deconvolution.
+* **Incremental:** uses `SQL` queries to dynamically determine which process needs be executed on which frame. 
+* **Semi-automatic:** create a `yaml` configuration file once for the first few frames, then run the 
+pipeline whenever a new frame is added, providing auto-updating light curves.
 
 ## Getting Started
-
 1. **Installation**: the short version, install via `pip`:
 
     ```
     pip install lightcurver
     ```
-[The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
-
-2. **Tutorial** follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
-
-## The implemented processing steps
-![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
+   [The slightly longer version](https://duxfrederic.github.io/lightcurver/installation/), in case you plan on using a GPU or the plate solving.
+2. **Tutorial**: follow the [tutorial](https://duxfrederic.github.io/lightcurver/tutorial/) of the documentation, which provides a dataset you can experiment with.
 
+You can also test your installation with a subset of the dataset provided in the tutorial:
+```bash
+cd /clone/of/lightcurver
+pytest .
+```
 
 ## Contributing
-
-Whether you're fixing a bug, implementing a new feature, or improving documentation, your efforts are highly appreciated. 
-If you are using this code and are encountering issues, feel free to contact me or to directly open an issue or pull request.
+If you're encountering problems, then I would like to hear about them and will try to fix them. Feel free to create an issue
+in this repository.
+If you're finding this package useful and want to contribute, please create a pull request after forking the repository.
+If you need general help, feel free to [reach out](mailto:frederic.dux@epfl.ch)!
 
 ## License
+`lightcurver` is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
 
-LightCurver is licensed under the GPL v3.0 License. See the [LICENSE](LICENSE) file for more details.
-
-## Contact
-
-Have questions or suggestions? Feel free to open an issue, a pull request, or [reach out](mailto:frederic.dux@epfl.ch)!
+## The implemented processing steps
+This is an overview of the steps taken by the pipeline.
+![flowdiagram](docs/flow_diagram/workflow_diagram.svg)
```

### Comparing `lightcurver-1.0.3/lightcurver.egg-info/SOURCES.txt` & `lightcurver-1.0.4/lightcurver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 ./lightcurver/structure/exceptions.py
 ./lightcurver/structure/user_config.py
 ./lightcurver/structure/user_header_parser.py
 ./lightcurver/utilities/__init__.py
 ./lightcurver/utilities/chi2_selector.py
 ./lightcurver/utilities/footprint.py
 ./lightcurver/utilities/gaia.py
+./lightcurver/utilities/lightcurves_postprocessing.py
 ./lightcurver/utilities/star_naming.py
 ./lightcurver/utilities/starred_utilities.py
 ./lightcurver/utilities/zeropoint_from_gaia.py
 lightcurver.egg-info/PKG-INFO
 lightcurver.egg-info/SOURCES.txt
 lightcurver.egg-info/dependency_links.txt
 lightcurver.egg-info/requires.txt
```

### Comparing `lightcurver-1.0.3/pyproject.toml` & `lightcurver-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.6.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightcurver"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{ name = "Frédéric Dux", email = "duxfrederic@gmail.com" }]
 description = "A thorough structure for precise photometry and deconvolution of time series of wide field images."
 readme = "README.md"
 keywords = ["photometry", "astronomy", "deconvolution", "PSF", "pipeline"]  
 classifiers = [] 
 dependencies = [
     "pyyaml",
```

