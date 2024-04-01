# Comparing `tmp/napari-cryoet-data-portal-0.3.0.tar.gz` & `tmp/napari-cryoet-data-portal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-cryoet-data-portal-0.3.0.tar", last modified: Wed Jan 31 22:48:30 2024, max compression
+gzip compressed data, was "napari-cryoet-data-portal-0.3.1.tar", last modified: Mon Apr  1 15:54:15 2024, max compression
```

## Comparing `napari-cryoet-data-portal-0.3.0.tar` & `napari-cryoet-data-portal-0.3.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.418544 napari-cryoet-data-portal-0.3.0/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.350921 napari-cryoet-data-portal-0.3.0/.github/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.360514 napari-cryoet-data-portal-0.3.0/.github/workflows/
--rw-r--r--   0 asweet     (503) staff       (20)     1649 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/.github/workflows/test.yml
--rw-r--r--   0 asweet     (503) staff       (20)      992 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/.gitignore
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.362542 napari-cryoet-data-portal-0.3.0/.napari-hub/
--rw-r--r--   0 asweet     (503) staff       (20)      463 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 asweet     (503) staff       (20)      542 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/.napari-hub/config.yml
--rw-r--r--   0 asweet     (503) staff       (20)      815 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 asweet     (503) staff       (20)     1093 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/LICENSE
--rw-r--r--   0 asweet     (503) staff       (20)       96 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/MANIFEST.in
--rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-01-31 22:48:30.417142 napari-cryoet-data-portal-0.3.0/PKG-INFO
--rw-r--r--   0 asweet     (503) staff       (20)     6693 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.0/README.md
--rw-r--r--   0 asweet     (503) staff       (20)      329 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/SECURITY.md
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.364146 napari-cryoet-data-portal-0.3.0/examples/
--rw-r--r--   0 asweet     (503) staff       (20)      205 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/examples/demo-sample.py
--rw-r--r--   0 asweet     (503) staff       (20)      194 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/examples/demo.py
--rw-r--r--   0 asweet     (503) staff       (20)     1272 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/pyproject.toml
--rw-r--r--   0 asweet     (503) staff       (20)     1776 2024-01-31 22:48:30.419968 napari-cryoet-data-portal-0.3.0/setup.cfg
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.352064 napari-cryoet-data-portal-0.3.0/src/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.384047 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/
--rw-r--r--   0 asweet     (503) staff       (20)      546 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)     3671 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_filter.py
--rw-r--r--   0 asweet     (503) staff       (20)     1145 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_listing_tree_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     2835 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_listing_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)      367 2023-11-14 01:00:32.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_logging.py
--rw-r--r--   0 asweet     (503) staff       (20)     2006 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_metadata_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     6598 2024-01-31 21:26:34.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_open_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     4178 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_progress_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     7256 2024-01-31 21:26:34.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_reader.py
--rw-r--r--   0 asweet     (503) staff       (20)     1779 2024-01-31 22:45:51.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_sample_data.py
--rw-r--r--   0 asweet     (503) staff       (20)     1605 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_task_worker.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.407013 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)      516 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/_utils.py
--rw-r--r--   0 asweet     (503) staff       (20)      489 2024-01-31 22:45:51.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/conftest.py
--rw-r--r--   0 asweet     (503) staff       (20)     3020 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_listing_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1081 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1561 2024-01-31 21:26:34.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_open_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1419 2024-01-31 21:26:34.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_reader.py
--rw-r--r--   0 asweet     (503) staff       (20)      962 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_sample.py
--rw-r--r--   0 asweet     (503) staff       (20)     2147 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_uri_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     2349 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     4670 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_uri_widget.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.408276 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/__init__.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.410058 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/superqt/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/superqt/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)     6472 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)      411 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_version.py
--rw-r--r--   0 asweet     (503) staff       (20)     3029 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1659 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/napari.yaml
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-01-31 22:48:30.414231 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/
--rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 asweet     (503) staff       (20)     1946 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 asweet     (503) staff       (20)        1 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 asweet     (503) staff       (20)       84 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/entry_points.txt
--rw-r--r--   0 asweet     (503) staff       (20)      155 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 asweet     (503) staff       (20)       26 2024-01-31 22:48:30.000000 napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/top_level.txt
--rw-r--r--   0 asweet     (503) staff       (20)      624 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.0/tox.ini
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.169181 napari-cryoet-data-portal-0.3.1/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.111757 napari-cryoet-data-portal-0.3.1/.github/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.121126 napari-cryoet-data-portal-0.3.1/.github/workflows/
+-rw-r--r--   0 asweet     (503) staff       (20)     1649 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0 asweet     (503) staff       (20)      992 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.gitignore
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.123386 napari-cryoet-data-portal-0.3.1/.napari-hub/
+-rw-r--r--   0 asweet     (503) staff       (20)      463 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 asweet     (503) staff       (20)      542 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.napari-hub/config.yml
+-rw-r--r--   0 asweet     (503) staff       (20)      815 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 asweet     (503) staff       (20)     1093 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/LICENSE
+-rw-r--r--   0 asweet     (503) staff       (20)       96 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/MANIFEST.in
+-rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-04-01 15:54:15.168736 napari-cryoet-data-portal-0.3.1/PKG-INFO
+-rw-r--r--   0 asweet     (503) staff       (20)     6693 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/README.md
+-rw-r--r--   0 asweet     (503) staff       (20)      329 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/SECURITY.md
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.125005 napari-cryoet-data-portal-0.3.1/examples/
+-rw-r--r--   0 asweet     (503) staff       (20)      205 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/examples/demo-sample.py
+-rw-r--r--   0 asweet     (503) staff       (20)      194 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/examples/demo.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1272 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/pyproject.toml
+-rw-r--r--   0 asweet     (503) staff       (20)     1776 2024-04-01 15:54:15.170489 napari-cryoet-data-portal-0.3.1/setup.cfg
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.113549 napari-cryoet-data-portal-0.3.1/src/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.143917 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/
+-rw-r--r--   0 asweet     (503) staff       (20)      546 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3671 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_filter.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1145 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_tree_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2835 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)      367 2023-11-14 01:00:32.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_logging.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2006 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_metadata_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     7095 2024-04-01 15:22:04.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_open_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     4178 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_progress_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     7256 2024-03-29 23:03:57.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_reader.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1779 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_sample_data.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1605 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_task_worker.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.161445 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)      516 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/_utils.py
+-rw-r--r--   0 asweet     (503) staff       (20)      489 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/conftest.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3020 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_listing_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1081 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1561 2024-03-29 22:23:36.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_open_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1419 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_reader.py
+-rw-r--r--   0 asweet     (503) staff       (20)      962 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_sample.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2147 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_uri_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2349 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     4670 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_uri_widget.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.163442 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/__init__.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.164543 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)     6472 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)      411 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_version.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3029 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1659 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/napari.yaml
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.166086 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/
+-rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 asweet     (503) staff       (20)     1946 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 asweet     (503) staff       (20)        1 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 asweet     (503) staff       (20)       84 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/entry_points.txt
+-rw-r--r--   0 asweet     (503) staff       (20)      155 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 asweet     (503) staff       (20)       26 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/top_level.txt
+-rw-r--r--   0 asweet     (503) staff       (20)      624 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/tox.ini
```

### Comparing `napari-cryoet-data-portal-0.3.0/.github/workflows/test.yml` & `napari-cryoet-data-portal-0.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/.gitignore` & `napari-cryoet-data-portal-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/.napari-hub/config.yml` & `napari-cryoet-data-portal-0.3.1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/.pre-commit-config.yaml` & `napari-cryoet-data-portal-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/LICENSE` & `napari-cryoet-data-portal-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/PKG-INFO` & `napari-cryoet-data-portal-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cryoet-data-portal
-Version: 0.3.0
+Version: 0.3.1
 Summary: List, preview, and open data from the CZII CryoET Data Portal
 Home-page: https://github.com/chanzuckerberg/napari-cryoet-data-portal
 Author: Andy Sweet
 Author-email: andrewdsweet@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/chanzuckerberg/napari-cryoet-data-portal/issues
 Project-URL: Documentation, https://github.com/chanzuckerberg/napari-cryoet-data-portal#README.md
