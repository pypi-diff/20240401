# Comparing `tmp/earthstat-0.7.0.tar.gz` & `tmp/earthstat-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthstat-0.7.0.tar", last modified: Sun Mar 31 08:18:47 2024, max compression
+gzip compressed data, was "earthstat-0.8.0.tar", last modified: Mon Apr  1 15:26:07 2024, max compression
```

## Comparing `earthstat-0.7.0.tar` & `earthstat-0.8.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.372549 earthstat-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-31 08:18:32.000000 earthstat-0.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.352549 earthstat-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.356549 earthstat-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.360549 earthstat-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-31 08:18:32.000000 earthstat-0.7.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-31 08:18:32.000000 earthstat-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-31 08:18:32.000000 earthstat-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-31 08:18:32.000000 earthstat-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-31 08:18:47.372549 earthstat-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-31 08:18:32.000000 earthstat-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.360549 earthstat-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/analysis_aggregation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.364549 earthstat-0.7.0/docs/assests/
--rw-r--r--   0 runner    (1001) docker     (127)   255545 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/assests/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/assests/logo_white.png
--rw-r--r--   0 runner    (1001) docker     (127)   751576 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/assests/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)   484549 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/assests/xES_workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/data_compatibility.md
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/data_converter.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/earthstat.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.364549 earthstat-0.7.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/examples/xES.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/geo_data_processing.md
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/geo_meta_extractor.md
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.364549 earthstat-0.7.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.364549 earthstat-0.7.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/usage/main_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/usage/xES_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-31 08:18:32.000000 earthstat-0.7.0/docs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.364549 earthstat-0.7.0/earthstat/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/analysis_aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/analysis_aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/analysis_aggregation/aggregate_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/data_compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_compatibility/compatibility_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_compatibility/data_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_compatibility/process_comp_issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/data_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_converter/hdf5_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/data_converter/netcdf_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/earthstat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/geo_data_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_data_processing/clip_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_data_processing/rescale_resample_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_data_processing/shapefile_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/geo_meta_extractors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_meta_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_meta_extractors/mask_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_meta_extractors/predictor_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/geo_meta_extractors/shapefile_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.368549 earthstat-0.7.0/earthstat/xES/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/DailyDatasetBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/DekadalDatasetBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/cds_api_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/cds_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/download_AgERA5py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/get_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xES/xES_utiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-03-31 08:18:32.000000 earthstat-0.7.0/earthstat/xearthstat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.372549 earthstat-0.7.0/earthstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 08:18:47.000000 earthstat-0.7.0/earthstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-31 08:18:32.000000 earthstat-0.7.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 08:18:32.000000 earthstat-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-31 08:18:32.000000 earthstat-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-31 08:18:32.000000 earthstat-0.7.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 08:18:47.372549 earthstat-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:18:47.372549 earthstat-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-31 08:18:32.000000 earthstat-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-31 08:18:32.000000 earthstat-0.7.0/tests/test_earthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.576895 earthstat-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 15:25:56.000000 earthstat-0.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.556894 earthstat-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.560894 earthstat-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.560894 earthstat-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-01 15:25:56.000000 earthstat-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 15:25:56.000000 earthstat-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 15:25:56.000000 earthstat-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-01 15:26:07.572894 earthstat-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-01 15:25:56.000000 earthstat-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.564894 earthstat-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/analysis_aggregation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.564894 earthstat-0.8.0/docs/assests/
+-rw-r--r--   0 runner    (1001) docker     (127)   255545 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)   751576 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)   484549 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/xES_workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/data_compatibility.md
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/data_converter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/earthstat.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/examples/xES.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/geo_data_processing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/geo_meta_extractor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/usage/main_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/usage/xES_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/analysis_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/aggregate_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/data_compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/compatibility_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/data_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/process_comp_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/data_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_converter/hdf5_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_converter/netcdf_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/earthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/geo_data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/clip_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/rescale_resample_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/shapefile_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/geo_meta_extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/mask_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/predictor_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/shapefile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/xES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/DailyDatasetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/DekadalDatasetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/cds_api_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/cds_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/download_AgERA5py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/get_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/xES_utiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xearthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-01 15:25:56.000000 earthstat-0.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 15:25:56.000000 earthstat-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 15:25:56.000000 earthstat-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 15:25:56.000000 earthstat-0.8.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:26:07.576895 earthstat-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 15:25:56.000000 earthstat-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 15:25:56.000000 earthstat-0.8.0/tests/test_earthstat.py
```

### Comparing `earthstat-0.7.0/.github/ISSUE_TEMPLATE/config.yml` & `earthstat-0.8.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/docs-build.yml` & `earthstat-0.8.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/docs.yml` & `earthstat-0.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/installation.yml` & `earthstat-0.8.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/macos.yml` & `earthstat-0.8.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/pypi.yml` & `earthstat-0.8.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/ubuntu.yml` & `earthstat-0.8.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.github/workflows/windows.yml` & `earthstat-0.8.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/.gitignore` & `earthstat-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/LICENSE` & `earthstat-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/PKG-INFO` & `earthstat-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthstat
-Version: 0.7.0
+Version: 0.8.0
 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh <abdulrahman.amr.ali@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AbdelrahmanAmr3/earthstat
 Keywords: earthstat
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthstat Version: 0.7.0 Summary: EarthStat Library
+Metadata-Version: 2.1 Name: earthstat Version: 0.8.0 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh
 gmail.com> License: MIT License Project-URL: Homepage, https://github.com/
 AbdelrahmanAmr3/earthstat Keywords: earthstat Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `earthstat-0.7.0/README.md` & `earthstat-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/assests/logo.png` & `earthstat-0.8.0/docs/assests/logo.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/assests/logo_white.png` & `earthstat-0.8.0/docs/assests/logo_white.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/assests/workflow.png` & `earthstat-0.8.0/docs/assests/workflow.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/assests/xES_workflow.png` & `earthstat-0.8.0/docs/assests/xES_workflow.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/contributing.md` & `earthstat-0.8.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/examples/intro.ipynb` & `earthstat-0.8.0/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/examples/xES.ipynb` & `earthstat-0.8.0/docs/examples/xES.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9701512398420293%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, '# install the EarthStat\\n'), (1, '\\n')]}}, 6: "*

 * *            "{'source': ['Create an instance of xEarthStat, and initialize the workflow']}, 7: "*

 * *            "{'metadata': {replace: OrderedDict()}, 'source': ['# create an instance of the "*

 * *            "workflow\\n', '\\n', 'EU_AgERA5 = xEarthStat()']}, 8: {'source': {insert: [(0, "*

 * *            "'initilize the workflow by:\\n'), (3, '- **shape_file_path** (`str`): shapefile file "*

 * *            "path')], delete: [5,  […]*

```diff
@@ -15,93 +15,116 @@
             "source": [
                 "### Installation\n",
                 "\n",
                 "To use xEarthStat for AgERA5, you first need to install the `earthstat` Python package. Run the following command in your Python environment:"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "!pip install earthstat"
+                "### Step 1:Install & Import xEarthStat"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Step 1: Import xEarthStat"
+                "# install the EarthStat\n",
+                "\n",
+                "!pip install earthstat"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "JMD972z6oV2e"
             },
             "outputs": [],
             "source": [
+                "# import the package\n",
+                "\n",
                 "from earthstat import xEarthStat as xES"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 2: Define Your Region of Interest (ROI)\n",
-                "Specify your ROI's name, bounding box, and the time range for the data you're interested in:\n",
-                "\n",
-                "- **ROI Name** (`str`): Unique identifier for your ROI.\n",
-                "- **Bounding Box** (`list` of `float`): Define the north, west, south, and east coordinates of your ROI.\n",
-                "- **Time Range** (`int`): Specify the start and end years."
+                "### Step 2: Initialize xEarthStat Workflow"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Create an instance of xEarthStat, and initialize the workflow"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "id": "DZxYyzRPo7C2"
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "ROI_name = 'EU_AgERA5'\n",
-                "start_year = 2000\n",
-                "end_year = 2001\n",
+                "# create an instance of the workflow\n",
                 "\n",
-                "ROI_bounding_box = [71, -31, 34.5, 40]  # [north, west, south, east]"
+                "EU_AgERA5 = xEarthStat()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 3: Set AgERA5 Parameters\n",
+                "initilize the workflow by:\n",
                 "\n",
-                "List the climate parameters you want to download for your ROI:"
+                "- **ROI Name** (`str`): Unique identifier for your ROI.\n",
+                "- **shape_file_path** (`str`): shapefile file path"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "AgERA5_parameters = [\n",
-                "    'Maximum_Temperature', 'Minimum_Temperature', 'Mean_Temperature',\n",
-                "    'Solar_Radiation_Flux', 'Precipitation_Flux', 'Wind_Speed','Vapour_Pressure'\n",
-                "    ]"
+                "ROI_name = 'EU'\n",
+                "shape_file_path = 'EU.shp'\n",
+                "\n",
+                "EU_AgERA5.init_workflow(\n",
+                "    ROI_name, \n",
+                "    shape_file_path # Adding shape file path is optional\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "> <span style=\"color:red;\">**Note & Caution:**</span> Adding shapefile(optional): for just downloading data without data aggregation you can pass the shapefile.  "
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Step 3: Download AgERA5 From CDS\n",
+                "\n",
+                "Download the AgERA5 data for your ROI by defining the following:\n",
+                "- **AgERA5_parameters** (`list`): Define the list of interested variables to download from CDS."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "> <span style=\"color:red;\">**Note & Caution:**</span> xEarthStat can just download 7 variables included in the table below.\n",
+                "> <span style=\"color:red;\">**Note & Caution:**</span> Currently, xEarthStat can just download 7 variables included in the table below.\n",
                 "\n",
                 "| Variable                 | AgERA5 Parameter            | Statistical Download Type |\n",
                 "|--------------------------|-----------------------------|---------------------------|\n",
                 "| Maximum Temperature      | 2m_temperature              | 24_hour_maximum           |\n",
                 "| Minimum Temperature      | 2m_temperature              | 24_hour_minimum           |\n",
                 "| Mean Temperature         | 2m_temperature              | 24_hour_mean              |\n",
                 "| Solar Radiation Flux     | solar_radiation_flux        | -                         |\n",
@@ -110,145 +133,177 @@
                 "| Vapour Pressure          | vapour_pressure             | 24_hour_mean              |\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 4: Define the Shapefile Path\n",
+                "- **Bounding Box** (`list` of `float`): `north`, `west`, `south`, and `east` coordinates of ROI.\n",
+                "- **start_year** (`int`): the start year for data.\n",
+                "- **end_year** (`int`):  the end year for data.\n",
                 "\n",
-                "Provide the file path to your shapefile:"
+                "***Example:***\n",
+                "To download data from 2000 to 2020, set start_year to 2000 and end_year to 2020. For a single year, set both to the same year."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "shapefile_file_path = 'EU/admin3.shp'"
+                "# Define the AgERA5's variables to be downloaded\n",
+                "\n",
+                "AgERA5_parameters = [\n",
+                "    'Maximum_Temperature', 'Minimum_Temperature', 'Mean_Temperature',\n",
+                "    'Solar_Radiation_Flux', 'Precipitation_Flux', 'Wind_Speed','Vapour_Pressure'\n",
+                "    ]\n",
+                "\n",
+                "# Define the ROI's bounding box, start year, and end year\n",
+                "\n",
+                "ROI_bounding_box = [71, -31, 34.5, 40]  # [north, west, south, east]\n",
+                "start_year = 2000\n",
+                "end_year = 2001"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 5: Initialize xEarthStat\n",
-                "\n",
-                "Create an instance of xEarthStat with the specified parameters:\n",
-                "- `workflow`: The type of final generated dataset, `dekadal` for aggregated dekadal (1,11,21 of month) dataset, `daily` for daily dataset.   \n",
-                "- `multi_processing`: Enables parallel processing."
+                "Next, initialize the AgERA5 downloader by defined parameters:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "id": "UacP556ko8hN"
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "EU_AgERA5 = xES(ROI_name,\n",
-                "                AgERA5_parameters,\n",
-                "                start_year,\n",
-                "                end_year,\n",
-                "                ROI_bounding_box,\n",
-                "                shapefile_path=shapefile_file_path,\n",
-                "                workflow='daily',\n",
-                "                multi_processing=True)"
+                "# Initialize the AgERA5 downloader\n",
+                "\n",
+                "EU_AgERA5.init_AgERA5_downloader(\n",
+                "    AgERA5_parameters,\n",
+                "    ROI_bounding_box,\n",
+                "    start_year,\n",
+                "    end_year\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 6: Download Data\n",
+                "**`xES.download_AgERA5`** options:\n",
                 "\n",
-                "Download the AgERA5 data for your ROI:\n",
                 "- `num_requests`: the number of downloading requests sends to CDS's API server until download all data.\n",
-                "- `extract`: Extract the downloaded AgERA5 zip files, set `False` if you don't want to extract them."
+                "- `extract`: `True` to Extract the downloaded AgERA5 zip files, set `False` if you don't want to extract zip files."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "q_-LmDg_pCME"
             },
             "outputs": [],
             "source": [
+                "# Start downloading the AgERA5 data\n",
+                "\n",
                 "EU_AgERA5.download_AgERA5(num_requests=6,\n",
                 "                          extract=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "> <span style=\"color:red;\">**Note & Caution:**</span> Don't send more than 6 requests to the server. That may lead to pressure on the server and may result in blocking your API key from downloading."
+                "> <span style=\"color:red;\">**Note & Caution:**</span> \n",
+                "- Don't send more than 5 requests to the server. That leads to the server to block your API key from downloading.\n",
+                "- If your ROI is to much small decrease the number of requests to two."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 7: Aggregate Data\n",
+                "### Step 4: Aggregate Data\n",
                 "\n",
                 "xEarthStat's Aggregation process utilize the availability of GPU for parallel computation, and using the avilalble CPU cores for multiprocessing. it automatically detect if there is a GPU or not, if not it shift computational processing on CPU.\n",
                 "\n",
-                "- `max_workers`: Default to total number of CPU's cores. You can change the number of cores that used in multiprocessing.\n",
-                "- `all_touched`: Default to `False` to just consider pixels within the geometry object. `True` to consider all touched pixels by geo-object. \n",
-                "- `stat`:  `\"mean\"`(Default), `\"median\"`, `\"min\"`, `\"max\"`, `\"sum\"`."
+                "`xES.Aggregate_AgERA5`:\n",
+                "\n",
+                "- `dataset_type`: Chosing the type of dataset, `dekadal` for aggregated dekadal (1,11,21 of month) dataset, `daily` for daily dataset.\n",
+                "\n",
+                "- `all_touched`: Default to `False` to just consider pixels within the geometry object. `True` to consider all touched pixels by geo-object.\n",
+                "\n",
+                "- `stat`:  `\"mean\"`(Default), `\"median\"`, `\"min\"`, `\"max\"`, `\"sum\"`.\n",
+                "\n",
+                "- `multi_processing`: Enables parallel processing.\n",
+                "\n",
+                "- `max_workers`: Default to total number of CPU's cores. You can change the number of cores that used in multiprocessing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Explore the number of all CPU cores\n",
+                "\n",
                 "import os\n",
                 "\n",
-                "# Get the number of all CPU cores\n",
                 "cpu_cores = os.cpu_count()\n",
                 "\n",
                 "print(f'Number of CPU cores: {cpu_cores}')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "kKNXUWKBvbkz"
             },
             "outputs": [],
             "source": [
-                "EU_AgERA5.Aggregate_AgERA5(max_workers=cpu_cores,\n",
-                "                           all_touched=False,\n",
-                "                           stat='mean')"
+                "# Start aggregating the downloaded AgERA5 data\n",
+                "\n",
+                "EU_AgERA5.Aggregate_AgERA5(\n",
+                "\n",
+                "    dataset_type = \"dekadal\",\n",
+                "    all_touched=False,\n",
+                "    stat='mean'\n",
+                "    multi_processing=False,\n",
+                "    max_workers=None, # None means using all CPU cores\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Step 8: Export Aggregated Data\n",
+                "### Step 5 (Optional): Merge Aggregated AgERA5's Variables CSVs\n",
                 "\n",
                 "Optionally, merge all generated datasets' csv files into one merged csv for all aggregated variables:\n",
+                "\n",
+                "`xES.AgERA5_merged_csv`:\n",
+                "\n",
                 "- `kelvin_to_celsius`: To convert the temperature unit from kelvin to celsius.\n",
+                "\n",
                 "- `output_name`: option to add the name of merged csv, it's default to `AgERA5_{ROI_name}_merged_parameters_{workflow}_{timestamp}.csv`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "EU_AgERA5.AgERA5_merged_csv(kelvin_to_celsius=False, output_name=None)"
+                "EU_AgERA5.AgERA5_merged_csv(kelvin_to_celsius=False, \n",
+                "                            output_name=None)"
             ]
         }
     ],
     "metadata": {
         "accelerator": "GPU",
         "colab": {
             "gpuType": "T4",
```

### Comparing `earthstat-0.7.0/docs/geo_data_processing.md` & `earthstat-0.8.0/docs/geo_data_processing.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/geo_meta_extractor.md` & `earthstat-0.8.0/docs/geo_meta_extractor.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/index.md` & `earthstat-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/installation.md` & `earthstat-0.8.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/usage/main_usage.md` & `earthstat-0.8.0/docs/usage/main_usage.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/docs/usage/xES_usage.md` & `earthstat-0.8.0/docs/usage/xES_usage.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/analysis_aggregation/aggregate_process.py` & `earthstat-0.8.0/earthstat/analysis_aggregation/aggregate_process.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py` & `earthstat-0.8.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/data_compatibility/compatibility_utils.py` & `earthstat-0.8.0/earthstat/data_compatibility/compatibility_utils.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/data_compatibility/data_compatibility.py` & `earthstat-0.8.0/earthstat/data_compatibility/data_compatibility.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/data_compatibility/process_comp_issues.py` & `earthstat-0.8.0/earthstat/data_compatibility/process_comp_issues.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/data_converter/netcdf_to_tiff.py` & `earthstat-0.8.0/earthstat/data_converter/netcdf_to_tiff.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/earthstat.py` & `earthstat-0.8.0/earthstat/earthstat.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_data_processing/clip_raster.py` & `earthstat-0.8.0/earthstat/geo_data_processing/clip_raster.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_data_processing/rescale_resample_raster.py` & `earthstat-0.8.0/earthstat/geo_data_processing/rescale_resample_raster.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_data_processing/shapefile_process.py` & `earthstat-0.8.0/earthstat/geo_data_processing/shapefile_process.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_meta_extractors/mask_meta.py` & `earthstat-0.8.0/earthstat/geo_meta_extractors/mask_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_meta_extractors/predictor_meta.py` & `earthstat-0.8.0/earthstat/geo_meta_extractors/predictor_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/geo_meta_extractors/shapefile_meta.py` & `earthstat-0.8.0/earthstat/geo_meta_extractors/shapefile_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/utils.py` & `earthstat-0.8.0/earthstat/utils.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/xES/DailyDatasetBuilder.py` & `earthstat-0.8.0/earthstat/xES/DailyDatasetBuilder.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/xES/DekadalDatasetBuilder.py` & `earthstat-0.8.0/earthstat/xES/DekadalDatasetBuilder.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/xES/cds_api_key_manager.py` & `earthstat-0.8.0/earthstat/xES/cds_api_key_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,25 @@
             print(f"CDS API Key already exists in {cdsapirc_path}")
             with cdsapirc_path.open() as f:
                 lines = f.readlines()
                 for line in lines:
                     print(line)
             overwrite = input(
                 f"API Key found in {cdsapirc_path}. Do you want to overwrite it? (y/n): ")
+
             if overwrite.lower() == "y":
                 cdsApiKey = input("Please enter your CDS API Key: ")
                 with cdsapirc_path.open("w") as f:
                     f.write("url: https://cds.climate.copernicus.eu/api/v2\n")
                     f.write(f"key: {cdsApiKey}\n")
                 print("\nCDS API Key overwritten successfully")
 
             elif overwrite.lower() == "n":
                 print("CDS API Key not overwritten")
+
             else:
                 print("Invalid input. Please enter 'y' or 'n'")
                 self.add_cds_api_key()
         else:
             self._request_and_save_key(cdsapirc_path)
 
     def _request_and_save_key(self, cdsapirc_path):
```

### Comparing `earthstat-0.7.0/earthstat/xES/cds_param.py` & `earthstat-0.8.0/earthstat/xES/cds_param.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/xES/download_AgERA5py.py` & `earthstat-0.8.0/earthstat/xES/download_AgERA5py.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 try:
     import cdsapi
 except ImportError:
     print("Please install the cdsapi package using 'pip install cdsapi'")
 
 
 class AgERA5Downloader:
-    def __init__(self, area_name, parameters, start_year, end_year, bounding_box):
+    def __init__(self, area_name, parameters, bounding_box, start_year, end_year):
+
         self.api_key_manager = APIKeyManager().add_cds_api_key()
         self.area_name = area_name
         self.parameters = parameters
         self.start_year = start_year
         self.end_year = end_year
         self.bounding_box = bounding_box
 
@@ -29,16 +30,20 @@
                 for parameter in self.parameters
             ]
 
             for future in concurrent.futures.as_completed(tasks):
                 future.result()
 
     def _AgERA5_Requests(self, year, parameter):
+
         parameter_path = os.path.join(self.area_name, parameter)
+
         os.makedirs(parameter_path, exist_ok=True)
+
         retrieve_params = get_retrieve_params(
             parameter, self.bounding_box, year)
+
         self.cds.retrieve(
             'sis-agrometeorological-indicators',
             retrieve_params,
             f'{parameter_path}/{self.area_name}_{year}_{parameter}.zip'
         )
```

### Comparing `earthstat-0.7.0/earthstat/xES/get_csv.py` & `earthstat-0.8.0/earthstat/xES/get_csv.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/earthstat/xES/xES_utiles.py` & `earthstat-0.8.0/earthstat/xES/xES_utiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import zipfile
 import os
 import glob
 import re
 import logging
 
 
-def create_directories(area_name, build_dekadal_data=False):
+def create_directories(area_name):
     for param_folder in glob.glob(f'{area_name}/*'):
         try:
             os.makedirs(f'{param_folder}/Extracted', exist_ok=True)
-            os.makedirs(f'{param_folder}/Aggregated_CSV', exist_ok=True)
             logging.info(f"Created directories in {param_folder}")
         except Exception as e:
             logging.error(
                 f"Failed to create directories in {param_folder}: {e}")
 
 
 def extract_zip(file_path, extract_path):
```

### Comparing `earthstat-0.7.0/earthstat/xearthstat.py` & `earthstat-0.8.0/earthstat/xearthstat.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,50 +7,51 @@
 
 # Python built-in Libraries
 import os
 import geopandas as gpd
 
 
 class xEarthStat():
+    """
+    xEarthStat is a Python package that provides a simple interface to download and aggregate AgERA5 data for a given region of interest (ROI).
+    """
+
+    def __init__(self):
+
+        self.area_name = None
+        self.shapefile = None
+        self.aggregation_workflow = None
+        self.processing = None
+    # create directories for xEarthStat workflow
 
-    def __init__(self, area_name, shapefile_path, workflow='daily', multi_processing=False):
-
-        self.area_name = area_name  # create directories
-        self.workflow = workflow
-        self.processing = multi_processing
+    def init_workflow(self, area_name, shapefile_path=None):
 
-        self._init_shapefile(
-            shapefile_path
-        )
-
-        self._check_missing(shapefile_path)
+        self.area_name = area_name  # Essential for creating directories
+        os.makedirs(self.area_name, exist_ok=True)
 
-    def _init_shapefile(self, shapefile_path):
-        self.shapefile = gpd.read_file(shapefile_path)
-        # make sure the shapefile with wg84 projection
-        self.shapefile = self.shapefile.to_crs(epsg=4326)
+        if shapefile_path:
+            self.shapefile = gpd.read_file(shapefile_path)
+            # make sure the shapefile with wg84 projection
+            self.shapefile = self.shapefile.to_crs(epsg=4326)
 
-    # create directories for xEarthStat workflow
-
-    def _check_missing(self, shapefile_path):
-        os.makedirs(self.area_name, exist_ok=True)
-        if not shapefile_path:
-            print("Shapefile not provided")
-            self.shapefile = input(
-                "Please provide the path to the shapefile: ")
+        else:
+            print("No Shapefile Provided. You can download data without aggregation.")
+            print(
+                "If you plan to aggregate the data later, you will be asked to provide the shapefile path.")
+            self.shapefile = None
 
-    def init_AgERA5_downloader(self, parameters, start_year, end_year, bounding_box):
+    def init_AgERA5_downloader(self, parameters, bounding_box, start_year, end_year):
 
         self.data_downloader = AgERA5Downloader(
 
             self.area_name,
             parameters,
+            bounding_box,
             start_year,
-            end_year,
-            bounding_box
+            end_year
         )
 
     def download_AgERA5(self, num_requests, extract=True):
 
         self.data_downloader.download_AgERA5(num_requests)
         # ask users if they want to extract the data
         if extract:
@@ -62,68 +63,68 @@
 
     def extract_AgERA5(self):
         create_directories(self.area_name)
         extract_AgERA5_zips(self.area_name)
         print("AgERA5 Data Extracted Successfully")
 
     def Aggregate_AgERA5(
+            self, dataset_type='dekadal', all_touched=False, stat='mean',
+            multi_processing=False, max_workers=os.cpu_count()):
 
-        self,
-        max_workers=os.cpu_count(),
-        all_touched=False,
-        stat='mean'
-    ):
+        self._check_shapefile()
 
-        self._init_aggregation_workflow(
+        self.aggregation_workflow = dataset_type
+        self.processing = multi_processing
 
-            self.workflow,
-            all_touched=all_touched,
-            stat=stat
-        )
+        self._init_aggregation_workflow(
+            self.aggregation_workflow, all_touched=all_touched, stat=stat)
 
-        print(f"Building {self.workflow} ({stat}) Datasets...")
+        print(f"Building {self.aggregation_workflow} ({stat}) Datasets...")
         self.dataset_builder.build_datasets(max_workers=max_workers)
-        print(f"{self.workflow} Datasets Aggregated Successfully")
+        print(f"{self.aggregation_workflow} Datasets Aggregated Successfully")
 
     def _init_aggregation_workflow(
+            self, dataset_type, max_workers=os.cpu_count(),
+            all_touched=False, stat='mean'):
 
-        self,
-        workflow,
-        max_workers=os.cpu_count(),
-        all_touched=False,
-        stat='mean'
-    ):
-
-        if workflow == 'dekadal':
+        if dataset_type == 'dekadal':
 
             self.dataset_builder = DekadalDatasetBuilder(
 
                 self.area_name,
                 self.shapefile,
                 multiprocessing=self.processing,
                 max_workers=max_workers,
                 all_touched=all_touched,
                 stat=stat
 
             )
 