```

### Comparing `napari-cryoet-data-portal-0.3.0/README.md` & `napari-cryoet-data-portal-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/pyproject.toml` & `napari-cryoet-data-portal-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/setup.cfg` & `napari-cryoet-data-portal-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/__init__.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_filter.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_filter.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_listing_tree_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_tree_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_listing_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_metadata_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_metadata_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_open_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_open_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,16 +142,18 @@
         # Skip indexing for multi-resolution to avoid adding any
         # unnecessary nodes to the dask compute graph.
         if resolution is not MULTI_RESOLUTION:
             image_data = image_data[resolution.indices[0]]
         # Materialize low resolution immediately on this thread to prevent napari blocking.
         if resolution is LOW_RESOLUTION:
             image_data = np.asarray(image_data)
+        # Get scale before resolution scaling for annotations.
+        image_scale = image_attrs["scale"]
         image_attrs["scale"] = tuple(
-            resolution.scale * s for s in image_attrs["scale"]
+            resolution.scale * s for s in image_scale
         )
         image_translate = image_attrs.get("translate", (0,) * len(image_attrs["scale"]))
         image_attrs["translate"] = tuple(
             resolution.offset + t for t in image_translate
         )
         yield image_data, image_attrs, "image"
 
@@ -167,15 +169,21 @@
         for annotation in annotations:
             point_paths = tuple(
                 f.https_path
                 for f in annotation.files
                 if f.shape_type == "Point"
             )
             if len(point_paths) > 0:
-                yield read_annotation(annotation, tomogram=tomogram)
+                anno_data, anno_attrs, anno_type = read_annotation(annotation, tomogram=tomogram)
+                # Inherit scale from full resolution image so that we can pick up
+                # that scale when it changes.
+                anno_attrs["scale"] = image_scale
+                # Scaling points also changes the size, so adjust accordingly.
+                anno_attrs["size"] /= np.mean(image_scale)
+                yield anno_data, anno_attrs, anno_type
             else:
                 logger.warn("Found no points annotations. Skipping.")
 
     def _onLayerLoaded(self, layer_data: FullLayerData) -> None:
         logger.debug("OpenWidget._onLayerLoaded")
         data, attrs, layer_type = layer_data
         if layer_type == "image":
```

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_progress_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_progress_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_reader.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_sample_data.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_task_worker.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_task_worker.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/_utils.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_listing_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_listing_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_open_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_open_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_reader.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_sample.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_uri_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_uri_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_tests/test_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_uri_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_uri_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/_widget.py` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal/napari.yaml` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/PKG-INFO` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cryoet-data-portal
-Version: 0.3.0
+Version: 0.3.1
 Summary: List, preview, and open data from the CZII CryoET Data Portal
 Home-page: https://github.com/chanzuckerberg/napari-cryoet-data-portal
 Author: Andy Sweet
 Author-email: andrewdsweet@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/chanzuckerberg/napari-cryoet-data-portal/issues
 Project-URL: Documentation, https://github.com/chanzuckerberg/napari-cryoet-data-portal#README.md
```

### Comparing `napari-cryoet-data-portal-0.3.0/src/napari_cryoet_data_portal.egg-info/SOURCES.txt` & `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.0/tox.ini` & `napari-cryoet-data-portal-0.3.1/tox.ini`

 * *Files identical despite different names*