-            self.workflow = workflow
-
         else:
 
             self.dataset_builder = DailyDatasetBuilder(
 
                 self.area_name,
                 self.shapefile,
                 multiprocessing=self.processing,
                 max_workers=max_workers,
                 all_touched=all_touched,
                 stat=stat
 
             )
 
-            self.workflow = 'daily'
-
     def AgERA5_merged_csv(self, kelvin_to_celsius=False, output_name=None):
-        get_merged_csv(self.area_name, self.workflow,
+        get_merged_csv(self.area_name, self.aggregation_workflow,
                        kelvin_to_celsius=kelvin_to_celsius, output_name=output_name)
         print("CSV Merged Successfully")
+
+    def _check_shapefile(self):
+        if not self.shapefile:
+
+            print("Shapefile not provided")
+
+            shapefile_path = input(
+                "Please provide the path to the shapefile: ")
+
+            self.shapefile = gpd.read_file(shapefile_path)
+            self.shapefile = self.shapefile.to_crs(epsg=4326)
+            print("Shapefile Loaded Successfully\n")
```

### Comparing `earthstat-0.7.0/earthstat.egg-info/PKG-INFO` & `earthstat-0.8.0/earthstat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthstat
-Version: 0.7.0
+Version: 0.8.0
 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh <abdulrahman.amr.ali@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AbdelrahmanAmr3/earthstat
 Keywords: earthstat
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthstat Version: 0.7.0 Summary: EarthStat Library
+Metadata-Version: 2.1 Name: earthstat Version: 0.8.0 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh
 gmail.com> License: MIT License Project-URL: Homepage, https://github.com/
 AbdelrahmanAmr3/earthstat Keywords: earthstat Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `earthstat-0.7.0/earthstat.egg-info/SOURCES.txt` & `earthstat-0.8.0/earthstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/mkdocs.yml` & `earthstat-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.7.0/pyproject.toml` & `earthstat-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earthstat"
-version = "0.7.0"
+version = "0.8.0"
 dynamic = [
     "dependencies",
 ]
 description = "EarthStat Library"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
@@ -50,15 +50,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.7.0"
+current_version = "0.8.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

