# Comparing `tmp/pystac-1.8.4.tar.gz` & `tmp/pystac-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-1.8.4.tar", last modified: Mon Sep 25 19:11:30 2023, max compression
+gzip compressed data, was "pystac-1.9.0.tar", last modified: Tue Oct 24 15:52:31 2023, max compression
```

## Comparing `pystac-1.8.4.tar` & `pystac-1.9.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.845000 pystac-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-25 19:11:08.000000 pystac-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-25 19:11:08.000000 pystac-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-09-25 19:11:30.841000 pystac-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-09-25 19:11:08.000000 pystac-1.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2023-09-25 19:11:08.000000 pystac-1.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.829000 pystac-1.8.4/pystac/
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    46142 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    28347 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.833000 pystac-1.8.4/pystac/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7608 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21024 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    22597 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/datacube.py
--rw-r--r--   0 runner    (1001) docker     (127)    24359 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/item_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)    28917 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6409 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/mgrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25804 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    22627 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/sat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/scientific.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/extensions/xarray_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.833000 pystac-1.8.4/pystac/html/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/html/JSON.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/html/Macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/html/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    20499 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    22081 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/media_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/rel_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.833000 pystac-1.8.4/pystac/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/serialization/common_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/serialization/identify.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/serialization/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/stac_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    24329 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/stac_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.833000 pystac-1.8.4/pystac/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24229 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/static/fields-normalized.json
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    17667 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.837000 pystac-1.8.4/pystac/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.837000 pystac-1.8.4/pystac/validation/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.837000 pystac-1.8.4/pystac/validation/jsonschemas/geojson/
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/geojson/Feature.json
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/geojson/Geometry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.817000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.837000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/local_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13733 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/schema_uri_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/validation/stac_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-09-25 19:11:08.000000 pystac-1.8.4/pystac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 19:11:30.829000 pystac-1.8.4/pystac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-09-25 19:11:30.000000 pystac-1.8.4/pystac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-09-25 19:11:30.000000 pystac-1.8.4/pystac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 19:11:30.000000 pystac-1.8.4/pystac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-09-25 19:11:30.000000 pystac-1.8.4/pystac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-25 19:11:30.000000 pystac-1.8.4/pystac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 19:11:30.845000 pystac-1.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.604045 pystac-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-24 15:52:09.000000 pystac-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-10-24 15:52:09.000000 pystac-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2023-10-24 15:52:31.600045 pystac-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-10-24 15:52:09.000000 pystac-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-10-24 15:52:09.000000 pystac-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.584045 pystac-1.9.0/pystac/
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46172 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25651 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.588045 pystac-1.9.0/pystac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25561 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25147 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13850 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/item_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29064 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15826 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/sat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/scientific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/extensions/xarray_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/html/JSON.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/html/Macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/html/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9446 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18179 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/rel_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/serialization/common_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/serialization/identify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/serialization/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/stac_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24132 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/stac_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24229 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/static/fields-normalized.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/validation/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.592045 pystac-1.9.0/pystac/validation/jsonschemas/geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)    13777 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/geojson/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/geojson/Geometry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.576044 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.596045 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/local_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13674 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/schema_uri_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/validation/stac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-10-24 15:52:09.000000 pystac-1.9.0/pystac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 15:52:31.584045 pystac-1.9.0/pystac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2023-10-24 15:52:31.000000 pystac-1.9.0/pystac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2023-10-24 15:52:31.000000 pystac-1.9.0/pystac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 15:52:31.000000 pystac-1.9.0/pystac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-24 15:52:31.000000 pystac-1.9.0/pystac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-24 15:52:31.000000 pystac-1.9.0/pystac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 15:52:31.604045 pystac-1.9.0/setup.cfg
```

### Comparing `pystac-1.8.4/LICENSE` & `pystac-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/PKG-INFO` & `pystac-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/stac-utils/pystac
 Project-URL: Documentation, https://pystac.readthedocs.io
 Project-URL: Repository, https://github.com/stac-utils/pystac.git
@@ -12,34 +12,35 @@
 Project-URL: Discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: importlib-resources>=5.12.0; python_version < "3.9"
 Requires-Dist: python-dateutil>=2.7.0
 Provides-Extra: bench
 Requires-Dist: asv~=0.6.0; extra == "bench"
 Requires-Dist: packaging~=23.1; extra == "bench"
 Requires-Dist: virtualenv~=20.22; extra == "bench"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.2; extra == "docs"
+Requires-Dist: boto3~=1.28; extra == "docs"
 Requires-Dist: ipython~=8.12; extra == "docs"
 Requires-Dist: jinja2<4.0; extra == "docs"
 Requires-Dist: jupyter~=1.0; extra == "docs"
 Requires-Dist: nbsphinx~=0.9.0; extra == "docs"
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
+Requires-Dist: rasterio~=1.3; extra == "docs"
+Requires-Dist: shapely~=2.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
 Requires-Dist: sphinx-design~=0.5.0; extra == "docs"
 Requires-Dist: sphinxcontrib-fulltoc~=1.2; extra == "docs"
 Provides-Extra: jinja2
 Requires-Dist: jinja2<4.0; extra == "jinja2"
 Provides-Extra: orjson
 Requires-Dist: orjson>=3.5; extra == "orjson"
@@ -54,17 +55,19 @@
 Requires-Dist: mypy~=1.2; extra == "test"
 Requires-Dist: orjson~=3.8; extra == "test"
 Requires-Dist: pre-commit~=3.2; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10; extra == "test"
 Requires-Dist: pytest-recording~=0.13.0; extra == "test"
 Requires-Dist: pytest~=7.3; extra == "test"
-Requires-Dist: ruff==0.0.291; extra == "test"
+Requires-Dist: requests-mock~=1.11; extra == "test"
+Requires-Dist: ruff==0.1.1; extra == "test"
 Requires-Dist: types-html5lib~=1.1; extra == "test"
 Requires-Dist: types-orjson~=3.6; extra == "test"
+Requires-Dist: types-jsonschema~=4.18; extra == "test"
 Requires-Dist: types-python-dateutil~=2.8; extra == "test"
 Requires-Dist: types-urllib3~=1.26; extra == "test"
 Provides-Extra: urllib3
 Requires-Dist: urllib3>=1.26; extra == "urllib3"
 Provides-Extra: validation
 Requires-Dist: jsonschema~=4.18; extra == "validation"
```

### Comparing `pystac-1.8.4/README.md` & `pystac-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pyproject.toml` & `pystac-1.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,35 +11,34 @@
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-requires-python = ">=3.8"
-dependencies = [
-    "importlib-resources>=5.12.0; python_version<'3.9'",
-    "python-dateutil>=2.7.0",
-]
+requires-python = ">=3.9"
+dependencies = ["python-dateutil>=2.7.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 bench = ["asv~=0.6.0", "packaging~=23.1", "virtualenv~=20.22"]
 docs = [
     "Sphinx~=6.2",
+    "boto3~=1.28",
     "ipython~=8.12",
     "jinja2<4.0",
     "jupyter~=1.0",
     "nbsphinx~=0.9.0",
     "pydata-sphinx-theme~=0.13",
+    "rasterio~=1.3",
+    "shapely~=2.0",
     "sphinx-autobuild==2021.3.14",
     "sphinx-design~=0.5.0",
     "sphinxcontrib-fulltoc~=1.2",
 ]
 jinja2 = ["jinja2<4.0"]
 orjson = ["orjson>=3.5"]
 test = [
@@ -53,17 +52,19 @@
     "mypy~=1.2",
     "orjson~=3.8",
     "pre-commit~=3.2",
     "pytest-cov~=4.0",
     "pytest-mock~=3.10",
     "pytest-recording~=0.13.0",
     "pytest~=7.3",
-    "ruff==0.0.291",
+    "requests-mock~=1.11",
+    "ruff==0.1.1",
     "types-html5lib~=1.1",
     "types-orjson~=3.6",
+    "types-jsonschema~=4.18",
     "types-python-dateutil~=2.8",
     "types-urllib3~=1.26",
 ]
 urllib3 = ["urllib3>=1.26"]
 validation = ["jsonschema~=4.18"]
 
 [project.urls]
@@ -76,14 +77,22 @@
 [tool.setuptools.packages.find]
 include = ["pystac*"]
 exclude = ["tests*", "benchmarks*"]
 
 [tool.setuptools.dynamic]
 version = { attr = "pystac.version.__version__" }
 
+[tool.mypy]
+show_error_codes = true
+strict = true
+
+[[tool.mypy.overrides]]
+module = ["jinja2"]
+ignore_missing_imports = true
+
 [tool.ruff]
 line-length = 88
 select = ["E", "F", "I"]
 
 [tool.pytest.ini_options]
 filterwarnings = ["error"]
```

### Comparing `pystac-1.8.4/pystac/__init__.py` & `pystac-1.9.0/pystac/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     "read_dict",
     "write_file",
     "get_stac_version",
     "set_stac_version",
 ]
 
 import os
-from typing import Any, Dict, Optional
+import warnings
+from typing import Any, Optional
 
 from pystac.errors import (
     TemplateError,
     STACError,
     STACTypeError,
     DuplicateObjectKeyError,
     ExtensionAlreadyExistsError,
@@ -87,15 +88,18 @@
 import pystac.extensions.hooks
 import pystac.extensions.classification
 import pystac.extensions.datacube
 import pystac.extensions.eo
 import pystac.extensions.file
 import pystac.extensions.grid
 import pystac.extensions.item_assets
-import pystac.extensions.label
+
+with warnings.catch_warnings():
+    warnings.filterwarnings("ignore", category=DeprecationWarning)
+    import pystac.extensions.label
 import pystac.extensions.mgrs
 import pystac.extensions.pointcloud
 import pystac.extensions.projection
 import pystac.extensions.raster
 import pystac.extensions.sar
 import pystac.extensions.sat
 import pystac.extensions.scientific
@@ -193,15 +197,15 @@
     dest_href = None if dest_href is None else str(os.fspath(dest_href))
     obj.save_object(
         include_self_link=include_self_link, dest_href=dest_href, stac_io=stac_io
     )
 
 
 def read_dict(
-    d: Dict[str, Any],
+    d: dict[str, Any],
     href: Optional[str] = None,
     root: Optional[Catalog] = None,
     stac_io: Optional[StacIO] = None,
 ) -> STACObject:
     """Reads a :class:`~STACObject` or :class:`~ItemCollection` from a JSON-like dict
     representing a serialized STAC object.
```

### Comparing `pystac-1.8.4/pystac/asset.py` & `pystac-1.9.0/pystac/extensions/item_assets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,278 +1,288 @@
+"""Implements the :stac-ext:`Item Assets Definition Extension <item-assets>`."""
+
 from __future__ import annotations
 
-import os
-import shutil
-from copy import copy, deepcopy
-from html import escape
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union
+from copy import deepcopy
+from typing import TYPE_CHECKING, Any, Literal
 
-from pystac import common_metadata, utils
-from pystac.html.jinja_env import get_jinja_env
+import pystac
+from pystac.extensions.base import ExtensionManagementMixin
+from pystac.extensions.hooks import ExtensionHooks
+from pystac.serialization.identify import STACJSONDescription, STACVersionID
+from pystac.utils import get_required
 
 if TYPE_CHECKING:
-    from pystac.collection import Collection
-    from pystac.common_metadata import CommonMetadata
-    from pystac.item import Item
-
-A = TypeVar("A", bound="Asset")
-
-
-class Asset:
-    """An object that contains a link to data associated with an Item or Collection that
-    can be downloaded or streamed.
-
-    Args:
-        href : Link to the asset object. Relative and absolute links are both
-            allowed.
-        title : Optional displayed title for clients and users.
-        description : A description of the Asset providing additional details,
-            such as how it was processed or created. CommonMark 0.29 syntax MAY be used
-            for rich text representation.
-        media_type : Optional description of the media type. Registered Media Types
-            are preferred. See :class:`~pystac.MediaType` for common media types.
-        roles : Optional, Semantic roles (i.e. thumbnail, overview,
-            data, metadata) of the asset.
-        extra_fields : Optional, additional fields for this asset. This is used
-            by extensions as a way to serialize and deserialize properties on asset
-            object JSON.
-    """
+    from pystac.extensions.ext import ItemAssetExt
+
+SCHEMA_URI = "https://stac-extensions.github.io/item-assets/v1.0.0/schema.json"
 
-    href: str
-    """Link to the asset object. Relative and absolute links are both allowed."""
+ITEM_ASSETS_PROP = "item_assets"
 
-    title: Optional[str]
-    """Optional displayed title for clients and users."""
+ASSET_TITLE_PROP = "title"
+ASSET_DESC_PROP = "description"
+ASSET_TYPE_PROP = "type"
+ASSET_ROLES_PROP = "roles"
 
-    description: Optional[str]
-    """A description of the Asset providing additional details, such as how it was
-    processed or created. CommonMark 0.29 syntax MAY be used for rich text
-    representation."""
-
-    media_type: Optional[str]
-    """Optional description of the media type. Registered Media Types are preferred.
-    See :class:`~pystac.MediaType` for common media types."""
-
-    roles: Optional[List[str]]
-    """Optional, Semantic roles (i.e. thumbnail, overview, data, metadata) of the
-    asset."""
-
-    owner: Optional[Union[Item, Collection]]
-    """The :class:`~pystac.Item` or :class:`~pystac.Collection` that this asset belongs
-    to, or ``None`` if it has no owner."""
-
-    extra_fields: Dict[str, Any]
-    """Optional, additional fields for this asset. This is used by extensions as a
-    way to serialize and deserialize properties on asset object JSON."""
+
+class AssetDefinition:
+    """Object that contains details about the datafiles that will be included in member
+    Items for this Collection.
+
+    See the :stac-ext:`Asset Object <item-assets#asset-object>` for details.
+    """
+
+    properties: dict[str, Any]
+
+    owner: pystac.Collection | None
 
     def __init__(
+        self, properties: dict[str, Any], owner: pystac.Collection | None = None
+    ) -> None:
+        self.properties = properties
+        self.owner = owner
+
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, AssetDefinition):
+            return NotImplemented
+        return self.to_dict() == o.to_dict()
+
+    @classmethod
+    def create(
+        cls,
+        title: str | None,
+        description: str | None,
+        media_type: str | None,
+        roles: list[str] | None,
+        extra_fields: dict[str, Any] | None = None,
+    ) -> AssetDefinition:
+        """
+        Creates a new asset definition.
+
+        Args:
+            title : Displayed title for clients and users.
+            description : Description of the Asset providing additional details,
+                such as how it was processed or created.
+                `CommonMark 0.29 <http://commonmark.org/>`__ syntax MAY be used
+                for rich text representation.
+            media_type : `media type\
+                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
+                 of the asset.
+            roles : `semantic roles
+                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
+                of the asset, similar to the use of rel in links.
+            extra_fields : Additional fields on the asset definition, e.g. from
+                extensions.
+        """
+        asset_defn = cls({})
+        asset_defn.apply(
+            title=title,
+            description=description,
+            media_type=media_type,
+            roles=roles,
+            extra_fields=extra_fields,
+        )
+        return asset_defn
+
+    def apply(
         self,
-        href: str,
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        media_type: Optional[str] = None,
-        roles: Optional[List[str]] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
+        title: str | None,
+        description: str | None,
+        media_type: str | None,
+        roles: list[str] | None,
+        extra_fields: dict[str, Any] | None = None,
     ) -> None:
-        self.href = utils.make_posix_style(href)
+        """
+        Sets the properties for this asset definition.
+
+        Args:
+            title : Displayed title for clients and users.
+            description : Description of the Asset providing additional details,
+                such as how it was processed or created.
+                `CommonMark 0.29 <http://commonmark.org/>`__ syntax MAY be used
+                for rich text representation.
+            media_type : `media type\
+                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
+                 of the asset.
+            roles : `semantic roles
+                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
+                of the asset, similar to the use of rel in links.
+            extra_fields : Additional fields on the asset definition, e.g. from
+                extensions.
+        """
+        if extra_fields:
+            self.properties.update(extra_fields)
         self.title = title
         self.description = description
         self.media_type = media_type
         self.roles = roles
-        self.extra_fields = extra_fields or {}
-
-        # The Item which owns this Asset.
         self.owner = None
 
-    def set_owner(self, obj: Union[Collection, Item]) -> None:
-        """Sets the owning item of this Asset.
+    def set_owner(self, obj: pystac.Collection) -> None:
+        """Sets the owning item of this AssetDefinition.
 
         The owning item will be used to resolve relative HREFs of this asset.
 
         Args:
-            obj: The Collection or Item that owns this asset.
+            obj: The Collection that owns this asset.
         """
         self.owner = obj
 
-    def get_absolute_href(self) -> Optional[str]:
-        """Gets the absolute href for this asset, if possible.
-
-        If this Asset has no associated Item, and the asset HREF is a relative path,
-            this method will return ``None``. If the Item that owns the Asset has no
-            self HREF, this will also return ``None``.
-
-        Returns:
-            str: The absolute HREF of this asset, or None if an absolute HREF could not
-                be determined.
-        """
-        if utils.is_absolute_href(self.href):
-            return self.href
+    @property
+    def title(self) -> str | None:
+        """Gets or sets the displayed title for clients and users."""
+        return self.properties.get(ASSET_TITLE_PROP)
+
+    @title.setter
+    def title(self, v: str | None) -> None:
+        if v is None:
+            self.properties.pop(ASSET_TITLE_PROP, None)
         else:
-            if self.owner is not None:
-                item_self = self.owner.get_self_href()
-                if item_self is not None:
-                    return utils.make_absolute_href(self.href, item_self)
-            return None
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Returns this Asset as a dictionary.
-
-        Returns:
-            dict: A serialization of the Asset.
-        """
-
-        d: Dict[str, Any] = {"href": self.href}
-
-        if self.media_type is not None:
-            d["type"] = self.media_type
-
-        if self.title is not None:
-            d["title"] = self.title
+            self.properties[ASSET_TITLE_PROP] = v
 
-        if self.description is not None:
-            d["description"] = self.description
-
-        if self.extra_fields is not None and len(self.extra_fields) > 0:
-            for k, v in self.extra_fields.items():
-                d[k] = v
-
-        if self.roles is not None:
-            d["roles"] = self.roles
+    @property
+    def description(self) -> str | None:
+        """Gets or sets a description of the Asset providing additional details, such as
+        how it was processed or created. `CommonMark 0.29 <http://commonmark.org/>`__
+        syntax MAY be used for rich text representation."""
+        return self.properties.get(ASSET_DESC_PROP)
+
+    @description.setter
+    def description(self, v: str | None) -> None:
+        if v is None:
+            self.properties.pop(ASSET_DESC_PROP, None)
+        else:
+            self.properties[ASSET_DESC_PROP] = v
 
-        return d
+    @property
+    def media_type(self) -> str | None:
+        """Gets or sets the `media type
+        <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
+        of the asset."""
+        return self.properties.get(ASSET_TYPE_PROP)
+
+    @media_type.setter
+    def media_type(self, v: str | None) -> None:
+        if v is None:
+            self.properties.pop(ASSET_TYPE_PROP, None)
+        else:
+            self.properties[ASSET_TYPE_PROP] = v
 
-    def clone(self) -> Asset:
-        """Clones this asset. Makes a ``deepcopy`` of the
-        :attr:`~pystac.Asset.extra_fields`.
+    @property
+    def roles(self) -> list[str] | None:
+        """Gets or sets the `semantic roles
+        <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
+        of the asset, similar to the use of rel in links."""
+        return self.properties.get(ASSET_ROLES_PROP)
+
+    @roles.setter
+    def roles(self, v: list[str] | None) -> None:
+        if v is None:
+            self.properties.pop(ASSET_ROLES_PROP, None)
+        else:
+            self.properties[ASSET_ROLES_PROP] = v
 
-        Returns:
-            Asset: The clone of this asset.
-        """
-        cls = self.__class__
-        return cls(
-            href=self.href,
+    def to_dict(self) -> dict[str, Any]:
+        """Returns a dictionary representing this ``AssetDefinition``."""
+        return deepcopy(self.properties)
+
+    def create_asset(self, href: str) -> pystac.Asset:
+        """Creates a new :class:`~pystac.Asset` instance using the fields from this
+        ``AssetDefinition`` and the given ``href``."""
+        return pystac.Asset(
+            href=href,
             title=self.title,
             description=self.description,
             media_type=self.media_type,
             roles=self.roles,
-            extra_fields=deepcopy(self.extra_fields),
+            extra_fields={
+                k: v
+                for k, v in self.properties.items()
+                if k
+                not in {
+                    ASSET_TITLE_PROP,
+                    ASSET_DESC_PROP,
+                    ASSET_TYPE_PROP,
+                    ASSET_ROLES_PROP,
+                }
+            },
         )
 
-    def has_role(self, role: str) -> bool:
-        """Check if a role exists in the Asset role list.
+    @property
+    def ext(self) -> ItemAssetExt:
+        """Accessor for extension classes on this item_asset
 
-        Args:
-            role: Role to check for existence.
+        Example::
 
-        Returns:
-            bool: True if role exists, else False.
+            collection.ext.item_assets["data"].ext.proj.epsg = 4326
         """
-        if self.roles is None:
-            return False
-        else:
-            return role in self.roles
+        from pystac.extensions.ext import ItemAssetExt
 
-    @property
-    def common_metadata(self) -> CommonMetadata:
-        """Access the asset's common metadata fields as a
-        :class:`~pystac.CommonMetadata` object."""
-        return common_metadata.CommonMetadata(self)
+        return ItemAssetExt(stac_object=self)
 
-    def __repr__(self) -> str:
-        return "<Asset href={}>".format(self.href)
-
-    def _repr_html_(self) -> str:
-        jinja_env = get_jinja_env()
-        if jinja_env:
-            template = jinja_env.get_template("JSON.jinja2")
-            return str(template.render(dict=self.to_dict()))
-        else:
-            return escape(repr(self))
 
-    @classmethod
-    def from_dict(cls: Type[A], d: Dict[str, Any]) -> A:
-        """Constructs an Asset from a dict.
+class ItemAssetsExtension(ExtensionManagementMixin[pystac.Collection]):
+    name: Literal["item_assets"] = "item_assets"
+    collection: pystac.Collection
 
-        Returns:
-            Asset: The Asset deserialized from the JSON dict.
-        """
-        d = copy(d)
-        href = d.pop("href")
-        media_type = d.pop("type", None)
-        title = d.pop("title", None)
-        description = d.pop("description", None)
-        roles = d.pop("roles", None)
-        properties = None
-        if any(d):
-            properties = d
+    def __init__(self, collection: pystac.Collection) -> None:
+        self.collection = collection
 
-        return cls(
-            href=href,
-            media_type=media_type,
-            title=title,
-            description=description,
-            roles=roles,
-            extra_fields=properties,
+    @property
+    def item_assets(self) -> dict[str, AssetDefinition]:
+        """Gets or sets a dictionary of assets that can be found in member Items. Maps
+        the asset key to an :class:`AssetDefinition` instance."""
+        result: dict[str, Any] = get_required(
+            self.collection.extra_fields.get(ITEM_ASSETS_PROP), self, ITEM_ASSETS_PROP
         )
+        return {k: AssetDefinition(v, self.collection) for k, v in result.items()}
 
-    def move(self, href: str) -> Asset:
-        """Moves this asset's file to a new location on the local filesystem,
-        setting the asset href accordingly.
+    @item_assets.setter
+    def item_assets(self, v: dict[str, AssetDefinition]) -> None:
+        self.collection.extra_fields[ITEM_ASSETS_PROP] = {
+            k: asset_def.properties for k, asset_def in v.items()
+        }
 
-        Modifies the asset in place, and returns the same asset.
+    def __repr__(self) -> str:
+        return f"<ItemAssetsExtension collection.id = {self.collection.id}>"
 
-        Args:
-            href: The new asset location. Must be a local path. If relative
-                it must be relative to the owner object.
+    @classmethod
+    def get_schema_uri(cls) -> str:
+        return SCHEMA_URI
+
+    @classmethod
+    def ext(
+        cls, obj: pystac.Collection, add_if_missing: bool = False
+    ) -> ItemAssetsExtension:
+        """Extends the given :class:`~pystac.Collection` with properties from the
+        :stac-ext:`Item Assets Extension <item-assets>`.
 
-        Returns:
-            Asset: The asset with the updated href.
+        Raises:
+
+            pystac.ExtensionTypeError : If an invalid object type is passed.
         """
-        src = _absolute_href(self.href, self.owner, "move")
-        dst = _absolute_href(href, self.owner, "move")
-        shutil.move(src, dst)
-        self.href = href
-        return self
-
-    def copy(self, href: str) -> Asset:
-        """Copies this asset's file to a new location on the local filesystem,
-        setting the asset href accordingly.
+        if isinstance(obj, pystac.Collection):
+            cls.ensure_has_extension(obj, add_if_missing)
+            return cls(obj)
+        else:
+            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
-        Modifies the asset in place, and returns the same asset.
 
-        Args:
-            href: The new asset location. Must be a local path. If relative
-                it must be relative to the owner object.
+class ItemAssetsExtensionHooks(ExtensionHooks):
+    schema_uri: str = SCHEMA_URI
+    prev_extension_ids = {"asset", "item-assets"}
+    stac_object_types = {pystac.STACObjectType.COLLECTION}
 
-        Returns:
-            Asset: The asset with the updated href.
-        """
-        src = _absolute_href(self.href, self.owner, "copy")
-        dst = _absolute_href(href, self.owner, "copy")
-        shutil.copy2(src, dst)
-        self.href = href
-        return self
-
-    def delete(self) -> None:
-        """Delete this asset's file. Does not delete the asset from the item
-        that owns it. See :func:`~pystac.Item.delete_asset` for that.
+    def migrate(
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
+    ) -> None:
+        # Handle that the "item-assets" extension had the id of "assets", before
+        # collection assets (since removed) took over the ID of "assets"
+        if version < "1.0.0-beta.1" and "asset" in info.extensions:
+            if "assets" in obj:
+                obj["item_assets"] = obj["assets"]
+                del obj["assets"]
 
-        Does not modify the asset.
-        """
-        href = _absolute_href(self.href, self.owner, "delete")
-        os.remove(href)
+        super().migrate(obj, version, info)
 
 
-def _absolute_href(
-    href: str, owner: Optional[Union[Item, Collection]], action: str = "access"
-) -> str:
-    if utils.is_absolute_href(href):
-        return href
-    else:
-        item_self = owner.get_self_href() if owner else None
-        if item_self is None:
-            raise ValueError(
-                f"Cannot {action} file if asset href ('{href}') is relative "
-                "and owner item is not set. Hint: try using "
-                ":func:`~pystac.Item.make_asset_hrefs_absolute`"
-            )
-        return utils.make_absolute_href(href, item_self)
+ITEM_ASSETS_EXTENSION_HOOKS: ExtensionHooks = ItemAssetsExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/cache.py` & `pystac-1.9.0/pystac/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from collections import ChainMap
 from copy import copy
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, cast
 
 import pystac
 
 if TYPE_CHECKING:
     from pystac.collection import Collection
     from pystac.stac_object import STACObject
 
 
-def get_cache_key(stac_object: STACObject) -> Tuple[str, bool]:
+def get_cache_key(stac_object: STACObject) -> tuple[str, bool]:
     """Produce a cache key for the given STAC object.
 
     If a self href is set, use that as the cache key.
     If not, use a key that combines this object's ID with
     it's parents' IDs.
 
     Returns:
@@ -23,16 +23,16 @@
             element and a boolean that is true if the cache key is
             the object's HREF as the second element.
     """
     href = stac_object.get_self_href()
     if href is not None:
         return href, True
     else:
-        ids: List[str] = []
-        obj: Optional[pystac.STACObject] = stac_object
+        ids: list[str] = []
+        obj: pystac.STACObject | None = stac_object
         while obj is not None:
             ids.append(obj.id)
             obj = obj.get_parent()
         return "/".join(ids), False
 
 
 class ResolvedObjectCache:
@@ -57,31 +57,31 @@
             to the cached STACObject.
         hrefs_to_objects : STAC Object HREFs matched to
             their cached object.
         ids_to_collections : Map of collection IDs
             to collections.
     """
 
-    id_keys_to_objects: Dict[str, STACObject]
+    id_keys_to_objects: dict[str, STACObject]
     """Existing cache of a key made up of the STACObject and it's parents IDs mapped
     to the cached STACObject."""
 
-    hrefs_to_objects: Dict[str, STACObject]
+    hrefs_to_objects: dict[str, STACObject]
     """STAC Object HREFs matched to their cached object."""
 
-    ids_to_collections: Dict[str, Collection]
+    ids_to_collections: dict[str, Collection]
     """Map of collection IDs to collections."""
 
-    _collection_cache: Optional["ResolvedObjectCollectionCache"]
+    _collection_cache: ResolvedObjectCollectionCache | None
 
     def __init__(
         self,
-        id_keys_to_objects: Optional[Dict[str, STACObject]] = None,
-        hrefs_to_objects: Optional[Dict[str, STACObject]] = None,
-        ids_to_collections: Optional[Dict[str, Collection]] = None,
+        id_keys_to_objects: dict[str, STACObject] | None = None,
+        hrefs_to_objects: dict[str, STACObject] | None = None,
+        ids_to_collections: dict[str, Collection] | None = None,
     ):
         self.id_keys_to_objects = id_keys_to_objects or {}
         self.hrefs_to_objects = hrefs_to_objects or {}
         self.ids_to_collections = ids_to_collections or {}
 
         self._collection_cache = None
 
@@ -107,15 +107,15 @@
         else:
             if key in self.id_keys_to_objects:
                 return self.id_keys_to_objects[key]
             else:
                 self.cache(obj)
                 return obj
 
-    def get(self, obj: STACObject) -> Optional[STACObject]:
+    def get(self, obj: STACObject) -> STACObject | None:
         """Get the cached object that has the same cache key as the given object.
 
         Args:
             obj : The given object who's cache key will be checked against
                 the cache.
 
         Returns:
@@ -124,26 +124,26 @@
         """
         key, is_href = get_cache_key(obj)
         if is_href:
             return self.get_by_href(key)
         else:
             return self.id_keys_to_objects.get(key)
 
-    def get_by_href(self, href: str) -> Optional[STACObject]:
+    def get_by_href(self, href: str) -> STACObject | None:
         """Gets the cached object at href.
 
         Args:
             href : The href to use as the key for the cached object.
 
         Returns:
             STACObject or None: Returns the STACObject if cached, otherwise None.
         """
         return self.hrefs_to_objects.get(href)
 
-    def get_collection_by_id(self, id: str) -> Optional[Collection]:
+    def get_collection_by_id(self, id: str) -> Collection | None:
         """Retrieved a cached Collection by its ID.
 
         Args:
             id : The ID of the collection.
 
         Returns:
             Collection or None: Returns the collection if there is one cached
@@ -195,15 +195,15 @@
     def as_collection_cache(self) -> CollectionCache:
         if self._collection_cache is None:
             self._collection_cache = ResolvedObjectCollectionCache(self)
         return self._collection_cache
 
     @staticmethod
     def merge(
-        first: "ResolvedObjectCache", second: "ResolvedObjectCache"
+        first: ResolvedObjectCache, second: ResolvedObjectCache
     ) -> ResolvedObjectCache:
         """Merges two ResolvedObjectCache.
 
         The merged cache will give preference to the first argument; that is, if there
         are cached keys that exist in both the first and second cache, the object cached
         in the first will be cached in the resulting merged ResolvedObjectCache.
 
@@ -243,40 +243,38 @@
     JSON in :func:`pystac.serialization.merge_common_properties
     <pystac.serialization.common_properties.merge_common_properties>`.
     The CollectionCache will contain collections as either as dicts or PySTAC
     Collections, and will set Collection JSON that it reads in order to merge
     in common properties.
     """
 
-    cached_ids: Dict[str, Union[Collection, Dict[str, Any]]]
-    cached_hrefs: Dict[str, Union[Collection, Dict[str, Any]]]
+    cached_ids: dict[str, Collection | dict[str, Any]]
+    cached_hrefs: dict[str, Collection | dict[str, Any]]
 
     def __init__(
         self,
-        cached_ids: Optional[Dict[str, Union[Collection, Dict[str, Any]]]] = None,
-        cached_hrefs: Optional[Dict[str, Union[Collection, Dict[str, Any]]]] = None,
+        cached_ids: dict[str, Collection | dict[str, Any]] | None = None,
+        cached_hrefs: dict[str, Collection | dict[str, Any]] | None = None,
     ):
         self.cached_ids = cached_ids or {}
         self.cached_hrefs = cached_hrefs or {}
 
-    def get_by_id(
-        self, collection_id: str
-    ) -> Optional[Union[Collection, Dict[str, Any]]]:
+    def get_by_id(self, collection_id: str) -> Collection | dict[str, Any] | None:
         return self.cached_ids.get(collection_id)
 
-    def get_by_href(self, href: str) -> Optional[Union[Collection, Dict[str, Any]]]:
+    def get_by_href(self, href: str) -> Collection | dict[str, Any] | None:
         return self.cached_hrefs.get(href)
 
     def contains_id(self, collection_id: str) -> bool:
         return collection_id in self.cached_ids
 
     def cache(
         self,
-        collection: Union[Collection, Dict[str, Any]],
-        href: Optional[str] = None,
+        collection: Collection | dict[str, Any],
+        href: str | None = None,
     ) -> None:
         """Caches a collection JSON."""
         if isinstance(collection, pystac.Collection):
             self.cached_ids[collection.id] = collection
         else:
             self.cached_ids[collection["id"]] = collection
 
@@ -286,53 +284,51 @@
 
 class ResolvedObjectCollectionCache(CollectionCache):
     resolved_object_cache: ResolvedObjectCache
 
     def __init__(
         self,
         resolved_object_cache: ResolvedObjectCache,
-        cached_ids: Optional[Dict[str, Union[Collection, Dict[str, Any]]]] = None,
-        cached_hrefs: Optional[Dict[str, Union[Collection, Dict[str, Any]]]] = None,
+        cached_ids: dict[str, Collection | dict[str, Any]] | None = None,
+        cached_hrefs: dict[str, Collection | dict[str, Any]] | None = None,
     ):
         super().__init__(cached_ids, cached_hrefs)
         self.resolved_object_cache = resolved_object_cache
 
-    def get_by_id(
-        self, collection_id: str
-    ) -> Optional[Union[Collection, Dict[str, Any]]]:
+    def get_by_id(self, collection_id: str) -> Collection | dict[str, Any] | None:
         result = self.resolved_object_cache.get_collection_by_id(collection_id)
         if result is None:
             return super().get_by_id(collection_id)
         else:
             return result
 
-    def get_by_href(self, href: str) -> Optional[Union[Collection, Dict[str, Any]]]:
+    def get_by_href(self, href: str) -> Collection | dict[str, Any] | None:
         result = self.resolved_object_cache.get_by_href(href)
         if result is None:
             return super().get_by_href(href)
         else:
             return cast(pystac.Collection, result)
 
     def contains_id(self, collection_id: str) -> bool:
         return self.resolved_object_cache.contains_collection_id(
             collection_id
         ) or super().contains_id(collection_id)
 
     def cache(
         self,
-        collection: Union[Collection, Dict[str, Any]],
-        href: Optional[str] = None,
+        collection: Collection | dict[str, Any],
+        href: str | None = None,
     ) -> None:
         super().cache(collection, href)
 
     @staticmethod
     def merge(
         resolved_object_cache: ResolvedObjectCache,
-        first: Optional["ResolvedObjectCollectionCache"],
-        second: Optional["ResolvedObjectCollectionCache"],
+        first: ResolvedObjectCollectionCache | None,
+        second: ResolvedObjectCollectionCache | None,
     ) -> ResolvedObjectCollectionCache:
         first_cached_ids = {}
         if first is not None:
             first_cached_ids = copy(first.cached_ids)
 
         second_cached_ids = {}
         if second is not None:
```

### Comparing `pystac-1.8.4/pystac/catalog.py` & `pystac-1.9.0/pystac/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from __future__ import annotations
 
 import os
 import warnings
+from collections.abc import Iterable, Iterator
 from copy import deepcopy
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    Type,
     TypeVar,
     Union,
     cast,
 )
 
 import pystac
 from pystac.cache import ResolvedObjectCache
@@ -32,23 +26,25 @@
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     migrate_to_latest,
 )
 from pystac.stac_object import STACObject, STACObjectType
 from pystac.utils import (
+    HREF,
     StringEnum,
     is_absolute_href,
     make_absolute_href,
     make_relative_href,
 )
 
 if TYPE_CHECKING:
     from pystac.asset import Asset
     from pystac.collection import Collection
+    from pystac.extensions.ext import CatalogExt
     from pystac.item import Item
 
 C = TypeVar("C", bound="Catalog")
 
 
 class CatalogType(StringEnum):
     SELF_CONTAINED = "SELF_CONTAINED"
@@ -78,15 +74,15 @@
 
     See:
         :stac-spec:`The best practices documentation on published catalogs
         <best-practices.md#published-catalogs>`
     """
 
     @classmethod
-    def determine_type(cls, stac_json: Dict[str, Any]) -> Optional[CatalogType]:
+    def determine_type(cls, stac_json: dict[str, Any]) -> CatalogType | None:
         """Determines the catalog type based on a STAC JSON dict.
 
         Only applies to Catalogs or Collections
 
         Args:
             stac_json : The STAC JSON dict to determine the catalog type
 
@@ -136,53 +132,53 @@
 
     catalog_type: CatalogType
     """The catalog type. Defaults to :attr:`CatalogType.ABSOLUTE_PUBLISHED`."""
 
     description: str
     """Detailed multi-line description to fully explain the catalog."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Extra fields that are part of the top-level JSON properties of the Catalog."""
 
     id: str
     """Identifier for the catalog."""
 
-    links: List[Link]
+    links: list[Link]
     """A list of :class:`~pystac.Link` objects representing all links associated with
     this Catalog."""
 
-    title: Optional[str]
+    title: str | None
     """Optional short descriptive one-line title for the catalog."""
 
-    stac_extensions: List[str]
+    stac_extensions: list[str]
     """List of extensions the Catalog implements."""
 
     _resolved_objects: ResolvedObjectCache
 
     STAC_OBJECT_TYPE = pystac.STACObjectType.CATALOG
 
-    _stac_io: Optional[pystac.StacIO] = None
+    _stac_io: pystac.StacIO | None = None
     """Optional instance of StacIO that will be used by default
     for any IO operations on objects contained by this catalog.
     Set while reading in a catalog. This is set when a catalog
     is read by a StacIO instance."""
 
     DEFAULT_FILE_NAME = "catalog.json"
     """Default file name that will be given to this STAC object in
     a canonical format.
     """
 
     def __init__(
         self,
         id: str,
         description: str,
-        title: Optional[str] = None,
-        stac_extensions: Optional[List[str]] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
-        href: Optional[str] = None,
+        title: str | None = None,
+        stac_extensions: list[str] | None = None,
+        extra_fields: dict[str, Any] | None = None,
+        href: str | None = None,
         catalog_type: CatalogType = CatalogType.ABSOLUTE_PUBLISHED,
     ):
         super().__init__(stac_extensions or [])
 
         self.id = id
         self.description = description
         self.title = title
@@ -199,17 +195,17 @@
             self.set_self_href(href)
 
         self.catalog_type: CatalogType = catalog_type
 
         self._resolved_objects.cache(self)
 
     def __repr__(self) -> str:
-        return "<Catalog id={}>".format(self.id)
+        return f"<Catalog id={self.id}>"
 
-    def set_root(self, root: Optional["Catalog"]) -> None:
+    def set_root(self, root: Catalog | None) -> None:
         STACObject.set_root(self, root)
         if root is not None:
             root._resolved_objects = ResolvedObjectCache.merge(
                 root._resolved_objects, self._resolved_objects
             )
 
             # Walk through resolved object links and update the root
@@ -223,17 +219,17 @@
         return self.catalog_type in [
             CatalogType.RELATIVE_PUBLISHED,
             CatalogType.SELF_CONTAINED,
         ]
 
     def add_child(
         self,
-        child: Union["Catalog", Collection],
-        title: Optional[str] = None,
-        strategy: Optional[HrefLayoutStrategy] = None,
+        child: Catalog | Collection,
+        title: str | None = None,
+        strategy: HrefLayoutStrategy | None = None,
         set_parent: bool = True,
     ) -> Link:
         """Adds a link to a child :class:`~pystac.Catalog` or
         :class:`~pystac.Collection`.
 
         This method will set the child's parent to this object and potentially
         override its self_link (unless ``set_parent`` is False).
@@ -272,17 +268,15 @@
             child_href = strategy.get_href(child, os.path.dirname(self_href))
             child.set_self_href(child_href)
 
         child_link = Link.child(child, title=title)
         self.add_link(child_link)
         return child_link
 
-    def add_children(
-        self, children: Iterable[Union["Catalog", Collection]]
-    ) -> List[Link]:
+    def add_children(self, children: Iterable[Catalog | Collection]) -> list[Link]:
         """Adds links to multiple :class:`~pystac.Catalog` or `~pystac.Collection`
         objects. This method will set each child's parent to this object, and their
         root to this Catalog's root.
 
         Args:
             children : The children to add.
 
@@ -290,16 +284,16 @@
             List[Link]: An array of links created for the children
         """
         return [self.add_child(child) for child in children]
 
     def add_item(
         self,
         item: Item,
-        title: Optional[str] = None,
-        strategy: Optional[HrefLayoutStrategy] = None,
+        title: str | None = None,
+        strategy: HrefLayoutStrategy | None = None,
         set_parent: bool = True,
     ) -> Link:
         """Adds a link to an :class:`~pystac.Item`.
 
         This method will set the item's parent to this object and potentially
         override its self_link (unless ``set_parent`` is False)
 
@@ -340,16 +334,16 @@
         item_link = Link.item(item, title=title)
         self.add_link(item_link)
         return item_link
 
     def add_items(
         self,
         items: Iterable[Item],
-        strategy: Optional[HrefLayoutStrategy] = None,
-    ) -> List[Link]:
+        strategy: HrefLayoutStrategy | None = None,
+    ) -> list[Link]:
         """Adds links to multiple :class:`Items <pystac.Item>`.
 
         This method will set each item's parent to this object, and their root to
         this Catalog's root.
 
         Args:
             items : The items to add.
@@ -360,15 +354,15 @@
         Returns:
             List[Link]: A list of links created for the item
         """
         return [self.add_item(item, strategy=strategy) for item in items]
 
     def get_child(
         self, id: str, recursive: bool = False, sort_links_by_id: bool = True
-    ) -> Optional[Union["Catalog", Collection]]:
+    ) -> Catalog | Collection | None:
         """Gets the child of this catalog with the given ID, if it exists.
 
         Args:
             id : The ID of the child to find.
             recursive : If True, search this catalog and all children for the
                 item; otherwise, only search the children of this catalog. Defaults
                 to False.
@@ -377,20 +371,20 @@
                 will improve performance. Defaults to True.
 
         Return:
             Optional Catalog or Collection: The child with the given ID,
             or None if not found.
         """
         if not recursive:
-            children: Iterable[Union[pystac.Catalog, pystac.Collection]]
+            children: Iterable[pystac.Catalog | pystac.Collection]
             if not sort_links_by_id:
                 children = self.get_children()
             else:
 
-                def sort_function(links: List[Link]) -> List[Link]:
+                def sort_function(links: list[Link]) -> list[Link]:
                     return sorted(
                         links,
                         key=lambda x: (href := x.get_href()) is None or id not in href,
                     )
 
                 children = map(
                     lambda x: cast(Union[pystac.Catalog, pystac.Collection], x),
@@ -402,15 +396,15 @@
         else:
             for root, _, _ in self.walk():
                 child = root.get_child(id, recursive=False)
                 if child is not None:
                     return child
             return None
 
-    def get_children(self) -> Iterable[Union["Catalog", Collection]]:
+    def get_children(self) -> Iterable[Catalog | Collection]:
         """Return all children of this catalog.
 
         Return:
             Iterable[Catalog or Collection]: Iterable of children who's parent
             is this catalog.
         """
         return map(
@@ -429,15 +423,15 @@
     def get_all_collections(self) -> Iterable[Collection]:
         """Get all collections from this catalog and all subcatalogs. Will traverse
         any subcatalogs recursively."""
         yield from self.get_collections()
         for child in self.get_children():
             yield from child.get_collections()
 
-    def get_child_links(self) -> List[Link]:
+    def get_child_links(self) -> list[Link]:
         """Return all child links of this catalog.
 
         Return:
             List[Link]: List of links of this catalog with ``rel == 'child'``
         """
         return self.get_links(pystac.RelType.CHILD)
 
@@ -453,30 +447,30 @@
 
     def remove_child(self, child_id: str) -> None:
         """Removes an child from this catalog.
 
         Args:
             child_id : The ID of the child to remove.
         """
-        new_links: List[pystac.Link] = []
+        new_links: list[pystac.Link] = []
         root = self.get_root()
         for link in self.links:
             if link.rel != pystac.RelType.CHILD:
                 new_links.append(link)
             else:
                 link.resolve_stac_object(root=root)
                 child = cast("Catalog", link.target)
                 if child.id != child_id:
                     new_links.append(link)
                 else:
                     child.set_parent(None)
                     child.set_root(None)
         self.links = new_links
 
-    def get_item(self, id: str, recursive: bool = False) -> Optional[Item]:
+    def get_item(self, id: str, recursive: bool = False) -> Item | None:
         """
         DEPRECATED.
 
         .. deprecated:: 1.8
             Use :meth:`next(pystac.Catalog.get_items(id), None)` instead.
 
         Returns an item with a given ID.
@@ -550,15 +544,15 @@
 
     def remove_item(self, item_id: str) -> None:
         """Removes an item from this catalog.
 
         Args:
             item_id : The ID of the item to remove.
         """
-        new_links: List[pystac.Link] = []
+        new_links: list[pystac.Link] = []
         root = self.get_root()
         for link in self.links:
             if link.rel != pystac.RelType.ITEM:
                 new_links.append(link)
             else:
                 link.resolve_stac_object(root=root)
                 item = cast(pystac.Item, link.target)
@@ -589,34 +583,34 @@
             DeprecationWarning,
         )
         return chain(
             self.get_items(),
             *(child.get_items(recursive=True) for child in self.get_children()),
         )
 
-    def get_item_links(self) -> List[Link]:
+    def get_item_links(self) -> list[Link]:
         """Return all item links of this catalog.
 
         Return:
             List[Link]: List of links of this catalog with ``rel == 'item'``
         """
         return self.get_links(pystac.RelType.ITEM)
 
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         links = [
             x
             for x in self.links
             if x.rel != pystac.RelType.ROOT or x.get_href(transform_hrefs) is not None
         ]
         if not include_self_link:
             links = [x for x in links if x.rel != pystac.RelType.SELF]
 
-        d: Dict[str, Any] = {
+        d: dict[str, Any] = {
             "type": self.STAC_OBJECT_TYPE.value.title(),
             "id": self.id,
             "stac_version": pystac.get_stac_version(),
             "description": self.description,
             "links": [link.to_dict(transform_href=transform_hrefs) for link in links],
         }
 
@@ -669,17 +663,17 @@
             item.make_asset_hrefs_absolute()
         for collection in self.get_all_collections():
             collection.make_asset_hrefs_absolute()
 
     def normalize_and_save(
         self,
         root_href: str,
-        catalog_type: Optional[CatalogType] = None,
-        strategy: Optional[HrefLayoutStrategy] = None,
-        stac_io: Optional[pystac.StacIO] = None,
+        catalog_type: CatalogType | None = None,
+        strategy: HrefLayoutStrategy | None = None,
+        stac_io: pystac.StacIO | None = None,
         skip_unresolved: bool = False,
     ) -> None:
         """Normalizes link HREFs to the given root_href, and saves the catalog.
 
         This is a convenience method that simply calls :func:`Catalog.normalize_hrefs
         <pystac.Catalog.normalize_hrefs>` and :func:`Catalog.save <pystac.Catalog.save>`
         in sequence.
@@ -706,15 +700,15 @@
             root_href, strategy=strategy, skip_unresolved=skip_unresolved
         )
         self.save(catalog_type, stac_io=stac_io)
 
     def normalize_hrefs(
         self,
         root_href: str,
-        strategy: Optional[HrefLayoutStrategy] = None,
+        strategy: HrefLayoutStrategy | None = None,
         skip_unresolved: bool = False,
     ) -> None:
         """Normalize HREFs will regenerate all link HREFs based on
         an absolute root_href and the canonical catalog layout as specified
         in the STAC specification's best practices.
 
         This method mutates the entire catalog tree, unless ``skip_unresolved``
@@ -741,16 +735,16 @@
             _strategy = strategy
 
         # Normalizing requires an absolute path
         if not is_absolute_href(root_href):
             root_href = make_absolute_href(root_href, os.getcwd(), start_is_dir=True)
 
         def process_item(
-            item: Item, _root_href: str, parent: Optional[Catalog]
-        ) -> Optional[Callable[[], None]]:
+            item: Item, _root_href: str, parent: Catalog | None
+        ) -> Callable[[], None] | None:
             if not skip_unresolved:
                 item.resolve_links()
 
             # Abort as the intended parent is not the actual parent
             # https://github.com/stac-utils/pystac/issues/1116
             if parent is not None and item.get_parent() != parent:
                 return None
@@ -762,17 +756,17 @@
 
             return fn
 
         def process_catalog(
             cat: Catalog,
             _root_href: str,
             is_root: bool,
-            parent: Optional[Catalog] = None,
-        ) -> List[Callable[[], None]]:
-            setter_funcs: List[Callable[[], None]] = []
+            parent: Catalog | None = None,
+        ) -> list[Callable[[], None]]:
+            setter_funcs: list[Callable[[], None]] = []
 
             if not skip_unresolved:
                 cat.resolve_links()
 
             # Abort as the intended parent is not the actual parent
             # https://github.com/stac-utils/pystac/issues/1116
             if parent is not None and cat.get_parent() != parent:
@@ -816,17 +810,17 @@
 
         for fn in setter_funcs:
             fn()
 
     def generate_subcatalogs(
         self,
         template: str,
-        defaults: Optional[Dict[str, Any]] = None,
-        parent_ids: Optional[List[str]] = None,
-    ) -> List["Catalog"]:
+        defaults: dict[str, Any] | None = None,
+        parent_ids: list[str] | None = None,
+    ) -> list[Catalog]:
         """Walks through the catalog and generates subcatalogs
         for items based on the template string.
 
         See :class:`~pystac.layout.LayoutTemplate`
         for details on the construction of template strings. This template string
         will be applied to the items, and subcatalogs will be created that separate
         and organize the items based on template values.
@@ -840,36 +834,34 @@
             parent_ids : Optional list of the parent catalogs'
                 identifiers. If the bottom-most subcatalogs already match the
                 template, no subcatalog is added.
 
         Returns:
             [catalog]: List of new catalogs created
         """
-        result: List[Catalog] = []
+        result: list[Catalog] = []
         parent_ids = parent_ids or list()
         parent_ids.append(self.id)
         for child in self.get_children():
             result.extend(
                 child.generate_subcatalogs(
                     template, defaults=defaults, parent_ids=parent_ids.copy()
                 )
             )
 
         layout_template = LayoutTemplate(template, defaults=defaults)
 
-        keep_item_links: List[Link] = []
+        keep_item_links: list[Link] = []
         item_links = [lk for lk in self.links if lk.rel == pystac.RelType.ITEM]
         for link in item_links:
             link.resolve_stac_object(root=self.get_root())
             item = cast(pystac.Item, link.target)
             subcat_ids = layout_template.substitute(item).split("/")
             id_iter = reversed(parent_ids)
-            if all(
-                ["{}".format(id) == next(id_iter, None) for id in reversed(subcat_ids)]
-            ):
+            if all([f"{id}" == next(id_iter, None) for id in reversed(subcat_ids)]):
                 # Skip items for which the sub-catalog structure already
                 # matches the template. The list of parent IDs can include more
                 # elements on the root side, so compare the reversed sequences.
                 keep_item_links.append(link)
                 continue
             curr_parent = self
             for subcat_id in subcat_ids:
@@ -895,17 +887,17 @@
             lk for lk in self.links if lk.rel != pystac.RelType.ITEM
         ] + keep_item_links
 
         return result
 
     def save(
         self,
-        catalog_type: Optional[CatalogType] = None,
-        dest_href: Optional[str] = None,
-        stac_io: Optional[pystac.StacIO] = None,
+        catalog_type: CatalogType | None = None,
+        dest_href: str | None = None,
+        stac_io: pystac.StacIO | None = None,
     ) -> None:
         """Save this catalog and all it's children/item to files determined by the
         object's self link HREF or a specified path.
 
         Args:
             catalog_type : The catalog type that dictates the structure of
                 the catalog to save. Use a member of :class:`~pystac.CatalogType`.
@@ -991,15 +983,15 @@
             stac_io=stac_io,
         )
         if catalog_type is not None:
             self.catalog_type = catalog_type
 
     def walk(
         self,
-    ) -> Iterable[Tuple["Catalog", Iterable["Catalog"], Iterable[Item]]]:
+    ) -> Iterable[tuple[Catalog, Iterable[Catalog], Iterable[Item]]]:
         """Walks through children and items of catalogs.
 
         For each catalog in the STAC's tree rooted at this catalog (including this
         catalog itself), it yields a 3-tuple (root, subcatalogs, items). The root in
         that 3-tuple refers to the current catalog being walked, the subcatalogs are any
         catalogs or collections for which the root is a parent, and items represents
         any items that have the root as a parent.
@@ -1027,17 +1019,15 @@
         """
         for _, _, items in self.walk():
             # items is a generator, so we need to consume it to resolve the
             # items
             for item in items:
                 pass
 
-    def validate_all(
-        self, max_items: Optional[int] = None, recursive: bool = True
-    ) -> int:
+    def validate_all(self, max_items: int | None = None, recursive: bool = True) -> int:
         """Validates each catalog, collection, item contained within this catalog.
 
         Walks through the children and items of the catalog and validates each
         stac object.
 
         Args:
             max_items : The maximum number of STAC items to validate. Default
@@ -1063,24 +1053,24 @@
         for item in self.get_items():
             if max_items is not None and n >= max_items:
                 break
             item.validate()
             n += 1
         return n
 
-    def _object_links(self) -> List[Union[str, pystac.RelType]]:
+    def _object_links(self) -> list[str | pystac.RelType]:
         return [
             pystac.RelType.CHILD,
             pystac.RelType.ITEM,
             *pystac.EXTENSION_HOOKS.get_extended_object_links(self),
         ]
 
     def map_items(
         self,
-        item_mapper: Callable[[Item], Union[Item, List[Item]]],
+        item_mapper: Callable[[Item], Item | list[Item]],
     ) -> Catalog:
         """Creates a copy of a catalog, with each item passed through the
         item_mapper function.
 
         Args:
             item_mapper :   A function that takes in an item, and returns
                 either an item or list of items. The item that is passed into the
@@ -1093,15 +1083,15 @@
 
         new_cat = self.full_copy()
 
         def process_catalog(catalog: Catalog) -> None:
             for child in catalog.get_children():
                 process_catalog(child)
 
-            item_links: List[Link] = []
+            item_links: list[Link] = []
             for item_link in catalog.get_item_links():
                 item_link.resolve_stac_object(root=self.get_root())
                 mapped = item_mapper(cast(pystac.Item, item_link.target))
                 if mapped is None:
                     raise Exception("item_mapper cannot return None.")
                 if isinstance(mapped, pystac.Item):
                     item_link.target = mapped
@@ -1117,15 +1107,15 @@
         process_catalog(new_cat)
         return new_cat
 
     def map_assets(
         self,
         asset_mapper: Callable[
             [str, Asset],
-            Union[Asset, Tuple[str, Asset], Dict[str, Asset]],
+            Asset | tuple[str, Asset] | dict[str, Asset],
         ],
     ) -> Catalog:
         """Creates a copy of a catalog, with each Asset for each Item passed
         through the asset_mapper function.
 
         Args:
             asset_mapper : A function that takes in an key and an Asset, and
@@ -1135,16 +1125,16 @@
 
         Returns:
             Catalog: A full copy of this catalog, with assets manipulated according
             to the asset_mapper function.
         """
 
         def apply_asset_mapper(
-            tup: Tuple[str, Asset]
-        ) -> List[Tuple[str, pystac.Asset]]:
+            tup: tuple[str, Asset]
+        ) -> list[tuple[str, pystac.Asset]]:
             k, v = tup
             result = asset_mapper(k, v)
             if result is None:
                 raise Exception("asset_mapper cannot return None.")
             if isinstance(result, pystac.Asset):
                 return [(k, result)]
             elif isinstance(result, tuple):
@@ -1172,30 +1162,30 @@
 
         Args:
             include_hrefs (bool) - If True, print out each object's self link
                 HREF along with the object ID.
         """
         s = "{}* {}".format(" " * _indent, self)
         if include_hrefs:
-            s += " {}".format(self.get_self_href())
+            s += f" {self.get_self_href()}"
         print(s)
         for child in self.get_children():
             child.describe(include_hrefs=include_hrefs, _indent=_indent + 4)
         for item in self.get_items():
             s = "{}* {}".format(" " * (_indent + 2), item)
             if include_hrefs:
-                s += " {}".format(item.get_self_href())
+                s += f" {item.get_self_href()}"
             print(s)
 
     @classmethod
     def from_dict(
-        cls: Type[C],
-        d: Dict[str, Any],
-        href: Optional[str] = None,
-        root: Optional["Catalog"] = None,
+        cls: type[C],
+        d: dict[str, Any],
+        href: str | None = None,
+        root: Catalog | None = None,
         migrate: bool = False,
         preserve_dict: bool = True,
     ) -> C:
         if migrate:
             info = identify_stac_object(d)
             d = migrate_to_latest(d, info)
 
@@ -1235,26 +1225,36 @@
 
         if root:
             cat.set_root(root)
 
         return cat
 
     def full_copy(
-        self, root: Optional["Catalog"] = None, parent: Optional["Catalog"] = None
+        self, root: Catalog | None = None, parent: Catalog | None = None
     ) -> Catalog:
         return cast(Catalog, super().full_copy(root, parent))
 
     @classmethod
-    def from_file(
-        cls: Type[C], href: str, stac_io: Optional[pystac.StacIO] = None
-    ) -> C:
+    def from_file(cls: type[C], href: HREF, stac_io: pystac.StacIO | None = None) -> C:
         if stac_io is None:
             stac_io = pystac.StacIO.default()
 
         result = super().from_file(href, stac_io)
         result._stac_io = stac_io
 
         return result
 
     @classmethod
-    def matches_object_type(cls, d: Dict[str, Any]) -> bool:
+    def matches_object_type(cls, d: dict[str, Any]) -> bool:
         return identify_stac_object_type(d) == STACObjectType.CATALOG
+
+    @property
+    def ext(self) -> CatalogExt:
+        """Accessor for extension classes on this catalog
+
+        Example::
+
+            print(collection.ext.version)
+        """
+        from pystac.extensions.ext import CatalogExt
+
+        return CatalogExt(stac_object=self)
```

### Comparing `pystac-1.8.4/pystac/collection.py` & `pystac-1.9.0/pystac/collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 from __future__ import annotations
 
 import warnings
+from collections.abc import Iterable
 from copy import deepcopy
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
-    Iterable,
-    List,
     Optional,
-    Tuple,
-    Type,
     TypeVar,
     Union,
     cast,
 )
 
 from dateutil import tz
 
 import pystac
-from pystac import CatalogType, STACError, STACObjectType
-from pystac.asset import Asset
+from pystac import CatalogType, STACObjectType
+from pystac.asset import Asset, Assets
 from pystac.catalog import Catalog
 from pystac.errors import DeprecatedWarning, ExtensionNotImplemented, STACTypeError
 from pystac.layout import HrefLayoutStrategy
 from pystac.link import Link
 from pystac.provider import Provider
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
     migrate_to_latest,
 )
 from pystac.summaries import Summaries
 from pystac.utils import (
     datetime_to_str,
-    is_absolute_href,
-    make_absolute_href,
-    make_relative_href,
     str_to_datetime,
 )
 
 if TYPE_CHECKING:
+    from pystac.extensions.ext import CollectionExt
     from pystac.item import Item
 
 C = TypeVar("C", bound="Collection")
 
-TemporalIntervals = Union[List[List[datetime]], List[List[Optional[datetime]]]]
+Bboxes = list[list[Union[float, int]]]
+TemporalIntervals = Union[list[list[datetime]], list[list[Optional[datetime]]]]
 TemporalIntervalsLike = Union[
-    TemporalIntervals, List[datetime], List[Optional[datetime]]
+    TemporalIntervals, list[datetime], list[Optional[datetime]]
 ]
 
 
 class SpatialExtent:
     """Describes the spatial extent of a Collection.
 
     Args:
@@ -61,39 +56,42 @@
             array must be 2*n where n is the number of dimensions. For example, a
             2D Collection with only one bbox would be [[xmin, ymin, xmax, ymax]]
 
         extra_fields : Dictionary containing additional top-level fields defined on the
             Spatial Extent object.
     """
 
-    bboxes: List[List[float]]
+    bboxes: Bboxes
     """A list of bboxes that represent the spatial
     extent of the collection. Each bbox can be 2D or 3D. The length of the bbox
     array must be 2*n where n is the number of dimensions. For example, a
     2D Collection with only one bbox would be [[xmin, ymin, xmax, ymax]]"""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Dictionary containing additional top-level fields defined on the Spatial
     Extent object."""
 
     def __init__(
         self,
-        bboxes: Union[List[List[float]], List[float]],
-        extra_fields: Optional[Dict[str, Any]] = None,
+        bboxes: Bboxes | list[float | int],
+        extra_fields: dict[str, Any] | None = None,
     ) -> None:
+        if not isinstance(bboxes, list):
+            raise TypeError("bboxes must be a list")
+
         # A common mistake is to pass in a single bbox instead of a list of bboxes.
         # Account for this by transforming the input in that case.
-        if isinstance(bboxes, list) and isinstance(bboxes[0], float):
-            self.bboxes: List[List[float]] = [cast(List[float], bboxes)]
+        if isinstance(bboxes[0], (float, int)):
+            self.bboxes = [cast(list[Union[float, int]], bboxes)]
         else:
-            self.bboxes = cast(List[List[float]], bboxes)
+            self.bboxes = cast(Bboxes, bboxes)
 
         self.extra_fields = extra_fields or {}
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this spatial extent as a dictionary.
 
         Returns:
             dict: A serialization of the SpatialExtent.
         """
         d = {"bbox": self.bboxes, **self.extra_fields}
         return d
@@ -106,27 +104,27 @@
         """
         cls = self.__class__
         return cls(
             bboxes=deepcopy(self.bboxes), extra_fields=deepcopy(self.extra_fields)
         )
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> SpatialExtent:
+    def from_dict(d: dict[str, Any]) -> SpatialExtent:
         """Constructs a SpatialExtent from a dict.
 
         Returns:
             SpatialExtent: The SpatialExtent deserialized from the JSON dict.
         """
         return SpatialExtent(
             bboxes=d["bbox"], extra_fields={k: v for k, v in d.items() if k != "bbox"}
         )
 
     @staticmethod
     def from_coordinates(
-        coordinates: List[Any], extra_fields: Optional[Dict[str, Any]] = None
+        coordinates: list[Any], extra_fields: dict[str, Any] | None = None
     ) -> SpatialExtent:
         """Constructs a SpatialExtent from a set of coordinates.
 
         This method will only produce a single bbox that covers all points
         in the coordinate set.
 
         Args:
@@ -136,20 +134,20 @@
 
         Returns:
             SpatialExtent: A SpatialExtent with a single bbox that covers the
             given coordinates.
         """
 
         def process_coords(
-            coord_lists: List[Any],
-            xmin: Optional[float] = None,
-            ymin: Optional[float] = None,
-            xmax: Optional[float] = None,
-            ymax: Optional[float] = None,
-        ) -> Tuple[Optional[float], Optional[float], Optional[float], Optional[float]]:
+            coord_lists: list[Any],
+            xmin: float | None = None,
+            ymin: float | None = None,
+            xmax: float | None = None,
+            ymax: float | None = None,
+        ) -> tuple[float | None, float | None, float | None, float | None]:
             for coord in coord_lists:
                 if isinstance(coord[0], list):
                     xmin, ymin, xmax, ymax = process_coords(
                         coord, xmin, ymin, xmax, ymax
                     )
                 else:
                     x, y = coord
@@ -192,40 +190,42 @@
 
     intervals: TemporalIntervals
     """A list of two datetimes wrapped in a list,
     representing the temporal extent of a Collection. Open date ranges are
     represented by either the start (the first element of the interval) or the
     end (the second element of the interval) being None."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Dictionary containing additional top-level fields defined on the Temporal
     Extent object."""
 
     def __init__(
         self,
-        intervals: TemporalIntervals,
-        extra_fields: Optional[Dict[str, Any]] = None,
+        intervals: TemporalIntervals | list[datetime | None],
+        extra_fields: dict[str, Any] | None = None,
     ):
+        if not isinstance(intervals, list):
+            raise TypeError("intervals must be a list")
         # A common mistake is to pass in a single interval instead of a
         # list of intervals. Account for this by transforming the input
         # in that case.
-        if isinstance(intervals, list) and isinstance(intervals[0], datetime):
-            self.intervals = intervals
+        if isinstance(intervals[0], datetime) or intervals[0] is None:
+            self.intervals = [cast(list[Optional[datetime]], intervals)]
         else:
-            self.intervals = intervals
+            self.intervals = cast(TemporalIntervals, intervals)
 
         self.extra_fields = extra_fields or {}
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this temporal extent as a dictionary.
 
         Returns:
             dict: A serialization of the TemporalExtent.
         """
-        encoded_intervals: List[List[Optional[str]]] = []
+        encoded_intervals: list[list[str | None]] = []
         for i in self.intervals:
             start = None
             end = None
 
             if i[0] is not None:
                 start = datetime_to_str(i[0])
 
@@ -245,21 +245,21 @@
         """
         cls = self.__class__
         return cls(
             intervals=deepcopy(self.intervals), extra_fields=deepcopy(self.extra_fields)
         )
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> TemporalExtent:
+    def from_dict(d: dict[str, Any]) -> TemporalExtent:
         """Constructs an TemporalExtent from a dict.
 
         Returns:
             TemporalExtent: The TemporalExtent deserialized from the JSON dict.
         """
-        parsed_intervals: List[List[Optional[datetime]]] = []
+        parsed_intervals: list[list[datetime | None]] = []
         for i in d["interval"]:
             if isinstance(i, str):
                 # d["interval"] is a list of strings, so we correct the list and
                 # try again
                 # https://github.com/stac-utils/pystac/issues/1221
                 warnings.warn(
                     "A collection's temporal extent should be a list of lists, but "
@@ -310,29 +310,29 @@
 
     spatial: SpatialExtent
     """Potential spatial extent covered by the collection."""
 
     temporal: TemporalExtent
     """Potential temporal extent covered by the collection."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Dictionary containing additional top-level fields defined on the Extent
     object."""
 
     def __init__(
         self,
         spatial: SpatialExtent,
         temporal: TemporalExtent,
-        extra_fields: Optional[Dict[str, Any]] = None,
+        extra_fields: dict[str, Any] | None = None,
     ):
         self.spatial = spatial
         self.temporal = temporal
         self.extra_fields = extra_fields or {}
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this extent as a dictionary.
 
         Returns:
             dict: A serialization of the Extent.
         """
         d = {
             "spatial": self.spatial.to_dict(),
@@ -352,15 +352,15 @@
         return cls(
             spatial=self.spatial.clone(),
             temporal=self.temporal.clone(),
             extra_fields=deepcopy(self.extra_fields),
         )
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> Extent:
+    def from_dict(d: dict[str, Any]) -> Extent:
         """Constructs an Extent from a dict.
 
         Returns:
             Extent: The Extent deserialized from the JSON dict.
         """
         return Extent(
             spatial=SpatialExtent.from_dict(d["spatial"]),
@@ -368,36 +368,36 @@
             extra_fields={
                 k: v for k, v in d.items() if k not in {"spatial", "temporal"}
             },
         )
 
     @staticmethod
     def from_items(
-        items: Iterable[Item], extra_fields: Optional[Dict[str, Any]] = None
+        items: Iterable[Item], extra_fields: dict[str, Any] | None = None
     ) -> Extent:
         """Create an Extent based on the datetimes and bboxes of a list of items.
 
         Args:
             items : A list of items to derive the extent from.
             extra_fields : Optional dictionary containing additional top-level fields
                 defined on the Extent object.
 
         Returns:
             Extent: An Extent that spatially and temporally covers all of the
             given items.
         """
-        bounds_values: List[List[float]] = [
+        bounds_values: list[list[float]] = [
             [float("inf")],
             [float("inf")],
             [float("-inf")],
             [float("-inf")],
         ]
-        datetimes: List[datetime] = []
-        starts: List[datetime] = []
-        ends: List[datetime] = []
+        datetimes: list[datetime] = []
+        starts: list[datetime] = []
+        ends: list[datetime] = []
 
         for item in items:
             if item.bbox is not None:
                 for i in range(0, 4):
                     bounds_values[i].append(item.bbox[i])
             if item.datetime is not None:
                 datetimes.append(item.datetime)
@@ -436,15 +436,15 @@
             ]
         )
         temporal = TemporalExtent([[start_timestamp, end_timestamp]])
 
         return Extent(spatial=spatial, temporal=temporal, extra_fields=extra_fields)
 
 
-class Collection(Catalog):
+class Collection(Catalog, Assets):
     """A Collection extends the Catalog spec with additional metadata that helps
     enable discovery.
 
     Args:
         id : Identifier for the collection. Must be unique within the STAC.
         description : Detailed multi-line description to fully explain the
             collection. `CommonMark 0.29 syntax <https://commonmark.org/>`_ MAY
@@ -471,111 +471,108 @@
         extra_fields : Extra fields that are part of the top-level
             JSON properties of the Collection.
         assets : A dictionary mapping string keys to :class:`~pystac.Asset` objects. All
             :class:`~pystac.Asset` values in the dictionary will have their
             :attr:`~pystac.Asset.owner` attribute set to the created Collection.
     """
 
-    assets: Dict[str, Asset]
-    """Map of Assets"""
-
     description: str
     """Detailed multi-line description to fully explain the collection."""
 
     extent: Extent
     """Spatial and temporal extents that describe the bounds of all items contained
     within this Collection."""
 
     id: str
     """Identifier for the collection."""
 
-    stac_extensions: List[str]
+    stac_extensions: list[str]
     """List of extensions the Collection implements."""
 
-    title: Optional[str]
+    title: str | None
     """Optional short descriptive one-line title for the collection."""
 
-    keywords: Optional[List[str]]
+    keywords: list[str] | None
     """Optional list of keywords describing the collection."""
 
-    providers: Optional[List[Provider]]
+    providers: list[Provider] | None
     """Optional list of providers of this Collection."""
 
     summaries: Summaries
     """A map of property summaries, either a set of values or statistics such as a
     range."""
 
-    links: List[Link]
+    links: list[Link]
     """A list of :class:`~pystac.Link` objects representing all links associated with
     this Collection."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Extra fields that are part of the top-level JSON properties of the Collection."""
 
     STAC_OBJECT_TYPE = STACObjectType.COLLECTION
 
     DEFAULT_FILE_NAME = "collection.json"
     """Default file name that will be given to this STAC object
     in a canonical format."""
 
     def __init__(
         self,
         id: str,
         description: str,
         extent: Extent,
-        title: Optional[str] = None,
-        stac_extensions: Optional[List[str]] = None,
-        href: Optional[str] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
-        catalog_type: Optional[CatalogType] = None,
+        title: str | None = None,
+        stac_extensions: list[str] | None = None,
+        href: str | None = None,
+        extra_fields: dict[str, Any] | None = None,
+        catalog_type: CatalogType | None = None,
         license: str = "proprietary",
-        keywords: Optional[List[str]] = None,
-        providers: Optional[List[Provider]] = None,
-        summaries: Optional[Summaries] = None,
-        assets: Optional[Dict[str, Asset]] = None,
+        keywords: list[str] | None = None,
+        providers: list[Provider] | None = None,
+        summaries: Summaries | None = None,
+        assets: dict[str, Asset] | None = None,
     ):
         super().__init__(
             id,
             description,
             title,
             stac_extensions,
             extra_fields,
             href,
             catalog_type or CatalogType.ABSOLUTE_PUBLISHED,
         )
         self.extent = extent
         self.license = license
 
-        self.stac_extensions: List[str] = stac_extensions or []
+        self.stac_extensions: list[str] = stac_extensions or []
         self.keywords = keywords
         self.providers = providers
         self.summaries = summaries or Summaries.empty()
 
         self.assets = {}
         if assets is not None:
             for k, asset in assets.items():
                 self.add_asset(k, asset)
 
     def __repr__(self) -> str:
-        return "<Collection id={}>".format(self.id)
+        return f"<Collection id={self.id}>"
 
     def add_item(
         self,
         item: Item,
-        title: Optional[str] = None,
-        strategy: Optional[HrefLayoutStrategy] = None,
+        title: str | None = None,
+        strategy: HrefLayoutStrategy | None = None,
         set_parent: bool = True,
     ) -> Link:
         link = super().add_item(item, title, strategy, set_parent)
         item.set_collection(self)
         return link
 
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         d = super().to_dict(
             include_self_link=include_self_link, transform_hrefs=transform_hrefs
         )
         d["extent"] = self.extent.to_dict()
         d["license"] = self.license
         if self.stac_extensions:
             d["stac_extensions"] = self.stac_extensions
@@ -620,18 +617,18 @@
             else:
                 clone.add_link(link.clone())
 
         return clone
 
     @classmethod
     def from_dict(
-        cls: Type[C],
-        d: Dict[str, Any],
-        href: Optional[str] = None,
-        root: Optional[Catalog] = None,
+        cls: type[C],
+        d: dict[str, Any],
+        href: str | None = None,
+        root: Catalog | None = None,
         migrate: bool = False,
         preserve_dict: bool = True,
     ) -> C:
         from pystac.extensions.version import CollectionVersionExtension
 
         if migrate:
             info = identify_stac_object(d)
@@ -702,15 +699,15 @@
                 )
             # Collection asset deprecation checks pending version extension support
         except ExtensionNotImplemented:
             pass
 
         return collection
 
-    def get_item(self, id: str, recursive: bool = False) -> Optional[Item]:
+    def get_item(self, id: str, recursive: bool = False) -> Item | None:
         """Returns an item with a given ID.
 
         Args:
             id : The ID of the item to find.
             recursive : If True, search this collection and all children for the
                 item; otherwise, only search the items of this collection. Defaults
                 to False.
@@ -723,110 +720,33 @@
         except TypeError as e:
             if any("recursive" in arg for arg in e.args):
                 # For inherited classes that do not yet support recursive
                 # See https://github.com/stac-utils/pystac-client/issues/485
                 return super().get_item(id, recursive=recursive)
             raise e
 
-    def get_assets(
-        self,
-        media_type: Optional[Union[str, pystac.MediaType]] = None,
-        role: Optional[str] = None,
-    ) -> Dict[str, Asset]:
-        """Get this collection's assets.
-
-        Args:
-            media_type: If set, filter the assets such that only those with a
-                matching ``media_type`` are returned.
-            role: If set, filter the assets such that only those with a matching
-                ``role`` are returned.
-
-        Returns:
-            Dict[str, Asset]: A dictionary of assets that match ``media_type``
-            and/or ``role`` if set or else all of this collection's assets.
-        """
-        return {
-            k: deepcopy(v)
-            for k, v in self.assets.items()
-            if (media_type is None or v.media_type == media_type)
-            and (role is None or v.has_role(role))
-        }
-
-    def add_asset(self, key: str, asset: Asset) -> None:
-        """Adds an Asset to this collection.
-
-        Args:
-            key : The unique key of this asset.
-            asset : The Asset to add.
-        """
-        asset.set_owner(self)
-        self.assets[key] = asset
-
-    def delete_asset(self, key: str) -> None:
-        """Deletes the asset at the given key, and removes the asset's data
-        file from the local filesystem.
-
-        It is an error to attempt to delete an asset's file if it is on a
-        remote filesystem.
-
-        To delete the asset without removing the file, use
-        `del collection.assets["key"]`.
-
-        Args:
-            key: The unique key of this asset.
-        """
-        asset = self.assets[key]
-        asset.set_owner(self)
-        asset.delete()
-
-        del self.assets[key]
-
-    def make_asset_hrefs_relative(self) -> Collection:
-        """Modify each asset's HREF to be relative to this collection's self HREF.
-
-        Returns:
-            Collection: self
-        """
-        self_href = self.get_self_href()
-        for asset in self.assets.values():
-            if is_absolute_href(asset.href):
-                if self_href is None:
-                    raise STACError(
-                        "Cannot make asset HREFs relative " "if no self_href is set."
-                    )
-                asset.href = make_relative_href(asset.href, self_href)
-        return self
-
-    def make_asset_hrefs_absolute(self) -> Collection:
-        """Modify each asset's HREF to be absolute.
-
-        Any asset HREFs that are relative will be modified to absolute based on this
-        collection's self HREF.
-
-        Returns:
-            Collection: self
-        """
-        self_href = self.get_self_href()
-        for asset in self.assets.values():
-            if not is_absolute_href(asset.href):
-                if self_href is None:
-                    raise STACError(
-                        "Cannot make relative asset HREFs absolute "
-                        "if no self_href is set."
-                    )
-                asset.href = make_absolute_href(asset.href, self_href)
-        return self
-
     def update_extent_from_items(self) -> None:
         """
         Update datetime and bbox based on all items to a single bbox and time window.
         """
         self.extent = Extent.from_items(self.get_items(recursive=True))
 
     def full_copy(
-        self, root: Optional["Catalog"] = None, parent: Optional["Catalog"] = None
+        self, root: Catalog | None = None, parent: Catalog | None = None
     ) -> Collection:
         return cast(Collection, super().full_copy(root, parent))
 
     @classmethod
-    def matches_object_type(cls, d: Dict[str, Any]) -> bool:
+    def matches_object_type(cls, d: dict[str, Any]) -> bool:
         return identify_stac_object_type(d) == STACObjectType.COLLECTION
+
+    @property
+    def ext(self) -> CollectionExt:
+        """Accessor for extension classes on this collection
+
+        Example::
+
+            print(collection.ext.xarray)
+        """
+        from pystac.extensions.ext import CollectionExt
+
+        return CollectionExt(stac_object=self)
```

### Comparing `pystac-1.8.4/pystac/common_metadata.py` & `pystac-1.9.0/pystac/common_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Optional, TypeVar, cast
 
 import pystac
 from pystac import utils
 from pystac.errors import STACError
 
 if TYPE_CHECKING:
     from pystac.asset import Asset
@@ -21,195 +21,195 @@
     are still commonly used. All attributes are defined within the properties of
     this item and are optional
 
     Args:
         properties : Dictionary of attributes that is the Item's properties
     """
 
-    object: Union[Asset, Item]
+    object: Asset | Item
     """The object from which common metadata is obtained."""
 
-    def __init__(self, object: Union[Asset, Item]):
+    def __init__(self, object: Asset | Item):
         self.object = object
 
-    def _set_field(self, prop_name: str, v: Optional[Any]) -> None:
+    def _set_field(self, prop_name: str, v: Any | None) -> None:
         if hasattr(self.object, prop_name):
             setattr(self.object, prop_name, v)
         elif hasattr(self.object, "properties"):
             item = cast(pystac.Item, self.object)
             if v is None:
                 item.properties.pop(prop_name, None)
             else:
                 item.properties[prop_name] = v
         elif hasattr(self.object, "extra_fields") and isinstance(
-            self.object.extra_fields, Dict
+            self.object.extra_fields, dict
         ):
             if v is None:
                 self.object.extra_fields.pop(prop_name, None)
             else:
                 self.object.extra_fields[prop_name] = v
         else:
             raise pystac.STACError(f"Cannot set field {prop_name} on {self}.")
 
-    def _get_field(self, prop_name: str, _typ: Type[P]) -> Optional[P]:
+    def _get_field(self, prop_name: str, _typ: type[P]) -> P | None:
         if hasattr(self.object, prop_name):
             return cast(Optional[P], getattr(self.object, prop_name))
         elif hasattr(self.object, "properties"):
             item = cast(pystac.Item, self.object)
             return item.properties.get(prop_name)
         elif hasattr(self.object, "extra_fields") and isinstance(
-            self.object.extra_fields, Dict
+            self.object.extra_fields, dict
         ):
             return self.object.extra_fields.get(prop_name)
         else:
             raise STACError(f"Cannot get field {prop_name} from {self}.")
 
     # Basics
     @property
-    def title(self) -> Optional[str]:
+    def title(self) -> str | None:
         """Gets or set the object's title."""
         return self._get_field("title", str)
 
     @title.setter
-    def title(self, v: Optional[str]) -> None:
+    def title(self, v: str | None) -> None:
         self._set_field("title", v)
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Gets or set the object's description."""
         return self._get_field("description", str)
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         self._set_field("description", v)
 
     # Date and Time Range
     @property
-    def start_datetime(self) -> Optional[datetime]:
+    def start_datetime(self) -> datetime | None:
         """Get or set the object's start_datetime."""
         return utils.map_opt(
             utils.str_to_datetime, self._get_field("start_datetime", str)
         )
 
     @start_datetime.setter
-    def start_datetime(self, v: Optional[datetime]) -> None:
+    def start_datetime(self, v: datetime | None) -> None:
         self._set_field("start_datetime", utils.map_opt(utils.datetime_to_str, v))
 
     @property
-    def end_datetime(self) -> Optional[datetime]:
+    def end_datetime(self) -> datetime | None:
         """Get or set the item's end_datetime."""
         return utils.map_opt(
             utils.str_to_datetime, self._get_field("end_datetime", str)
         )
 
     @end_datetime.setter
-    def end_datetime(self, v: Optional[datetime]) -> None:
+    def end_datetime(self, v: datetime | None) -> None:
         self._set_field("end_datetime", utils.map_opt(utils.datetime_to_str, v))
 
     # License
     @property
-    def license(self) -> Optional[str]:
+    def license(self) -> str | None:
         """Get or set the current license."""
         return self._get_field("license", str)
 
     @license.setter
-    def license(self, v: Optional[str]) -> None:
+    def license(self, v: str | None) -> None:
         self._set_field("license", v)
 
     # Providers
     @property
-    def providers(self) -> Optional[List[Provider]]:
+    def providers(self) -> list[Provider] | None:
         """Get or set a list of the object's providers."""
         return utils.map_opt(
             lambda providers: [pystac.Provider.from_dict(d) for d in providers],
-            self._get_field("providers", List[Dict[str, Any]]),
+            self._get_field("providers", list[dict[str, Any]]),
         )
 
     @providers.setter
-    def providers(self, v: Optional[List[Provider]]) -> None:
+    def providers(self, v: list[Provider] | None) -> None:
         self._set_field(
             "providers",
             utils.map_opt(lambda providers: [p.to_dict() for p in providers], v),
         )
 
     # Instrument
     @property
-    def platform(self) -> Optional[str]:
+    def platform(self) -> str | None:
         """Gets or set the object's platform attribute."""
         return self._get_field("platform", str)
 
     @platform.setter
-    def platform(self, v: Optional[str]) -> None:
+    def platform(self, v: str | None) -> None:
         self._set_field("platform", v)
 
     @property
-    def instruments(self) -> Optional[List[str]]:
+    def instruments(self) -> list[str] | None:
         """Gets or sets the names of the instruments used."""
-        return self._get_field("instruments", List[str])
+        return self._get_field("instruments", list[str])
 
     @instruments.setter
-    def instruments(self, v: Optional[List[str]]) -> None:
+    def instruments(self, v: list[str] | None) -> None:
         self._set_field("instruments", v)
 
     @property
-    def constellation(self) -> Optional[str]:
+    def constellation(self) -> str | None:
         """Gets or set the name of the constellation associate with an object."""
         return self._get_field("constellation", str)
 
     @constellation.setter
-    def constellation(self, v: Optional[str]) -> None:
+    def constellation(self, v: str | None) -> None:
         self._set_field("constellation", v)
 
     @property
-    def mission(self) -> Optional[str]:
+    def mission(self) -> str | None:
         """Gets or set the name of the mission associated with an object."""
         return self._get_field("mission", str)
 
     @mission.setter
-    def mission(self, v: Optional[str]) -> None:
+    def mission(self, v: str | None) -> None:
         self._set_field("mission", v)
 
     @property
-    def gsd(self) -> Optional[float]:
+    def gsd(self) -> float | None:
         """Gets or sets the Ground Sample Distance at the sensor."""
         return self._get_field("gsd", float)
 
     @gsd.setter
-    def gsd(self, v: Optional[float]) -> None:
+    def gsd(self, v: float | None) -> None:
         self._set_field("gsd", v)
 
     # Metadata
     @property
-    def created(self) -> Optional[datetime]:
+    def created(self) -> datetime | None:
         """Get or set the metadata file's creation date. All datetime attributes have
         setters that can take either a string or a datetime, but always stores
         the attribute as a string.
 
         Note:
             ``created`` has a different meaning depending on the type of STAC object.
             On an :class:`~pystac.Item`, it refers to the creation time of the
             metadata. On an :class:`~pystac.Asset`, it refers to the creation time of
             the actual data linked to in :attr:`Asset.href <pystac.Asset.href`.
         """
         return utils.map_opt(utils.str_to_datetime, self._get_field("created", str))
 
     @created.setter
-    def created(self, v: Optional[datetime]) -> None:
+    def created(self, v: datetime | None) -> None:
         self._set_field("created", utils.map_opt(utils.datetime_to_str, v))
 
     @property
-    def updated(self) -> Optional[datetime]:
+    def updated(self) -> datetime | None:
         """Get or set the metadata file's update date. All datetime attributes have
         setters that can take either a string or a datetime, but always stores
         the attribute as a string
 
         Note:
             ``updated`` has a different meaning depending on the type of STAC object.
             On an :class:`~pystac.Item`, it refers to the update time of the
             metadata. On an :class:`~pystac.Asset`, it refers to the update time of
             the actual data linked to in :attr:`Asset.href <pystac.Asset.href`.
         """
         return utils.map_opt(utils.str_to_datetime, self._get_field("updated", str))
 
     @updated.setter
-    def updated(self, v: Optional[datetime]) -> None:
+    def updated(self, v: datetime | None) -> None:
         self._set_field("updated", utils.map_opt(utils.datetime_to_str, v))
```

### Comparing `pystac-1.8.4/pystac/errors.py` & `pystac-1.9.0/pystac/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 
 class TemplateError(Exception):
     """Exception thrown when an error occurs during converting a template
     string into data for :class:`~pystac.layout.LayoutTemplate`
     """
 
@@ -22,15 +22,15 @@
     """A STACTypeError is raised when encountering a representation of
     a STAC entity that is not correct for the context; for example, if
     a Catalog JSON was read in as an Item.
     """
 
     def __init__(
         self,
-        bad_dict: Dict[str, Any],
+        bad_dict: dict[str, Any],
         expected: type,
         extra_message: Optional[str] = "",
     ):
         """
         Construct an exception with an appropriate error message from bad_dict and the
         expected that it didn't align with.
```

### Comparing `pystac-1.8.4/pystac/extensions/classification.py` & `pystac-1.9.0/pystac/extensions/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Implements the :stac-ext:`Classification <classification>`."""
 
 from __future__ import annotations
 
 import re
+import warnings
+from collections.abc import Iterable
+from re import Pattern
 from typing import (
     Any,
-    Dict,
     Generic,
-    Iterable,
-    List,
-    Optional,
-    Pattern,
+    Literal,
     TypeVar,
     Union,
     cast,
 )
 
 import pystac
-import pystac.extensions.item_assets as item_assets
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.extensions.raster import RasterBand
@@ -30,15 +29,15 @@
 
 T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition, RasterBand)
 
 SCHEMA_URI_PATTERN: str = (
     "https://stac-extensions.github.io/classification/v{version}/schema.json"
 )
 DEFAULT_VERSION: str = "1.1.0"
-SUPPORTED_VERSIONS: List[str] = ["1.1.0", "1.0.0"]
+SUPPORTED_VERSIONS: list[str] = ["1.1.0", "1.0.0"]
 
 # Field names
 PREFIX: str = "classification:"
 BITFIELDS_PROP: str = PREFIX + "bitfields"
 CLASSES_PROP: str = PREFIX + "classes"
 RASTER_BANDS_PROP: str = "raster:bands"
 
@@ -47,25 +46,25 @@
 
 class Classification:
     """Represents a single category of a classification.
 
     Use Classification.create to create a new Classification.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     def apply(
         self,
         value: int,
         description: str,
-        name: Optional[str] = None,
-        color_hint: Optional[str] = None,
+        name: str | None = None,
+        color_hint: str | None = None,
     ) -> None:
         """
         Set the properties for a new Classification.
 
         Args:
             value: The integer value corresponding to this class
             description: The description of this class
@@ -92,16 +91,16 @@
             ), "Must format color hints as '^([0-9A-F]{6})$'"
 
     @classmethod
     def create(
         cls,
         value: int,
         description: str,
-        name: Optional[str] = None,
-        color_hint: Optional[str] = None,
+        name: str | None = None,
+        color_hint: str | None = None,
     ) -> Classification:
         """
         Create a new Classification.
 
         Args:
             value: The integer value corresponding to this class
             name: The human-readable short name for this class
@@ -142,53 +141,53 @@
         return get_required(self.properties.get("description"), self, "description")
 
     @description.setter
     def description(self, v: str) -> None:
         self.properties["description"] = v
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """Get or set the name of the class
 
         Returns:
             Optional[str]
         """
         return self.properties.get("name")
 
     @name.setter
-    def name(self, v: Optional[str]) -> None:
+    def name(self, v: str | None) -> None:
         if v is not None:
             self.properties["name"] = v
         else:
             self.properties.pop("name", None)
 
     @property
-    def color_hint(self) -> Optional[str]:
+    def color_hint(self) -> str | None:
         """Get or set the optional color hint for this class.
 
         The color hint must be a six-character string of capitalized hexadecimal
         characters ([0-9A-F]).
 
         Returns:
             Optional[str]
         """
-        return self.properties.get("color-hint")
+        return self.properties.get("color_hint")
 
     @color_hint.setter
-    def color_hint(self, v: Optional[str]) -> None:
+    def color_hint(self, v: str | None) -> None:
         if v is not None:
             match = COLOR_HINT_PATTERN.match(v)
             assert (
                 v is None or match is not None and match.group() == v
             ), "Must format color hints as '^([0-9A-F]{6})$'"
-            self.properties["color-hint"] = v
+            self.properties["color_hint"] = v
         else:
-            self.properties.pop("color-hint", None)
+            self.properties.pop("color_hint", None)
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns the dictionary encoding of this class
 
         Returns:
             dict: The serialization of the Classification
         """
         return self.properties
 
@@ -208,27 +207,27 @@
 
 class Bitfield:
     """Encodes the representation of values as bits in an integer.
 
     Use Bitfield.create to create a new Bitfield.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     def apply(
         self,
         offset: int,
         length: int,
-        classes: List[Classification],
-        roles: Optional[List[str]] = None,
-        description: Optional[str] = None,
-        name: Optional[str] = None,
+        classes: list[Classification],
+        roles: list[str] | None = None,
+        description: str | None = None,
+        name: str | None = None,
     ) -> None:
         """Sets the properties for this Bitfield.
 
         Args:
             offset: describes the position of the least significant bit captured
                 by this bitfield, with zero indicating the least significant binary
                 digit
@@ -255,18 +254,18 @@
         ), "When set, roles must contain at least one item"
 
     @classmethod
     def create(
         cls,
         offset: int,
         length: int,
-        classes: List[Classification],
-        roles: Optional[List[str]] = None,
-        description: Optional[str] = None,
-        name: Optional[str] = None,
+        classes: list[Classification],
+        roles: list[str] | None = None,
+        description: str | None = None,
+        name: str | None = None,
     ) -> Bitfield:
         """Sets the properties for this Bitfield.
 
         Args:
             offset: describes the position of the least significant bit captured
                 by this bitfield, with zero indicating the least significant binary
                 digit
@@ -315,95 +314,95 @@
         return get_required(self.properties.get("length"), self, "length")
 
     @length.setter
     def length(self, v: int) -> None:
         self.properties["length"] = v
 
     @property
-    def classes(self) -> List[Classification]:
+    def classes(self) -> list[Classification]:
         """Get or set the class definitions for the bitfield
 
         Returns:
             List[Classification]
         """
 
         return [
             Classification(d)
             for d in cast(
-                List[Dict[str, Any]],
+                list[dict[str, Any]],
                 get_required(
                     self.properties.get("classes"),
                     self,
                     "classes",
                 ),
             )
         ]
 
     @classes.setter
-    def classes(self, v: List[Classification]) -> None:
+    def classes(self, v: list[Classification]) -> None:
         self.properties["classes"] = [c.to_dict() for c in v]
 
     @property
-    def roles(self) -> Optional[List[str]]:
+    def roles(self) -> list[str] | None:
         """Get or set the role of the bitfield.
 
         See `Asset Roles
         <https://github.com/radiantearth/stac-spec/blob/master/item-spec/item-spec.md#asset-roles>`
 
         Returns:
             Optional[List[str]]
         """
         return self.properties.get("roles")
 
     @roles.setter
-    def roles(self, v: Optional[List[str]]) -> None:
+    def roles(self, v: list[str] | None) -> None:
         if v is not None:
             self.properties["roles"] = v
         else:
             self.properties.pop("roles", None)
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Get or set the optional description of a bitfield.
 
         Returns:
             Optional[str]
         """
         return self.properties.get("description")
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         if v is not None:
             self.properties["description"] = v
         else:
             self.properties.pop("description", None)
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """Get or set the optional name of the bitfield.
 
         Returns:
             Optional[str]
         """
         return self.properties.get("name")
 
     @name.setter
-    def name(self, v: Optional[str]) -> None:
+    def name(self, v: str | None) -> None:
         if v is not None:
             self.properties["name"] = v
         else:
             self.properties.pop("name", None)
 
     def __repr__(self) -> str:
         return (
             f"<Bitfield offset={self.offset} length={self.length} "
             f"classes={self.classes}>"
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns the dictionary encoding of this bitfield
 
         Returns:
             dict: The serialization of the Bitfield
         """
         return self.properties
 
@@ -421,21 +420,22 @@
     over the type of STAC object being extended.
 
     This class is not to be instantiated directly.  One can either directly use the
     subclass corresponding to the object you are extending, or the `ext` class
     method can be used to construct the proper class for you.
     """
 
-    properties: Dict[str, Any]
+    name: Literal["classification"] = "classification"
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
     def apply(
         self,
-        classes: Optional[List[Classification]] = None,
-        bitfields: Optional[List[Bitfield]] = None,
+        classes: list[Classification] | None = None,
+        bitfields: list[Bitfield] | None = None,
     ) -> None:
         """Applies the classifiation extension fields to the extended object.
 
         Note: one may set either the classes or bitfields objects, but not both.
 
         Args:
             classes: a list of
@@ -448,72 +448,76 @@
             or bitfields is None
             and classes is not None
         ), "Must set exactly one of `classes` or `bitfields`"
         self.classes = classes
         self.bitfields = bitfields
 
     @property
-    def classes(self) -> Optional[List[Classification]]:
+    def classes(self) -> list[Classification] | None:
         """Get or set the classes for the base object
 
         Note: Setting the classes will clear the object's bitfields if they are
         not None
 
         Returns:
             Optional[List[Classification]]
         """
         return self._get_classes()
 
     @classes.setter
-    def classes(self, v: Optional[List[Classification]]) -> None:
+    def classes(self, v: list[Classification] | None) -> None:
         if self._get_bitfields() is not None:
             self.bitfields = None
         self._set_property(
             CLASSES_PROP, map_opt(lambda classes: [c.to_dict() for c in classes], v)
         )
 
-    def _get_classes(self) -> Optional[List[Classification]]:
+    def _get_classes(self) -> list[Classification] | None:
         return map_opt(
             lambda classes: [Classification(c) for c in classes],
-            self._get_property(CLASSES_PROP, List[Dict[str, Any]]),
+            self._get_property(CLASSES_PROP, list[dict[str, Any]]),
         )
 
     @property
-    def bitfields(self) -> Optional[List[Bitfield]]:
+    def bitfields(self) -> list[Bitfield] | None:
         """Get or set the bitfields for the base object
 
         Note: Setting the bitfields will clear the object's classes if they are
         not None
 
         Returns:
             Optional[List[Bitfield]]
         """
         return self._get_bitfields()
 
     @bitfields.setter
-    def bitfields(self, v: Optional[List[Bitfield]]) -> None:
+    def bitfields(self, v: list[Bitfield] | None) -> None:
         if self._get_classes() is not None:
             self.classes = None
         self._set_property(
             BITFIELDS_PROP,
             map_opt(lambda bitfields: [b.to_dict() for b in bitfields], v),
         )
 
-    def _get_bitfields(self) -> Optional[List[Bitfield]]:
+    def _get_bitfields(self) -> list[Bitfield] | None:
         return map_opt(
             lambda bitfields: [Bitfield(b) for b in bitfields],
-            self._get_property(BITFIELDS_PROP, List[Dict[str, Any]]),
+            self._get_property(BITFIELDS_PROP, list[dict[str, Any]]),
         )
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI_PATTERN.format(version=DEFAULT_VERSION)
 
     @classmethod
-    def get_schema_uris(cls) -> List[str]:
+    def get_schema_uris(cls) -> list[str]:
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
         return [SCHEMA_URI_PATTERN.format(version=v) for v in SUPPORTED_VERSIONS]
 
     @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> ClassificationExtension[T]:
         """Extends the given STAC object with propertied from the
         :stac-ext:`Classification Extension <classification>`
 
@@ -522,59 +526,57 @@
         :class:`~pystac.extensions.item_assets.AssetDefinition`, or
         :class:`~pystac.extension.raster.RasterBand`.
 
         Raises:
             pystac.ExtensionTypeError : If an invalid object type is passed
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(ClassificationExtension[T], ItemClassificationExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(ClassificationExtension[T], AssetClassificationExtension(obj))
         elif isinstance(obj, item_assets.AssetDefinition):
-            cls.validate_has_extension(
-                cast(Union[pystac.Item, pystac.Collection], obj.owner), add_if_missing
-            )
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(
                 ClassificationExtension[T], ItemAssetsClassificationExtension(obj)
             )
         elif isinstance(obj, RasterBand):
             return cast(
                 ClassificationExtension[T], RasterBandClassificationExtension(obj)
             )
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesClassificationExtension:
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesClassificationExtension(obj)
 
 
 class ItemClassificationExtension(ClassificationExtension[pystac.Item]):
     item: pystac.Item
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
         return f"<ItemClassificationExtension Item id={self.item.id}>"
 
 
 class AssetClassificationExtension(ClassificationExtension[pystac.Asset]):
     asset: pystac.Asset
     asset_href: str
-    properties: Dict[str, Any]
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]]
+    properties: dict[str, Any]
+    additional_read_properties: Iterable[dict[str, Any]] | None
 
     def __init__(self, asset: pystac.Asset):
         self.asset = asset
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
@@ -582,70 +584,83 @@
     def __repr__(self) -> str:
         return f"<AssetClassificationExtension Asset href={self.asset_href}>"
 
 
 class ItemAssetsClassificationExtension(
     ClassificationExtension[item_assets.AssetDefinition]
 ):
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     asset_defn: item_assets.AssetDefinition
 
     def __init__(self, item_asset: item_assets.AssetDefinition):
         self.asset_defn = item_asset
         self.properties = item_asset.properties
 
     def __repr__(self) -> str:
         return f"<ItemAssetsClassificationExtension AssetDefinition={self.asset_defn}"
 
 
 class RasterBandClassificationExtension(ClassificationExtension[RasterBand]):
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     raster_band: RasterBand
 
     def __init__(self, raster_band: RasterBand):
         self.raster_band = raster_band
         self.properties = raster_band.properties
 
     def __repr__(self) -> str:
         return f"<RasterBandClassificationExtension RasterBand={self.raster_band}>"
 
 
 class SummariesClassificationExtension(SummariesExtension):
     @property
-    def classes(self) -> Optional[List[Classification]]:
+    def classes(self) -> list[Classification] | None:
         return map_opt(
             lambda classes: [Classification(c) for c in classes],
             self.summaries.get_list(CLASSES_PROP),
         )
 
     @classes.setter
-    def classes(self, v: Optional[List[Classification]]) -> None:
+    def classes(self, v: list[Classification] | None) -> None:
         self._set_summary(CLASSES_PROP, map_opt(lambda x: [c.to_dict() for c in x], v))
 
     @property
-    def bitfields(self) -> Optional[List[Bitfield]]:
+    def bitfields(self) -> list[Bitfield] | None:
         return map_opt(
             lambda bitfields: [Bitfield(b) for b in bitfields],
             self.summaries.get_list(BITFIELDS_PROP),
         )
 
     @bitfields.setter
-    def bitfields(self, v: Optional[List[Bitfield]]) -> None:
+    def bitfields(self, v: list[Bitfield] | None) -> None:
         self._set_summary(
             BITFIELDS_PROP, map_opt(lambda x: [b.to_dict() for b in x], v)
         )
 
 
 class ClassificationExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI_PATTERN.format(version=DEFAULT_VERSION)
-    prev_extension_ids = set(ClassificationExtension.get_schema_uris()) - set(
-        [ClassificationExtension.get_schema_uri()]
-    )
+    prev_extension_ids = {
+        SCHEMA_URI_PATTERN.format(version=v)
+        for v in SUPPORTED_VERSIONS
+        if v != DEFAULT_VERSION
+    }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
     def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
+        if SCHEMA_URI_PATTERN.format(version="1.0.0") in info.extensions:
+            for asset in obj.get("assets", {}).values():
+                classification_classes = asset.get(CLASSES_PROP, None)
+                if classification_classes is None or not isinstance(
+                    classification_classes, list
+                ):
+                    continue
+                for class_object in classification_classes:
+                    if "color-hint" in class_object:
+                        class_object["color_hint"] = class_object["color-hint"]
+                        del class_object["color-hint"]
         super().migrate(obj, version, info)
 
 
 CLASSIFICATION_EXTENSION_HOOKS: ExtensionHooks = ClassificationExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/datacube.py` & `pystac-1.9.0/pystac/extensions/datacube.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Implements the :stac-ext:`Datacube Extension <datacube>`."""
 
 from __future__ import annotations
 
 from abc import ABC
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, cast
+from typing import Any, Generic, Literal, TypeVar, Union, cast
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.utils import StringEnum, get_required, map_opt
 
-T = TypeVar("T", pystac.Collection, pystac.Item, pystac.Asset)
+T = TypeVar(
+    "T", pystac.Collection, pystac.Item, pystac.Asset, item_assets.AssetDefinition
+)
 
-SCHEMA_URI = "https://stac-extensions.github.io/datacube/v2.0.0/schema.json"
+SCHEMA_URI = "https://stac-extensions.github.io/datacube/v2.2.0/schema.json"
 
 PREFIX: str = "cube:"
 DIMENSIONS_PROP = PREFIX + "dimensions"
 VARIABLES_PROP = PREFIX + "variables"
 
 # Dimension properties
 DIM_TYPE_PROP = "type"
@@ -37,14 +40,15 @@
 VAR_UNIT_PROP = "unit"
 
 
 class DimensionType(StringEnum):
     """Dimension object types for spatial and temporal Dimension Objects."""
 
     SPATIAL = "spatial"
+    GEOMETRIES = "geometries"
     TEMPORAL = "temporal"
 
 
 class HorizontalSpatialDimensionAxis(StringEnum):
     """Allowed values for ``axis`` field of :class:`HorizontalSpatialDimension`
     object."""
 
@@ -61,126 +65,132 @@
 
 class Dimension(ABC):
     """Object representing a dimension of the datacube. The fields contained in
     Dimension Object vary by ``type``. See the :stac-ext:`Datacube Dimension Object
     <datacube#dimension-object>` docs for details.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     @property
-    def dim_type(self) -> Union[DimensionType, str]:
-        """The type of the dimension. Must be ``"spatial"`` for :stac-ext:`Horizontal
-        Spatial Dimension Objects <datacube#horizontal-spatial-dimension-object>` or
+    def dim_type(self) -> DimensionType | str:
+        """The type of the dimension. Must be ``"spatial"`` for
+        :stac-ext:`Horizontal Spatial Dimension Objects
+        <datacube#horizontal-raster-spatial-dimension-object>` or
         :stac-ext:`Vertical Spatial Dimension Objects
-        <datacube#vertical-spatial-dimension-object>`, and ``"temporal"`` for
-        :stac-ext:`Temporal Dimension Objects <datacube#temporal-dimension-object>`. May
-        be an arbitrary string for :stac-ext:`Additional Dimension Objects
+        <datacube#vertical-spatial-dimension-object>`, ``geometries`` for
+        :stac-ext:`Spatial Vector Dimension Objects
+        <datacube#spatial-vector-dimension-object>` ``"temporal"`` for
+        :stac-ext:`Temporal Dimension Objects
+        <datacube#temporal-dimension-object>`. May be an arbitrary string for
+        :stac-ext:`Additional Dimension Objects
         <datacube#additional-dimension-object>`."""
         return get_required(
             self.properties.get(DIM_TYPE_PROP), "cube:dimension", DIM_TYPE_PROP
         )
 
     @dim_type.setter
-    def dim_type(self, v: Union[DimensionType, str]) -> None:
+    def dim_type(self, v: DimensionType | str) -> None:
         self.properties[DIM_TYPE_PROP] = v
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Detailed multi-line description to explain the dimension. `CommonMark 0.29
         <http://commonmark.org/>`__ syntax MAY be used for rich text representation."""
         return self.properties.get(DIM_DESC_PROP)
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(DIM_DESC_PROP, None)
         else:
             self.properties[DIM_DESC_PROP] = v
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return self.properties
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> Dimension:
+    def from_dict(d: dict[str, Any]) -> Dimension:
         dim_type: str = get_required(
             d.get(DIM_TYPE_PROP), "cube_dimension", DIM_TYPE_PROP
         )
         if dim_type == DimensionType.SPATIAL:
             axis: str = get_required(
                 d.get(DIM_AXIS_PROP), "cube_dimension", DIM_AXIS_PROP
             )
             if axis == "z":
                 return VerticalSpatialDimension(d)
             else:
                 return HorizontalSpatialDimension(d)
+        elif dim_type == DimensionType.GEOMETRIES:
+            return VectorSpatialDimension(d)
         elif dim_type == DimensionType.TEMPORAL:
             # The v1.0.0 spec says that AdditionalDimensions can have
             # type 'temporal', but it is unclear how to differentiate that
             # from a temporal dimension. Just key off of type for now.
             # See https://github.com/stac-extensions/datacube/issues/5
             return TemporalDimension(d)
         else:
             return AdditionalDimension(d)
 
 
 class SpatialDimension(Dimension):
     @property
-    def extent(self) -> List[float]:
+    def extent(self) -> list[float]:
         """Extent (lower and upper bounds) of the dimension as two-dimensional array.
         Open intervals with ``None`` are not allowed."""
         return get_required(
             self.properties.get(DIM_EXTENT_PROP), "cube:dimension", DIM_EXTENT_PROP
         )
 
     @extent.setter
-    def extent(self, v: List[float]) -> None:
+    def extent(self, v: list[float]) -> None:
         self.properties[DIM_EXTENT_PROP] = v
 
     @property
-    def values(self) -> Optional[List[float]]:
+    def values(self) -> list[float] | None:
         """Optional set of all potential values."""
         return self.properties.get(DIM_VALUES_PROP)
 
     @values.setter
-    def values(self, v: Optional[List[float]]) -> None:
+    def values(self, v: list[float] | None) -> None:
         if v is None:
             self.properties.pop(DIM_VALUES_PROP, None)
         else:
             self.properties[DIM_VALUES_PROP] = v
 
     @property
-    def step(self) -> Optional[float]:
+    def step(self) -> float | None:
         """The space between the values. Use ``None`` for irregularly spaced steps."""
         return self.properties.get(DIM_STEP_PROP)
 
     @step.setter
-    def step(self, v: Optional[float]) -> None:
+    def step(self, v: float | None) -> None:
         self.properties[DIM_STEP_PROP] = v
 
     def clear_step(self) -> None:
         """Setting step to None sets it to the null value,
         which means irregularly spaced steps. Use clear_step
         to remove it from the properties."""
         self.properties.pop(DIM_STEP_PROP, None)
 
     @property
-    def reference_system(self) -> Optional[Union[str, float, Dict[str, Any]]]:
+    def reference_system(self) -> str | float | dict[str, Any] | None:
         """The spatial reference system for the data, specified as `numerical EPSG code
         <http://www.epsg-registry.org/>`__, `WKT2 (ISO 19162) string
         <http://docs.opengeospatial.org/is/18-010r7/18-010r7.html>`__ or `PROJJSON
         object <https://proj.org/specifications/projjson.html>`__.
         Defaults to EPSG code 4326."""
         return self.properties.get(DIM_REF_SYS_PROP)
 
     @reference_system.setter
-    def reference_system(self, v: Optional[Union[str, float, Dict[str, Any]]]) -> None:
+    def reference_system(self, v: str | float | dict[str, Any] | None) -> None:
         if v is None:
             self.properties.pop(DIM_REF_SYS_PROP, None)
         else:
             self.properties[DIM_REF_SYS_PROP] = v
 
 
 class HorizontalSpatialDimension(SpatialDimension):
@@ -205,141 +215,203 @@
         )
 
     @axis.setter
     def axis(self, v: VerticalSpatialDimensionAxis) -> None:
         self.properties[DIM_AXIS_PROP] = v
 
     @property
-    def unit(self) -> Optional[str]:
+    def unit(self) -> str | None:
         """The unit of measurement for the data, preferably compliant to `UDUNITS-2
         <https://ncics.org/portfolio/other-resources/udunits2/>`__ units (singular)."""
         return self.properties.get(DIM_UNIT_PROP)
 
     @unit.setter
-    def unit(self, v: Optional[str]) -> None:
+    def unit(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(DIM_UNIT_PROP, None)
         else:
             self.properties[DIM_UNIT_PROP] = v
 
 
+class VectorSpatialDimension(Dimension):
+    @property
+    def axes(self) -> list[str] | None:
+        """Axes of the vector dimension as an ordered set of `x`, `y` and `z`."""
+        return self.properties.get("axes")
+
+    @axes.setter
+    def axes(self, v: list[str]) -> None:
+        if v is None:
+            self.properties.pop("axes", None)
+        else:
+            self.properties["axes"] = v
+
+    @property
+    def bbox(self) -> list[float]:
+        """A single bounding box of the geometries as defined for STAC
+        Collections but not nested."""
+        return get_required(self.properties.get("bbox"), "cube:bbox", "bbox")
+
+    @bbox.setter
+    def bbox(self, v: list[float]) -> None:
+        self.properties["bbox"] = v
+
+    @property
+    def values(self) -> list[str] | None:
+        """Optionally, a representation of the geometries. This could be a list
+        of WKT strings or other identifiers."""
+        return self.properties.get(DIM_VALUES_PROP)
+
+    @values.setter
+    def values(self, v: list[str] | None) -> None:
+        if v is None:
+            self.properties.pop(DIM_VALUES_PROP, None)
+        else:
+            self.properties[DIM_VALUES_PROP] = v
+
+    @property
+    def geometry_types(self) -> list[str] | None:
+        """A set of geometry types. If not present, mixed geometry types must be
+        assumed."""
+        return self.properties.get("geometry_types")
+
+    @geometry_types.setter
+    def geometry_types(self, v: list[str] | None) -> None:
+        if v is None:
+            self.properties.pop("geometry_types", None)
+        else:
+            self.properties["geometry_types"] = v
+
+    @property
+    def reference_system(self) -> str | float | dict[str, Any] | None:
+        """The reference system for the data."""
+        return self.properties.get(DIM_REF_SYS_PROP)
+
+    @reference_system.setter
+    def reference_system(self, v: str | float | dict[str, Any] | None) -> None:
+        if v is None:
+            self.properties.pop(DIM_REF_SYS_PROP, None)
+        else:
+            self.properties[DIM_REF_SYS_PROP] = v
+
+
 class TemporalDimension(Dimension):
     @property
-    def extent(self) -> Optional[List[Optional[str]]]:
+    def extent(self) -> list[str | None] | None:
         """Extent (lower and upper bounds) of the dimension as two-dimensional array.
         The dates and/or times must be strings compliant to `ISO 8601
         <https://en.wikipedia.org/wiki/ISO_8601>`__. ``None`` is allowed for open date
         ranges."""
         return self.properties.get(DIM_EXTENT_PROP)
 
     @extent.setter
-    def extent(self, v: Optional[List[Optional[str]]]) -> None:
+    def extent(self, v: list[str | None] | None) -> None:
         if v is None:
             self.properties.pop(DIM_EXTENT_PROP, None)
         else:
             self.properties[DIM_EXTENT_PROP] = v
 
     @property
-    def values(self) -> Optional[List[str]]:
+    def values(self) -> list[str] | None:
         """If the dimension consists of set of specific values they can be listed here.
         The dates and/or times must be strings compliant to `ISO 8601
         <https://en.wikipedia.org/wiki/ISO_8601>`__."""
         return self.properties.get(DIM_VALUES_PROP)
 
     @values.setter
-    def values(self, v: Optional[List[str]]) -> None:
+    def values(self, v: list[str] | None) -> None:
         if v is None:
             self.properties.pop(DIM_VALUES_PROP, None)
         else:
             self.properties[DIM_VALUES_PROP] = v
 
     @property
-    def step(self) -> Optional[str]:
+    def step(self) -> str | None:
         """The space between the temporal instances as `ISO 8601 duration
         <https://en.wikipedia.org/wiki/ISO_8601#Durations>`__, e.g. P1D. Use null for
         irregularly spaced steps."""
         return self.properties.get(DIM_STEP_PROP)
 
     @step.setter
-    def step(self, v: Optional[str]) -> None:
+    def step(self, v: str | None) -> None:
         self.properties[DIM_STEP_PROP] = v
 
     def clear_step(self) -> None:
         """Setting step to None sets it to the null value,
         which means irregularly spaced steps. Use clear_step
         to remove it from the properties."""
         self.properties.pop(DIM_STEP_PROP, None)
 
 
 class AdditionalDimension(Dimension):
     @property
-    def extent(self) -> Optional[List[Optional[float]]]:
+    def extent(self) -> list[float | None] | None:
         """If the dimension consists of `ordinal
         <https://en.wikipedia.org/wiki/Level_of_measurement#Ordinal_scale>`__ values,
         the extent (lower and upper bounds) of the values as two-dimensional array. Use
         null for open intervals."""
         return self.properties.get(DIM_EXTENT_PROP)
 
     @extent.setter
-    def extent(self, v: Optional[List[Optional[float]]]) -> None:
+    def extent(self, v: list[float | None] | None) -> None:
         if v is None:
             self.properties.pop(DIM_EXTENT_PROP, None)
         else:
             self.properties[DIM_EXTENT_PROP] = v
 
     @property
-    def values(self) -> Optional[Union[List[str], List[float]]]:
+    def values(self) -> list[str] | list[float] | None:
         """A set of all potential values, especially useful for `nominal
         <https://en.wikipedia.org/wiki/Level_of_measurement#Nominal_level>`__ values."""
         return self.properties.get(DIM_VALUES_PROP)
 
     @values.setter
-    def values(self, v: Optional[Union[List[str], List[float]]]) -> None:
+    def values(self, v: list[str] | list[float] | None) -> None:
         if v is None:
             self.properties.pop(DIM_VALUES_PROP, None)
         else:
             self.properties[DIM_VALUES_PROP] = v
 
     @property
-    def step(self) -> Optional[float]:
+    def step(self) -> float | None:
         """If the dimension consists of `interval
         <https://en.wikipedia.org/wiki/Level_of_measurement#Interval_scale>`__ values,
         the space between the values. Use null for irregularly spaced steps."""
         return self.properties.get(DIM_STEP_PROP)
 
     @step.setter
-    def step(self, v: Optional[float]) -> None:
+    def step(self, v: float | None) -> None:
         self.properties[DIM_STEP_PROP] = v
 
     def clear_step(self) -> None:
         """Setting step to None sets it to the null value,
         which means irregularly spaced steps. Use clear_step
         to remove it from the properties."""
         self.properties.pop(DIM_STEP_PROP, None)
 
     @property
-    def unit(self) -> Optional[str]:
+    def unit(self) -> str | None:
         """The unit of measurement for the data, preferably compliant to `UDUNITS-2
         units <https://ncics.org/portfolio/other-resources/udunits2/>`__ (singular)."""
         return self.properties.get(DIM_UNIT_PROP)
 
     @unit.setter
-    def unit(self, v: Optional[str]) -> None:
+    def unit(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(DIM_UNIT_PROP, None)
         else:
             self.properties[DIM_UNIT_PROP] = v
 
     @property
-    def reference_system(self) -> Optional[Union[str, float, Dict[str, Any]]]:
+    def reference_system(self) -> str | float | dict[str, Any] | None:
         """The reference system for the data."""
         return self.properties.get(DIM_REF_SYS_PROP)
 
     @reference_system.setter
-    def reference_system(self, v: Optional[Union[str, float, Dict[str, Any]]]) -> None:
+    def reference_system(self, v: str | float | dict[str, Any] | None) -> None:
         if v is None:
             self.properties.pop(DIM_REF_SYS_PROP, None)
         else:
             self.properties[DIM_REF_SYS_PROP] = v
 
 
 class VariableType(StringEnum):
@@ -352,104 +424,104 @@
 class Variable:
     """Object representing a variable in the datacube. The dimensions field lists
     zero or more :stac-ext:`Datacube Dimension Object <datacube#dimension-object>`
     instances. See the :stac-ext:`Datacube Variable Object
     <datacube#variable-object>` docs for details.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     @property
-    def dimensions(self) -> List[str]:
+    def dimensions(self) -> list[str]:
         """The dimensions of the variable. Should refer to keys in the
         ``cube:dimensions`` object or be an empty list if the variable has no
         dimensions
         """
         return get_required(
             self.properties.get(VAR_DIMENSIONS_PROP),
             "cube:variable",
             VAR_DIMENSIONS_PROP,
         )
 
     @dimensions.setter
-    def dimensions(self, v: List[str]) -> None:
+    def dimensions(self, v: list[str]) -> None:
         self.properties[VAR_DIMENSIONS_PROP] = v
 
     @property
-    def var_type(self) -> Union[VariableType, str]:
+    def var_type(self) -> VariableType | str:
         """Type of the variable, either ``data`` or ``auxiliary``"""
         return get_required(
             self.properties.get(VAR_TYPE_PROP), "cube:variable", VAR_TYPE_PROP
         )
 
     @var_type.setter
-    def var_type(self, v: Union[VariableType, str]) -> None:
+    def var_type(self, v: VariableType | str) -> None:
         self.properties[VAR_TYPE_PROP] = v
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Detailed multi-line description to explain the variable. `CommonMark 0.29
         <http://commonmark.org/>`__ syntax MAY be used for rich text representation."""
         return self.properties.get(VAR_DESC_PROP)
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(VAR_DESC_PROP, None)
         else:
             self.properties[VAR_DESC_PROP] = v
 
     @property
-    def extent(self) -> List[Union[float, str, None]]:
+    def extent(self) -> list[float | str | None]:
         """If the variable consists of `ordinal values
         <https://en.wikipedia.org/wiki/Level_of_measurement#Ordinal_scale>`, the extent
         (lower and upper bounds) of the values as two-dimensional array. Use ``None``
         for open intervals"""
         return get_required(
             self.properties.get(VAR_EXTENT_PROP), "cube:variable", VAR_EXTENT_PROP
         )
 
     @extent.setter
-    def extent(self, v: List[Union[float, str, None]]) -> None:
+    def extent(self, v: list[float | str | None]) -> None:
         self.properties[VAR_EXTENT_PROP] = v
 
     @property
-    def values(self) -> Optional[List[Union[float, str]]]:
+    def values(self) -> list[float | str] | None:
         """A set of all potential values, especially useful for `nominal values
         <https://en.wikipedia.org/wiki/Level_of_measurement#Nominal_level>`."""
         return self.properties.get(VAR_VALUES_PROP)
 
     @values.setter
-    def values(self, v: Optional[List[Union[float, str]]]) -> None:
+    def values(self, v: list[float | str] | None) -> None:
         if v is None:
             self.properties.pop(VAR_VALUES_PROP)
         else:
             self.properties[VAR_VALUES_PROP] = v
 
     @property
-    def unit(self) -> Optional[str]:
+    def unit(self) -> str | None:
         """The unit of measurement for the data, preferably compliant to `UDUNITS-2
         <https://ncics.org/portfolio/other-resources/udunits2/>` units (singular)"""
         return self.properties.get(VAR_UNIT_PROP)
 
     @unit.setter
-    def unit(self, v: Optional[str]) -> None:
+    def unit(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(VAR_UNIT_PROP)
         else:
             self.properties[VAR_UNIT_PROP] = v
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> Variable:
+    def from_dict(d: dict[str, Any]) -> Variable:
         return Variable(d)
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return self.properties
 
 
 class DatacubeExtension(
     Generic[T],
     PropertiesExtension,
     ExtensionManagementMixin[Union[pystac.Collection, pystac.Item]],
@@ -465,58 +537,60 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> dc_ext = DatacubeExtension.ext(item)
     """
 
+    name: Literal["cube"] = "cube"
+
     def apply(
         self,
-        dimensions: Dict[str, Dimension],
-        variables: Optional[Dict[str, Variable]] = None,
+        dimensions: dict[str, Dimension],
+        variables: dict[str, Variable] | None = None,
     ) -> None:
         """Applies Datacube Extension properties to the extended
         :class:`~pystac.Collection`, :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Args:
             dimensions : Dictionary mapping dimension name to :class:`Dimension`
                 objects.
             variables : Dictionary mapping variable name to a :class:`Variable`
                 object.
         """
         self.dimensions = dimensions
         self.variables = variables
 
     @property
-    def dimensions(self) -> Dict[str, Dimension]:
+    def dimensions(self) -> dict[str, Dimension]:
         """A dictionary where each key is the name of a dimension and each
         value is a :class:`~Dimension` object.
         """
         result = get_required(
-            self._get_property(DIMENSIONS_PROP, Dict[str, Any]), self, DIMENSIONS_PROP
+            self._get_property(DIMENSIONS_PROP, dict[str, Any]), self, DIMENSIONS_PROP
         )
         return {k: Dimension.from_dict(v) for k, v in result.items()}
 
     @dimensions.setter
-    def dimensions(self, v: Dict[str, Dimension]) -> None:
+    def dimensions(self, v: dict[str, Dimension]) -> None:
         self._set_property(DIMENSIONS_PROP, {k: dim.to_dict() for k, dim in v.items()})
 
     @property
-    def variables(self) -> Optional[Dict[str, Variable]]:
+    def variables(self) -> dict[str, Variable] | None:
         """A dictionary where each key is the name of a variable and each
         value is a :class:`~Variable` object.
         """
-        result = self._get_property(VARIABLES_PROP, Dict[str, Any])
+        result = self._get_property(VARIABLES_PROP, dict[str, Any])
 
         if result is None:
             return None
         return {k: Variable.from_dict(v) for k, v in result.items()}
 
     @variables.setter
-    def variables(self, v: Optional[Dict[str, Variable]]) -> None:
+    def variables(self, v: dict[str, Variable] | None) -> None:
         self._set_property(
             VARIABLES_PROP,
             map_opt(
                 lambda variables: {k: var.to_dict() for k, var in variables.items()}, v
             ),
         )
 
@@ -533,94 +607,111 @@
         :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Collection):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(DatacubeExtension[T], CollectionDatacubeExtension(obj))
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(DatacubeExtension[T], ItemDatacubeExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(DatacubeExtension[T], AssetDatacubeExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(DatacubeExtension[T], ItemAssetsDatacubeExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class CollectionDatacubeExtension(DatacubeExtension[pystac.Collection]):
     """A concrete implementation of :class:`DatacubeExtension` on an
     :class:`~pystac.Collection` that extends the properties of the Item to include
     properties defined in the :stac-ext:`Datacube Extension <datacube>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`DatacubeExtension.ext` on an :class:`~pystac.Collection` to extend it.
     """
 
     collection: pystac.Collection
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, collection: pystac.Collection):
         self.collection = collection
         self.properties = collection.extra_fields
 
     def __repr__(self) -> str:
-        return "<CollectionDatacubeExtension Item id={}>".format(self.collection.id)
+        return f"<CollectionDatacubeExtension Item id={self.collection.id}>"
 
 
 class ItemDatacubeExtension(DatacubeExtension[pystac.Item]):
     """A concrete implementation of :class:`DatacubeExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`Datacube Extension <datacube>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`DatacubeExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemDatacubeExtension Item id={}>".format(self.item.id)
+        return f"<ItemDatacubeExtension Item id={self.item.id}>"
 
 
 class AssetDatacubeExtension(DatacubeExtension[pystac.Asset]):
     """A concrete implementation of :class:`DatacubeExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties defined
     in the :stac-ext:`Datacube Extension <datacube>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`EOExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
-    properties: Dict[str, Any]
-    additional_read_properties: Optional[List[Dict[str, Any]]]
+    properties: dict[str, Any]
+    additional_read_properties: list[dict[str, Any]] | None
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
         else:
             self.additional_read_properties = None
 
     def __repr__(self) -> str:
-        return "<AssetDatacubeExtension Item id={}>".format(self.asset_href)
+        return f"<AssetDatacubeExtension Item id={self.asset_href}>"
+
+
+class ItemAssetsDatacubeExtension(DatacubeExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
 
 class DatacubeExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"datacube"}
+    prev_extension_ids = {
+        "datacube",
+        "https://stac-extensions.github.io/datacube/v1.0.0/schema.json",
+        "https://stac-extensions.github.io/datacube/v2.0.0/schema.json",
+        "https://stac-extensions.github.io/datacube/v2.1.0/schema.json",
+    }
     stac_object_types = {
         pystac.STACObjectType.COLLECTION,
         pystac.STACObjectType.ITEM,
     }
 
 
 DATACUBE_EXTENSION_HOOKS: ExtensionHooks = DatacubeExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/eo.py` & `pystac-1.9.0/pystac/extensions/raster.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,670 +1,820 @@
-"""Implements the :stac-ext:`Electro-Optical Extension <eo>`."""
+"""Implements the :stac-ext:`Raster Extension <raster>`."""
 
 from __future__ import annotations
 
+import warnings
+from collections.abc import Iterable
 from typing import (
     Any,
-    Dict,
     Generic,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
+    Literal,
     TypeVar,
     Union,
     cast,
 )
 
 import pystac
-from pystac.extensions import projection, view
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
-from pystac.serialization.identify import STACJSONDescription, STACVersionID
-from pystac.summaries import RangeSummary
-from pystac.utils import get_required, map_opt
-
-T = TypeVar("T", pystac.Item, pystac.Asset)
-
-SCHEMA_URI: str = "https://stac-extensions.github.io/eo/v1.1.0/schema.json"
-SCHEMA_URIS: List[str] = [
-    "https://stac-extensions.github.io/eo/v1.0.0/schema.json",
+from pystac.utils import StringEnum, get_opt, get_required, map_opt
+
+T = TypeVar("T", pystac.Asset, item_assets.AssetDefinition)
+
+SCHEMA_URI = "https://stac-extensions.github.io/raster/v1.1.0/schema.json"
+SCHEMA_URIS = [
+    "https://stac-extensions.github.io/raster/v1.0.0/schema.json",
     SCHEMA_URI,
 ]
-PREFIX: str = "eo:"
+SCHEMA_STARTWITH = "https://stac-extensions.github.io/raster/"
+BANDS_PROP = "raster:bands"
+
+
+class Sampling(StringEnum):
+    AREA = "area"
+    POINT = "point"
+
+
+class DataType(StringEnum):
+    INT8 = "int8"
+    INT16 = "int16"
+    INT32 = "int32"
+    INT64 = "int64"
+    UINT8 = "uint8"
+    UINT16 = "uint16"
+    UINT32 = "uint32"
+    UINT64 = "uint64"
+    FLOAT16 = "float16"
+    FLOAT32 = "float32"
+    FLOAT64 = "float64"
+    CINT16 = "cint16"
+    CINT32 = "cint32"
+    CFLOAT32 = "cfloat32"
+    CFLOAT64 = "cfloat64"
+    OTHER = "other"
+
+
+class NoDataStrings(StringEnum):
+    INF = "inf"
+    NINF = "-inf"
+    NAN = "nan"
+
+
+class Statistics:
+    """Represents statistics information attached to a band in the raster extension.
+
+    Use Statistics.create to create a new Statistics instance.
+    """
+
+    properties: dict[str, Any]
+
+    def __init__(self, properties: dict[str, float | None]) -> None:
+        self.properties = properties
+
+    def apply(
+        self,
+        minimum: float | None = None,
+        maximum: float | None = None,
+        mean: float | None = None,
+        stddev: float | None = None,
+        valid_percent: float | None = None,
+    ) -> None:
+        """
+        Sets the properties for this raster Band.
+
+        Args:
+            minimum : Minimum value of all the pixels in the band.
+            maximum : Maximum value of all the pixels in the band.
+            mean : Mean value of all the pixels in the band.
+            stddev : Standard Deviation value of all the pixels in the band.
+            valid_percent : Percentage of valid (not nodata) pixel.
+        """
+        self.minimum = minimum
+        self.maximum = maximum
+        self.mean = mean
+        self.stddev = stddev
+        self.valid_percent = valid_percent
+
+    @classmethod
+    def create(
+        cls,
+        minimum: float | None = None,
+        maximum: float | None = None,
+        mean: float | None = None,
+        stddev: float | None = None,
+        valid_percent: float | None = None,
+    ) -> Statistics:
+        """
+        Creates a new band.
+
+        Args:
+            minimum : Minimum value of all the pixels in the band.
+            maximum : Maximum value of all the pixels in the band.
+            mean : Mean value of all the pixels in the band.
+            stddev : Standard Deviation value of all the pixels in the band.
+            valid_percent : Percentage of valid (not nodata) pixel.
+        """
+        b = cls({})
+        b.apply(
+            minimum=minimum,
+            maximum=maximum,
+            mean=mean,
+            stddev=stddev,
+            valid_percent=valid_percent,
+        )
+        return b
+
+    @property
+    def minimum(self) -> float | None:
+        """Get or sets the minimum pixel value
+
+        Returns:
+            Optional[float]
+        """
+        return self.properties.get("minimum")
+
+    @minimum.setter
+    def minimum(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["minimum"] = v
+        else:
+            self.properties.pop("minimum", None)
+
+    @property
+    def maximum(self) -> float | None:
+        """Get or sets the maximum pixel value
+
+        Returns:
+            Optional[float]
+        """
+        return self.properties.get("maximum")
+
+    @maximum.setter
+    def maximum(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["maximum"] = v
+        else:
+            self.properties.pop("maximum", None)
+
+    @property
+    def mean(self) -> float | None:
+        """Get or sets the mean pixel value
+
+        Returns:
+            Optional[float]
+        """
+        return self.properties.get("mean")
+
+    @mean.setter
+    def mean(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["mean"] = v
+        else:
+            self.properties.pop("mean", None)
+
+    @property
+    def stddev(self) -> float | None:
+        """Get or sets the standard deviation pixel value
+
+        Returns:
+            Optional[float]
+        """
+        return self.properties.get("stddev")
+
+    @stddev.setter
+    def stddev(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["stddev"] = v
+        else:
+            self.properties.pop("stddev", None)
+
+    @property
+    def valid_percent(self) -> float | None:
+        """Get or sets the Percentage of valid (not nodata) pixel
+
+        Returns:
+            Optional[float]
+        """
+        return self.properties.get("valid_percent")
+
+    @valid_percent.setter
+    def valid_percent(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["valid_percent"] = v
+        else:
+            self.properties.pop("valid_percent", None)
+
+    def to_dict(self) -> dict[str, Any]:
+        """Returns these statistics as a dictionary.
+
+        Returns:
+            dict: The serialization of the Statistics.
+        """
+        return self.properties
+
+    @staticmethod
+    def from_dict(d: dict[str, Any]) -> Statistics:
+        """Constructs an Statistics from a dict.
+
+        Returns:
+            Statistics: The Statistics deserialized from the JSON dict.
+        """
+        return Statistics(properties=d)
+
+
+class Histogram:
+    """Represents pixel distribution information attached to a band in the raster
+    extension.
+
+    Use Band.create to create a new Band.
+    """
+
+    properties: dict[str, Any]
+
+    def __init__(self, properties: dict[str, Any]) -> None:
+        self.properties = properties
+
+    def apply(
+        self,
+        count: int,
+        min: float,
+        max: float,
+        buckets: list[int],
+    ) -> None:
+        """
+        Sets the properties for this raster Band.
+
+        Args:
+            count : number of buckets of the distribution.
+            min : minimum value of the distribution.
+                Also the mean value of the first bucket.
+            max : maximum value of the distribution.
+                Also the mean value of the last bucket.
+            buckets : Array of integer indicating the number
+                of pixels included in the bucket.
+        """
+        self.count = count
+        self.min = min
+        self.max = max
+        self.buckets = buckets
+
+    @classmethod
+    def create(
+        cls,
+        count: int,
+        min: float,
+        max: float,
+        buckets: list[int],
+    ) -> Histogram:
+        """
+        Creates a new band.
+
+        Args:
+            count : number of buckets of the distribution.
+            min : minimum value of the distribution.
+                Also the mean value of the first bucket.
+            max : maximum value of the distribution.
+                Also the mean value of the last bucket.
+            buckets : Array of integer indicating the number
+                of pixels included in the bucket.
+        """
+        b = cls({})
+        b.apply(
+            count=count,
+            min=min,
+            max=max,
+            buckets=buckets,
+        )
+        return b
+
+    @property
+    def count(self) -> int:
+        """Get or sets the number of buckets of the distribution.
+
+        Returns:
+            int
+        """
+        return get_required(self.properties.get("count"), self, "count")
+
+    @count.setter
+    def count(self, v: int) -> None:
+        self.properties["count"] = v
+
+    @property
+    def min(self) -> float:
+        """Get or sets the minimum value of the distribution.
+
+        Returns:
+            float
+        """
+        return get_required(self.properties.get("min"), self, "min")
 
-# Field names
-BANDS_PROP: str = PREFIX + "bands"
-CLOUD_COVER_PROP: str = PREFIX + "cloud_cover"
-SNOW_COVER_PROP: str = PREFIX + "snow_cover"
+    @min.setter
+    def min(self, v: float) -> None:
+        self.properties["min"] = v
 
+    @property
+    def max(self) -> float:
+        """Get or sets the maximum value of the distribution.
+
+        Returns:
+            float
+        """
+        return get_required(self.properties.get("max"), self, "max")
+
+    @max.setter
+    def max(self, v: float) -> None:
+        self.properties["max"] = v
+
+    @property
+    def buckets(self) -> list[int]:
+        """Get or sets the Array of integer indicating
+        the number of pixels included in the bucket.
+
+        Returns:
+            List[int]
+        """
+        return get_required(self.properties.get("buckets"), self, "buckets")
+
+    @buckets.setter
+    def buckets(self, v: list[int]) -> None:
+        self.properties["buckets"] = v
+
+    def to_dict(self) -> dict[str, Any]:
+        """Returns this histogram as a dictionary.
+
+        Returns:
+            dict: The serialization of the Histogram.
+        """
+        return self.properties
+
+    @staticmethod
+    def from_dict(d: dict[str, Any]) -> Histogram:
+        """Constructs an Histogram from a dict.
 
-def validated_percentage(v: Optional[float]) -> Optional[float]:
-    if v is not None and not isinstance(v, (float, int)) or isinstance(v, bool):
-        raise ValueError(f"Invalid percentage: {v} must be number")
-    if v is not None and not 0 <= v <= 100:
-        raise ValueError(f"Invalid percentage: {v} must be between 0 and 100")
-    return v
+        Returns:
+            Histogram: The Histogram deserialized from the JSON dict.
+        """
+        return Histogram(properties=d)
 
 
-class Band:
-    """Represents Band information attached to an Item that implements the eo extension.
+class RasterBand:
+    """Represents a Raster Band information attached to an Item
+    that implements the raster extension.
 
-    Use :meth:`Band.create` to create a new Band.
+    Use Band.create to create a new Band.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     def apply(
         self,
-        name: str,
-        common_name: Optional[str] = None,
-        description: Optional[str] = None,
-        center_wavelength: Optional[float] = None,
-        full_width_half_max: Optional[float] = None,
-        solar_illumination: Optional[float] = None,
+        nodata: float | NoDataStrings | None = None,
+        sampling: Sampling | None = None,
+        data_type: DataType | None = None,
+        bits_per_sample: float | None = None,
+        spatial_resolution: float | None = None,
+        statistics: Statistics | None = None,
+        unit: str | None = None,
+        scale: float | None = None,
+        offset: float | None = None,
+        histogram: Histogram | None = None,
     ) -> None:
         """
-        Sets the properties for this Band.
+        Sets the properties for this raster Band.
 
         Args:
-            name : The name of the band (e.g., "B01", "B02", "B1", "B5", "QA").
-            common_name : The name commonly used to refer to the band to make it
-                easier to search for bands across instruments. See the :stac-ext:`list
-                of accepted common names <eo#common-band-names>`.
-            description : Description to fully explain the band.
-            center_wavelength : The center wavelength of the band, in micrometers (μm).
-            full_width_half_max : Full width at half maximum (FWHM). The width of the
-                band, as measured at half the maximum transmission, in micrometers (μm).
-            solar_illumination: The solar illumination of the band,
-                as measured at half the maximum transmission, in W/m2/micrometers.
-        """
-        self.name = name
-        self.common_name = common_name
-        self.description = description
-        self.center_wavelength = center_wavelength
-        self.full_width_half_max = full_width_half_max
-        self.solar_illumination = solar_illumination
+            nodata : Pixel values used to identify pixels that are nodata in the assets.
+            sampling : One of area or point. Indicates whether a pixel value should be
+                assumed to represent a sampling over the region of the pixel or a point
+                sample at the center of the pixel.
+            data_type :The data type of the band.
+                One of the data types as described in the
+                :stac-ext:`Raster Data Types <raster/#data-types> docs`.
+            bits_per_sample : The actual number of bits used for this band.
+                Normally only present when the number of bits is non-standard for the
+                datatype, such as when a 1 bit TIFF is represented as byte
+            spatial_resolution : Average spatial resolution (in meters) of the pixels in
+                the band.
+            statistics: Statistics of all the pixels in the band
+            unit: unit denomination of the pixel value
+            scale: multiplicator factor of the pixel value to transform into the value
+                (i.e. translate digital number to reflectance).
+            offset: number to be added to the pixel value (after scaling) to transform
+                into the value (i.e. translate digital number to reflectance).
+            histogram: Histogram distribution information of the pixels values in the
+                band
+        """
+        self.nodata = nodata
+        self.sampling = sampling
+        self.data_type = data_type
+        self.bits_per_sample = bits_per_sample
+        self.spatial_resolution = spatial_resolution
+        self.statistics = statistics
+        self.unit = unit
+        self.scale = scale
+        self.offset = offset
+        self.histogram = histogram
 
     @classmethod
     def create(
         cls,
-        name: str,
-        common_name: Optional[str] = None,
-        description: Optional[str] = None,
-        center_wavelength: Optional[float] = None,
-        full_width_half_max: Optional[float] = None,
-        solar_illumination: Optional[float] = None,
-    ) -> Band:
+        nodata: float | NoDataStrings | None = None,
+        sampling: Sampling | None = None,
+        data_type: DataType | None = None,
+        bits_per_sample: float | None = None,
+        spatial_resolution: float | None = None,
+        statistics: Statistics | None = None,
+        unit: str | None = None,
+        scale: float | None = None,
+        offset: float | None = None,
+        histogram: Histogram | None = None,
+    ) -> RasterBand:
         """
         Creates a new band.
 
         Args:
-            name : The name of the band (e.g., "B01", "B02", "B1", "B5", "QA").
-            common_name : The name commonly used to refer to the band to make it easier
-                to search for bands across instruments. See the :stac-ext:`list of
-                accepted common names <eo#common-band-names>`.
-            description : Description to fully explain the band.
-            center_wavelength : The center wavelength of the band, in micrometers (μm).
-            full_width_half_max : Full width at half maximum (FWHM). The width of the
-                band, as measured at half the maximum transmission, in micrometers (μm).
-            solar_illumination: The solar illumination of the band,
-                as measured at half the maximum transmission, in W/m2/micrometers.
+            nodata : Pixel values used to identify pixels that are nodata in the assets.
+            sampling : One of area or point. Indicates whether a pixel value should be
+                assumed to represent a sampling over the region of the pixel or a point
+                sample at the center of the pixel.
+            data_type :The data type of the band.
+                One of the data types as described in the
+                :stac-ext:`Raster Data Types <raster/#data-types> docs`.
+            bits_per_sample : The actual number of bits used for this band.
+                Normally only present when the number of bits is non-standard for the
+                datatype, such as when a 1 bit TIFF is represented as byte
+            spatial_resolution : Average spatial resolution (in meters) of the pixels in
+                the band.
+            statistics: Statistics of all the pixels in the band
+            unit: unit denomination of the pixel value
+            scale: multiplicator factor of the pixel value to transform into the value
+                (i.e. translate digital number to reflectance).
+            offset: number to be added to the pixel value (after scaling) to transform
+                into the value (i.e. translate digital number to reflectance).
+            histogram: Histogram distribution information of the pixels values in the
+                band
         """
         b = cls({})
         b.apply(
-            name=name,
-            common_name=common_name,
-            description=description,
-            center_wavelength=center_wavelength,
-            full_width_half_max=full_width_half_max,
-            solar_illumination=solar_illumination,
+            nodata=nodata,
+            sampling=sampling,
+            data_type=data_type,
+            bits_per_sample=bits_per_sample,
+            spatial_resolution=spatial_resolution,
+            statistics=statistics,
+            unit=unit,
+            scale=scale,
+            offset=offset,
+            histogram=histogram,
         )
         return b
 
     @property
-    def name(self) -> str:
-        """Get or sets the name of the band (e.g., "B01", "B02", "B1", "B5", "QA").
+    def nodata(self) -> float | NoDataStrings | None:
+        """Get or sets the nodata pixel value
 
         Returns:
-            str
+            Optional[float]
         """
-        return get_required(self.properties.get("name"), self, "name")
+        return self.properties.get("nodata")
 
-    @name.setter
-    def name(self, v: str) -> None:
-        self.properties["name"] = v
+    @nodata.setter
+    def nodata(self, v: float | NoDataStrings | None) -> None:
+        if v is not None:
+            self.properties["nodata"] = v
+        else:
+            self.properties.pop("nodata", None)
 
     @property
-    def common_name(self) -> Optional[str]:
-        """Get or sets the name commonly used to refer to the band to make it easier
-            to search for bands across instruments. See the :stac-ext:`list of accepted
-            common names <eo#common-band-names>`.
+    def sampling(self) -> Sampling | None:
+        """Get or sets the property indicating whether a pixel value should be assumed
+        to represent a sampling over the region of the pixel or a point sample
+        at the center of the pixel.
 
         Returns:
-            Optional[str]
+            Optional[Sampling]
         """
-        return self.properties.get("common_name")
+        return self.properties.get("sampling")
 
-    @common_name.setter
-    def common_name(self, v: Optional[str]) -> None:
+    @sampling.setter
+    def sampling(self, v: Sampling | None) -> None:
         if v is not None:
-            self.properties["common_name"] = v
+            self.properties["sampling"] = v
         else:
-            self.properties.pop("common_name", None)
+            self.properties.pop("sampling", None)
 
     @property
-    def description(self) -> Optional[str]:
-        """Get or sets the description to fully explain the band. CommonMark 0.29
-        syntax MAY be used for rich text representation.
+    def data_type(self) -> DataType | None:
+        """Get or sets the data type of the band.
 
         Returns:
-            str
+            Optional[DataType]
         """
-        return self.properties.get("description")
+        return self.properties.get("data_type")
 
-    @description.setter
-    def description(self, v: Optional[str]) -> None:
+    @data_type.setter
+    def data_type(self, v: DataType | None) -> None:
         if v is not None:
-            self.properties["description"] = v
+            self.properties["data_type"] = v
         else:
-            self.properties.pop("description", None)
+            self.properties.pop("data_type", None)
 
     @property
-    def center_wavelength(self) -> Optional[float]:
-        """Get or sets the center wavelength of the band, in micrometers (μm).
+    def bits_per_sample(self) -> float | None:
+        """Get or sets the actual number of bits used for this band.
 
         Returns:
             float
         """
-        return self.properties.get("center_wavelength")
+        return self.properties.get("bits_per_sample")
 
-    @center_wavelength.setter
-    def center_wavelength(self, v: Optional[float]) -> None:
+    @bits_per_sample.setter
+    def bits_per_sample(self, v: float | None) -> None:
         if v is not None:
-            self.properties["center_wavelength"] = v
+            self.properties["bits_per_sample"] = v
         else:
-            self.properties.pop("center_wavelength", None)
+            self.properties.pop("bits_per_sample", None)
 
     @property
-    def full_width_half_max(self) -> Optional[float]:
-        """Get or sets the full width at half maximum (FWHM). The width of the band,
-            as measured at half the maximum transmission, in micrometers (μm).
+    def spatial_resolution(self) -> float | None:
+        """Get or sets the average spatial resolution (in meters) of the pixels in the
+        band.
 
         Returns:
             [float]
         """
-        return self.properties.get("full_width_half_max")
+        return self.properties.get("spatial_resolution")
 
-    @full_width_half_max.setter
-    def full_width_half_max(self, v: Optional[float]) -> None:
+    @spatial_resolution.setter
+    def spatial_resolution(self, v: float | None) -> None:
         if v is not None:
-            self.properties["full_width_half_max"] = v
+            self.properties["spatial_resolution"] = v
         else:
-            self.properties.pop("full_width_half_max", None)
+            self.properties.pop("spatial_resolution", None)
 
     @property
-    def solar_illumination(self) -> Optional[float]:
-        """Get or sets the solar illumination of the band,
-            as measured at half the maximum transmission, in W/m2/micrometers.
+    def statistics(self) -> Statistics | None:
+        """Get or sets the average spatial resolution (in meters) of the pixels in the
+        band.
 
         Returns:
-            [float]
+            [Statistics]
         """
-        return self.properties.get("solar_illumination")
+        return Statistics.from_dict(get_opt(self.properties.get("statistics")))
 
-    @solar_illumination.setter
-    def solar_illumination(self, v: Optional[float]) -> None:
+    @statistics.setter
+    def statistics(self, v: Statistics | None) -> None:
         if v is not None:
-            self.properties["solar_illumination"] = v
+            self.properties["statistics"] = v.to_dict()
         else:
-            self.properties.pop("solar_illumination", None)
+            self.properties.pop("statistics", None)
 
-    def __repr__(self) -> str:
-        return "<Band name={}>".format(self.name)
+    @property
+    def unit(self) -> str | None:
+        """Get or sets the unit denomination of the pixel value
 
-    def to_dict(self) -> Dict[str, Any]:
-        """Returns this band as a dictionary.
+        Returns:
+            [str]
+        """
+        return self.properties.get("unit")
+
+    @unit.setter
+    def unit(self, v: str | None) -> None:
+        if v is not None:
+            self.properties["unit"] = v
+        else:
+            self.properties.pop("unit", None)
+
+    @property
+    def scale(self) -> float | None:
+        """Get or sets the multiplicator factor of the pixel value to transform
+        into the value (i.e. translate digital number to reflectance).
 
         Returns:
-            dict: The serialization of this Band.
+            [float]
         """
-        return self.properties
+        return self.properties.get("scale")
 
-    @staticmethod
-    def band_range(common_name: str) -> Optional[Tuple[float, float]]:
-        """Gets the band range for a common band name.
+    @scale.setter
+    def scale(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["scale"] = v
+        else:
+            self.properties.pop("scale", None)
 
-        Args:
-            common_name : The common band name. Must be one of the :stac-ext:`list of
-                accepted common names <eo#common-band-names>`.
+    @property
+    def offset(self) -> float | None:
+        """Get or sets the number to be added to the pixel value (after scaling)
+        to transform into the value (i.e. translate digital number to reflectance).
 
         Returns:
-            Tuple[float, float] or None: The band range for this name as (min, max), or
-            None if this is not a recognized common name.
+            [float]
         """
-        name_to_range = {
-            "coastal": (0.40, 0.45),
-            "blue": (0.45, 0.50),
-            "green": (0.50, 0.60),
-            "red": (0.60, 0.70),
-            "yellow": (0.58, 0.62),
-            "pan": (0.50, 0.70),
-            "rededge": (0.70, 0.75),
-            "nir": (0.75, 1.00),
-            "nir08": (0.75, 0.90),
-            "nir09": (0.85, 1.05),
-            "cirrus": (1.35, 1.40),
-            "swir16": (1.55, 1.75),
-            "swir22": (2.10, 2.30),
-            "lwir": (10.5, 12.5),
-            "lwir11": (10.5, 11.5),
-            "lwir12": (11.5, 12.5),
-        }
+        return self.properties.get("offset")
 
-        return name_to_range.get(common_name)
+    @offset.setter
+    def offset(self, v: float | None) -> None:
+        if v is not None:
+            self.properties["offset"] = v
+        else:
+            self.properties.pop("offset", None)
 
-    @staticmethod
-    def band_description(common_name: str) -> Optional[str]:
-        """Returns a description of the band for one with a common name.
+    @property
+    def histogram(self) -> Histogram | None:
+        """Get or sets the histogram distribution information of the pixels values in
+        the band.
 
-        Args:
-            common_name : The common band name. Must be one of the :stac-ext:`list of
-                accepted common names <eo#common-band-names>`.
+        Returns:
+            [Histogram]
+        """
+        return Histogram.from_dict(get_opt(self.properties.get("histogram")))
+
+    @histogram.setter
+    def histogram(self, v: Histogram | None) -> None:
+        if v is not None:
+            self.properties["histogram"] = v.to_dict()
+        else:
+            self.properties.pop("histogram", None)
+
+    def __repr__(self) -> str:
+        return "<Raster Band>"
+
+    def to_dict(self) -> dict[str, Any]:
+        """Returns this band as a dictionary.
 
         Returns:
-            str or None: If a recognized common name, returns a description including
-            the band range. Otherwise returns None.
+            dict: The serialization of the Band.
         """
-        r = Band.band_range(common_name)
-        if r is not None:
-            return "Common name: {}, Range: {} to {}".format(common_name, r[0], r[1])
-        return None
+        return self.properties
 
 
-class EOExtension(
+class RasterExtension(
     Generic[T],
     PropertiesExtension,
     ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]],
 ):
     """An abstract class that can be used to extend the properties of an
-    :class:`~pystac.Item` or :class:`~pystac.Asset` with properties from the
-    :stac-ext:`Electro-Optical Extension <eo>`. This class is generic over the type of
-    STAC Object to be extended (e.g. :class:`~pystac.Item`,
+    :class:`~pystac.Item`, :class:`~pystac.Asset`, or
+    :class:`~pystac.extension.item_assets.AssetDefinition` with properties from
+    the :stac-ext:`Raster Extension <raster>`. This class is generic over
+    the type of STAC Object to be extended (e.g. :class:`~pystac.Item`,
     :class:`~pystac.Asset`).
 
-    To create a concrete instance of :class:`EOExtension`, use the
-    :meth:`EOExtension.ext` method. For example:
+    This class will generally not be used directly. Instead, use the concrete
+    implementation associated with the STAC Object you want to extend (e.g.
+    :class:`~ItemRasterExtension` to extend an :class:`~pystac.Item`).  You may
+    prefer to use the `ext` class method of this class to construct the correct
+    instance type for you.
+    """
 
-    .. code-block:: python
+    name: Literal["raster"] = "raster"
 
-       >>> item: pystac.Item = ...
-       >>> eo_ext = EOExtension.ext(item)
-    """
+    properties: dict[str, Any]
+    """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    def apply(
-        self,
-        bands: Optional[List[Band]] = None,
-        cloud_cover: Optional[float] = None,
-        snow_cover: Optional[float] = None,
-    ) -> None:
-        """Applies Electro-Optical Extension properties to the extended
-        :class:`~pystac.Item` or :class:`~pystac.Asset`.
+    def apply(self, bands: list[RasterBand]) -> None:
+        """Applies raster extension properties to the extended :class:`pystac.Item` or
+        :class:`pystac.Asset`.
 
         Args:
-            bands : A list of available bands where each item is a :class:`~Band`
-                object. If given, requires at least one band.
-            cloud_cover : The estimate of cloud cover as a percentage
-                (0-100) of the entire scene. If not available the field should not
-                be provided.
-            snow_cover : The estimate of snow cover as a percentage
-                (0-100) of the entire scene. If not available the field should not
-                be provided.
+            bands : a list of :class:`~pystac.RasterBand` objects that represent
+                the available raster bands.
         """
         self.bands = bands
-        self.cloud_cover = validated_percentage(cloud_cover)
-        self.snow_cover = validated_percentage(snow_cover)
 
     @property
-    def bands(self) -> Optional[List[Band]]:
-        """Gets or sets a list of available bands where each item is a :class:`~Band`
-        object (or ``None`` if no bands have been set). If not available the field
-        should not be provided.
+    def bands(self) -> list[RasterBand] | None:
+        """Gets or sets a list of available bands where each item is a
+        :class:`~RasterBand` object (or ``None`` if no bands have been set). If not
+        available the field should not be provided.
         """
         return self._get_bands()
 
     @bands.setter
-    def bands(self, v: Optional[List[Band]]) -> None:
+    def bands(self, v: list[RasterBand] | None) -> None:
         self._set_property(
             BANDS_PROP, map_opt(lambda bands: [b.to_dict() for b in bands], v)
         )
 
-    def _get_bands(self) -> Optional[List[Band]]:
+    def _get_bands(self) -> list[RasterBand] | None:
         return map_opt(
-            lambda bands: [Band(b) for b in bands],
-            self._get_property(BANDS_PROP, List[Dict[str, Any]]),
+            lambda bands: [RasterBand(b) for b in bands],
+            self._get_property(BANDS_PROP, list[dict[str, Any]]),
         )
 
-    @property
-    def cloud_cover(self) -> Optional[float]:
-        """Get or sets the estimate of cloud cover as a percentage
-        (0-100) of the entire scene. If not available the field should not be provided.
-
-        Returns:
-            float or None
-        """
-        return self._get_property(CLOUD_COVER_PROP, float)
-
-    @cloud_cover.setter
-    def cloud_cover(self, v: Optional[float]) -> None:
-        self._set_property(CLOUD_COVER_PROP, validated_percentage(v), pop_if_none=True)
-
-    @property
-    def snow_cover(self) -> Optional[float]:
-        """Get or sets the estimate of snow cover as a percentage
-        (0-100) of the entire scene. If not available the field should not be provided.
-
-        Returns:
-            float or None
-        """
-        return self._get_property(SNOW_COVER_PROP, float)
-
-    @snow_cover.setter
-    def snow_cover(self, v: Optional[float]) -> None:
-        self._set_property(SNOW_COVER_PROP, validated_percentage(v), pop_if_none=True)
-
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def get_schema_uris(cls) -> List[str]:
+    def get_schema_uris(cls) -> list[str]:
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
         return SCHEMA_URIS
 
     @classmethod
-    def ext(cls, obj: T, add_if_missing: bool = False) -> EOExtension[T]:
-        """Extends the given STAC Object with properties from the
-        :stac-ext:`Electro-Optical Extension <eo>`.
+    def ext(cls, obj: T, add_if_missing: bool = False) -> RasterExtension[T]:
+        """Extends the given STAC Object with properties from the :stac-ext:`Raster
+        Extension <raster>`.
 
-        This extension can be applied to instances of :class:`~pystac.Item` or
-        :class:`~pystac.Asset`.
+        This extension can be applied to instances of :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
-        if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
-            return cast(EOExtension[T], ItemEOExtension(obj))
-        elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
-            return cast(EOExtension[T], AssetEOExtension(obj))
+        if isinstance(obj, pystac.Asset):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(RasterExtension[T], AssetRasterExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(RasterExtension[T], ItemAssetsRasterExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
-    ) -> SummariesEOExtension:
-        """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
-        return SummariesEOExtension(obj)
-
-
-class ItemEOExtension(EOExtension[pystac.Item]):
-    """A concrete implementation of :class:`EOExtension` on an :class:`~pystac.Item`
-    that extends the properties of the Item to include properties defined in the
-    :stac-ext:`Electro-Optical Extension <eo>`.
-
-    This class should generally not be instantiated directly. Instead, call
-    :meth:`EOExtension.ext` on an :class:`~pystac.Item` to extend it.
-    """
-
-    item: pystac.Item
-    """The :class:`~pystac.Item` being extended."""
-
-    properties: Dict[str, Any]
-    """The :class:`~pystac.Item` properties, including extension properties."""
-
-    def __init__(self, item: pystac.Item):
-        self.item = item
-        self.properties = item.properties
-
-    def _get_bands(self) -> Optional[List[Band]]:
-        """Get or sets a list of :class:`~pystac.Band` objects that represent
-        the available bands.
-        """
-        bands = self._get_property(BANDS_PROP, List[Dict[str, Any]])
-
-        # get assets with eo:bands even if not in item
-        if bands is None:
-            asset_bands: List[Dict[str, Any]] = []
-            for _, value in self.item.get_assets().items():
-                if BANDS_PROP in value.extra_fields:
-                    asset_bands.extend(
-                        cast(List[Dict[str, Any]], value.extra_fields.get(BANDS_PROP))
-                    )
-            if any(asset_bands):
-                bands = asset_bands
-
-        if bands is not None:
-            return [Band(b) for b in bands]
-        return None
-
-    def get_assets(
-        self,
-        name: Optional[str] = None,
-        common_name: Optional[str] = None,
-    ) -> Dict[str, pystac.Asset]:
-        """Get the item's assets where eo:bands are defined.
-
-        Args:
-            name: If set, filter the assets such that only those with a
-                matching ``eo:band.name`` are returned.
-            common_name: If set, filter the assets such that only those with a matching
-                ``eo:band.common_name`` are returned.
-
-        Returns:
-            Dict[str, Asset]: A dictionary of assets that match ``name``
-                and/or ``common_name`` if set or else all of this item's assets were
-                eo:bands are defined.
-        """
-        kwargs = {"name": name, "common_name": common_name}
-        return {
-            key: asset
-            for key, asset in self.item.get_assets().items()
-            if BANDS_PROP in asset.extra_fields
-            and all(
-                v is None or any(v == b.get(k) for b in asset.extra_fields[BANDS_PROP])
-                for k, v in kwargs.items()
-            )
-        }
-
-    def __repr__(self) -> str:
-        return "<ItemEOExtension Item id={}>".format(self.item.id)
+    ) -> SummariesRasterExtension:
+        cls.ensure_has_extension(obj, add_if_missing)
+        return SummariesRasterExtension(obj)
 
 
-class AssetEOExtension(EOExtension[pystac.Asset]):
-    """A concrete implementation of :class:`EOExtension` on an :class:`~pystac.Asset`
-    that extends the Asset fields to include properties defined in the
-    :stac-ext:`Electro-Optical Extension <eo>`.
-
-    This class should generally not be instantiated directly. Instead, call
-    :meth:`EOExtension.ext` on an :class:`~pystac.Asset` to extend it.
-    """
-
+class AssetRasterExtension(RasterExtension[pystac.Asset]):
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
-    def _get_bands(self) -> Optional[List[Band]]:
-        if BANDS_PROP not in self.properties:
-            return None
-        return list(
-            map(
-                lambda band: Band(band),
-                cast(List[Dict[str, Any]], self.properties.get(BANDS_PROP)),
-            )
-        )
-
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetEOExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetRasterExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsRasterExtension(RasterExtension[item_assets.AssetDefinition]):
+    asset_definition: item_assets.AssetDefinition
+    """A reference to the :class:`~pystac.extensions.item_assets.AssetDefinition`
+    being extended."""
+
+    properties: dict[str, Any]
+    """The :class:`~pystac.extensions.item_assets.AssetDefinition` fields, including
+    extension properties."""
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.properties = item_asset.properties
+        self.asset_definition = item_asset
+
+    def __repr__(self) -> str:
+        return "<ItemAssetsRasterExtension AssetDefinition={}>".format(
+            self.asset_definition
+        )
 
 
-class SummariesEOExtension(SummariesExtension):
+class SummariesRasterExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
-    defined in the :stac-ext:`Electro-Optical Extension <eo>`.
+    defined in the :stac-ext:`Raster Extension <raster>`.
     """
 
     @property
-    def bands(self) -> Optional[List[Band]]:
-        """Get or sets the summary of :attr:`EOExtension.bands` values
-        for this Collection.
+    def bands(self) -> list[RasterBand] | None:
+        """Get or sets a list of :class:`~pystac.Band` objects that represent
+        the available bands.
         """
-
         return map_opt(
-            lambda bands: [Band(b) for b in bands],
+            lambda bands: [RasterBand(b) for b in bands],
             self.summaries.get_list(BANDS_PROP),
         )
 
     @bands.setter
-    def bands(self, v: Optional[List[Band]]) -> None:
+    def bands(self, v: list[RasterBand] | None) -> None:
         self._set_summary(BANDS_PROP, map_opt(lambda x: [b.to_dict() for b in x], v))
 
-    @property
-    def cloud_cover(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`EOExtension.cloud_cover` values
-        for this Collection.
-        """
-        return self.summaries.get_range(CLOUD_COVER_PROP)
 
-    @cloud_cover.setter
-    def cloud_cover(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(CLOUD_COVER_PROP, v)
-
-    @property
-    def snow_cover(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`EOExtension.snow_cover` values
-        for this Collection.
-        """
-        return self.summaries.get_range(SNOW_COVER_PROP)
-
-    @snow_cover.setter
-    def snow_cover(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(SNOW_COVER_PROP, v)
-
-
-class EOExtensionHooks(ExtensionHooks):
+class RasterExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {
-        "eo",
-        *[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI],
-    }
-    stac_object_types = {pystac.STACObjectType.ITEM}
-
-    def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
-    ) -> None:
-        if version < "0.9":
-            # Some eo fields became common_metadata
-            if (
-                "eo:platform" in obj["properties"]
-                and "platform" not in obj["properties"]
-            ):
-                obj["properties"]["platform"] = obj["properties"]["eo:platform"]
-                del obj["properties"]["eo:platform"]
-
-            if (
-                "eo:instrument" in obj["properties"]
-                and "instruments" not in obj["properties"]
-            ):
-                obj["properties"]["instruments"] = [obj["properties"]["eo:instrument"]]
-                del obj["properties"]["eo:instrument"]
-
-            if (
-                "eo:constellation" in obj["properties"]
-                and "constellation" not in obj["properties"]
-            ):
-                obj["properties"]["constellation"] = obj["properties"][
-                    "eo:constellation"
-                ]
-                del obj["properties"]["eo:constellation"]
-
-            # Some eo fields became view extension fields
-            eo_to_view_fields = [
-                "off_nadir",
-                "azimuth",
-                "incidence_angle",
-                "sun_azimuth",
-                "sun_elevation",
-            ]
-
-            for field in eo_to_view_fields:
-                if "eo:{}".format(field) in obj["properties"]:
-                    if "stac_extensions" not in obj:
-                        obj["stac_extensions"] = []
-                    if view.SCHEMA_URI not in obj["stac_extensions"]:
-                        obj["stac_extensions"].append(view.SCHEMA_URI)
-                    if "view:{}".format(field) not in obj["properties"]:
-                        obj["properties"]["view:{}".format(field)] = obj["properties"][
-                            "eo:{}".format(field)
-                        ]
-                        del obj["properties"]["eo:{}".format(field)]
-
-            # eo:epsg became proj:epsg
-            eo_epsg = PREFIX + "epsg"
-            proj_epsg = projection.PREFIX + "epsg"
-            if eo_epsg in obj["properties"] and proj_epsg not in obj["properties"]:
-                obj["properties"][proj_epsg] = obj["properties"].pop(eo_epsg)
-                obj["stac_extensions"] = obj.get("stac_extensions", [])
-                if (
-                    projection.ProjectionExtension.get_schema_uri()
-                    not in obj["stac_extensions"]
-                ):
-                    obj["stac_extensions"].append(
-                        projection.ProjectionExtension.get_schema_uri()
-                    )
-                if not any(prop.startswith(PREFIX) for prop in obj["properties"]):
-                    obj["stac_extensions"].remove(EOExtension.get_schema_uri())
-
-        if version < "1.0.0-beta.1" and info.object_type == pystac.STACObjectType.ITEM:
-            # gsd moved from eo to common metadata
-            if "eo:gsd" in obj["properties"]:
-                obj["properties"]["gsd"] = obj["properties"]["eo:gsd"]
-                del obj["properties"]["eo:gsd"]
-
-            # The way bands were declared in assets changed.
-            # In 1.0.0-beta.1 they are inlined into assets as
-            # opposed to having indices back into a property-level array.
-            if "eo:bands" in obj["properties"]:
-                bands = obj["properties"]["eo:bands"]
-                for asset in obj["assets"].values():
-                    if "eo:bands" in asset:
-                        new_bands: List[Dict[str, Any]] = []
-                        for band_index in asset["eo:bands"]:
-                            new_bands.append(bands[band_index])
-                        asset["eo:bands"] = new_bands
-
-        super().migrate(obj, version, info)
+    prev_extension_ids: set[str] = {*[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI]}
+    stac_object_types = {pystac.STACObjectType.ITEM, pystac.STACObjectType.COLLECTION}
 
 
-EO_EXTENSION_HOOKS: ExtensionHooks = EOExtensionHooks()
+RASTER_EXTENSION_HOOKS: ExtensionHooks = RasterExtensionHooks()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pystac-1.8.4/pystac/extensions/file.py` & `pystac-1.9.0/pystac/extensions/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,274 +1,276 @@
-"""Implements the :stac-ext:`File Info Extension <file>`."""
-
 from __future__ import annotations
 
-from typing import Any, Dict, Iterable, List, Optional, Union
+import re
+import warnings
+from abc import ABC, abstractmethod
+from collections.abc import Iterable
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Generic,
+    TypeVar,
+    cast,
+)
 
 import pystac
-from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
-from pystac.extensions.hooks import ExtensionHooks
-from pystac.serialization.identify import (
-    OldExtensionShortIDs,
-    STACJSONDescription,
-    STACVersionID,
-)
-from pystac.utils import StringEnum, get_required, map_opt
 
-SCHEMA_URI = "https://stac-extensions.github.io/file/v2.0.0/schema.json"
+if TYPE_CHECKING:
+    from pystac.extensions.item_assets import AssetDefinition
 
-PREFIX = "file:"
-BYTE_ORDER_PROP = PREFIX + "byte_order"
-CHECKSUM_PROP = PREFIX + "checksum"
-HEADER_SIZE_PROP = PREFIX + "header_size"
-SIZE_PROP = PREFIX + "size"
-VALUES_PROP = PREFIX + "values"
+VERSION_REGEX = re.compile("/v[0-9].[0-9].*/")
 
 
-class ByteOrder(StringEnum):
-    """List of allows values for the ``"file:byte_order"`` field defined by the
-    :stac-ext:`File Info Extension <file>`."""
+class SummariesExtension:
+    """Base class for extending the properties in :attr:`pystac.Collection.summaries`
+    to include properties defined by a STAC Extension.
 
-    LITTLE_ENDIAN = "little-endian"
-    BIG_ENDIAN = "big-endian"
+    This class should generally not be instantiated directly. Instead, create an
+    extension-specific class that inherits from this class and instantiate that. See
+    :class:`~pystac.extensions.eo.SummariesEOExtension` for an example."""
 
+    summaries: pystac.Summaries
+    """The summaries for the :class:`~pystac.Collection` being extended."""
 
-class MappingObject:
-    """Represents a value map used by assets that are used as classification layers, and
-    give details about the values in the asset and their meanings."""
+    def __init__(self, collection: pystac.Collection) -> None:
+        self.summaries = collection.summaries
 
-    properties: Dict[str, Any]
+    def _set_summary(
+        self,
+        prop_key: str,
+        v: list[Any] | pystac.RangeSummary[Any] | dict[str, Any] | None,
+    ) -> None:
+        if v is None:
+            self.summaries.remove(prop_key)
+        else:
+            self.summaries.add(prop_key, v)
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
-        self.properties = properties
 
-    def apply(self, values: List[Any], summary: str) -> None:
-        """Sets the properties for this :class:`~MappingObject` instance.
+P = TypeVar("P")
 
-        Args:
-            values : The value(s) in the file. At least one array element is required.
-            summary : A short description of the value(s).
-        """
-        self.values = values
-        self.summary = summary
 
-    @classmethod
-    def create(cls, values: List[Any], summary: str) -> MappingObject:
-        """Creates a new :class:`~MappingObject` instance.
+class PropertiesExtension(ABC):
+    """Abstract base class for extending the properties of an :class:`~pystac.Item`
+    to include properties defined by a STAC Extension.
 
-        Args:
-            values : The value(s) in the file. At least one array element is required.
-            summary : A short description of the value(s).
-        """
-        m = cls({})
-        m.apply(values=values, summary=summary)
-        return m
-
-    @property
-    def values(self) -> List[Any]:
-        """Gets or sets the list of value(s) in the file. At least one array element is
-        required."""
-        return get_required(self.properties.get("values"), self, "values")
-
-    @values.setter
-    def values(self, v: List[Any]) -> None:
-        self.properties["values"] = v
-
-    @property
-    def summary(self) -> str:
-        """Gets or sets the short description of the value(s)."""
-        return get_required(self.properties.get("summary"), self, "summary")
-
-    @summary.setter
-    def summary(self, v: str) -> None:
-        self.properties["summary"] = v
+    This class should not be instantiated directly. Instead, create an
+    extension-specific class that inherits from this class and instantiate that. See
+    :class:`~pystac.extensions.eo.PropertiesEOExtension` for an example.
+    """
 
-    @classmethod
-    def from_dict(cls, d: Dict[str, Any]) -> MappingObject:
-        return cls.create(**d)
+    properties: dict[str, Any]
+    """The properties that this extension wraps.
 
-    def to_dict(self) -> Dict[str, Any]:
-        return self.properties
+    The extension which implements PropertiesExtension can use ``_get_property`` and
+    ``_set_property`` to get and set values on this instance. Note that _set_properties
+    mutates the properties directly."""
+
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
+    """Additional read-only properties accessible from the extended object.
+
+    These are used when extending an :class:`~pystac.Asset` to give access to the
+    properties of the owning :class:`~pystac.Item`. If a property exists in both
+    ``additional_read_properties`` and ``properties``, the value in
+    ``additional_read_properties`` will take precedence.
+    """
+
+    def _get_property(self, prop_name: str, _typ: type[P]) -> P | None:
+        maybe_property: P | None = self.properties.get(prop_name)
+        if maybe_property is not None:
+            return maybe_property
+        if self.additional_read_properties is not None:
+            for props in self.additional_read_properties:
+                maybe_additional_property: P | None = props.get(prop_name)
+                if maybe_additional_property is not None:
+                    return maybe_additional_property
+        return None
 
+    def _set_property(
+        self, prop_name: str, v: Any | None, pop_if_none: bool = True
+    ) -> None:
+        if v is None and pop_if_none:
+            self.properties.pop(prop_name, None)
+        elif isinstance(v, list):
+            self.properties[prop_name] = [
+                x.to_dict() if hasattr(x, "to_dict") else x for x in v
+            ]
+        else:
+            self.properties[prop_name] = v
 
-class FileExtension(
-    PropertiesExtension, ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]]
-):
-    """A class that can be used to extend the properties of an :class:`~pystac.Asset`
-    with properties from the :stac-ext:`File Info Extension <file>`.
 
-    To create an instance of :class:`FileExtension`, use the
-    :meth:`FileExtension.ext` method. For example:
+S = TypeVar("S", bound=pystac.STACObject)
 
-    .. code-block:: python
 
-       >>> asset: pystac.Asset = ...
-       >>> file_ext = FileExtension.ext(asset)
+class ExtensionManagementMixin(Generic[S], ABC):
+    """Abstract base class with methods for adding and removing extensions from STAC
+    Objects. This class is generic over the type of object being extended (e.g.
+    :class:`~pystac.Item`).
+
+    Concrete extension implementations should inherit from this class and either
+    provide a concrete type or a bounded type variable.
+
+    See :class:`~pystac.extensions.eo.EOExtension` for an example implementation.
     """
 
-    asset_href: str
-    """The ``href`` value of the :class:`~pystac.Asset` being extended."""
+    @classmethod
+    @abstractmethod
+    def get_schema_uri(cls) -> str:
+        """Gets the schema URI associated with this extension."""
+        raise NotImplementedError
 
-    properties: Dict[str, Any]
-    """The :class:`~pystac.Asset` fields, including extension properties."""
+    @classmethod
+    def get_schema_uris(cls) -> list[str]:
+        """Gets a list of schema URIs associated with this extension."""
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
+        return [cls.get_schema_uri()]
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
-    """If present, this will be a list containing 1 dictionary representing the
-    properties of the owning :class:`~pystac.Item`."""
-
-    def __init__(self, asset: pystac.Asset):
-        self.asset_href = asset.href
-        self.properties = asset.extra_fields
-        if asset.owner and isinstance(asset.owner, pystac.Item):
-            self.additional_read_properties = [asset.owner.properties]
+    @classmethod
+    def add_to(cls, obj: S) -> None:
+        """Add the schema URI for this extension to the
+        :attr:`~pystac.STACObject.stac_extensions` list for the given object, if it is
+        not already present."""
+        if obj.stac_extensions is None:
+            obj.stac_extensions = [cls.get_schema_uri()]
+        elif not cls.has_extension(obj):
+            obj.stac_extensions.append(cls.get_schema_uri())
 
-    def __repr__(self) -> str:
-        return "<AssetFileExtension Asset href={}>".format(self.asset_href)
+    @classmethod
+    def remove_from(cls, obj: S) -> None:
+        """Remove the schema URI for this extension from the
+        :attr:`pystac.STACObject.stac_extensions` list for the given object."""
+        if obj.stac_extensions is not None:
+            obj.stac_extensions = [
+                uri for uri in obj.stac_extensions if uri != cls.get_schema_uri()
+            ]
 
-    def apply(
-        self,
-        byte_order: Optional[ByteOrder] = None,
-        checksum: Optional[str] = None,
-        header_size: Optional[int] = None,
-        size: Optional[int] = None,
-        values: Optional[List[MappingObject]] = None,
+    @classmethod
+    def has_extension(cls, obj: S) -> bool:
+        """Check if the given object implements this extension by checking
+        :attr:`pystac.STACObject.stac_extensions` for this extension's schema URI."""
+        schema_startswith = VERSION_REGEX.split(cls.get_schema_uri())[0] + "/"
+
+        return obj.stac_extensions is not None and any(
+            uri.startswith(schema_startswith) for uri in obj.stac_extensions
+        )
+
+    @classmethod
+    def validate_owner_has_extension(
+        cls,
+        asset: pystac.Asset | AssetDefinition,
+        add_if_missing: bool = False,
     ) -> None:
-        """Applies file extension properties to the extended Item.
+        """
+        DEPRECATED
+
+        .. deprecated:: 1.9
+            Use :meth:`ensure_owner_has_extension` instead.
+
+        Given an :class:`~pystac.Asset`, checks if the asset's owner has this
+        extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
+        If ``add_if_missing`` is ``True``, the schema URI will be added to the owner.
 
         Args:
-            byte_order : Optional byte order of integer values in the file. One of
-                ``"big-endian"`` or ``"little-endian"``.
-            checksum : Optional multihash for the corresponding file,
-                encoded as hexadecimal (base 16) string with lowercase letters.
-            header_size : Optional header size of the file, in bytes.
-            size : Optional size of the file, in bytes.
-            values : Optional list of :class:`~MappingObject` instances that lists the
-                values that are in the file and describe their meaning. See the
-                :stac-ext:`Mapping Object <file#mapping-object>` docs for an example.
-                If given, at least one array element is required.
+            asset : The asset whose owner should be validated.
+            add_if_missing : Whether to add the schema URI to the owner if it is
+                not already present. Defaults to False.
+
+        Raises:
+            STACError : If ``add_if_missing`` is ``True`` and ``asset.owner`` is
+                ``None``.
         """
-        self.byte_order = byte_order
-        self.checksum = checksum
-        self.header_size = header_size
-        self.size = size
-        self.values = values
-
-    @property
-    def byte_order(self) -> Optional[ByteOrder]:
-        """Gets or sets the byte order of integer values in the file. One of big-endian
-        or little-endian."""
-        return self._get_property(BYTE_ORDER_PROP, ByteOrder)
-
-    @byte_order.setter
-    def byte_order(self, v: Optional[ByteOrder]) -> None:
-        self._set_property(BYTE_ORDER_PROP, v)
-
-    @property
-    def checksum(self) -> Optional[str]:
-        """Get or sets the multihash for the corresponding file, encoded as hexadecimal
-        (base 16) string with lowercase letters."""
-        return self._get_property(CHECKSUM_PROP, str)
-
-    @checksum.setter
-    def checksum(self, v: Optional[str]) -> None:
-        self._set_property(CHECKSUM_PROP, v)
-
-    @property
-    def header_size(self) -> Optional[int]:
-        """Get or sets the header size of the file, in bytes."""
-        return self._get_property(HEADER_SIZE_PROP, int)
-
-    @header_size.setter
-    def header_size(self, v: Optional[int]) -> None:
-        self._set_property(HEADER_SIZE_PROP, v)
-
-    @property
-    def size(self) -> Optional[int]:
-        """Get or sets the size of the file, in bytes."""
-        return self._get_property(SIZE_PROP, int)
-
-    @size.setter
-    def size(self, v: Optional[int]) -> None:
-        self._set_property(SIZE_PROP, v)
-
-    @property
-    def values(self) -> Optional[List[MappingObject]]:
-        """Get or sets the list of :class:`~MappingObject` instances that lists the
-        values that are in the file and describe their meaning. See the
-        :stac-ext:`Mapping Object <file#mapping-object>` docs for an example. If given,
-        at least one array element is required."""
-        return map_opt(
-            lambda values: [
-                MappingObject.from_dict(mapping_obj) for mapping_obj in values
-            ],
-            self._get_property(VALUES_PROP, List[Dict[str, Any]]),
-        )
-
-    @values.setter
-    def values(self, v: Optional[List[MappingObject]]) -> None:
-        self._set_property(
-            VALUES_PROP,
-            map_opt(
-                lambda values: [mapping_obj.to_dict() for mapping_obj in values], v
-            ),
+        warnings.warn(
+            "ensure_owner_has_extension is deprecated. "
+            "Use ensure_owner_has_extension instead",
+            DeprecationWarning,
         )
+        return cls.ensure_owner_has_extension(asset, add_if_missing)
 
     @classmethod
-    def get_schema_uri(cls) -> str:
-        return SCHEMA_URI
+    def ensure_owner_has_extension(
+        cls,
+        asset_or_link: pystac.Asset | AssetDefinition | pystac.Link,
+        add_if_missing: bool = False,
+    ) -> None:
+        """Given an :class:`~pystac.Asset`, checks if the asset's owner has this
+        extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
+        If ``add_if_missing`` is ``True``, the schema URI will be added to the owner.
+
+        Args:
+            asset : The asset whose owner should be validated.
+            add_if_missing : Whether to add the schema URI to the owner if it is
+                not already present. Defaults to False.
+
+        Raises:
+            STACError : If ``add_if_missing`` is ``True`` and ``asset.owner`` is
+                ``None``.
+        """
+        if asset_or_link.owner is None:
+            if add_if_missing:
+                raise pystac.STACError(
+                    f"Attempted to use add_if_missing=True for a {type(asset_or_link)} "
+                    "with no owner. Use .set_owner or set add_if_missing=False."
+                )
+            else:
+                return
+        return cls.ensure_has_extension(cast(S, asset_or_link.owner), add_if_missing)
 
     @classmethod
-    def ext(cls, obj: pystac.Asset, add_if_missing: bool = False) -> FileExtension:
-        """Extends the given STAC Object with properties from the :stac-ext:`File Info
-        Extension <file>`.
+    def validate_has_extension(cls, obj: S, add_if_missing: bool = False) -> None:
+        """
+        DEPRECATED
+
+        .. deprecated:: 1.9
+            Use :meth:`ensure_has_extension` instead.
 
-        This extension can be applied to instances of :class:`~pystac.Asset`.
+        Given a :class:`~pystac.STACObject`, checks if the object has this
+        extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
+        If ``add_if_missing`` is ``True``, the schema URI will be added to the object.
+
+        Args:
+            obj : The object to validate.
+            add_if_missing : Whether to add the schema URI to the object if it is
+                not already present. Defaults to False.
         """
-        if isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
-            return cls(obj)
-        else:
-            raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
+        warnings.warn(
+            "validate_has_extension is deprecated. Use ensure_has_extension instead",
+            DeprecationWarning,
+        )
 
+        return cls.ensure_has_extension(obj, add_if_missing)
 
-class FileExtensionHooks(ExtensionHooks):
-    schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"file"}
-    stac_object_types = {pystac.STACObjectType.ITEM}
+    @classmethod
+    def ensure_has_extension(cls, obj: S, add_if_missing: bool = False) -> None:
+        """Given a :class:`~pystac.STACObject`, checks if the object has this
+        extension's schema URI in its :attr:`~pystac.STACObject.stac_extensions` list.
+        If ``add_if_missing`` is ``True``, the schema URI will be added to the object.
 
-    def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
-    ) -> None:
-        # The checksum field was previously it's own extension.
-        old_checksum: Optional[Dict[str, str]] = None
-        if info.version_range.latest_valid_version() < "v1.0.0-rc.2":
-            if OldExtensionShortIDs.CHECKSUM.value in info.extensions:
-                old_item_checksum = obj["properties"].get("checksum:multihash")
-                if old_item_checksum is not None:
-                    if old_checksum is None:
-                        old_checksum = {}
-                    old_checksum["__item__"] = old_item_checksum
-                for asset_key, asset in obj["assets"].items():
-                    old_asset_checksum = asset.get("checksum:multihash")
-                    if old_asset_checksum is not None:
-                        if old_checksum is None:
-                            old_checksum = {}
-                        old_checksum[asset_key] = old_asset_checksum
-
-                try:
-                    obj["stac_extensions"].remove(OldExtensionShortIDs.CHECKSUM.value)
-                except ValueError:
-                    pass
-
-        super().migrate(obj, version, info)
-
-        if old_checksum is not None:
-            if SCHEMA_URI not in obj["stac_extensions"]:
-                obj["stac_extensions"].append(SCHEMA_URI)
-            for key in old_checksum:
-                if key == "__item__":
-                    obj["properties"][CHECKSUM_PROP] = old_checksum[key]
-                else:
-                    obj["assets"][key][CHECKSUM_PROP] = old_checksum[key]
+        Args:
+            obj : The object to validate.
+            add_if_missing : Whether to add the schema URI to the object if it is
+                not already present. Defaults to False.
+        """
+        if add_if_missing:
+            cls.add_to(obj)
 
+        if not cls.has_extension(obj):
+            name = getattr(cls, "name", cls.__name__)
+            suggestion = (
+                f"``obj.ext.add('{name}')"
+                if hasattr(cls, "name")
+                else f"``{name}.add_to(obj)``"
+            )
+
+            raise pystac.ExtensionNotImplemented(
+                f"Extension '{name}' is not implemented on object."
+                f"STAC producers can add the extension using {suggestion}"
+            )
 
-FILE_EXTENSION_HOOKS: ExtensionHooks = FileExtensionHooks()
+    @classmethod
+    def _ext_error_message(cls, obj: Any) -> str:
+        contents = [f"{cls.__name__} does not apply to type '{type(obj).__name__}'"]
+        if hasattr(cls, "summaries") and isinstance(obj, pystac.Collection):
+            hint = f"Hint: Did you mean to use `{cls.__name__}.summaries` instead?"
+            contents.append(hint)
+        return ". ".join(contents)
```

### Comparing `pystac-1.8.4/pystac/extensions/grid.py` & `pystac-1.9.0/pystac/extensions/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Implements the :stac-ext:`Grid Extension <grid>`."""
 
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, List, Optional, Pattern, Set, Union
+import warnings
+from re import Pattern
+from typing import Any, Literal, Union
 
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/grid/v1.1.0/schema.json"
-SCHEMA_URIS: List[str] = [
+SCHEMA_URIS: list[str] = [
     "https://stac-extensions.github.io/grid/v1.0.0/schema.json",
     SCHEMA_URI,
 ]
 PREFIX: str = "grid:"
 
 # Field names
 CODE_PROP: str = PREFIX + "code"  # required
@@ -46,70 +48,76 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> proj_ext = GridExtension.ext(item)
     """
 
+    name: Literal["grid"] = "grid"
+
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemGridExtension Item id={}>".format(self.item.id)
+        return f"<ItemGridExtension Item id={self.item.id}>"
 
     def apply(self, code: str) -> None:
         """Applies Grid extension properties to the extended Item.
 
         Args:
             code : REQUIRED. The code of the Item's grid location.
         """
         self.code = validated_code(code)
 
     @property
-    def code(self) -> Optional[str]:
+    def code(self) -> str | None:
         """Get or sets the latitude band of the datasource."""
         return self._get_property(CODE_PROP, str)
 
     @code.setter
     def code(self, v: str) -> None:
         self._set_property(CODE_PROP, validated_code(v), pop_if_none=False)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def get_schema_uris(cls) -> List[str]:
+    def get_schema_uris(cls) -> list[str]:
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
         return SCHEMA_URIS
 
     @classmethod
     def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> GridExtension:
         """Extends the given STAC Object with properties from the :stac-ext:`Grid
         Extension <grid>`.
 
         This extension can be applied to instances of :class:`~pystac.Item`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return GridExtension(obj)
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class GridExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids: Set[str] = {*[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI]}
+    prev_extension_ids: set[str] = {*[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI]}
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
 GRID_EXTENSION_HOOKS: ExtensionHooks = GridExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/hooks.py` & `pystac-1.9.0/pystac/extensions/hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 from functools import lru_cache
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Set, Union
+from typing import TYPE_CHECKING, Any
 
 import pystac
 from pystac.serialization.identify import STACJSONDescription, STACVersionID
 
 if TYPE_CHECKING:
     from pystac.stac_object import STACObject
 
@@ -16,40 +17,38 @@
     @abstractmethod
     def schema_uri(self) -> str:
         """The schema_uri for the current version of this extension"""
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def prev_extension_ids(self) -> Set[str]:
+    def prev_extension_ids(self) -> set[str]:
         """A set of previous extension IDs (schema URIs or old short ids)
         that should be migrated to the latest schema URI in the 'stac_extensions'
         property. Override with a class attribute so that the set of previous
         IDs is only created once.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def stac_object_types(self) -> Set[pystac.STACObjectType]:
+    def stac_object_types(self) -> set[pystac.STACObjectType]:
         """A set of STACObjectType for which migration logic will be applied."""
         raise NotImplementedError
 
-    @lru_cache()
-    def _get_stac_object_types(self) -> Set[str]:
+    @lru_cache
+    def _get_stac_object_types(self) -> set[str]:
         """Translation of stac_object_types to strings, cached"""
-        return set([x.value for x in self.stac_object_types])
+        return {x.value for x in self.stac_object_types}
 
-    def get_object_links(
-        self, obj: STACObject
-    ) -> Optional[List[Union[str, pystac.RelType]]]:
+    def get_object_links(self, obj: STACObject) -> list[str | pystac.RelType] | None:
         return None
 
     def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
         """Migrate a STAC Object in dict format from a previous version.
         The base implementation will update the stac_extensions to the latest
         schema ID. This method will only be called for STAC objects that have been
         identified as a previous version of STAC. Implementations should directly
         manipulate the obj dict. Remember to call super() in order to change out
         the old 'stac_extension' entry with the latest schema URI.
@@ -62,45 +61,43 @@
                     obj["stac_extensions"][i] = self.schema_uri
                 except ValueError:
                     obj["stac_extensions"].append(self.schema_uri)
                 break
 
 
 class RegisteredExtensionHooks:
-    hooks: Dict[str, ExtensionHooks]
+    hooks: dict[str, ExtensionHooks]
 
     def __init__(self, hooks: Iterable[ExtensionHooks]):
-        self.hooks = dict([(e.schema_uri, e) for e in hooks])
+        self.hooks = {e.schema_uri: e for e in hooks}
 
     def add_extension_hooks(self, hooks: ExtensionHooks) -> None:
         e_id = hooks.schema_uri
         if e_id in self.hooks:
             raise pystac.ExtensionAlreadyExistsError(
-                "ExtensionDefinition with id '{}' already exists.".format(e_id)
+                f"ExtensionDefinition with id '{e_id}' already exists."
             )
 
         self.hooks[e_id] = hooks
 
     def remove_extension_hooks(self, extension_id: str) -> None:
         if extension_id in self.hooks:
             del self.hooks[extension_id]
 
-    def get_extended_object_links(
-        self, obj: STACObject
-    ) -> List[Union[str, pystac.RelType]]:
-        result: Optional[List[Union[str, pystac.RelType]]] = None
+    def get_extended_object_links(self, obj: STACObject) -> list[str | pystac.RelType]:
+        result: list[str | pystac.RelType] | None = None
         for ext in obj.stac_extensions:
             if ext in self.hooks:
                 ext_result = self.hooks[ext].get_object_links(obj)
                 if ext_result is not None:
                     if result is None:
                         result = ext_result
                     else:
                         result.extend(ext_result)
         return result or []
 
     def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
         for hooks in self.hooks.values():
             if info.object_type in hooks._get_stac_object_types():
                 hooks.migrate(obj, version, info)
```

### Comparing `pystac-1.8.4/pystac/extensions/item_assets.py` & `pystac-1.9.0/pystac/extensions/storage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,272 +1,293 @@
-"""Implements the :stac-ext:`Item Assets Definition Extension <item-assets>`."""
+"""Implements the Storage Extension.
+
+https://github.com/stac-extensions/storage
+"""
 
 from __future__ import annotations
 
-from copy import deepcopy
-from typing import Any, Dict, List, Optional
+from collections.abc import Iterable
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
-from pystac.extensions.base import ExtensionManagementMixin
+from pystac.extensions import item_assets
+from pystac.extensions.base import (
+    ExtensionManagementMixin,
+    PropertiesExtension,
+    SummariesExtension,
+)
 from pystac.extensions.hooks import ExtensionHooks
-from pystac.serialization.identify import STACJSONDescription, STACVersionID
-from pystac.utils import get_required
+from pystac.utils import StringEnum
 
-SCHEMA_URI = "https://stac-extensions.github.io/item-assets/v1.0.0/schema.json"
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
-ITEM_ASSETS_PROP = "item_assets"
+SCHEMA_URI: str = "https://stac-extensions.github.io/storage/v1.0.0/schema.json"
+PREFIX: str = "storage:"
 
-ASSET_TITLE_PROP = "title"
-ASSET_DESC_PROP = "description"
-ASSET_TYPE_PROP = "type"
-ASSET_ROLES_PROP = "roles"
+# Field names
+PLATFORM_PROP: str = PREFIX + "platform"
+REGION_PROP: str = PREFIX + "region"
+REQUESTER_PAYS_PROP: str = PREFIX + "requester_pays"
+TIER_PROP: str = PREFIX + "tier"
+
+
+class CloudPlatform(StringEnum):
+    ALIBABA = "ALIBABA"
+    AWS = "AWS"
+    AZURE = "AZURE"
+    GCP = "GCP"
+    IBM = "IBM"
+    ORACLE = "ORACLE"
+    OTHER = "OTHER"
+
+
+class StorageExtension(
+    Generic[T],
+    PropertiesExtension,
+    ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]],
+):
+    """An abstract class that can be used to extend the properties of an
+    :class:`~pystac.Item` or :class:`~pystac.Asset` with properties from the
+    :stac-ext:`Storage Extension <storage>`. This class is generic over the type of
+    STAC Object to be extended (e.g. :class:`~pystac.Item`,
+    :class:`~pystac.Asset`).
 
+    To create a concrete instance of :class:`StorageExtension`, use the
+    :meth:`StorageExtension.ext` method. For example:
 
-class AssetDefinition:
-    """Object that contains details about the datafiles that will be included in member
-    Items for this Collection.
+    .. code-block:: python
 
-    See the :stac-ext:`Asset Object <item-assets#asset-object>` for details.
+       >>> item: pystac.Item = ...
+       >>> storage_ext = StorageExtension.ext(item)
     """
 
-    properties: Dict[str, Any]
-
-    owner: Optional[pystac.Collection]
-
-    def __init__(
-        self, properties: Dict[str, Any], owner: Optional[pystac.Collection] = None
-    ) -> None:
-        self.properties = properties
-        self.owner = owner
-
-    def __eq__(self, o: object) -> bool:
-        if not isinstance(o, AssetDefinition):
-            return NotImplemented
-        return self.to_dict() == o.to_dict()
-
-    @classmethod
-    def create(
-        cls,
-        title: Optional[str],
-        description: Optional[str],
-        media_type: Optional[str],
-        roles: Optional[List[str]],
-        extra_fields: Optional[Dict[str, Any]] = None,
-    ) -> AssetDefinition:
-        """
-        Creates a new asset definition.
-
-        Args:
-            title : Displayed title for clients and users.
-            description : Description of the Asset providing additional details,
-                such as how it was processed or created.
-                `CommonMark 0.29 <http://commonmark.org/>`__ syntax MAY be used
-                for rich text representation.
-            media_type : `media type\
-                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
-                 of the asset.
-            roles : `semantic roles
-                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
-                of the asset, similar to the use of rel in links.
-            extra_fields : Additional fields on the asset definition, e.g. from
-                extensions.
-        """
-        asset_defn = cls({})
-        asset_defn.apply(
-            title=title,
-            description=description,
-            media_type=media_type,
-            roles=roles,
-            extra_fields=extra_fields,
-        )
-        return asset_defn
+    name: Literal["storage"] = "storage"
 
     def apply(
         self,
-        title: Optional[str],
-        description: Optional[str],
-        media_type: Optional[str],
-        roles: Optional[List[str]],
-        extra_fields: Optional[Dict[str, Any]] = None,
+        platform: CloudPlatform | None = None,
+        region: str | None = None,
+        requester_pays: bool | None = None,
+        tier: str | None = None,
     ) -> None:
-        """
-        Sets the properties for this asset definition.
+        """Applies Storage Extension properties to the extended :class:`~pystac.Item` or
+        :class:`~pystac.Asset`.
 
         Args:
-            title : Displayed title for clients and users.
-            description : Description of the Asset providing additional details,
-                such as how it was processed or created.
-                `CommonMark 0.29 <http://commonmark.org/>`__ syntax MAY be used
-                for rich text representation.
-            media_type : `media type\
-                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
-                 of the asset.
-            roles : `semantic roles
-                <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
-                of the asset, similar to the use of rel in links.
-            extra_fields : Additional fields on the asset definition, e.g. from
-                extensions.
+            platform (str, CloudProvider) : The cloud provider where data is stored.
+            region (str) : The region where the data is stored. Relevant to speed of
+                access and inter-region egress costs (as defined by PaaS provider).
+            requester_pays (bool) : Is the data requester pays or is it data
+                manager/cloud provider pays.
+            tier (str) : The title for the tier type (as defined by PaaS provider).
         """
-        if extra_fields:
-            self.properties.update(extra_fields)
-        self.title = title
-        self.description = description
-        self.media_type = media_type
-        self.roles = roles
-        self.owner = None
-
-    def set_owner(self, obj: pystac.Collection) -> None:
-        """Sets the owning item of this AssetDefinition.
+        self.platform = platform
+        self.region = region
+        self.requester_pays = requester_pays
+        self.tier = tier
 
-        The owning item will be used to resolve relative HREFs of this asset.
+    @property
+    def platform(self) -> CloudPlatform | None:
+        """Get or sets the cloud provider where data is stored.
 
-        Args:
-            obj: The Collection that owns this asset.
+        Returns:
+            str or None
         """
-        self.owner = obj
+        return self._get_property(PLATFORM_PROP, CloudPlatform)
 
-    @property
-    def title(self) -> Optional[str]:
-        """Gets or sets the displayed title for clients and users."""
-        return self.properties.get(ASSET_TITLE_PROP)
-
-    @title.setter
-    def title(self, v: Optional[str]) -> None:
-        if v is None:
-            self.properties.pop(ASSET_TITLE_PROP, None)
-        else:
-            self.properties[ASSET_TITLE_PROP] = v
+    @platform.setter
+    def platform(self, v: CloudPlatform | None) -> None:
+        self._set_property(PLATFORM_PROP, v)
 
     @property
-    def description(self) -> Optional[str]:
-        """Gets or sets a description of the Asset providing additional details, such as
-        how it was processed or created. `CommonMark 0.29 <http://commonmark.org/>`__
-        syntax MAY be used for rich text representation."""
-        return self.properties.get(ASSET_DESC_PROP)
-
-    @description.setter
-    def description(self, v: Optional[str]) -> None:
-        if v is None:
-            self.properties.pop(ASSET_DESC_PROP, None)
-        else:
-            self.properties[ASSET_DESC_PROP] = v
+    def region(self) -> str | None:
+        """Gets or sets the region where the data is stored. Relevant to speed of
+        access and inter-region egress costs (as defined by PaaS provider)."""
+        return self._get_property(REGION_PROP, str)
+
+    @region.setter
+    def region(self, v: str | None) -> None:
+        self._set_property(REGION_PROP, v)
 
     @property
-    def media_type(self) -> Optional[str]:
-        """Gets or sets the `media type
-        <https://github.com/radiantearth/stac-spec/tree/v1.0.0/catalog-spec/catalog-spec.md#media-types>`__
-        of the asset."""
-        return self.properties.get(ASSET_TYPE_PROP)
-
-    @media_type.setter
-    def media_type(self, v: Optional[str]) -> None:
-        if v is None:
-            self.properties.pop(ASSET_TYPE_PROP, None)
-        else:
-            self.properties[ASSET_TYPE_PROP] = v
+    def requester_pays(self) -> bool | None:
+        # This value "defaults to false", according to the extension spec.
+        return self._get_property(REQUESTER_PAYS_PROP, bool)
+
+    @requester_pays.setter
+    def requester_pays(self, v: bool | None) -> None:
+        self._set_property(REQUESTER_PAYS_PROP, v)
 
     @property
-    def roles(self) -> Optional[List[str]]:
-        """Gets or sets the `semantic roles
-        <https://github.com/radiantearth/stac-spec/tree/v1.0.0/item-spec/item-spec.md#asset-role-types>`__
-        of the asset, similar to the use of rel in links."""
-        return self.properties.get(ASSET_ROLES_PROP)
-
-    @roles.setter
-    def roles(self, v: Optional[List[str]]) -> None:
-        if v is None:
-            self.properties.pop(ASSET_ROLES_PROP, None)
-        else:
-            self.properties[ASSET_ROLES_PROP] = v
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Returns a dictionary representing this ``AssetDefinition``."""
-        return deepcopy(self.properties)
-
-    def create_asset(self, href: str) -> pystac.Asset:
-        """Creates a new :class:`~pystac.Asset` instance using the fields from this
-        ``AssetDefinition`` and the given ``href``."""
-        return pystac.Asset(
-            href=href,
-            title=self.title,
-            description=self.description,
-            media_type=self.media_type,
-            roles=self.roles,
-            extra_fields={
-                k: v
-                for k, v in self.properties.items()
-                if k
-                not in {
-                    ASSET_TITLE_PROP,
-                    ASSET_DESC_PROP,
-                    ASSET_TYPE_PROP,
-                    ASSET_ROLES_PROP,
-                }
-            },
-        )
-
+    def tier(self) -> str | None:
+        return self._get_property(TIER_PROP, str)
 
-class ItemAssetsExtension(ExtensionManagementMixin[pystac.Collection]):
-    collection: pystac.Collection
-
-    def __init__(self, collection: pystac.Collection) -> None:
-        self.collection = collection
-
-    @property
-    def item_assets(self) -> Dict[str, AssetDefinition]:
-        """Gets or sets a dictionary of assets that can be found in member Items. Maps
-        the asset key to an :class:`AssetDefinition` instance."""
-        result: Dict[str, Any] = get_required(
-            self.collection.extra_fields.get(ITEM_ASSETS_PROP), self, ITEM_ASSETS_PROP
-        )
-        return {k: AssetDefinition(v, self.collection) for k, v in result.items()}
-
-    @item_assets.setter
-    def item_assets(self, v: Dict[str, AssetDefinition]) -> None:
-        self.collection.extra_fields[ITEM_ASSETS_PROP] = {
-            k: asset_def.properties for k, asset_def in v.items()
-        }
-
-    def __repr__(self) -> str:
-        return f"<ItemAssetsExtension collection.id = {self.collection.id}>"
+    @tier.setter
+    def tier(self, v: str | None) -> None:
+        self._set_property(TIER_PROP, v)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def ext(
-        cls, obj: pystac.Collection, add_if_missing: bool = False
-    ) -> ItemAssetsExtension:
-        """Extends the given :class:`~pystac.Collection` with properties from the
-        :stac-ext:`Item Assets Extension <item-assets>`.
+    def ext(cls, obj: T, add_if_missing: bool = False) -> StorageExtension[T]:
+        """Extends the given STAC Object with properties from the :stac-ext:`Storage
+        Extension <storage>`.
+
+        This extension can be applied to instances of :class:`~pystac.Item` or
+        :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
-        if isinstance(obj, pystac.Collection):
-            cls.validate_has_extension(obj, add_if_missing)
-            return cls(obj)
+        if isinstance(obj, pystac.Item):
+            cls.ensure_has_extension(obj, add_if_missing)
+            return cast(StorageExtension[T], ItemStorageExtension(obj))
+        elif isinstance(obj, pystac.Asset):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(StorageExtension[T], AssetStorageExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(StorageExtension[T], ItemAssetsStorageExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
+    @classmethod
+    def summaries(
+        cls, obj: pystac.Collection, add_if_missing: bool = False
+    ) -> SummariesStorageExtension:
+        """Returns the extended summaries object for the given collection."""
+        cls.ensure_has_extension(obj, add_if_missing)
+        return SummariesStorageExtension(obj)
 
-class ItemAssetsExtensionHooks(ExtensionHooks):
-    schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"asset", "item-assets"}
-    stac_object_types = {pystac.STACObjectType.COLLECTION}
 
-    def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
-    ) -> None:
-        # Handle that the "item-assets" extension had the id of "assets", before
-        # collection assets (since removed) took over the ID of "assets"
-        if version < "1.0.0-beta.1" and "asset" in info.extensions:
-            if "assets" in obj:
-                obj["item_assets"] = obj["assets"]
-                del obj["assets"]
+class ItemStorageExtension(StorageExtension[pystac.Item]):
+    """A concrete implementation of :class:`StorageExtension` on an
+    :class:`~pystac.Item` that extends the properties of the Item to include
+    properties defined in the :stac-ext:`Storage Extension <storage>`.
+
+    This class should generally not be instantiated directly. Instead, call
+    :meth:`StorageExtension.ext` on an :class:`~pystac.Item` to extend it.
+    """
+
+    item: pystac.Item
+    """The :class:`~pystac.Item` being extended."""
+
+    properties: dict[str, Any]
+    """The :class:`~pystac.Item` properties, including extension properties."""
 
-        super().migrate(obj, version, info)
+    def __init__(self, item: pystac.Item):
+        self.item = item
+        self.properties = item.properties
+
+    def __repr__(self) -> str:
+        return f"<ItemStorageExtension Item id={self.item.id}>"
+
+
+class AssetStorageExtension(StorageExtension[pystac.Asset]):
+    """A concrete implementation of :class:`StorageExtension` on an
+    :class:`~pystac.Asset` that extends the Asset fields to include properties defined
+    in the :stac-ext:`Storage Extension <storage>`.
+
+    This class should generally not be instantiated directly. Instead, call
+    :meth:`StorageExtension.ext` on an :class:`~pystac.Asset` to extend it.
+    """
+
+    asset_href: str
+    """The ``href`` value of the :class:`~pystac.Asset` being extended."""
+
+    properties: dict[str, Any]
+    """The :class:`~pystac.Asset` fields, including extension properties."""
+
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
+    """If present, this will be a list containing 1 dictionary representing the
+    properties of the owning :class:`~pystac.Item`."""
+
+    def __init__(self, asset: pystac.Asset):
+        self.asset_href = asset.href
+        self.properties = asset.extra_fields
+        if asset.owner and isinstance(asset.owner, pystac.Item):
+            self.additional_read_properties = [asset.owner.properties]
+
+    def __repr__(self) -> str:
+        return f"<AssetStorageExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsStorageExtension(StorageExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
+
+
+class SummariesStorageExtension(SummariesExtension):
+    """A concrete implementation of :class:`~SummariesExtension` that extends
+    the ``summaries`` field of a :class:`~pystac.Collection` to include properties
+    defined in the :stac-ext:`Storage Extension <storage>`.
+    """
+
+    @property
+    def platform(self) -> list[CloudPlatform] | None:
+        """Get or sets the summary of :attr:`StorageExtension.platform` values
+        for this Collection.
+        """
+        return self.summaries.get_list(PLATFORM_PROP)
+
+    @platform.setter
+    def platform(self, v: list[CloudPlatform] | None) -> None:
+        self._set_summary(PLATFORM_PROP, v)
+
+    @property
+    def region(self) -> list[str] | None:
+        """Get or sets the summary of :attr:`StorageExtension.region` values
+        for this Collection.
+        """
+        return self.summaries.get_list(REGION_PROP)
+
+    @region.setter
+    def region(self, v: list[str] | None) -> None:
+        self._set_summary(REGION_PROP, v)
+
+    @property
+    def requester_pays(self) -> list[bool] | None:
+        """Get or sets the summary of :attr:`StorageExtension.requester_pays` values
+        for this Collection.
+        """
+        return self.summaries.get_list(REQUESTER_PAYS_PROP)
+
+    @requester_pays.setter
+    def requester_pays(self, v: list[bool] | None) -> None:
+        self._set_summary(REQUESTER_PAYS_PROP, v)
+
+    @property
+    def tier(self) -> list[str] | None:
+        """Get or sets the summary of :attr:`StorageExtension.tier` values
+        for this Collection.
+        """
+        return self.summaries.get_list(TIER_PROP)
+
+    @tier.setter
+    def tier(self, v: list[str] | None) -> None:
+        self._set_summary(TIER_PROP, v)
+
+
+class StorageExtensionHooks(ExtensionHooks):
+    schema_uri: str = SCHEMA_URI
+    prev_extension_ids: set[str] = set()
+    stac_object_types = {
+        pystac.STACObjectType.COLLECTION,
+        pystac.STACObjectType.ITEM,
+    }
 
 
-ITEM_ASSETS_EXTENSION_HOOKS: ExtensionHooks = ItemAssetsExtensionHooks()
+STORAGE_EXTENSION_HOOKS: ExtensionHooks = StorageExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/label.py` & `pystac-1.9.0/pystac/extensions/label.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """Implements the :stac-ext:`Label Extension <label>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Union, cast
+import warnings
+from collections.abc import Iterable, Sequence
+from typing import Any, Literal, Union, cast
 
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, SummariesExtension
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.serialization.identify import STACJSONDescription, STACVersionID
 from pystac.utils import StringEnum, get_required, map_opt
 
+warnings.warn(
+    "The PySTAC Label Extension is deprecated. The extension itself "
+    '(https://github.com/stac-extensions/label) is currently unmaintained, in "pilot" '
+    "maturity, and has significant issues.",
+    DeprecationWarning,
+)
+
 SCHEMA_URI = "https://stac-extensions.github.io/label/v1.0.1/schema.json"
 SCHEMA_URIS = [
     "https://stac-extensions.github.io/label/v1.0.0/schema.json",
     SCHEMA_URI,
 ]
 PREFIX = "label:"
 
@@ -65,23 +74,23 @@
 
 class LabelClasses:
     """Defines the list of possible class names (e.g., tree, building, car, hippo).
 
     Use :meth:`LabelClasses.create` to create a new instance from property values.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     def apply(
         self,
-        classes: Sequence[Union[str, int, float]],
-        name: Optional[str] = None,
+        classes: Sequence[str | int | float],
+        name: str | None = None,
     ) -> None:
         """Sets the properties for this instance.
 
         Args:
             classes : The different possible class values.
             name : The property key within the asset's each Feature corresponding
                 to class labels. If labels are raster-formatted, do not supply;
@@ -89,47 +98,47 @@
         """
         self.classes = classes
         self.name = name
 
     @classmethod
     def create(
         cls,
-        classes: Sequence[Union[str, int, float]],
-        name: Optional[str] = None,
+        classes: Sequence[str | int | float],
+        name: str | None = None,
     ) -> LabelClasses:
         """Creates a new :class:`~LabelClasses` instance.
 
         Args:
             classes : The different possible class values.
             name : The property key within the asset's each Feature corresponding
                 to class labels. If labels are raster-formatted, do not supply;
                 required otherwise.
         """
         c = cls({})
         c.apply(classes, name)
         return c
 
     @property
-    def classes(self) -> Sequence[Union[str, int, float]]:
+    def classes(self) -> Sequence[str | int | float]:
         """Gets or sets the class values."""
         return get_required(self.properties.get("classes"), self, "classes")
 
     @classes.setter
-    def classes(self, v: Sequence[Union[str, int, float]]) -> None:
+    def classes(self, v: Sequence[str | int | float]) -> None:
         self.properties["classes"] = v
 
     @property
-    def name(self) -> Optional[str]:
+    def name(self) -> str | None:
         """Gets or sets the property key within each Feature in the asset corresponding
         to class labels. If labels are raster-formatted, use ``None``.
         """
         return self.properties.get("name")
 
     @name.setter
-    def name(self, v: Optional[str]) -> None:
+    def name(self, v: str | None) -> None:
         # The "name" property is required but may be null
         self.properties["name"] = v
 
     def __repr__(self) -> str:
         return "<ClassObject classes={}>".format(
             ",".join([str(x) for x in self.classes])
         )
@@ -139,28 +148,28 @@
             o = o.to_dict()
 
         if not isinstance(o, dict):
             return NotImplemented
 
         return self.to_dict() == o
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this label classes object as a dictionary."""
         return self.properties
 
 
 class LabelCount:
     """Contains counts for categorical data.
 
     Use :meth:`LabelCount.create` to create a new instance.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     def apply(self, name: str, count: int) -> None:
         """Sets the properties for this instance.
 
         Args:
             name : One of the different possible classes within the property.
@@ -195,15 +204,15 @@
         """Get or sets the number of occurrences of the class."""
         return get_required(self.properties.get("count"), self, "count")
 
     @count.setter
     def count(self, v: int) -> None:
         self.properties["count"] = v
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this label count object as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelCount):
             o = o.to_dict()
 
@@ -215,17 +224,17 @@
 
 class LabelStatistics:
     """Contains statistics for regression/continuous numeric value data.
 
     Use :meth:`LabelStatistics.create` to create a new instance.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     def apply(self, name: str, value: float) -> None:
         """Sets the property values for this instance.
 
         Args:
             name : The name of the statistic being reported.
@@ -260,15 +269,15 @@
         """Gets or sets the value of the statistic."""
         return get_required(self.properties.get("value"), self, "value")
 
     @value.setter
     def value(self, v: float) -> None:
         self.properties["value"] = v
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this label statistics object as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelStatistics):
             o = o.to_dict()
 
@@ -281,24 +290,24 @@
 class LabelOverview:
     """Stores counts (for classification-type data) or summary statistics (for
     continuous numerical/regression data).
 
     Use :meth:`LabelOverview.create` to create a new instance.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     def apply(
         self,
-        property_key: Optional[str],
-        counts: Optional[List[LabelCount]] = None,
-        statistics: Optional[List[LabelStatistics]] = None,
+        property_key: str | None,
+        counts: list[LabelCount] | None = None,
+        statistics: list[LabelStatistics] | None = None,
     ) -> None:
         """Sets the properties for this instance.
 
         Either ``counts`` or ``statistics``, or both, can be placed in an overview;
         at least one is required.
 
         Args:
@@ -313,17 +322,17 @@
         self.property_key = property_key
         self.counts = counts
         self.statistics = statistics
 
     @classmethod
     def create(
         cls,
-        property_key: Optional[str],
-        counts: Optional[List[LabelCount]] = None,
-        statistics: Optional[List[LabelStatistics]] = None,
+        property_key: str | None,
+        counts: list[LabelCount] | None = None,
+        statistics: list[LabelStatistics] | None = None,
     ) -> LabelOverview:
         """Creates a new instance.
 
         Either ``counts`` or ``statistics``, or both, can be placed in an overview;
         at least one is required.
 
         Args:
@@ -335,62 +344,60 @@
                 for regression/continuous numeric value data.
         """
         x = LabelOverview({})
         x.apply(property_key, counts, statistics)
         return x
 
     @property
-    def property_key(self) -> Optional[str]:
+    def property_key(self) -> str | None:
         """Gets or sets the property key within the asset corresponding to class
         labels."""
         return self.properties.get("property_key")
 
     @property_key.setter
-    def property_key(self, v: Optional[str]) -> None:
+    def property_key(self, v: str | None) -> None:
         self.properties["property_key"] = v
 
     @property
-    def counts(self) -> Optional[List[LabelCount]]:
+    def counts(self) -> list[LabelCount] | None:
         """Gets or sets the list of :class:`LabelCounts` containing counts for
         categorical data."""
         counts = self.properties.get("counts")
         if counts is None:
             return None
         return [LabelCount(c) for c in counts]
 
     @counts.setter
-    def counts(self, v: Optional[List[LabelCount]]) -> None:
+    def counts(self, v: list[LabelCount] | None) -> None:
         if v is None:
             self.properties.pop("counts", None)
         else:
             if not isinstance(v, list):
-                raise pystac.STACError(
-                    "counts must be a list! Invalid input: {}".format(v)
-                )
+                raise pystac.STACError(f"counts must be a list! Invalid input: {v}")
 
             self.properties["counts"] = [c.to_dict() for c in v]
 
     @property
-    def statistics(self) -> Optional[List[LabelStatistics]]:
+    def statistics(self) -> list[LabelStatistics] | None:
         """Gets or sets the list of :class:`LabelStatistics` containing statistics for
         regression/continuous numeric value data."""
         statistics = self.properties.get("statistics")
         if statistics is None:
             return None
 
         return [LabelStatistics(s) for s in statistics]
 
     @statistics.setter
-    def statistics(self, v: Optional[List[LabelStatistics]]) -> None:
+    def statistics(self, v: list[LabelStatistics] | None) -> None:
         if v is None:
             self.properties.pop("statistics", None)
         else:
             self.properties["statistics"] = [s.to_dict() for s in v]
 
-    def merge_counts(self, other: "LabelOverview") -> LabelOverview:
+    def merge_counts(self, other: LabelOverview) -> LabelOverview:
         """Merges the counts associated with this overview with another overview.
         Creates a new instance.
 
         Args:
             other : The other LabelOverview to merge.
 
         Returns:
@@ -401,29 +408,29 @@
 
         if self.counts is None:
             new_counts = other.counts
         else:
             if other.counts is None:
                 new_counts = self.counts
             else:
-                count_by_prop: Dict[str, int] = {}
+                count_by_prop: dict[str, int] = {}
 
-                def add_counts(counts: List[LabelCount]) -> None:
+                def add_counts(counts: list[LabelCount]) -> None:
                     for c in counts:
                         if c.name not in count_by_prop:
                             count_by_prop[c.name] = c.count
                         else:
                             count_by_prop[c.name] += c.count
 
                 add_counts(self.counts)
                 add_counts(other.counts)
                 new_counts = [LabelCount.create(k, v) for k, v in count_by_prop.items()]
         return LabelOverview.create(self.property_key, counts=new_counts)
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this label overview as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if isinstance(o, LabelOverview):
             o = o.to_dict()
 
@@ -442,30 +449,31 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> label_ext = LabelExtension.ext(item)
     """
 
+    name: Literal["label"] = "label"
     obj: pystac.Item
     schema_uri: str
 
     def __init__(self, item: pystac.Item) -> None:
         self.obj = item
         self.schema_uri = SCHEMA_URI
 
     def apply(
         self,
         label_description: str,
         label_type: LabelType,
-        label_properties: Optional[List[str]] = None,
-        label_classes: Optional[List[LabelClasses]] = None,
-        label_tasks: Optional[List[Union[LabelTask, str]]] = None,
-        label_methods: Optional[List[Union[LabelMethod, str]]] = None,
-        label_overviews: Optional[List[LabelOverview]] = None,
+        label_properties: list[str] | None = None,
+        label_classes: list[LabelClasses] | None = None,
+        label_tasks: list[LabelTask | str] | None = None,
+        label_methods: list[LabelMethod | str] | None = None,
+        label_overviews: list[LabelOverview] | None = None,
     ) -> None:
         """Applies label extension properties to the extended Item.
 
         Args:
             label_description : A description of the label, how it was created,
                 and what it is recommended for
             label_type : An Enum of either vector label type or raster label type. Use
@@ -514,104 +522,104 @@
         )
 
     @label_type.setter
     def label_type(self, v: LabelType) -> None:
         self.obj.properties[TYPE_PROP] = v
 
     @property
-    def label_properties(self) -> Optional[List[str]]:
+    def label_properties(self) -> list[str] | None:
         """Gets or sets the names of the property field(s) in each
         Feature of the label asset's FeatureCollection that contains the classes
         (keywords from label:classes if the property defines classes).
         If labels are rasters, this should be None."""
         return self.obj.properties.get(PROPERTIES_PROP)
 
     @label_properties.setter
-    def label_properties(self, v: Optional[List[str]]) -> None:
+    def label_properties(self, v: list[str] | None) -> None:
         self.obj.properties[PROPERTIES_PROP] = v
 
     @property
-    def label_classes(self) -> Optional[List[LabelClasses]]:
+    def label_classes(self) -> list[LabelClasses] | None:
         """Gets or set a list of :class:`LabelClasses` defining the list of possible
         class names for each label:properties. (e.g., tree, building, car, hippo).
 
         Optional, but required if using categorical data."""
         label_classes = self.obj.properties.get(CLASSES_PROP)
         if label_classes is not None:
             return [LabelClasses(classes) for classes in label_classes]
         else:
             return None
 
     @label_classes.setter
-    def label_classes(self, v: Optional[List[LabelClasses]]) -> None:
+    def label_classes(self, v: list[LabelClasses] | None) -> None:
         if v is None:
             self.obj.properties.pop(CLASSES_PROP, None)
         else:
             if not isinstance(v, list):
                 raise pystac.STACError(
-                    "label_classes must be a list! Invalid input: {}".format(v)
+                    f"label_classes must be a list! Invalid input: {v}"
                 )
 
             classes = [x.to_dict() for x in v]
             self.obj.properties[CLASSES_PROP] = classes
 
     @property
-    def label_tasks(self) -> Optional[List[Union[LabelTask, str]]]:
+    def label_tasks(self) -> list[LabelTask | str] | None:
         """Gets or set a list of tasks these labels apply to. Usually a subset of
         'regression', 'classification', 'detection', or 'segmentation', but may be
         arbitrary values."""
         return self.obj.properties.get(TASKS_PROP)
 
     @label_tasks.setter
-    def label_tasks(self, v: Optional[List[Union[LabelTask, str]]]) -> None:
+    def label_tasks(self, v: list[LabelTask | str] | None) -> None:
         if v is None:
             self.obj.properties.pop(TASKS_PROP, None)
         else:
             self.obj.properties[TASKS_PROP] = v
 
     @property
-    def label_methods(self) -> Optional[List[Union[LabelMethod, str]]]:
+    def label_methods(self) -> list[LabelMethod | str] | None:
         """Gets or set a list of methods used for labeling.
 
         Usually a subset of 'automated' or 'manual', but may be arbitrary values."""
         return self.obj.properties.get("label:methods")
 
     @label_methods.setter
-    def label_methods(self, v: Optional[List[Union[LabelMethod, str]]]) -> None:
+    def label_methods(self, v: list[LabelMethod | str] | None) -> None:
         if v is None:
             self.obj.properties.pop("label:methods", None)
         else:
             self.obj.properties["label:methods"] = v
 
     @property
-    def label_overviews(self) -> Optional[List[LabelOverview]]:
+    def label_overviews(self) -> list[LabelOverview] | None:
         """Gets or set a list of :class:`LabelOverview` instances
         that store counts (for classification-type data) or summary statistics (for
         continuous numerical/regression data)."""
         overviews = self.obj.properties.get(OVERVIEWS_PROP)
         if overviews is not None:
             return [LabelOverview(overview) for overview in overviews]
         else:
             return None
 
     @label_overviews.setter
-    def label_overviews(self, v: Optional[List[LabelOverview]]) -> None:
+    def label_overviews(self, v: list[LabelOverview] | None) -> None:
         if v is None:
             self.obj.properties.pop(OVERVIEWS_PROP, None)
         else:
             self.obj.properties[OVERVIEWS_PROP] = [x.to_dict() for x in v]
 
     def __repr__(self) -> str:
-        return "<LabelItemExt Item id={}>".format(self.obj.id)
+        return f"<LabelItemExt Item id={self.obj.id}>"
 
     def add_source(
         self,
         source_item: pystac.Item,
-        title: Optional[str] = None,
-        assets: Optional[List[str]] = None,
+        title: str | None = None,
+        assets: list[str] | None = None,
     ) -> None:
         """Adds a link to a source item.
 
         Args:
             source_item : Source imagery that the LabelItem applies to.
             title : Optional title for the link.
             assets : Optional list of assets that determine what
@@ -638,17 +646,17 @@
             LabelItem that have ``rel=='source'``.
         """
         return map(lambda x: cast(pystac.Item, x), self.obj.get_stac_objects("source"))
 
     def add_labels(
         self,
         href: str,
-        title: Optional[str] = None,
-        media_type: Optional[str] = None,
-        properties: Optional[Dict[str, Any]] = None,
+        title: str | None = None,
+        media_type: str | None = None,
+        properties: dict[str, Any] | None = None,
     ) -> None:
         """Adds a label asset to this LabelItem.
 
         Args:
             href : Link to the asset object. Relative and absolute links are both
                 allowed.
             title : Optional displayed title for clients and users.
@@ -666,16 +674,16 @@
                 href=href, title=title, media_type=media_type, extra_fields=properties
             ),
         )
 
     def add_geojson_labels(
         self,
         href: str,
-        title: Optional[str] = None,
-        properties: Optional[Dict[str, Any]] = None,
+        title: str | None = None,
+        properties: dict[str, Any] | None = None,
     ) -> None:
         """Adds a GeoJSON label asset to this LabelItem.
 
         Args:
             href : Link to the asset object. Relative and absolute links are both
                 allowed.
             title : Optional displayed title for clients and users.
@@ -691,128 +699,132 @@
         )
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def get_schema_uris(cls) -> List[str]:
+    def get_schema_uris(cls) -> list[str]:
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
         return SCHEMA_URIS
 
     @classmethod
     def ext(cls, obj: pystac.Item, add_if_missing: bool = False) -> LabelExtension:
         """Extends the given STAC Object with properties from the :stac-ext:`Label
         Extension <label>`.
 
         This extension can be applied to instances of :class:`~pystac.Item`.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cls(obj)
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesLabelExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesLabelExtension(obj)
 
 
 class SummariesLabelExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Label Extension <label>`.
     """
 
     @property
-    def label_properties(self) -> Optional[List[str]]:
+    def label_properties(self) -> list[str] | None:
         """Get or sets the summary of :attr:`LabelExtension.label_properties` values
         for this Collection.
         """
 
         return self.summaries.get_list(PROPERTIES_PROP)
 
     @label_properties.setter
-    def label_properties(self, v: Optional[List[str]]) -> None:
+    def label_properties(self, v: list[str] | None) -> None:
         self._set_summary(PROPERTIES_PROP, v)
 
     @property
-    def label_classes(self) -> Optional[List[LabelClasses]]:
+    def label_classes(self) -> list[LabelClasses] | None:
         """Get or sets the summary of :attr:`LabelExtension.label_classes` values
         for this Collection.
         """
 
         return map_opt(
             lambda classes: [LabelClasses(c) for c in classes],
             self.summaries.get_list(CLASSES_PROP),
         )
 
     @label_classes.setter
-    def label_classes(self, v: Optional[List[LabelClasses]]) -> None:
+    def label_classes(self, v: list[LabelClasses] | None) -> None:
         self._set_summary(
             CLASSES_PROP, map_opt(lambda classes: [c.to_dict() for c in classes], v)
         )
 
     @property
-    def label_type(self) -> Optional[List[LabelType]]:
+    def label_type(self) -> list[LabelType] | None:
         """Get or sets the summary of :attr:`LabelExtension.label_type` values
         for this Collection.
         """
 
         return self.summaries.get_list(TYPE_PROP)
 
     @label_type.setter
-    def label_type(self, v: Optional[List[LabelType]]) -> None:
+    def label_type(self, v: list[LabelType] | None) -> None:
         self._set_summary(TYPE_PROP, v)
 
     @property
-    def label_tasks(self) -> Optional[List[Union[LabelTask, str]]]:
+    def label_tasks(self) -> list[LabelTask | str] | None:
         """Get or sets the summary of :attr:`LabelExtension.label_tasks` values
         for this Collection.
         """
 
         return self.summaries.get_list(TASKS_PROP)
 
     @label_tasks.setter
-    def label_tasks(self, v: Optional[List[Union[LabelTask, str]]]) -> None:
+    def label_tasks(self, v: list[LabelTask | str] | None) -> None:
         self._set_summary(TASKS_PROP, v)
 
     @property
-    def label_methods(self) -> Optional[List[Union[LabelMethod, str]]]:
+    def label_methods(self) -> list[LabelMethod | str] | None:
         """Get or sets the summary of :attr:`LabelExtension.label_methods` values
         for this Collection.
         """
 
         return self.summaries.get_list(METHODS_PROP)
 
     @label_methods.setter
-    def label_methods(self, v: Optional[List[Union[LabelMethod, str]]]) -> None:
+    def label_methods(self, v: list[LabelMethod | str] | None) -> None:
         self._set_summary(METHODS_PROP, v)
 
 
 class LabelExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {
         "label",
         *[uri for uri in SCHEMA_URIS if uri != SCHEMA_URI],
     }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
     def get_object_links(
         self, so: pystac.STACObject
-    ) -> Optional[List[Union[str, pystac.RelType]]]:
+    ) -> list[str | pystac.RelType] | None:
         if isinstance(so, pystac.Item):
             return [LabelRelType.SOURCE]
         return None
 
     def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
         if info.object_type == pystac.STACObjectType.ITEM and version < "1.0.0":
             props = obj["properties"]
             # Migrate 0.8.0-rc1 non-pluralized forms
             # As it's a common mistake, convert for any pre-1.0.0 version.
             if "label:property" in props and PROPERTIES_PROP not in props:
                 props[PROPERTIES_PROP] = props["label:property"]
```

### Comparing `pystac-1.8.4/pystac/extensions/mgrs.py` & `pystac-1.9.0/pystac/extensions/mgrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Implements the :stac-ext:`MGRS Extension <mgrs>`."""
 
 import re
-from typing import Any, Dict, FrozenSet, Optional, Pattern, Set, Union
+from re import Pattern
+from typing import Any, Literal, Optional, Union
 
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/mgrs/v1.0.0/schema.json"
+SCHEMA_STARTSWITH: str = "https://stac-extensions.github.io/mgrs/"
 PREFIX: str = "mgrs:"
 
 # Field names
 LATITUDE_BAND_PROP: str = PREFIX + "latitude_band"  # required
 GRID_SQUARE_PROP: str = PREFIX + "grid_square"  # required
 UTM_ZONE_PROP: str = PREFIX + "utm_zone"
 
-LATITUDE_BANDS: FrozenSet[str] = frozenset(
+LATITUDE_BANDS: frozenset[str] = frozenset(
     {
         "C",
         "D",
         "E",
         "F",
         "G",
         "H",
@@ -36,15 +38,15 @@
         "U",
         "V",
         "W",
         "X",
     }
 )
 
-UTM_ZONES: FrozenSet[int] = frozenset(
+UTM_ZONES: frozenset[int] = frozenset(
     {
         1,
         2,
         3,
         4,
         5,
         6,
@@ -151,26 +153,27 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> proj_ext = MgrsExtension.ext(item)
     """
 
+    name: Literal["mgrs"] = "mgrs"
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemMgrsExtension Item id={}>".format(self.item.id)
+        return f"<ItemMgrsExtension Item id={self.item.id}>"
 
     def apply(
         self,
         latitude_band: str,
         grid_square: str,
         utm_zone: Optional[int] = None,
     ) -> None:
@@ -228,20 +231,20 @@
         This extension can be applied to instances of :class:`~pystac.Item`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return MgrsExtension(obj)
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class MgrsExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids: Set[str] = set()
+    prev_extension_ids: set[str] = set()
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
 MGRS_EXTENSION_HOOKS: ExtensionHooks = MgrsExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/pointcloud.py` & `pystac-1.9.0/pystac/extensions/pointcloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """Implements the :stac-ext:`Point Cloud Extension <pointcloud>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union, cast
+from collections.abc import Iterable
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.summaries import RangeSummary
 from pystac.utils import StringEnum, get_required, map_opt
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/pointcloud/v1.0.0/schema.json"
 PREFIX: str = "pc:"
 
 COUNT_PROP = PREFIX + "count"
 TYPE_PROP = PREFIX + "type"
 ENCODING_PROP = PREFIX + "encoding"
@@ -50,17 +59,17 @@
 class Schema:
     """Defines a schema for dimension of a pointcloud (e.g., name, size, type)
 
     Use :meth:`Schema.create` to create a new instance of ``Schema`` from
     properties.
     """
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     def apply(self, name: str, size: int, type: SchemaType) -> None:
         """Sets the properties for this Schema.
 
         Args:
            name : The name of dimension.
@@ -90,15 +99,15 @@
     def size(self) -> int:
         """Gets or sets the size value."""
         return get_required(self.properties.get("size"), self, "size")
 
     @size.setter
     def size(self, v: int) -> None:
         if not isinstance(v, int):
-            raise pystac.STACError("size must be an int! Invalid input: {}".format(v))
+            raise pystac.STACError(f"size must be an int! Invalid input: {v}")
 
         self.properties["size"] = v
 
     @property
     def name(self) -> str:
         """Gets or sets the name property for this Schema."""
         return get_required(self.properties.get("name"), self, "name")
@@ -120,40 +129,40 @@
     def __repr__(self) -> str:
         return "<Schema name={} size={} type={}>".format(
             self.properties.get("name"),
             self.properties.get("size"),
             self.properties.get("type"),
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this schema as a dictionary."""
         return self.properties
 
 
 class Statistic:
     """Defines a single statistic for Pointcloud channel or dimension
 
     Use :meth:`Statistic.create` to create a new instance of
     ``Statistic`` from property values."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]) -> None:
+    def __init__(self, properties: dict[str, Any]) -> None:
         self.properties = properties
 
     def apply(
         self,
         name: str,
-        position: Optional[int] = None,
-        average: Optional[float] = None,
-        count: Optional[int] = None,
-        maximum: Optional[float] = None,
-        minimum: Optional[float] = None,
-        stddev: Optional[float] = None,
-        variance: Optional[float] = None,
+        position: int | None = None,
+        average: float | None = None,
+        count: int | None = None,
+        maximum: float | None = None,
+        minimum: float | None = None,
+        stddev: float | None = None,
+        variance: float | None = None,
     ) -> None:
         """Sets the properties for this Statistic.
 
         Args:
             name : REQUIRED. The name of the channel.
             position : Optional position of the channel in the schema.
             average : Optional average of the channel.
@@ -172,21 +181,21 @@
         self.properties["stddev"] = stddev
         self.properties["variance"] = variance
 
     @classmethod
     def create(
         cls,
         name: str,
-        position: Optional[int] = None,
-        average: Optional[float] = None,
-        count: Optional[int] = None,
-        maximum: Optional[float] = None,
-        minimum: Optional[float] = None,
-        stddev: Optional[float] = None,
-        variance: Optional[float] = None,
+        position: int | None = None,
+        average: float | None = None,
+        count: int | None = None,
+        maximum: float | None = None,
+        minimum: float | None = None,
+        stddev: float | None = None,
+        variance: float | None = None,
     ) -> Statistic:
         """Creates a new Statistic class.
 
         Args:
             name : REQUIRED. The name of the channel.
             position : Optional position of the channel in the schema.
             average : Optional average of the channel.
@@ -218,101 +227,101 @@
     def name(self, v: str) -> None:
         if v is not None:
             self.properties["name"] = v
         else:
             self.properties.pop("name", None)
 
     @property
-    def position(self) -> Optional[int]:
+    def position(self) -> int | None:
         """Gets or sets the position property."""
         return self.properties.get("position")
 
     @position.setter
-    def position(self, v: Optional[int]) -> None:
+    def position(self, v: int | None) -> None:
         if v is not None:
             self.properties["position"] = v
         else:
             self.properties.pop("position", None)
 
     @property
-    def average(self) -> Optional[float]:
+    def average(self) -> float | None:
         """Gets or sets the average property."""
         return self.properties.get("average")
 
     @average.setter
-    def average(self, v: Optional[float]) -> None:
+    def average(self, v: float | None) -> None:
         if v is not None:
             self.properties["average"] = v
         else:
             self.properties.pop("average", None)
 
     @property
-    def count(self) -> Optional[int]:
+    def count(self) -> int | None:
         """Gets or sets the count property."""
         return self.properties.get("count")
 
     @count.setter
-    def count(self, v: Optional[int]) -> None:
+    def count(self, v: int | None) -> None:
         if v is not None:
             self.properties["count"] = v
         else:
             self.properties.pop("count", None)
 
     @property
-    def maximum(self) -> Optional[float]:
+    def maximum(self) -> float | None:
         """Gets or sets the maximum property."""
         return self.properties.get("maximum")
 
     @maximum.setter
-    def maximum(self, v: Optional[float]) -> None:
+    def maximum(self, v: float | None) -> None:
         if v is not None:
             self.properties["maximum"] = v
         else:
             self.properties.pop("maximum", None)
 
     @property
-    def minimum(self) -> Optional[float]:
+    def minimum(self) -> float | None:
         """Gets or sets the minimum property."""
         return self.properties.get("minimum")
 
     @minimum.setter
-    def minimum(self, v: Optional[float]) -> None:
+    def minimum(self, v: float | None) -> None:
         if v is not None:
             self.properties["minimum"] = v
         else:
             self.properties.pop("minimum", None)
 
     @property
-    def stddev(self) -> Optional[float]:
+    def stddev(self) -> float | None:
         """Gets or sets the stddev property."""
         return self.properties.get("stddev")
 
     @stddev.setter
-    def stddev(self, v: Optional[float]) -> None:
+    def stddev(self, v: float | None) -> None:
         if v is not None:
             self.properties["stddev"] = v
         else:
             self.properties.pop("stddev", None)
 
     @property
-    def variance(self) -> Optional[float]:
+    def variance(self) -> float | None:
         """Gets or sets the variance property."""
         return self.properties.get("variance")
 
     @variance.setter
-    def variance(self, v: Optional[float]) -> None:
+    def variance(self, v: float | None) -> None:
         if v is not None:
             self.properties["variance"] = v
         else:
             self.properties.pop("variance", None)
 
     def __repr__(self) -> str:
-        return "<Statistic statistics={}>".format(str(self.properties))
+        return f"<Statistic statistics={str(self.properties)}>"
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this statistic as a dictionary."""
         return self.properties
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, Statistic):
             return NotImplemented
         return self.to_dict() == o.to_dict()
@@ -334,22 +343,24 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> pc_ext = PointcloudExtension.ext(item)
     """
 
+    name: Literal["pc"] = "pc"
+
     def apply(
         self,
         count: int,
-        type: Union[PhenomenologyType, str],
+        type: PhenomenologyType | str,
         encoding: str,
-        schemas: List[Schema],
-        density: Optional[float] = None,
-        statistics: Optional[List[Statistic]] = None,
+        schemas: list[Schema],
+        density: float | None = None,
+        statistics: list[Statistic] | None = None,
     ) -> None:
         """Applies Pointcloud extension properties to the extended Item.
 
         Args:
             count : REQUIRED. The number of points in the cloud.
             type : REQUIRED. Phenomenology type for the point cloud. Possible valid
                 values might include lidar, eopc, radar, sonar, or otherThe type of file
@@ -374,64 +385,64 @@
         return get_required(self._get_property(COUNT_PROP, int), self, COUNT_PROP)
 
     @count.setter
     def count(self, v: int) -> None:
         self._set_property(COUNT_PROP, v, pop_if_none=False)
 
     @property
-    def type(self) -> Union[PhenomenologyType, str]:
+    def type(self) -> PhenomenologyType | str:
         """Gets or sets the phenomenology type for the point cloud."""
         return get_required(self._get_property(TYPE_PROP, str), self, TYPE_PROP)
 
     @type.setter
-    def type(self, v: Union[PhenomenologyType, str]) -> None:
+    def type(self, v: PhenomenologyType | str) -> None:
         self._set_property(TYPE_PROP, v, pop_if_none=False)
 
     @property
     def encoding(self) -> str:
         """Gets or sets the content encoding or format of the data."""
         return get_required(self._get_property(ENCODING_PROP, str), self, ENCODING_PROP)
 
     @encoding.setter
     def encoding(self, v: str) -> None:
         self._set_property(ENCODING_PROP, v, pop_if_none=False)
 
     @property
-    def schemas(self) -> List[Schema]:
+    def schemas(self) -> list[Schema]:
         """Gets or sets the list of :class:`Schema` instances defining
         dimensions and types for the data.
         """
         result = get_required(
-            self._get_property(SCHEMAS_PROP, List[Dict[str, Any]]), self, SCHEMAS_PROP
+            self._get_property(SCHEMAS_PROP, list[dict[str, Any]]), self, SCHEMAS_PROP
         )
         return [Schema(s) for s in result]
 
     @schemas.setter
-    def schemas(self, v: List[Schema]) -> None:
+    def schemas(self, v: list[Schema]) -> None:
         self._set_property(SCHEMAS_PROP, [x.to_dict() for x in v], pop_if_none=False)
 
     @property
-    def density(self) -> Optional[float]:
+    def density(self) -> float | None:
         """Gets or sets the number of points per square unit area."""
         return self._get_property(DENSITY_PROP, float)
 
     @density.setter
-    def density(self, v: Optional[float]) -> None:
+    def density(self, v: float | None) -> None:
         self._set_property(DENSITY_PROP, v)
 
     @property
-    def statistics(self) -> Optional[List[Statistic]]:
+    def statistics(self) -> list[Statistic] | None:
         """Gets or sets the list of :class:`Statistic` instances describing
         the pre-channel statistics. Elements in this list map to elements in the
         :attr:`PointcloudExtension.schemas` list."""
-        result = self._get_property(STATISTICS_PROP, List[Dict[str, Any]])
+        result = self._get_property(STATISTICS_PROP, list[dict[str, Any]])
         return map_opt(lambda stats: [Statistic(s) for s in stats], result)
 
     @statistics.setter
-    def statistics(self, v: Optional[List[Statistic]]) -> None:
+    def statistics(self, v: list[Statistic] | None) -> None:
         set_value = map_opt(lambda stats: [s.to_dict() for s in stats], v)
         self._set_property(STATISTICS_PROP, set_value)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
@@ -444,70 +455,73 @@
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(PointcloudExtension[T], ItemPointcloudExtension(obj))
         elif isinstance(obj, pystac.Asset):
             if obj.owner is not None and not isinstance(obj.owner, pystac.Item):
                 raise pystac.ExtensionTypeError(
                     "Pointcloud extension does not apply to Collection Assets."
                 )
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(PointcloudExtension[T], AssetPointcloudExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(PointcloudExtension[T], ItemAssetsPointcloudExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesPointcloudExtension:
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesPointcloudExtension(obj)
 
 
 class ItemPointcloudExtension(PointcloudExtension[pystac.Item]):
     """A concrete implementation of :class:`PointcloudExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include
     properties defined in the :stac-ext:`Point Cloud Extension <pointcloud>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`PointcloudExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemPointcloudExtension Item id={}>".format(self.item.id)
+        return f"<ItemPointcloudExtension Item id={self.item.id}>"
 
 
 class AssetPointcloudExtension(PointcloudExtension[pystac.Asset]):
     """A concrete implementation of :class:`PointcloudExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties defined
     in the :stac-ext:`Point Cloud Extension <pointcloud>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`PointcloudExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
@@ -516,61 +530,70 @@
         else:
             self.repr_id = f"href={asset.href}"
 
     def __repr__(self) -> str:
         return f"<AssetPointcloudExtension Asset {self.repr_id}>"
 
 
+class ItemAssetsPointcloudExtension(PointcloudExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
+
+
 class SummariesPointcloudExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Point Cloud Extension <pointcloud>`.
     """
 
     @property
-    def count(self) -> Optional[RangeSummary[int]]:
+    def count(self) -> RangeSummary[int] | None:
         return self.summaries.get_range(COUNT_PROP)
 
     @count.setter
-    def count(self, v: Optional[RangeSummary[int]]) -> None:
+    def count(self, v: RangeSummary[int] | None) -> None:
         self._set_summary(COUNT_PROP, v)
 
     @property
-    def type(self) -> Optional[List[Union[PhenomenologyType, str]]]:
+    def type(self) -> list[PhenomenologyType | str] | None:
         return self.summaries.get_list(TYPE_PROP)
 
     @type.setter
-    def type(self, v: Optional[List[Union[PhenomenologyType, str]]]) -> None:
+    def type(self, v: list[PhenomenologyType | str] | None) -> None:
         self._set_summary(TYPE_PROP, v)
 
     @property
-    def encoding(self) -> Optional[List[str]]:
+    def encoding(self) -> list[str] | None:
         return self.summaries.get_list(ENCODING_PROP)
 
     @encoding.setter
-    def encoding(self, v: Optional[List[str]]) -> None:
+    def encoding(self, v: list[str] | None) -> None:
         self._set_summary(ENCODING_PROP, v)
 
     @property
-    def density(self) -> Optional[RangeSummary[float]]:
+    def density(self) -> RangeSummary[float] | None:
         return self.summaries.get_range(DENSITY_PROP)
 
     @density.setter
-    def density(self, v: Optional[RangeSummary[float]]) -> None:
+    def density(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(DENSITY_PROP, v)
 
     @property
-    def statistics(self) -> Optional[List[Statistic]]:
+    def statistics(self) -> list[Statistic] | None:
         return map_opt(
             lambda stats: [Statistic(d) for d in stats],
             self.summaries.get_list(STATISTICS_PROP),
         )
 
     @statistics.setter
-    def statistics(self, v: Optional[List[Statistic]]) -> None:
+    def statistics(self, v: list[Statistic] | None) -> None:
         self._set_summary(
             STATISTICS_PROP,
             map_opt(lambda stats: [s.to_dict() for s in stats], v),
         )
 
 
 class PointcloudExtensionHooks(ExtensionHooks):
```

### Comparing `pystac-1.8.4/pystac/extensions/projection.py` & `pystac-1.9.0/pystac/extensions/projection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 """Implements the :stac-ext:`Projection Extension <projection>`."""
 
 from __future__ import annotations
 
 import json
-from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union, cast
+import warnings
+from collections.abc import Iterable
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/projection/v1.1.0/schema.json"
-SCHEMA_URIS: List[str] = [
+SCHEMA_URIS: list[str] = [
     "https://stac-extensions.github.io/projection/v1.0.0/schema.json",
     SCHEMA_URI,
 ]
 PREFIX: str = "proj:"
 
 # Field names
 EPSG_PROP: str = PREFIX + "epsg"
@@ -48,24 +58,26 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> proj_ext = ProjectionExtension.ext(item)
     """
 
+    name: Literal["proj"] = "proj"
+
     def apply(
         self,
-        epsg: Optional[int],
-        wkt2: Optional[str] = None,
-        projjson: Optional[Dict[str, Any]] = None,
-        geometry: Optional[Dict[str, Any]] = None,
-        bbox: Optional[List[float]] = None,
-        centroid: Optional[Dict[str, float]] = None,
-        shape: Optional[List[int]] = None,
-        transform: Optional[List[float]] = None,
+        epsg: int | None,
+        wkt2: str | None = None,
+        projjson: dict[str, Any] | None = None,
+        geometry: dict[str, Any] | None = None,
+        bbox: list[float] | None = None,
+        centroid: dict[str, float] | None = None,
+        shape: list[int] | None = None,
+        transform: list[float] | None = None,
     ) -> None:
         """Applies Projection extension properties to the extended Item.
 
         Args:
             epsg : REQUIRED. EPSG code of the datasource.
             wkt2 : WKT2 string representing the Coordinate Reference
                 System (CRS) that the ``geometry`` and ``bbox`` fields represent
@@ -91,71 +103,71 @@
         self.geometry = geometry
         self.bbox = bbox
         self.centroid = centroid
         self.shape = shape
         self.transform = transform
 
     @property
-    def epsg(self) -> Optional[int]:
+    def epsg(self) -> int | None:
         """Get or sets the EPSG code of the datasource.
 
         A Coordinate Reference System (CRS) is the data reference system (sometimes
         called a 'projection') used by the asset data, and can usually be referenced
         using an `EPSG code <https://epsg.io/>`_.
         If the asset data does not have a CRS, such as in the case of non-rectified
         imagery with Ground Control Points, ``epsg`` should be set to ``None``.
         It should also be set to ``None`` if a CRS exists, but for which there is no
         valid EPSG code.
         """
         return self._get_property(EPSG_PROP, int)
 
     @epsg.setter
-    def epsg(self, v: Optional[int]) -> None:
+    def epsg(self, v: int | None) -> None:
         self._set_property(EPSG_PROP, v, pop_if_none=False)
 
     @property
-    def wkt2(self) -> Optional[str]:
+    def wkt2(self) -> str | None:
         """Get or sets the WKT2 string representing the Coordinate Reference System
         (CRS) that the ``proj:geometry`` and ``proj:bbox`` fields represent
 
         This value is a
         `WKT2 string <https://docs.opengeospatial.org/is/12-063r5/12-063r5.html>`_.
         If the data does not have a CRS, such as in the case of non-rectified imagery
         with Ground Control Points, ``wkt2`` should be set to ``None``. It should also
         be set to ``None`` if a CRS exists, but for which a WKT2 string does not exist.
         """
         return self._get_property(WKT2_PROP, str)
 
     @wkt2.setter
-    def wkt2(self, v: Optional[str]) -> None:
+    def wkt2(self, v: str | None) -> None:
         self._set_property(WKT2_PROP, v)
 
     @property
-    def projjson(self) -> Optional[Dict[str, Any]]:
+    def projjson(self) -> dict[str, Any] | None:
         """Get or sets the PROJJSON string representing the Coordinate Reference System
         (CRS) that the ``proj:geometry`` and ``proj:bbox`` fields represent
 
         This value is a
         `PROJJSON object <https://proj.org/specifications/projjson.html>`_.
         If the data does not have a CRS, such as in the case of non-rectified imagery
         with Ground Control Points, ``projjson`` should be set to ``None``. It should
         also be set to ``None`` if a CRS exists, but for which a PROJJSON string does
         not exist.
 
         The schema for this object can be found
         `here <https://proj.org/schemas/v0.2/projjson.schema.json>`_.
         """
-        return self._get_property(PROJJSON_PROP, Dict[str, Any])
+        return self._get_property(PROJJSON_PROP, dict[str, Any])
 
     @projjson.setter
-    def projjson(self, v: Optional[Dict[str, Any]]) -> None:
+    def projjson(self, v: dict[str, Any] | None) -> None:
         self._set_property(PROJJSON_PROP, v)
 
     @property
-    def crs_string(self) -> Optional[str]:
+    def crs_string(self) -> str | None:
         """Returns the coordinate reference system (CRS) string for the extension.
 
         This string can be used to feed, e.g., ``rasterio.crs.CRS.from_string``.
         The string is determined by the following heuristic:
 
         1. If an EPSG code is set, return "EPSG:{code}", else
         2. If wkt2 is set, return the WKT string, else,
@@ -168,107 +180,111 @@
             return self.wkt2
         elif self.projjson:
             return json.dumps(self.projjson)
         else:
             return None
 
     @property
-    def geometry(self) -> Optional[Dict[str, Any]]:
+    def geometry(self) -> dict[str, Any] | None:
         """Get or sets a Polygon GeoJSON dict representing the footprint of this item.
 
         This dict should be formatted according the Polygon object format specified in
         `RFC 7946, sections 3.1.6 <https://tools.ietf.org/html/rfc7946>`_,
         except not necessarily in EPSG:4326 as required by RFC7946. Specified based on
         the ``epsg``, ``projjson`` or ``wkt2`` fields (not necessarily EPSG:4326).
         Ideally, this will be represented by a Polygon with five coordinates, as the
         item in the asset data CRS should be a square aligned to the original CRS grid.
         """
-        return self._get_property(GEOM_PROP, Dict[str, Any])
+        return self._get_property(GEOM_PROP, dict[str, Any])
 
     @geometry.setter
-    def geometry(self, v: Optional[Dict[str, Any]]) -> None:
+    def geometry(self, v: dict[str, Any] | None) -> None:
         self._set_property(GEOM_PROP, v)
 
     @property
-    def bbox(self) -> Optional[List[float]]:
+    def bbox(self) -> list[float] | None:
         """Get or sets the bounding box of the assets represented by this item in the
         asset data CRS.
 
         Specified as 4 or 6 coordinates based on the CRS defined in the ``epsg``,
         ``projjson`` or ``wkt2`` properties. First two numbers are coordinates of the
         lower left corner, followed by coordinates of upper right corner, e.g.,
         ``[west, south, east, north]``, ``[xmin, ymin, xmax, ymax]``,
         ``[left, down, right, up]``, or ``[west, south, lowest, east, north,
         highest]``. The length of the array must be 2*n where n is the number of
         dimensions.
         """
-        return self._get_property(BBOX_PROP, List[float])
+        return self._get_property(BBOX_PROP, list[float])
 
     @bbox.setter
-    def bbox(self, v: Optional[List[float]]) -> None:
+    def bbox(self, v: list[float] | None) -> None:
         self._set_property(BBOX_PROP, v)
 
     @property
-    def centroid(self) -> Optional[Dict[str, float]]:
+    def centroid(self) -> dict[str, float] | None:
         """Get or sets coordinates representing the centroid of the item in the asset
         data CRS.
 
         Coordinates are defined in latitude and longitude, even if the data coordinate
         system does not use lat/long.
 
         Example::
 
             item.ext.proj.centroid = { 'lat': 0.0, 'lon': 0.0 }
         """
-        return self._get_property(CENTROID_PROP, Dict[str, float])
+        return self._get_property(CENTROID_PROP, dict[str, float])
 
     @centroid.setter
-    def centroid(self, v: Optional[Dict[str, float]]) -> None:
+    def centroid(self, v: dict[str, float] | None) -> None:
         self._set_property(CENTROID_PROP, v)
 
     @property
-    def shape(self) -> Optional[List[int]]:
+    def shape(self) -> list[int] | None:
         """Get or sets the number of pixels in Y and X directions for the default grid.
 
         The shape is an array of integers that represents the number of pixels in the
         most common pixel grid used by the item's assets. The number of pixels should
         be specified in Y, X order. If the shape is defined in an item's properties it
         is used as the default shape for all assets that don't have an overriding shape.
         """
-        return self._get_property(SHAPE_PROP, List[int])
+        return self._get_property(SHAPE_PROP, list[int])
 
     @shape.setter
-    def shape(self, v: Optional[List[int]]) -> None:
+    def shape(self, v: list[int] | None) -> None:
         self._set_property(SHAPE_PROP, v)
 
     @property
-    def transform(self) -> Optional[List[float]]:
+    def transform(self) -> list[float] | None:
         """Get or sets the the affine transformation coefficients for the default grid.
 
         The transform is a linear mapping from pixel coordinate space (Pixel, Line) to
         projection coordinate space (Xp, Yp). It is a 3x3 matrix stored as a flat array
         of 9 elements in row major order. Since the last row is always 0,0,1 it can be
         omitted, in which case only 6 elements are recorded. This mapping can be
         obtained from GDAL `GetGeoTransform <https://gdal.org/api/gdaldataset_cpp.html\
 #_CPPv4N11GDALDataset15GetGeoTransformEPd>`_
         or the Rasterio `Transform <https://rasterio.readthedocs.io/en/stable/api\
 /rasterio.io.html#rasterio.io.BufferedDatasetWriter.transform>`_.
         """
-        return self._get_property(TRANSFORM_PROP, List[float])
+        return self._get_property(TRANSFORM_PROP, list[float])
 
     @transform.setter
-    def transform(self, v: Optional[List[float]]) -> None:
+    def transform(self, v: list[float] | None) -> None:
         self._set_property(TRANSFORM_PROP, v)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def get_schema_uris(cls) -> List[str]:
+    def get_schema_uris(cls) -> list[str]:
+        warnings.warn(
+            "get_schema_uris is deprecated and will be removed in v2",
+            DeprecationWarning,
+        )
         return SCHEMA_URIS
 
     @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> ProjectionExtension[T]:
         """Extends the given STAC Object with properties from the :stac-ext:`Projection
         Extension <projection>`.
 
@@ -276,28 +292,31 @@
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(ProjectionExtension[T], ItemProjectionExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(ProjectionExtension[T], AssetProjectionExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(ProjectionExtension[T], ItemAssetsProjectionExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesProjectionExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesProjectionExtension(obj)
 
 
 class ItemProjectionExtension(ProjectionExtension[pystac.Item]):
     """A concrete implementation of :class:`ProjectionExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`Projection Extension <projection>`.
@@ -305,69 +324,78 @@
     This class should generally not be instantiated directly. Instead, call
     :meth:`ProjectionExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemProjectionExtension Item id={}>".format(self.item.id)
+        return f"<ItemProjectionExtension Item id={self.item.id}>"
 
 
 class AssetProjectionExtension(ProjectionExtension[pystac.Asset]):
     """A concrete implementation of :class:`ProjectionExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties defined
     in the :stac-ext:`Projection Extension <projection>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`ProjectionExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetProjectionExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetProjectionExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsProjectionExtension(ProjectionExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
 
 class SummariesProjectionExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Projection Extension <projection>`.
     """
 
     @property
-    def epsg(self) -> Optional[List[int]]:
+    def epsg(self) -> list[int] | None:
         """Get or sets the summary of :attr:`ProjectionExtension.epsg` values
         for this Collection.
         """
         return self.summaries.get_list(EPSG_PROP)
 
     @epsg.setter
-    def epsg(self, v: Optional[List[int]]) -> None:
+    def epsg(self, v: list[int] | None) -> None:
         self._set_summary(EPSG_PROP, v)
 
 
 class ProjectionExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {
         "proj",
```

### Comparing `pystac-1.8.4/pystac/extensions/sar.py` & `pystac-1.9.0/pystac/extensions/sar.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 """Implements the :stac-ext:`Synthetic-Aperture Radar (SAR) Extension <sar>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union, cast
+from collections.abc import Iterable
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.serialization.identify import STACJSONDescription, STACVersionID
 from pystac.summaries import RangeSummary
 from pystac.utils import StringEnum, get_required, map_opt
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
 SCHEMA_URI: str = "https://stac-extensions.github.io/sar/v1.0.0/schema.json"
 PREFIX: str = "sar:"
 
 # Required
 INSTRUMENT_MODE_PROP: str = PREFIX + "instrument_mode"
 FREQUENCY_BAND_PROP: str = PREFIX + "frequency_band"
@@ -77,29 +86,31 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> sar_ext = SARExtension.ext(item)
     """
 
+    name: Literal["sar"] = "sar"
+
     def apply(
         self,
         instrument_mode: str,
         frequency_band: FrequencyBand,
-        polarizations: List[Polarization],
+        polarizations: list[Polarization],
         product_type: str,
-        center_frequency: Optional[float] = None,
-        resolution_range: Optional[float] = None,
-        resolution_azimuth: Optional[float] = None,
-        pixel_spacing_range: Optional[float] = None,
-        pixel_spacing_azimuth: Optional[float] = None,
-        looks_range: Optional[int] = None,
-        looks_azimuth: Optional[int] = None,
-        looks_equivalent_number: Optional[float] = None,
-        observation_direction: Optional[ObservationDirection] = None,
+        center_frequency: float | None = None,
+        resolution_range: float | None = None,
+        resolution_azimuth: float | None = None,
+        pixel_spacing_range: float | None = None,
+        pixel_spacing_azimuth: float | None = None,
+        looks_range: int | None = None,
+        looks_azimuth: int | None = None,
+        looks_equivalent_number: float | None = None,
+        observation_direction: ObservationDirection | None = None,
     ) -> None:
         """Applies sar extension properties to the extended Item.
 
         Args:
             instrument_mode : The name of the sensor acquisition mode that is
                 commonly used. This should be the short name, if available. For example,
                 WV for "Wave mode."
@@ -178,27 +189,27 @@
         )
 
     @frequency_band.setter
     def frequency_band(self, v: FrequencyBand) -> None:
         self._set_property(FREQUENCY_BAND_PROP, v.value, pop_if_none=False)
 
     @property
-    def polarizations(self) -> List[Polarization]:
+    def polarizations(self) -> list[Polarization]:
         """Gets or sets a list of polarizations for the item."""
         return get_required(
             map_opt(
                 lambda values: [Polarization(v) for v in values],
-                self._get_property(POLARIZATIONS_PROP, List[str]),
+                self._get_property(POLARIZATIONS_PROP, list[str]),
             ),
             self,
             POLARIZATIONS_PROP,
         )
 
     @polarizations.setter
-    def polarizations(self, values: List[Polarization]) -> None:
+    def polarizations(self, values: list[Polarization]) -> None:
         if not isinstance(values, list):
             raise pystac.STACError(f'polarizations must be a list. Invalid "{values}"')
         self._set_property(
             POLARIZATIONS_PROP, [v.value for v in values], pop_if_none=False
         )
 
     @property
@@ -209,94 +220,94 @@
         )
 
     @product_type.setter
     def product_type(self, v: str) -> None:
         self._set_property(PRODUCT_TYPE_PROP, v, pop_if_none=False)
 
     @property
-    def center_frequency(self) -> Optional[float]:
+    def center_frequency(self) -> float | None:
         """Gets or sets a center frequency for the item."""
         return self._get_property(CENTER_FREQUENCY_PROP, float)
 
     @center_frequency.setter
-    def center_frequency(self, v: Optional[float]) -> None:
+    def center_frequency(self, v: float | None) -> None:
         self._set_property(CENTER_FREQUENCY_PROP, v)
 
     @property
-    def resolution_range(self) -> Optional[float]:
+    def resolution_range(self) -> float | None:
         """Gets or sets a resolution range for the item."""
         return self._get_property(RESOLUTION_RANGE_PROP, float)
 
     @resolution_range.setter
-    def resolution_range(self, v: Optional[float]) -> None:
+    def resolution_range(self, v: float | None) -> None:
         self._set_property(RESOLUTION_RANGE_PROP, v)
 
     @property
-    def resolution_azimuth(self) -> Optional[float]:
+    def resolution_azimuth(self) -> float | None:
         """Gets or sets a resolution azimuth for the item."""
         return self._get_property(RESOLUTION_AZIMUTH_PROP, float)
 
     @resolution_azimuth.setter
-    def resolution_azimuth(self, v: Optional[float]) -> None:
+    def resolution_azimuth(self, v: float | None) -> None:
         self._set_property(RESOLUTION_AZIMUTH_PROP, v)
 
     @property
-    def pixel_spacing_range(self) -> Optional[float]:
+    def pixel_spacing_range(self) -> float | None:
         """Gets or sets a pixel spacing range for the item."""
         return self._get_property(PIXEL_SPACING_RANGE_PROP, float)
 
     @pixel_spacing_range.setter
-    def pixel_spacing_range(self, v: Optional[float]) -> None:
+    def pixel_spacing_range(self, v: float | None) -> None:
         self._set_property(PIXEL_SPACING_RANGE_PROP, v)
 
     @property
-    def pixel_spacing_azimuth(self) -> Optional[float]:
+    def pixel_spacing_azimuth(self) -> float | None:
         """Gets or sets a pixel spacing azimuth for the item."""
         return self._get_property(PIXEL_SPACING_AZIMUTH_PROP, float)
 
     @pixel_spacing_azimuth.setter
-    def pixel_spacing_azimuth(self, v: Optional[float]) -> None:
+    def pixel_spacing_azimuth(self, v: float | None) -> None:
         self._set_property(PIXEL_SPACING_AZIMUTH_PROP, v)
 
     @property
-    def looks_range(self) -> Optional[int]:
+    def looks_range(self) -> int | None:
         """Gets or sets a looks range for the item."""
         return self._get_property(LOOKS_RANGE_PROP, int)
 
     @looks_range.setter
-    def looks_range(self, v: Optional[int]) -> None:
+    def looks_range(self, v: int | None) -> None:
         self._set_property(LOOKS_RANGE_PROP, v)
 
     @property
-    def looks_azimuth(self) -> Optional[int]:
+    def looks_azimuth(self) -> int | None:
         """Gets or sets a looks azimuth for the item."""
         return self._get_property(LOOKS_AZIMUTH_PROP, int)
 
     @looks_azimuth.setter
-    def looks_azimuth(self, v: Optional[int]) -> None:
+    def looks_azimuth(self, v: int | None) -> None:
         self._set_property(LOOKS_AZIMUTH_PROP, v)
 
     @property
-    def looks_equivalent_number(self) -> Optional[float]:
+    def looks_equivalent_number(self) -> float | None:
         """Gets or sets a looks equivalent number for the item."""
         return self._get_property(LOOKS_EQUIVALENT_NUMBER_PROP, float)
 
     @looks_equivalent_number.setter
-    def looks_equivalent_number(self, v: Optional[float]) -> None:
+    def looks_equivalent_number(self, v: float | None) -> None:
         self._set_property(LOOKS_EQUIVALENT_NUMBER_PROP, v)
 
     @property
-    def observation_direction(self) -> Optional[ObservationDirection]:
+    def observation_direction(self) -> ObservationDirection | None:
         """Gets or sets an observation direction for the item."""
         return map_opt(
             ObservationDirection, self._get_property(OBSERVATION_DIRECTION_PROP, str)
         )
 
     @observation_direction.setter
-    def observation_direction(self, v: Optional[ObservationDirection]) -> None:
+    def observation_direction(self, v: ObservationDirection | None) -> None:
         self._set_property(OBSERVATION_DIRECTION_PROP, map_opt(lambda x: x.value, v))
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
@@ -308,32 +319,35 @@
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(SarExtension[T], ItemSarExtension(obj))
         elif isinstance(obj, pystac.Asset):
             if obj.owner is not None and not isinstance(obj.owner, pystac.Item):
                 raise pystac.ExtensionTypeError(
                     "SAR extension does not apply to Collection Assets."
                 )
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(SarExtension[T], AssetSarExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(SarExtension[T], ItemAssetsSarExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesSarExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesSarExtension(obj)
 
 
 class ItemSarExtension(SarExtension[pystac.Item]):
     """A concrete implementation of :class:`SARExtension` on an :class:`~pystac.Item`
     that extends the properties of the Item to include properties defined in the
     :stac-ext:`SAR Extension <sar>`.
@@ -341,224 +355,233 @@
     This class should generally not be instantiated directly. Instead, call
     :meth:`SARExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemSarExtension Item id={}>".format(self.item.id)
+        return f"<ItemSarExtension Item id={self.item.id}>"
 
 
 class AssetSarExtension(SarExtension[pystac.Asset]):
     """A concrete implementation of :class:`SARExtension` on an :class:`~pystac.Asset`
     that extends the Asset fields to include properties defined in the
     :stac-ext:`SAR Extension <sar>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`SARExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetSarExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetSarExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsSarExtension(SarExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
 
 class SummariesSarExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`SAR Extension <sar>`.
     """
 
     @property
-    def instrument_mode(self) -> Optional[List[str]]:
+    def instrument_mode(self) -> list[str] | None:
         """Get or sets the summary of :attr:`SarExtension.instrument_mode` values
         for this Collection.
         """
 
         return self.summaries.get_list(INSTRUMENT_MODE_PROP)
 
     @instrument_mode.setter
-    def instrument_mode(self, v: Optional[List[str]]) -> None:
+    def instrument_mode(self, v: list[str] | None) -> None:
         self._set_summary(INSTRUMENT_MODE_PROP, v)
 
     @property
-    def frequency_band(self) -> Optional[List[FrequencyBand]]:
+    def frequency_band(self) -> list[FrequencyBand] | None:
         """Get or sets the summary of :attr:`SarExtension.frequency_band` values
         for this Collection.
         """
 
         return self.summaries.get_list(FREQUENCY_BAND_PROP)
 
     @frequency_band.setter
-    def frequency_band(self, v: Optional[List[FrequencyBand]]) -> None:
+    def frequency_band(self, v: list[FrequencyBand] | None) -> None:
         self._set_summary(FREQUENCY_BAND_PROP, v)
 
     @property
-    def center_frequency(self) -> Optional[RangeSummary[float]]:
+    def center_frequency(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.center_frequency` values
         for this Collection.
         """
 
         return self.summaries.get_range(CENTER_FREQUENCY_PROP)
 
     @center_frequency.setter
-    def center_frequency(self, v: Optional[RangeSummary[float]]) -> None:
+    def center_frequency(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(CENTER_FREQUENCY_PROP, v)
 
     @property
-    def polarizations(self) -> Optional[List[Polarization]]:
+    def polarizations(self) -> list[Polarization] | None:
         """Get or sets the summary of :attr:`SarExtension.polarizations` values
         for this Collection.
         """
 
         return self.summaries.get_list(POLARIZATIONS_PROP)
 
     @polarizations.setter
-    def polarizations(self, v: Optional[List[Polarization]]) -> None:
+    def polarizations(self, v: list[Polarization] | None) -> None:
         self._set_summary(POLARIZATIONS_PROP, v)
 
     @property
-    def product_type(self) -> Optional[List[str]]:
+    def product_type(self) -> list[str] | None:
         """Get or sets the summary of :attr:`SarExtension.product_type` values
         for this Collection.
         """
 
         return self.summaries.get_list(PRODUCT_TYPE_PROP)
 
     @product_type.setter
-    def product_type(self, v: Optional[List[str]]) -> None:
+    def product_type(self, v: list[str] | None) -> None:
         self._set_summary(PRODUCT_TYPE_PROP, v)
 
     @property
-    def resolution_range(self) -> Optional[RangeSummary[float]]:
+    def resolution_range(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.resolution_range` values
         for this Collection.
         """
 
         return self.summaries.get_range(RESOLUTION_RANGE_PROP)
 
     @resolution_range.setter
-    def resolution_range(self, v: Optional[RangeSummary[float]]) -> None:
+    def resolution_range(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(RESOLUTION_RANGE_PROP, v)
 
     @property
-    def resolution_azimuth(self) -> Optional[RangeSummary[float]]:
+    def resolution_azimuth(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.resolution_azimuth` values
         for this Collection.
         """
 
         return self.summaries.get_range(RESOLUTION_AZIMUTH_PROP)
 
     @resolution_azimuth.setter
-    def resolution_azimuth(self, v: Optional[RangeSummary[float]]) -> None:
+    def resolution_azimuth(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(RESOLUTION_AZIMUTH_PROP, v)
 
     @property
-    def pixel_spacing_range(self) -> Optional[RangeSummary[float]]:
+    def pixel_spacing_range(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.pixel_spacing_range` values
         for this Collection.
         """
 
         return self.summaries.get_range(PIXEL_SPACING_RANGE_PROP)
 
     @pixel_spacing_range.setter
-    def pixel_spacing_range(self, v: Optional[RangeSummary[float]]) -> None:
+    def pixel_spacing_range(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(PIXEL_SPACING_RANGE_PROP, v)
 
     @property
-    def pixel_spacing_azimuth(self) -> Optional[RangeSummary[float]]:
+    def pixel_spacing_azimuth(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.pixel_spacing_azimuth` values
         for this Collection.
         """
 
         return self.summaries.get_range(PIXEL_SPACING_AZIMUTH_PROP)
 
     @pixel_spacing_azimuth.setter
-    def pixel_spacing_azimuth(self, v: Optional[RangeSummary[float]]) -> None:
+    def pixel_spacing_azimuth(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(PIXEL_SPACING_AZIMUTH_PROP, v)
 
     @property
-    def looks_range(self) -> Optional[RangeSummary[int]]:
+    def looks_range(self) -> RangeSummary[int] | None:
         """Get or sets the summary of :attr:`SarExtension.looks_range` values
         for this Collection.
         """
 
         return self.summaries.get_range(LOOKS_RANGE_PROP)
 
     @looks_range.setter
-    def looks_range(self, v: Optional[RangeSummary[int]]) -> None:
+    def looks_range(self, v: RangeSummary[int] | None) -> None:
         self._set_summary(LOOKS_RANGE_PROP, v)
 
     @property
-    def looks_azimuth(self) -> Optional[RangeSummary[int]]:
+    def looks_azimuth(self) -> RangeSummary[int] | None:
         """Get or sets the summary of :attr:`SarExtension.looks_azimuth` values
         for this Collection.
         """
 
         return self.summaries.get_range(LOOKS_AZIMUTH_PROP)
 
     @looks_azimuth.setter
-    def looks_azimuth(self, v: Optional[RangeSummary[int]]) -> None:
+    def looks_azimuth(self, v: RangeSummary[int] | None) -> None:
         self._set_summary(LOOKS_AZIMUTH_PROP, v)
 
     @property
-    def looks_equivalent_number(self) -> Optional[RangeSummary[float]]:
+    def looks_equivalent_number(self) -> RangeSummary[float] | None:
         """Get or sets the summary of :attr:`SarExtension.looks_equivalent_number`
         values for this Collection.
         """
 
         return self.summaries.get_range(LOOKS_EQUIVALENT_NUMBER_PROP)
 
     @looks_equivalent_number.setter
-    def looks_equivalent_number(self, v: Optional[RangeSummary[float]]) -> None:
+    def looks_equivalent_number(self, v: RangeSummary[float] | None) -> None:
         self._set_summary(LOOKS_EQUIVALENT_NUMBER_PROP, v)
 
     @property
-    def observation_direction(self) -> Optional[List[ObservationDirection]]:
+    def observation_direction(self) -> list[ObservationDirection] | None:
         """Get or sets the summary of :attr:`SarExtension.observation_direction` values
         for this Collection.
         """
 
         return self.summaries.get_list(OBSERVATION_DIRECTION_PROP)
 
     @observation_direction.setter
-    def observation_direction(self, v: Optional[List[ObservationDirection]]) -> None:
+    def observation_direction(self, v: list[ObservationDirection] | None) -> None:
         self._set_summary(OBSERVATION_DIRECTION_PROP, v)
 
 
 class SarExtensionHooks(ExtensionHooks):
     schema_uri = SCHEMA_URI
     prev_extension_ids = {"sar"}
     stac_object_types = {pystac.STACObjectType.ITEM}
 
     def migrate(
-        self, obj: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+        self, obj: dict[str, Any], version: STACVersionID, info: STACJSONDescription
     ) -> None:
         if version < "0.9":
             # Some sar fields became common_metadata
             if (
                 PREFIX + "platform" in obj["properties"]
                 and "platform" not in obj["properties"]
             ):
```

### Comparing `pystac-1.8.4/pystac/extensions/sat.py` & `pystac-1.9.0/pystac/extensions/view.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,296 +1,313 @@
-"""Implements the :stac-ext:`Satellite Extension <sat>`."""
+"""Implement the :stac-ext:`View Geometry Extension <view>`."""
 
 from __future__ import annotations
 
-from datetime import datetime
-from typing import Any, Dict, Generic, Iterable, List, Optional, TypeVar, Union, cast
+from collections.abc import Iterable
+from typing import Any, Generic, Literal, TypeVar, Union, cast
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.summaries import RangeSummary
-from pystac.utils import StringEnum, datetime_to_str, map_opt, str_to_datetime
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
-SCHEMA_URI = "https://stac-extensions.github.io/sat/v1.0.0/schema.json"
-
-PREFIX: str = "sat:"
-PLATFORM_INTERNATIONAL_DESIGNATOR_PROP: str = (
-    PREFIX + "platform_international_designator"
-)
-ABSOLUTE_ORBIT_PROP: str = PREFIX + "absolute_orbit"
-ORBIT_STATE_PROP: str = PREFIX + "orbit_state"
-RELATIVE_ORBIT_PROP: str = PREFIX + "relative_orbit"
-ANX_DATETIME_PROP: str = PREFIX + "anx_datetime"
+SCHEMA_URI: str = "https://stac-extensions.github.io/view/v1.0.0/schema.json"
+PREFIX: str = "view:"
 
+OFF_NADIR_PROP: str = PREFIX + "off_nadir"
+INCIDENCE_ANGLE_PROP: str = PREFIX + "incidence_angle"
+AZIMUTH_PROP: str = PREFIX + "azimuth"
+SUN_AZIMUTH_PROP: str = PREFIX + "sun_azimuth"
+SUN_ELEVATION_PROP: str = PREFIX + "sun_elevation"
 
-class OrbitState(StringEnum):
-    ASCENDING = "ascending"
-    DESCENDING = "descending"
-    GEOSTATIONARY = "geostationary"
 
-
-class SatExtension(
+class ViewExtension(
     Generic[T],
     PropertiesExtension,
     ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]],
 ):
     """An abstract class that can be used to extend the properties of an
-    :class:`~pystac.Item` or :class:`~pystac.Asset` with properties from the
-    :stac-ext:`Satellite Extension <sat>`. This class is generic over the type of
-    STAC Object to be extended (e.g. :class:`~pystac.Item`,
-    :class:`~pystac.Collection`).
+    :class:`~pystac.Item` with properties from the :stac-ext:`View Geometry
+    Extension <view>`. This class is generic over the type of STAC Object to be
+    extended (e.g. :class:`~pystac.Item`, :class:`~pystac.Asset`).
 
-    To create a concrete instance of :class:`SatExtension`, use the
-    :meth:`SatExtension.ext` method. For example:
+    To create a concrete instance of :class:`ViewExtension`, use the
+    :meth:`ViewExtension.ext` method. For example:
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
-       >>> sat_ext = SatExtension.ext(item)
+       >>> view_ext = ViewExtension.ext(item)
     """
 
+    name: Literal["view"] = "view"
+
     def apply(
         self,
-        orbit_state: Optional[OrbitState] = None,
-        relative_orbit: Optional[int] = None,
-        absolute_orbit: Optional[int] = None,
-        platform_international_designator: Optional[str] = None,
-        anx_datetime: Optional[datetime] = None,
+        off_nadir: float | None = None,
+        incidence_angle: float | None = None,
+        azimuth: float | None = None,
+        sun_azimuth: float | None = None,
+        sun_elevation: float | None = None,
     ) -> None:
-        """Applies ext extension properties to the extended :class:`~pystac.Item` or
-        class:`~pystac.Asset`.
-
-        Must specify at least one of orbit_state or relative_orbit in order
-        for the sat extension to properties to be valid.
+        """Applies View Geometry extension properties to the extended
+        :class:`~pystac.Item`.
 
         Args:
-            orbit_state : Optional state of the orbit. Either ascending or
-                descending for polar orbiting satellites, or geostationary for
-                geosynchronous satellites.
-            relative_orbit : Optional non-negative integer of the orbit number at
-                the time of acquisition.
+            off_nadir : The angle from the sensor between nadir (straight down)
+                and the scene center. Measured in degrees (0-90).
+            incidence_angle : The incidence angle is the angle between the
+                vertical (normal) to the intercepting surface and the line of sight
+                back to the satellite at the scene center. Measured in degrees (0-90).
+            azimuth : Viewing azimuth angle. The angle measured from the
+                sub-satellite point (point on the ground below the platform) between
+                the scene center and true north. Measured clockwise from north in
+                degrees (0-360).
+            sun_azimuth : Sun azimuth angle. From the scene center point on the
+                ground, this is the angle between truth north and the sun. Measured
+                clockwise in degrees (0-360).
+            sun_elevation : Sun elevation angle. The angle from the tangent of
+                the scene center point to the sun. Measured from the horizon in
+                degrees (0-90).
         """
-
-        self.platform_international_designator = platform_international_designator
-        self.orbit_state = orbit_state
-        self.absolute_orbit = absolute_orbit
-        self.relative_orbit = relative_orbit
-        self.anx_datetime = anx_datetime
+        self.off_nadir = off_nadir
+        self.incidence_angle = incidence_angle
+        self.azimuth = azimuth
+        self.sun_azimuth = sun_azimuth
+        self.sun_elevation = sun_elevation
 
     @property
-    def platform_international_designator(self) -> Optional[str]:
-        """Gets or sets the International Designator, also known as COSPAR ID, and
-        NSSDCA ID."""
-        return self._get_property(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, str)
-
-    @platform_international_designator.setter
-    def platform_international_designator(self, v: Optional[str]) -> None:
-        self._set_property(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, v)
+    def off_nadir(self) -> float | None:
+        """Get or sets the angle from the sensor between nadir (straight down)
+        and the scene center. Measured in degrees (0-90).
+        """
+        return self._get_property(OFF_NADIR_PROP, float)
+
+    @off_nadir.setter
+    def off_nadir(self, v: float | None) -> None:
+        self._set_property(OFF_NADIR_PROP, v)
 
     @property
-    def orbit_state(self) -> Optional[OrbitState]:
-        """Get or sets an orbit state of the object."""
-        return map_opt(
-            lambda x: OrbitState(x), self._get_property(ORBIT_STATE_PROP, str)
-        )
-
-    @orbit_state.setter
-    def orbit_state(self, v: Optional[OrbitState]) -> None:
-        self._set_property(ORBIT_STATE_PROP, map_opt(lambda x: x.value, v))
+    def incidence_angle(self) -> float | None:
+        """Get or sets the incidence angle is the angle between the vertical (normal)
+        to the intercepting surface and the line of sight back to the satellite at
+        the scene center. Measured in degrees (0-90).
+        """
+        return self._get_property(INCIDENCE_ANGLE_PROP, float)
+
+    @incidence_angle.setter
+    def incidence_angle(self, v: float | None) -> None:
+        self._set_property(INCIDENCE_ANGLE_PROP, v)
 
     @property
-    def absolute_orbit(self) -> Optional[int]:
-        """Get or sets a absolute orbit number of the item."""
-        return self._get_property(ABSOLUTE_ORBIT_PROP, int)
-
-    @absolute_orbit.setter
-    def absolute_orbit(self, v: Optional[int]) -> None:
-        self._set_property(ABSOLUTE_ORBIT_PROP, v)
+    def azimuth(self) -> float | None:
+        """Get or sets the viewing azimuth angle.
+
+        The angle measured from the sub-satellite
+        point (point on the ground below the platform) between the scene center and true
+        north. Measured clockwise from north in degrees (0-360).
+        """
+        return self._get_property(AZIMUTH_PROP, float)
+
+    @azimuth.setter
+    def azimuth(self, v: float | None) -> None:
+        self._set_property(AZIMUTH_PROP, v)
 
     @property
-    def relative_orbit(self) -> Optional[int]:
-        """Get or sets a relative orbit number of the item."""
-        return self._get_property(RELATIVE_ORBIT_PROP, int)
-
-    @relative_orbit.setter
-    def relative_orbit(self, v: Optional[int]) -> None:
-        self._set_property(RELATIVE_ORBIT_PROP, v)
+    def sun_azimuth(self) -> float | None:
+        """Get or sets the sun azimuth angle.
+
+        From the scene center point on the ground, this
+        is the angle between truth north and the sun. Measured clockwise in
+        degrees (0-360).
+        """
+        return self._get_property(SUN_AZIMUTH_PROP, float)
+
+    @sun_azimuth.setter
+    def sun_azimuth(self, v: float | None) -> None:
+        self._set_property(SUN_AZIMUTH_PROP, v)
 
     @property
-    def anx_datetime(self) -> Optional[datetime]:
-        return map_opt(str_to_datetime, self._get_property(ANX_DATETIME_PROP, str))
+    def sun_elevation(self) -> float | None:
+        """Get or sets the sun elevation angle. The angle from the tangent of the scene
+        center point to the sun. Measured from the horizon in degrees (0-90).
+        """
+        return self._get_property(SUN_ELEVATION_PROP, float)
 
-    @anx_datetime.setter
-    def anx_datetime(self, v: Optional[datetime]) -> None:
-        self._set_property(ANX_DATETIME_PROP, map_opt(datetime_to_str, v))
+    @sun_elevation.setter
+    def sun_elevation(self, v: float | None) -> None:
+        self._set_property(SUN_ELEVATION_PROP, v)
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def ext(cls, obj: T, add_if_missing: bool = False) -> SatExtension[T]:
-        """Extends the given STAC Object with properties from the :stac-ext:`Satellite
-        Extension <sat>`.
+    def ext(cls, obj: T, add_if_missing: bool = False) -> ViewExtension[T]:
+        """Extends the given STAC Object with properties from the :stac-ext:`View
+        Geometry Extension <scientific>`.
 
         This extension can be applied to instances of :class:`~pystac.Item` or
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
-            return cast(SatExtension[T], ItemSatExtension(obj))
+            cls.ensure_has_extension(obj, add_if_missing)
+            return cast(ViewExtension[T], ItemViewExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
-            return cast(SatExtension[T], AssetSatExtension(obj))
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(ViewExtension[T], AssetViewExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(ViewExtension[T], ItemAssetsViewExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
-    ) -> SummariesSatExtension:
+    ) -> SummariesViewExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
-        return SummariesSatExtension(obj)
+        cls.ensure_has_extension(obj, add_if_missing)
+        return SummariesViewExtension(obj)
 
 
-class ItemSatExtension(SatExtension[pystac.Item]):
-    """A concrete implementation of :class:`SatExtension` on an :class:`~pystac.Item`
+class ItemViewExtension(ViewExtension[pystac.Item]):
+    """A concrete implementation of :class:`ViewExtension` on an :class:`~pystac.Item`
     that extends the properties of the Item to include properties defined in the
-    :stac-ext:`Satellite Extension <sat>`.
+    :stac-ext:`View Geometry Extension <view>`.
 
     This class should generally not be instantiated directly. Instead, call
-    :meth:`SatExtension.ext` on an :class:`~pystac.Item` to
-    extend it.
+    :meth:`ViewExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemSatExtension Item id={}>".format(self.item.id)
+        return f"<ItemViewExtension Item id={self.item.id}>"
 
 
-class AssetSatExtension(SatExtension[pystac.Asset]):
-    """A concrete implementation of :class:`SatExtension` on an :class:`~pystac.Asset`
-    that extends the properties of the Asset to include properties defined in the
-    :stac-ext:`Satellite Extension <sat>`.
+class AssetViewExtension(ViewExtension[pystac.Asset]):
+    """A concrete implementation of :class:`ViewExtension` on an :class:`~pystac.Asset`
+    that extends the Asset fields to include properties defined in the
+    :stac-ext:`View Geometry Extension <view>`.
 
     This class should generally not be instantiated directly. Instead, call
-    :meth:`SatExtension.ext` on an :class:`~pystac.Asset` to
-    extend it.
+    :meth:`ViewExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetSatExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetViewExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsViewExtension(ViewExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
 
-class SummariesSatExtension(SummariesExtension):
+class SummariesViewExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
-    defined in the :stac-ext:`Satellite Extension <sat>`.
+    defined in the :stac-ext:`View Object Extension <view>`.
     """
 
     @property
-    def platform_international_designator(self) -> Optional[List[str]]:
-        """Get or sets the summary of
-        :attr:`SatExtension.platform_international_designator` values for this
-        Collection.
+    def off_nadir(self) -> RangeSummary[float] | None:
+        """Get or sets the summary of :attr:`ViewExtension.off_nadir` values for
+        this Collection.
         """
+        return self.summaries.get_range(OFF_NADIR_PROP)
 
-        return self.summaries.get_list(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP)
-
-    @platform_international_designator.setter
-    def platform_international_designator(self, v: Optional[List[str]]) -> None:
-        self._set_summary(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, v)
+    @off_nadir.setter
+    def off_nadir(self, v: RangeSummary[float] | None) -> None:
+        self._set_summary(OFF_NADIR_PROP, v)
 
     @property
-    def orbit_state(self) -> Optional[List[OrbitState]]:
-        """Get or sets the summary of :attr:`SatExtension.orbit_state` values
+    def incidence_angle(self) -> RangeSummary[float] | None:
+        """Get or sets the summary of :attr:`ViewExtension.incidence_angle` values
         for this Collection.
         """
+        return self.summaries.get_range(INCIDENCE_ANGLE_PROP)
 
-        return self.summaries.get_list(ORBIT_STATE_PROP)
-
-    @orbit_state.setter
-    def orbit_state(self, v: Optional[List[OrbitState]]) -> None:
-        self._set_summary(ORBIT_STATE_PROP, v)
+    @incidence_angle.setter
+    def incidence_angle(self, v: RangeSummary[float] | None) -> None:
+        self._set_summary(INCIDENCE_ANGLE_PROP, v)
 
     @property
-    def absolute_orbit(self) -> Optional[RangeSummary[int]]:
-        return self.summaries.get_range(ABSOLUTE_ORBIT_PROP)
+    def azimuth(self) -> RangeSummary[float] | None:
+        """Get or sets the summary of :attr:`ViewExtension.azimuth` values
+        for this Collection.
+        """
+        return self.summaries.get_range(AZIMUTH_PROP)
 
-    @absolute_orbit.setter
-    def absolute_orbit(self, v: Optional[RangeSummary[int]]) -> None:
-        self._set_summary(ABSOLUTE_ORBIT_PROP, v)
+    @azimuth.setter
+    def azimuth(self, v: RangeSummary[float] | None) -> None:
+        self._set_summary(AZIMUTH_PROP, v)
 
     @property
-    def relative_orbit(self) -> Optional[RangeSummary[int]]:
-        return self.summaries.get_range(RELATIVE_ORBIT_PROP)
+    def sun_azimuth(self) -> RangeSummary[float] | None:
+        """Get or sets the summary of :attr:`ViewExtension.sun_azimuth` values
+        for this Collection.
+        """
+        return self.summaries.get_range(SUN_AZIMUTH_PROP)
 
-    @relative_orbit.setter
-    def relative_orbit(self, v: Optional[RangeSummary[int]]) -> None:
-        self._set_summary(RELATIVE_ORBIT_PROP, v)
+    @sun_azimuth.setter
+    def sun_azimuth(self, v: RangeSummary[float] | None) -> None:
+        self._set_summary(SUN_AZIMUTH_PROP, v)
 
     @property
-    def anx_datetime(self) -> Optional[RangeSummary[datetime]]:
-        return map_opt(
-            lambda s: RangeSummary(
-                str_to_datetime(s.minimum), str_to_datetime(s.maximum)
-            ),
-            self.summaries.get_range(ANX_DATETIME_PROP),
-        )
-
-    @anx_datetime.setter
-    def anx_datetime(self, v: Optional[RangeSummary[datetime]]) -> None:
-        self._set_summary(
-            ANX_DATETIME_PROP,
-            map_opt(
-                lambda s: RangeSummary(
-                    datetime_to_str(s.minimum), datetime_to_str(s.maximum)
-                ),
-                v,
-            ),
-        )
-
-
-class SatExtensionHooks(ExtensionHooks):
-    schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"sat"}
+    def sun_elevation(self) -> RangeSummary[float] | None:
+        """Get or sets the summary of :attr:`ViewExtension.sun_elevation` values
+        for this Collection.
+        """
+        return self.summaries.get_range(SUN_ELEVATION_PROP)
+
+    @sun_elevation.setter
+    def sun_elevation(self, v: RangeSummary[float] | None) -> None:
+        self._set_summary(SUN_ELEVATION_PROP, v)
+
+
+class ViewExtensionHooks(ExtensionHooks):
+    schema_uri = SCHEMA_URI
+    prev_extension_ids = {"view"}
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
-SAT_EXTENSION_HOOKS: ExtensionHooks = SatExtensionHooks()
+VIEW_EXTENSION_HOOKS: ExtensionHooks = ViewExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/scientific.py` & `pystac-1.9.0/pystac/extensions/scientific.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 https://doi.org/10.1000/182
 """
 
 from __future__ import annotations
 
 import copy
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, cast
+from typing import Any, Generic, Literal, TypeVar, Union, cast
 from urllib import parse
 
 import pystac
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
@@ -50,46 +50,46 @@
     """Converts a DOI to the corresponding URL."""
     return DOI_URL_BASE + parse.quote(doi)
 
 
 class Publication:
     """Helper for Publication entries."""
 
-    citation: Optional[str]
-    doi: Optional[str]
+    citation: str | None
+    doi: str | None
 
-    def __init__(self, doi: Optional[str], citation: Optional[str]) -> None:
+    def __init__(self, doi: str | None, citation: str | None) -> None:
         self.doi = doi
         self.citation = citation
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Publication):
             return NotImplemented
 
         return self.doi == other.doi and self.citation == other.citation
 
     def __repr__(self) -> str:
         return f"<Publication doi={self.doi} target={self.citation}>"
 
-    def to_dict(self) -> Dict[str, Optional[str]]:
+    def to_dict(self) -> dict[str, str | None]:
         return copy.deepcopy({"doi": self.doi, "citation": self.citation})
 
     @staticmethod
-    def from_dict(d: Dict[str, str]) -> Publication:
+    def from_dict(d: dict[str, str]) -> Publication:
         return Publication(d.get("doi"), d.get("citation"))
 
-    def get_link(self) -> Optional[pystac.Link]:
+    def get_link(self) -> pystac.Link | None:
         """Gets a :class:`~pystac.Link` for the DOI for this publication. If
         :attr:`Publication.doi` is ``None``, this method will also return ``None``."""
         if self.doi is None:
             return None
         return pystac.Link(ScientificRelType.CITE_AS, doi_to_url(self.doi))
 
 
-def remove_link(links: List[pystac.Link], doi: Optional[str]) -> None:
+def remove_link(links: list[pystac.Link], doi: str | None) -> None:
     if doi is None:
         return
     url = doi_to_url(doi)
     for i, a_link in enumerate(links):
         if a_link.rel != ScientificRelType.CITE_AS:
             continue
         if a_link.target == url:
@@ -113,24 +113,25 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> sci_ext = ScientificExtension.ext(item)
     """
 
+    name: Literal["sci"] = "sci"
     obj: pystac.STACObject
 
     def __init__(self, obj: pystac.STACObject) -> None:
         self.obj = obj
 
     def apply(
         self,
-        doi: Optional[str] = None,
-        citation: Optional[str] = None,
-        publications: Optional[List[Publication]] = None,
+        doi: str | None = None,
+        citation: str | None = None,
+        publications: list[Publication] | None = None,
     ) -> None:
         """Applies scientific extension properties to the extended
         :class:`~pystac.Item`.
 
         Args:
             doi : Optional DOI string for the item.  Must not be a DOI link.
             citation : Optional human-readable reference.
@@ -138,70 +139,70 @@
                 referencing and describing the data.
         """
         self.doi = doi
         self.citation = citation
         self.publications = publications
 
     @property
-    def doi(self) -> Optional[str]:
+    def doi(self) -> str | None:
         """Get or sets the DOI for the item.
 
         This MUST NOT be a DOIs link. For all DOI names respective DOI links SHOULD be
         added to the links section.
         """
         return self._get_property(DOI_PROP, str)
 
     @doi.setter
-    def doi(self, v: Optional[str]) -> None:
+    def doi(self, v: str | None) -> None:
         if DOI_PROP in self.properties:
             if v == self.properties[DOI_PROP]:
                 return
             remove_link(self.obj.links, self.properties[DOI_PROP])
 
         if v is not None:
             self.properties[DOI_PROP] = v
             url = doi_to_url(v)
             self.obj.add_link(pystac.Link(ScientificRelType.CITE_AS, url))
 
     @property
-    def citation(self) -> Optional[str]:
+    def citation(self) -> str | None:
         """Get or sets the recommended human-readable reference (citation) to be used by
         publications citing the data.
 
         No specific citation style is suggested, but the citation should contain all
         information required to find the publication distinctively.
         """
         return self._get_property(CITATION_PROP, str)
 
     @citation.setter
-    def citation(self, v: Optional[str]) -> None:
+    def citation(self, v: str | None) -> None:
         self._set_property(CITATION_PROP, v)
 
     @property
-    def publications(self) -> Optional[List[Publication]]:
+    def publications(self) -> list[Publication] | None:
         """Get or sets the list of relevant publications referencing and describing the
         data."""
         return map_opt(
             lambda pubs: [Publication.from_dict(pub) for pub in pubs],
-            self._get_property(PUBLICATIONS_PROP, List[Dict[str, Any]]),
+            self._get_property(PUBLICATIONS_PROP, list[dict[str, Any]]),
         )
 
     @publications.setter
-    def publications(self, v: Optional[List[Publication]]) -> None:
+    def publications(self, v: list[Publication] | None) -> None:
         self._set_property(
             PUBLICATIONS_PROP, map_opt(lambda pubs: [pub.to_dict() for pub in pubs], v)
         )
         if v is not None:
             for pub in v:
                 pub_link = pub.get_link()
                 if pub_link is not None:
                     self.obj.add_link(pub_link)
 
     # None for publication will clear all.
-    def remove_publication(self, publication: Optional[Publication] = None) -> None:
+    def remove_publication(self, publication: Publication | None = None) -> None:
         """Removes the given :class:`Publication` from the extended
         :class:`~pystac.Item`. If the ``publication`` argument is ``None``, all
         publications will be removed from the :class:`~pystac.Item`."""
         if PUBLICATIONS_PROP not in self.properties:
             return
 
         if not publication:
@@ -234,28 +235,28 @@
         :class:`~pystac.Collection`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Collection):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(ScientificExtension[T], CollectionScientificExtension(obj))
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(ScientificExtension[T], ItemScientificExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesScientificExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesScientificExtension(obj)
 
 
 class CollectionScientificExtension(ScientificExtension[pystac.Collection]):
     """A concrete implementation of :class:`ScientificExtension` on an
     :class:`~pystac.Collection` that extends the properties of the Item to include
     properties defined in the :stac-ext:`Scientific Citation Extension <scientific>`.
@@ -263,18 +264,18 @@
     This class should generally not be instantiated directly. Instead, call
     :meth:`ScientificExtension.ext` on an :class:`~pystac.Collection` to extend it.
     """
 
     collection: pystac.Collection
     """The :class:`~pystac.Collection` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Collection` properties, including extension properties."""
 
-    links: List[pystac.Link]
+    links: list[pystac.Link]
     """The list of :class:`~pystac.Link` objects associated with the
     :class:`~pystac.Collection` being extended, including links added by this extension.
     """
 
     def __init__(self, collection: pystac.Collection):
         self.collection = collection
         self.properties = collection.extra_fields
@@ -296,58 +297,58 @@
     This class should generally not be instantiated directly. Instead, call
     :meth:`ScientificExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
-    links: List[pystac.Link]
+    links: list[pystac.Link]
     """The list of :class:`~pystac.Link` objects associated with the
     :class:`~pystac.Item` being extended, including links added by this extension.
     """
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
         self.links = item.links
         super().__init__(self.item)
 
     def __repr__(self) -> str:
-        return "<ItemScientificExtension Item id={}>".format(self.item.id)
+        return f"<ItemScientificExtension Item id={self.item.id}>"
 
 
 class SummariesScientificExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Scientific Citation Extension <scientific>`.
     """
 
     @property
-    def citation(self) -> Optional[List[str]]:
+    def citation(self) -> list[str] | None:
         """Get or sets the summary of :attr:`ScientificExtension.citation` values
         for this Collection.
         """
         return self.summaries.get_list(CITATION_PROP)
 
     @citation.setter
-    def citation(self, v: Optional[List[str]]) -> None:
+    def citation(self, v: list[str] | None) -> None:
         self._set_summary(CITATION_PROP, v)
 
     @property
-    def doi(self) -> Optional[List[str]]:
+    def doi(self) -> list[str] | None:
         """Get or sets the summary of :attr:`ScientificExtension.citation` values
         for this Collection.
         """
         return self.summaries.get_list(DOI_PROP)
 
     @doi.setter
-    def doi(self, v: Optional[List[str]]) -> None:
+    def doi(self, v: list[str] | None) -> None:
         self._set_summary(DOI_PROP, v)
 
 
 class ScientificExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {"scientific"}
     stac_object_types = {pystac.STACObjectType.COLLECTION, pystac.STACObjectType.ITEM}
```

### Comparing `pystac-1.8.4/pystac/extensions/table.py` & `pystac-1.9.0/pystac/extensions/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Implements the :stac-ext:`Table Extension <table>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union, cast
+from typing import Any, Generic, Literal, TypeVar, Union, cast
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.utils import get_required
 
-T = TypeVar("T", pystac.Collection, pystac.Item, pystac.Asset)
+T = TypeVar(
+    "T", pystac.Collection, pystac.Item, pystac.Asset, item_assets.AssetDefinition
+)
 
 SCHEMA_URI = "https://stac-extensions.github.io/table/v1.2.0/schema.json"
 
 PREFIX: str = "table:"
 COLUMNS_PROP = PREFIX + "columns"
 PRIMARY_GEOMETRY_PROP = PREFIX + "primary_geometry"
 ROW_COUNT_PROP = PREFIX + "row_count"
@@ -29,92 +32,92 @@
 TBL_NAME_PROP = "name"
 TBL_DESCRIPTION_PROP = "description"
 
 
 class Column:
     """Object representing a column of a table."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     @property
     def name(self) -> str:
         """The column name"""
         return get_required(
             self.properties.get(COL_NAME_PROP), "table:column", COL_NAME_PROP
         )
 
     @name.setter
     def name(self, v: str) -> None:
         self.properties[COL_NAME_PROP] = v
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Detailed multi-line description to explain the column. `CommonMark 0.29
         <http://commonmark.org/>`__ syntax MAY be used for rich text representation."""
         return self.properties.get(COL_DESCRIPTION_PROP)
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(COL_DESCRIPTION_PROP, None)
         else:
             self.properties[COL_DESCRIPTION_PROP] = v
 
     @property
-    def col_type(self) -> Optional[str]:
+    def col_type(self) -> str | None:
         """Data type of the column. If using a file format with a type system (like
         Parquet), we recommend you use those types"""
         return self.properties.get(COL_TYPE_PROP)
 
     @col_type.setter
-    def col_type(self, v: Optional[str]) -> None:
+    def col_type(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(COL_TYPE_PROP, None)
         else:
             self.properties[COL_TYPE_PROP] = v
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns a dictionary representing this ``Column``."""
         return self.properties
 
 
 class Table:
     """Object containing a high-level summary about a table"""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
-    def __init__(self, properties: Dict[str, Any]):
+    def __init__(self, properties: dict[str, Any]):
         self.properties = properties
 
     @property
     def name(self) -> str:
         """The table name"""
         return get_required(self.properties.get(TBL_NAME_PROP), self, TBL_NAME_PROP)
 
     @name.setter
     def name(self, v: str) -> None:
         self.properties[COL_NAME_PROP] = v
 
     @property
-    def description(self) -> Optional[str]:
+    def description(self) -> str | None:
         """Detailed multi-line description to explain the table. `CommonMark 0.29
         <http://commonmark.org/>`__ syntax MAY be used for rich text representation."""
         return self.properties.get(COL_DESCRIPTION_PROP)
 
     @description.setter
-    def description(self, v: Optional[str]) -> None:
+    def description(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(COL_DESCRIPTION_PROP, None)
         else:
             self.properties[COL_DESCRIPTION_PROP] = v
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns a dictionary representing this ``Table``."""
         return self.properties
 
 
 class TableExtension(
     Generic[T],
     PropertiesExtension,
@@ -132,14 +135,16 @@
     .. code-block:: python
 
         >>> item: pystac.Item = ...
         >>> tbl_ext = TableExtension.ext(item)
 
     """
 
+    name: Literal["table"] = "table"
+
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> TableExtension[T]:
         """Extend the given STAC Object with properties from the
@@ -148,56 +153,59 @@
         This extension can be applied to instances of :class:`~pystac.Collection`,
         :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Raises:
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Collection):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(TableExtension[T], CollectionTableExtension(obj))
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(TableExtension[T], ItemTableExtension(obj))
         if isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(TableExtension[T], AssetTableExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(TableExtension[T], ItemAssetsTableExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @property
-    def columns(self) -> Optional[List[Column]]:
+    def columns(self) -> list[Column] | None:
         """A list of :class:`Column` objects describing each column"""
         v = self.properties.get(COLUMNS_PROP)
         if v is None:
             return None
         return [Column(x) for x in v]
 
     @columns.setter
-    def columns(self, v: Optional[List[Column]]) -> None:
+    def columns(self, v: list[Column] | None) -> None:
         self._set_property(COLUMNS_PROP, v)
 
     @property
-    def primary_geometry(self) -> Optional[str]:
+    def primary_geometry(self) -> str | None:
         """The primary geometry column name"""
         return self._get_property(PRIMARY_GEOMETRY_PROP, str)
 
     @primary_geometry.setter
-    def primary_geometry(self, v: Optional[str]) -> None:
+    def primary_geometry(self, v: str | None) -> None:
         if v is None:
             self.properties.pop(PRIMARY_GEOMETRY_PROP, None)
         else:
             self.properties[PRIMARY_GEOMETRY_PROP] = v
 
     @property
-    def row_count(self) -> Optional[int]:
+    def row_count(self) -> int | None:
         """The number of rows in the dataset"""
         return self._get_property(ROW_COUNT_PROP, int)
 
     @row_count.setter
-    def row_count(self, v: Optional[int]) -> None:
+    def row_count(self, v: int | None) -> None:
         if v is None:
             self.properties.pop(ROW_COUNT_PROP, None)
         else:
             self.properties[ROW_COUNT_PROP] = v
 
 
 class CollectionTableExtension(TableExtension[pystac.Collection]):
@@ -206,90 +214,104 @@
     properties defined in the :stac-ext:`Table Extension <table>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`TableExtension.ext` on an :class:`~pystac.Collection` to extend it.
     """
 
     collection: pystac.Collection
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, collection: pystac.Collection):
         self.collection = collection
         self.properties = collection.extra_fields
 
     @property
-    def tables(self) -> Dict[str, Table]:
+    def tables(self) -> dict[str, Table]:
         """A mapping of table names to table objects"""
         return get_required(self.properties.get(TABLES_PROP), self, TABLES_PROP)
 
     @tables.setter
-    def tables(self, v: Dict[str, Table]) -> None:
+    def tables(self, v: dict[str, Table]) -> None:
         self.properties[TABLES_PROP] = v
 
     def __repr__(self) -> str:
-        return "<CollectionTableExtension Item id={}>".format(self.collection.id)
+        return f"<CollectionTableExtension Item id={self.collection.id}>"
 
 
 class ItemTableExtension(TableExtension[pystac.Item]):
     """A concrete implementation of :class:`TableExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`Table Extension <table>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`TableExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemTableExtension Item id={}>".format(self.item.id)
+        return f"<ItemTableExtension Item id={self.item.id}>"
 
 
 class AssetTableExtension(TableExtension[pystac.Asset]):
     """A concrete implementation of :class:`TableExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties defined
     in the :stac-ext:`Table Extension <table>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`TableExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
-    properties: Dict[str, Any]
-    additional_read_properties: Optional[List[Dict[str, Any]]]
+    properties: dict[str, Any]
+    additional_read_properties: list[dict[str, Any]] | None
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
         else:
             self.additional_read_properties = None
 
     @property
-    def storage_options(self) -> Optional[Dict[str, Any]]:
+    def storage_options(self) -> dict[str, Any] | None:
         """Additional keywords for opening the dataset"""
         return self.properties.get(STORAGE_OPTIONS_PROP)
 
     @storage_options.setter
-    def storage_options(self, v: Optional[Dict[str, Any]]) -> Any:
+    def storage_options(self, v: dict[str, Any] | None) -> Any:
         if v is None:
             self.properties.pop(STORAGE_OPTIONS_PROP, None)
         else:
             self.properties[STORAGE_OPTIONS_PROP] = v
 
     def __repr__(self) -> str:
-        return "<AssetTableExtension Item id={}>".format(self.asset_href)
+        return f"<AssetTableExtension Item id={self.asset_href}>"
+
+
+class ItemAssetsTableExtension(TableExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
+
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
 
 class TableExtensinoHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"table"}
+    prev_extension_ids = {
+        "table",
+        "https://stac-extensions.github.io/table/v1.0.0/schema.json",
+        "https://stac-extensions.github.io/table/v1.0.1/schema.json",
+        "https://stac-extensions.github.io/table/v1.1.0/schema.json",
+    }
     stac_object_types = {pystac.STACObjectType.COLLECTION, pystac.STACObjectType.ITEM}
 
 
 TABLE_EXTENSION_HOOKS: ExtensionHooks = TableExtensinoHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/timestamps.py` & `pystac-1.9.0/pystac/extensions/timestamps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Implements the :stac-ext:`Timestamps Extension <timestamps>`."""
 
 from __future__ import annotations
 
+from collections.abc import Iterable
 from datetime import datetime
-from typing import Any, Dict, Generic, Iterable, Optional, TypeVar, Union, cast
+from typing import Any, Generic, Literal, TypeVar, Union, cast
 
 import pystac
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.summaries import RangeSummary
 from pystac.utils import datetime_to_str, map_opt, str_to_datetime
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+T = TypeVar("T", pystac.Item, pystac.Asset, pystac.Collection)
 
-SCHEMA_URI = "https://stac-extensions.github.io/timestamps/v1.0.0/schema.json"
+SCHEMA_URI = "https://stac-extensions.github.io/timestamps/v1.1.0/schema.json"
 
 PUBLISHED_PROP = "published"
 EXPIRES_PROP = "expires"
 UNPUBLISHED_PROP = "unpublished"
 
 
 class TimestampsExtension(
@@ -39,19 +40,21 @@
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
        >>> ts_ext = TimestampsExtension.ext(item)
     """
 
+    name: Literal["timestamps"] = "timestamps"
+
     def apply(
         self,
-        published: Optional[datetime] = None,
-        expires: Optional[datetime] = None,
-        unpublished: Optional[datetime] = None,
+        published: datetime | None = None,
+        expires: datetime | None = None,
+        unpublished: datetime | None = None,
     ) -> None:
         """Applies timestamps extension properties to the extended Item.
 
         Args:
             published : Date and time the corresponding data
                 was published the first time.
             expires : Date and time the corresponding data
@@ -60,59 +63,59 @@
                 was unpublished.
         """
         self.published = published
         self.expires = expires
         self.unpublished = unpublished
 
     @property
-    def published(self) -> Optional[datetime]:
+    def published(self) -> datetime | None:
         """Gets or sets a datetime object that represents the date and time that the
         corresponding data was published the first time.
 
         'Published' has a different meaning depending on where it is used. If available
         in the asset properties, it refers to the timestamps valid for the actual data
         linked to the Asset Object. If it comes from the Item properties, it refers to
         timestamp valid for the metadata.
         """
         return map_opt(str_to_datetime, self._get_property(PUBLISHED_PROP, str))
 
     @published.setter
-    def published(self, v: Optional[datetime]) -> None:
+    def published(self, v: datetime | None) -> None:
         self._set_property(PUBLISHED_PROP, map_opt(datetime_to_str, v))
 
     @property
-    def expires(self) -> Optional[datetime]:
+    def expires(self) -> datetime | None:
         """Gets or sets a datetime object that represents the date and time the
         corresponding data expires (is not valid any longer).
 
         'Expires' has a different meaning depending on where it is used. If
         available in the asset properties, it refers to the timestamps valid for the
         actual data linked to the Asset Object. If it comes from the Item properties,
         it refers to to the timestamp valid for the metadata.
         """
         return map_opt(str_to_datetime, self._get_property(EXPIRES_PROP, str))
 
     @expires.setter
-    def expires(self, v: Optional[datetime]) -> None:
+    def expires(self, v: datetime | None) -> None:
         self._set_property(EXPIRES_PROP, map_opt(datetime_to_str, v))
 
     @property
-    def unpublished(self) -> Optional[datetime]:
+    def unpublished(self) -> datetime | None:
         """Gets or sets a datetime object that represents the date and time the
         corresponding data was unpublished.
 
         'Unpublished' has a different meaning depending on where it is used. If
         available in the asset properties, it refers to the timestamps valid for the
         actual data linked to the Asset Object. If it comes from the Item properties,
         it's referencing to the timestamp valid for the metadata.
         """
         return map_opt(str_to_datetime, self._get_property(UNPUBLISHED_PROP, str))
 
     @unpublished.setter
-    def unpublished(self, v: Optional[datetime]) -> None:
+    def unpublished(self, v: datetime | None) -> None:
         self._set_property(UNPUBLISHED_PROP, map_opt(datetime_to_str, v))
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
@@ -124,28 +127,28 @@
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return cast(TimestampsExtension[T], ItemTimestampsExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return cast(TimestampsExtension[T], AssetTimestampsExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
     ) -> SummariesTimestampsExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
+        cls.ensure_has_extension(obj, add_if_missing)
         return SummariesTimestampsExtension(obj)
 
 
 class ItemTimestampsExtension(TimestampsExtension[pystac.Item]):
     """A concrete implementation of :class:`TimestampsExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`Timestamps Extension <timestamps>`.
@@ -153,136 +156,139 @@
     This class should generally not be instantiated directly. Instead, call
     :meth:`TimestampsExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemTimestampsExtension Item id={}>".format(self.item.id)
+        return f"<ItemTimestampsExtension Item id={self.item.id}>"
 
 
 class AssetTimestampsExtension(TimestampsExtension[pystac.Asset]):
     """A concrete implementation of :class:`TimestampsExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties
     defined in the :stac-ext:`Timestamps Extension <timestamps>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`TimestampsExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetTimestampsExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetTimestampsExtension Asset href={self.asset_href}>"
 
 
 class SummariesTimestampsExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
     defined in the :stac-ext:`Timestamps Extension <timestamps>`.
     """
 
     @property
-    def published(self) -> Optional[RangeSummary[datetime]]:
+    def published(self) -> RangeSummary[datetime] | None:
         """Get or sets the summary of :attr:`TimestampsExtension.published` values
         for this Collection.
         """
 
         return map_opt(
             lambda s: RangeSummary(
                 str_to_datetime(s.minimum), str_to_datetime(s.maximum)
             ),
             self.summaries.get_range(PUBLISHED_PROP),
         )
 
     @published.setter
-    def published(self, v: Optional[RangeSummary[datetime]]) -> None:
+    def published(self, v: RangeSummary[datetime] | None) -> None:
         self._set_summary(
             PUBLISHED_PROP,
             map_opt(
                 lambda s: RangeSummary(
                     datetime_to_str(s.minimum), datetime_to_str(s.maximum)
                 ),
                 v,
             ),
         )
 
     @property
-    def expires(self) -> Optional[RangeSummary[datetime]]:
+    def expires(self) -> RangeSummary[datetime] | None:
         """Get or sets the summary of :attr:`TimestampsExtension.expires` values
         for this Collection.
         """
 
         return map_opt(
             lambda s: RangeSummary(
                 str_to_datetime(s.minimum), str_to_datetime(s.maximum)
             ),
             self.summaries.get_range(EXPIRES_PROP),
         )
 
     @expires.setter
-    def expires(self, v: Optional[RangeSummary[datetime]]) -> None:
+    def expires(self, v: RangeSummary[datetime] | None) -> None:
         self._set_summary(
             EXPIRES_PROP,
             map_opt(
                 lambda s: RangeSummary(
                     datetime_to_str(s.minimum), datetime_to_str(s.maximum)
                 ),
                 v,
             ),
         )
 
     @property
-    def unpublished(self) -> Optional[RangeSummary[datetime]]:
+    def unpublished(self) -> RangeSummary[datetime] | None:
         """Get or sets the summary of :attr:`TimestampsExtension.unpublished` values
         for this Collection.
         """
 
         return map_opt(
             lambda s: RangeSummary(
                 str_to_datetime(s.minimum), str_to_datetime(s.maximum)
             ),
             self.summaries.get_range(UNPUBLISHED_PROP),
         )
 
     @unpublished.setter
-    def unpublished(self, v: Optional[RangeSummary[datetime]]) -> None:
+    def unpublished(self, v: RangeSummary[datetime] | None) -> None:
         self._set_summary(
             UNPUBLISHED_PROP,
             map_opt(
                 lambda s: RangeSummary(
                     datetime_to_str(s.minimum), datetime_to_str(s.maximum)
                 ),
                 v,
             ),
         )
 
 
 class TimestampsExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
-    prev_extension_ids = {"timestamps"}
+    prev_extension_ids = {
+        "timestamps",
+        "https://stac-extensions.github.io/timestamps/v1.0.0/schema.json",
+    }
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
 TIMESTAMPS_EXTENSION_HOOKS: ExtensionHooks = TimestampsExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/view.py` & `pystac-1.9.0/pystac/extensions/sat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,297 +1,319 @@
-"""Implement the :stac-ext:`View Geometry Extension <view>`."""
+"""Implements the :stac-ext:`Satellite Extension <sat>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Generic, Iterable, Optional, TypeVar, Union, cast
+from collections.abc import Iterable
+from datetime import datetime
+from typing import (
+    Any,
+    Generic,
+    Literal,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pystac
+from pystac.extensions import item_assets
 from pystac.extensions.base import (
     ExtensionManagementMixin,
     PropertiesExtension,
     SummariesExtension,
 )
 from pystac.extensions.hooks import ExtensionHooks
 from pystac.summaries import RangeSummary
+from pystac.utils import StringEnum, datetime_to_str, map_opt, str_to_datetime
+
+T = TypeVar("T", pystac.Item, pystac.Asset, item_assets.AssetDefinition)
 
-T = TypeVar("T", pystac.Item, pystac.Asset)
+SCHEMA_URI = "https://stac-extensions.github.io/sat/v1.0.0/schema.json"
+
+PREFIX: str = "sat:"
+PLATFORM_INTERNATIONAL_DESIGNATOR_PROP: str = (
+    PREFIX + "platform_international_designator"
+)
+ABSOLUTE_ORBIT_PROP: str = PREFIX + "absolute_orbit"
+ORBIT_STATE_PROP: str = PREFIX + "orbit_state"
+RELATIVE_ORBIT_PROP: str = PREFIX + "relative_orbit"
+ANX_DATETIME_PROP: str = PREFIX + "anx_datetime"
 
-SCHEMA_URI: str = "https://stac-extensions.github.io/view/v1.0.0/schema.json"
-PREFIX: str = "view:"
 
-OFF_NADIR_PROP: str = PREFIX + "off_nadir"
-INCIDENCE_ANGLE_PROP: str = PREFIX + "incidence_angle"
-AZIMUTH_PROP: str = PREFIX + "azimuth"
-SUN_AZIMUTH_PROP: str = PREFIX + "sun_azimuth"
-SUN_ELEVATION_PROP: str = PREFIX + "sun_elevation"
+class OrbitState(StringEnum):
+    ASCENDING = "ascending"
+    DESCENDING = "descending"
+    GEOSTATIONARY = "geostationary"
 
 
-class ViewExtension(
+class SatExtension(
     Generic[T],
     PropertiesExtension,
     ExtensionManagementMixin[Union[pystac.Item, pystac.Collection]],
 ):
     """An abstract class that can be used to extend the properties of an
-    :class:`~pystac.Item` with properties from the :stac-ext:`View Geometry
-    Extension <view>`. This class is generic over the type of STAC Object to be
-    extended (e.g. :class:`~pystac.Item`, :class:`~pystac.Asset`).
+    :class:`~pystac.Item` or :class:`~pystac.Asset` with properties from the
+    :stac-ext:`Satellite Extension <sat>`. This class is generic over the type of
+    STAC Object to be extended (e.g. :class:`~pystac.Item`,
+    :class:`~pystac.Collection`).
 
-    To create a concrete instance of :class:`ViewExtension`, use the
-    :meth:`ViewExtension.ext` method. For example:
+    To create a concrete instance of :class:`SatExtension`, use the
+    :meth:`SatExtension.ext` method. For example:
 
     .. code-block:: python
 
        >>> item: pystac.Item = ...
-       >>> view_ext = ViewExtension.ext(item)
+       >>> sat_ext = SatExtension.ext(item)
     """
 
+    name: Literal["sat"] = "sat"
+
     def apply(
         self,
-        off_nadir: Optional[float] = None,
-        incidence_angle: Optional[float] = None,
-        azimuth: Optional[float] = None,
-        sun_azimuth: Optional[float] = None,
-        sun_elevation: Optional[float] = None,
+        orbit_state: OrbitState | None = None,
+        relative_orbit: int | None = None,
+        absolute_orbit: int | None = None,
+        platform_international_designator: str | None = None,
+        anx_datetime: datetime | None = None,
     ) -> None:
-        """Applies View Geometry extension properties to the extended
-        :class:`~pystac.Item`.
+        """Applies ext extension properties to the extended :class:`~pystac.Item` or
+        class:`~pystac.Asset`.
 
-        Args:
-            off_nadir : The angle from the sensor between nadir (straight down)
-                and the scene center. Measured in degrees (0-90).
-            incidence_angle : The incidence angle is the angle between the
-                vertical (normal) to the intercepting surface and the line of sight
-                back to the satellite at the scene center. Measured in degrees (0-90).
-            azimuth : Viewing azimuth angle. The angle measured from the
-                sub-satellite point (point on the ground below the platform) between
-                the scene center and true north. Measured clockwise from north in
-                degrees (0-360).
-            sun_azimuth : Sun azimuth angle. From the scene center point on the
-                ground, this is the angle between truth north and the sun. Measured
-                clockwise in degrees (0-360).
-            sun_elevation : Sun elevation angle. The angle from the tangent of
-                the scene center point to the sun. Measured from the horizon in
-                degrees (0-90).
-        """
-        self.off_nadir = off_nadir
-        self.incidence_angle = incidence_angle
-        self.azimuth = azimuth
-        self.sun_azimuth = sun_azimuth
-        self.sun_elevation = sun_elevation
+        Must specify at least one of orbit_state or relative_orbit in order
+        for the sat extension to properties to be valid.
 
-    @property
-    def off_nadir(self) -> Optional[float]:
-        """Get or sets the angle from the sensor between nadir (straight down)
-        and the scene center. Measured in degrees (0-90).
+        Args:
+            orbit_state : Optional state of the orbit. Either ascending or
+                descending for polar orbiting satellites, or geostationary for
+                geosynchronous satellites.
+            relative_orbit : Optional non-negative integer of the orbit number at
+                the time of acquisition.
         """
-        return self._get_property(OFF_NADIR_PROP, float)
 
-    @off_nadir.setter
-    def off_nadir(self, v: Optional[float]) -> None:
-        self._set_property(OFF_NADIR_PROP, v)
+        self.platform_international_designator = platform_international_designator
+        self.orbit_state = orbit_state
+        self.absolute_orbit = absolute_orbit
+        self.relative_orbit = relative_orbit
+        self.anx_datetime = anx_datetime
 
     @property
-    def incidence_angle(self) -> Optional[float]:
-        """Get or sets the incidence angle is the angle between the vertical (normal)
-        to the intercepting surface and the line of sight back to the satellite at
-        the scene center. Measured in degrees (0-90).
-        """
-        return self._get_property(INCIDENCE_ANGLE_PROP, float)
-
-    @incidence_angle.setter
-    def incidence_angle(self, v: Optional[float]) -> None:
-        self._set_property(INCIDENCE_ANGLE_PROP, v)
+    def platform_international_designator(self) -> str | None:
+        """Gets or sets the International Designator, also known as COSPAR ID, and
+        NSSDCA ID."""
+        return self._get_property(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, str)
+
+    @platform_international_designator.setter
+    def platform_international_designator(self, v: str | None) -> None:
+        self._set_property(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, v)
 
     @property
-    def azimuth(self) -> Optional[float]:
-        """Get or sets the viewing azimuth angle.
-
-        The angle measured from the sub-satellite
-        point (point on the ground below the platform) between the scene center and true
-        north. Measured clockwise from north in degrees (0-360).
-        """
-        return self._get_property(AZIMUTH_PROP, float)
-
-    @azimuth.setter
-    def azimuth(self, v: Optional[float]) -> None:
-        self._set_property(AZIMUTH_PROP, v)
+    def orbit_state(self) -> OrbitState | None:
+        """Get or sets an orbit state of the object."""
+        return map_opt(
+            lambda x: OrbitState(x), self._get_property(ORBIT_STATE_PROP, str)
+        )
+
+    @orbit_state.setter
+    def orbit_state(self, v: OrbitState | None) -> None:
+        self._set_property(ORBIT_STATE_PROP, map_opt(lambda x: x.value, v))
 
     @property
-    def sun_azimuth(self) -> Optional[float]:
-        """Get or sets the sun azimuth angle.
-
-        From the scene center point on the ground, this
-        is the angle between truth north and the sun. Measured clockwise in
-        degrees (0-360).
-        """
-        return self._get_property(SUN_AZIMUTH_PROP, float)
+    def absolute_orbit(self) -> int | None:
+        """Get or sets a absolute orbit number of the item."""
+        return self._get_property(ABSOLUTE_ORBIT_PROP, int)
+
+    @absolute_orbit.setter
+    def absolute_orbit(self, v: int | None) -> None:
+        self._set_property(ABSOLUTE_ORBIT_PROP, v)
 
-    @sun_azimuth.setter
-    def sun_azimuth(self, v: Optional[float]) -> None:
-        self._set_property(SUN_AZIMUTH_PROP, v)
+    @property
+    def relative_orbit(self) -> int | None:
+        """Get or sets a relative orbit number of the item."""
+        return self._get_property(RELATIVE_ORBIT_PROP, int)
+
+    @relative_orbit.setter
+    def relative_orbit(self, v: int | None) -> None:
+        self._set_property(RELATIVE_ORBIT_PROP, v)
 
     @property
-    def sun_elevation(self) -> Optional[float]:
-        """Get or sets the sun elevation angle. The angle from the tangent of the scene
-        center point to the sun. Measured from the horizon in degrees (0-90).
-        """
-        return self._get_property(SUN_ELEVATION_PROP, float)
+    def anx_datetime(self) -> datetime | None:
+        return map_opt(str_to_datetime, self._get_property(ANX_DATETIME_PROP, str))
 
-    @sun_elevation.setter
-    def sun_elevation(self, v: Optional[float]) -> None:
-        self._set_property(SUN_ELEVATION_PROP, v)
+    @anx_datetime.setter
+    def anx_datetime(self, v: datetime | None) -> None:
+        self._set_property(ANX_DATETIME_PROP, map_opt(datetime_to_str, v))
 
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
-    def ext(cls, obj: T, add_if_missing: bool = False) -> ViewExtension[T]:
-        """Extends the given STAC Object with properties from the :stac-ext:`View
-        Geometry Extension <scientific>`.
+    def ext(cls, obj: T, add_if_missing: bool = False) -> SatExtension[T]:
+        """Extends the given STAC Object with properties from the :stac-ext:`Satellite
+        Extension <sat>`.
 
         This extension can be applied to instances of :class:`~pystac.Item` or
         :class:`~pystac.Asset`.
 
         Raises:
 
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
-            return cast(ViewExtension[T], ItemViewExtension(obj))
+            cls.ensure_has_extension(obj, add_if_missing)
+            return cast(SatExtension[T], ItemSatExtension(obj))
         elif isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
-            return cast(ViewExtension[T], AssetViewExtension(obj))
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(SatExtension[T], AssetSatExtension(obj))
+        elif isinstance(obj, item_assets.AssetDefinition):
+            cls.ensure_owner_has_extension(obj, add_if_missing)
+            return cast(SatExtension[T], ItemAssetsSatExtension(obj))
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
     @classmethod
     def summaries(
         cls, obj: pystac.Collection, add_if_missing: bool = False
-    ) -> SummariesViewExtension:
+    ) -> SummariesSatExtension:
         """Returns the extended summaries object for the given collection."""
-        cls.validate_has_extension(obj, add_if_missing)
-        return SummariesViewExtension(obj)
+        cls.ensure_has_extension(obj, add_if_missing)
+        return SummariesSatExtension(obj)
 
 
-class ItemViewExtension(ViewExtension[pystac.Item]):
-    """A concrete implementation of :class:`ViewExtension` on an :class:`~pystac.Item`
+class ItemSatExtension(SatExtension[pystac.Item]):
+    """A concrete implementation of :class:`SatExtension` on an :class:`~pystac.Item`
     that extends the properties of the Item to include properties defined in the
-    :stac-ext:`View Geometry Extension <view>`.
+    :stac-ext:`Satellite Extension <sat>`.
 
     This class should generally not be instantiated directly. Instead, call
-    :meth:`ViewExtension.ext` on an :class:`~pystac.Item` to extend it.
+    :meth:`SatExtension.ext` on an :class:`~pystac.Item` to
+    extend it.
     """
 
     item: pystac.Item
     """The :class:`~pystac.Item` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Item` properties, including extension properties."""
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemViewExtension Item id={}>".format(self.item.id)
+        return f"<ItemSatExtension Item id={self.item.id}>"
 
 
-class AssetViewExtension(ViewExtension[pystac.Asset]):
-    """A concrete implementation of :class:`ViewExtension` on an :class:`~pystac.Asset`
-    that extends the Asset fields to include properties defined in the
-    :stac-ext:`View Geometry Extension <view>`.
+class AssetSatExtension(SatExtension[pystac.Asset]):
+    """A concrete implementation of :class:`SatExtension` on an :class:`~pystac.Asset`
+    that extends the properties of the Asset to include properties defined in the
+    :stac-ext:`Satellite Extension <sat>`.
 
     This class should generally not be instantiated directly. Instead, call
-    :meth:`ViewExtension.ext` on an :class:`~pystac.Asset` to extend it.
+    :meth:`SatExtension.ext` on an :class:`~pystac.Asset` to
+    extend it.
     """
 
     asset_href: str
     """The ``href`` value of the :class:`~pystac.Asset` being extended."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """The :class:`~pystac.Asset` fields, including extension properties."""
 
-    additional_read_properties: Optional[Iterable[Dict[str, Any]]] = None
+    additional_read_properties: Iterable[dict[str, Any]] | None = None
     """If present, this will be a list containing 1 dictionary representing the
     properties of the owning :class:`~pystac.Item`."""
 
     def __init__(self, asset: pystac.Asset):
         self.asset_href = asset.href
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     def __repr__(self) -> str:
-        return "<AssetViewExtension Asset href={}>".format(self.asset_href)
+        return f"<AssetSatExtension Asset href={self.asset_href}>"
+
+
+class ItemAssetsSatExtension(SatExtension[item_assets.AssetDefinition]):
+    properties: dict[str, Any]
+    asset_defn: item_assets.AssetDefinition
 
+    def __init__(self, item_asset: item_assets.AssetDefinition):
+        self.asset_defn = item_asset
+        self.properties = item_asset.properties
 
-class SummariesViewExtension(SummariesExtension):
+
+class SummariesSatExtension(SummariesExtension):
     """A concrete implementation of :class:`~SummariesExtension` that extends
     the ``summaries`` field of a :class:`~pystac.Collection` to include properties
-    defined in the :stac-ext:`View Object Extension <view>`.
+    defined in the :stac-ext:`Satellite Extension <sat>`.
     """
 
     @property
-    def off_nadir(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`ViewExtension.off_nadir` values for
-        this Collection.
+    def platform_international_designator(self) -> list[str] | None:
+        """Get or sets the summary of
+        :attr:`SatExtension.platform_international_designator` values for this
+        Collection.
         """
-        return self.summaries.get_range(OFF_NADIR_PROP)
-
-    @off_nadir.setter
-    def off_nadir(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(OFF_NADIR_PROP, v)
 
-    @property
-    def incidence_angle(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`ViewExtension.incidence_angle` values
-        for this Collection.
-        """
-        return self.summaries.get_range(INCIDENCE_ANGLE_PROP)
+        return self.summaries.get_list(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP)
 
-    @incidence_angle.setter
-    def incidence_angle(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(INCIDENCE_ANGLE_PROP, v)
+    @platform_international_designator.setter
+    def platform_international_designator(self, v: list[str] | None) -> None:
+        self._set_summary(PLATFORM_INTERNATIONAL_DESIGNATOR_PROP, v)
 
     @property
-    def azimuth(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`ViewExtension.azimuth` values
+    def orbit_state(self) -> list[OrbitState] | None:
+        """Get or sets the summary of :attr:`SatExtension.orbit_state` values
         for this Collection.
         """
-        return self.summaries.get_range(AZIMUTH_PROP)
 
-    @azimuth.setter
-    def azimuth(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(AZIMUTH_PROP, v)
+        return self.summaries.get_list(ORBIT_STATE_PROP)
+
+    @orbit_state.setter
+    def orbit_state(self, v: list[OrbitState] | None) -> None:
+        self._set_summary(ORBIT_STATE_PROP, v)
 
     @property
-    def sun_azimuth(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`ViewExtension.sun_azimuth` values
-        for this Collection.
-        """
-        return self.summaries.get_range(SUN_AZIMUTH_PROP)
+    def absolute_orbit(self) -> RangeSummary[int] | None:
+        return self.summaries.get_range(ABSOLUTE_ORBIT_PROP)
 
-    @sun_azimuth.setter
-    def sun_azimuth(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(SUN_AZIMUTH_PROP, v)
+    @absolute_orbit.setter
+    def absolute_orbit(self, v: RangeSummary[int] | None) -> None:
+        self._set_summary(ABSOLUTE_ORBIT_PROP, v)
 
     @property
-    def sun_elevation(self) -> Optional[RangeSummary[float]]:
-        """Get or sets the summary of :attr:`ViewExtension.sun_elevation` values
-        for this Collection.
-        """
-        return self.summaries.get_range(SUN_ELEVATION_PROP)
+    def relative_orbit(self) -> RangeSummary[int] | None:
+        return self.summaries.get_range(RELATIVE_ORBIT_PROP)
 
-    @sun_elevation.setter
-    def sun_elevation(self, v: Optional[RangeSummary[float]]) -> None:
-        self._set_summary(SUN_ELEVATION_PROP, v)
+    @relative_orbit.setter
+    def relative_orbit(self, v: RangeSummary[int] | None) -> None:
+        self._set_summary(RELATIVE_ORBIT_PROP, v)
 
-
-class ViewExtensionHooks(ExtensionHooks):
-    schema_uri = SCHEMA_URI
-    prev_extension_ids = {"view"}
+    @property
+    def anx_datetime(self) -> RangeSummary[datetime] | None:
+        return map_opt(
+            lambda s: RangeSummary(
+                str_to_datetime(s.minimum), str_to_datetime(s.maximum)
+            ),
+            self.summaries.get_range(ANX_DATETIME_PROP),
+        )
+
+    @anx_datetime.setter
+    def anx_datetime(self, v: RangeSummary[datetime] | None) -> None:
+        self._set_summary(
+            ANX_DATETIME_PROP,
+            map_opt(
+                lambda s: RangeSummary(
+                    datetime_to_str(s.minimum), datetime_to_str(s.maximum)
+                ),
+                v,
+            ),
+        )
+
+
+class SatExtensionHooks(ExtensionHooks):
+    schema_uri: str = SCHEMA_URI
+    prev_extension_ids = {"sat"}
     stac_object_types = {pystac.STACObjectType.ITEM}
 
 
-VIEW_EXTENSION_HOOKS: ExtensionHooks = ViewExtensionHooks()
+SAT_EXTENSION_HOOKS: ExtensionHooks = SatExtensionHooks()
```

### Comparing `pystac-1.8.4/pystac/extensions/xarray_assets.py` & `pystac-1.9.0/pystac/extensions/xarray_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Implements the :stac-ext:`Xarray Assets Extension <xarray>`."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
+from typing import Any, Generic, Literal, TypeVar, Union
 
 import pystac
 from pystac.extensions.base import ExtensionManagementMixin, PropertiesExtension
 from pystac.extensions.hooks import ExtensionHooks
 
 T = TypeVar("T", pystac.Collection, pystac.Item, pystac.Asset)
 
@@ -34,14 +34,16 @@
     .. code-block:: python
 
         >>> item: pystac.Item = ...
         >>> xr_ext = XarrayAssetsExtension.ext(item)
 
     """
 
+    name: Literal["xarray"] = "xarray"
+
     @classmethod
     def get_schema_uri(cls) -> str:
         return SCHEMA_URI
 
     @classmethod
     def ext(cls, obj: T, add_if_missing: bool = False) -> XarrayAssetsExtension[T]:
         """Extend the given STAC Object with properties from the
@@ -50,21 +52,21 @@
         This extension can be applied to instances of :class:`~pystac.Collection`,
         :class:`~pystac.Item` or :class:`~pystac.Asset`.
 
         Raises:
             pystac.ExtensionTypeError : If an invalid object type is passed.
         """
         if isinstance(obj, pystac.Collection):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return CollectionXarrayAssetsExtension(obj)
         if isinstance(obj, pystac.Item):
-            cls.validate_has_extension(obj, add_if_missing)
+            cls.ensure_has_extension(obj, add_if_missing)
             return ItemXarrayAssetsExtension(obj)
         if isinstance(obj, pystac.Asset):
-            cls.validate_owner_has_extension(obj, add_if_missing)
+            cls.ensure_owner_has_extension(obj, add_if_missing)
             return AssetXarrayAssetsExtension(obj)
         else:
             raise pystac.ExtensionTypeError(cls._ext_error_message(obj))
 
 
 class CollectionXarrayAssetsExtension(XarrayAssetsExtension[pystac.Collection]):
     """A concrete implementation of :class:`XarrayAssetsExtension` on a
@@ -72,89 +74,89 @@
     properties defined in the :stac-ext:`XarrayAssets Extension <xarray>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`XarrayAssetsExtension.ext` on an :class:`~pystac.Collection` to extend it.
     """
 
     collection: pystac.Collection
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, collection: pystac.Collection):
         self.collection = collection
         self.properties = collection.extra_fields
 
     def __repr__(self) -> str:
-        return "<CollectionXarrayAssetsExtension Item id={}>".format(self.collection.id)
+        return f"<CollectionXarrayAssetsExtension Item id={self.collection.id}>"
 
 
 class ItemXarrayAssetsExtension(XarrayAssetsExtension[pystac.Item]):
     """A concrete implementation of :class:`XarrayAssetsExtension` on an
     :class:`~pystac.Item` that extends the properties of the Item to include properties
     defined in the :stac-ext:`XarrayAssets Extension <xarray>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`XarrayAssetsExtension.ext` on an :class:`~pystac.Item` to extend it.
     """
 
     item: pystac.Item
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
 
     def __init__(self, item: pystac.Item):
         self.item = item
         self.properties = item.properties
 
     def __repr__(self) -> str:
-        return "<ItemXarrayAssetsExtension Item id={}>".format(self.item.id)
+        return f"<ItemXarrayAssetsExtension Item id={self.item.id}>"
 
 
 class AssetXarrayAssetsExtension(XarrayAssetsExtension[pystac.Asset]):
     """A concrete implementation of :class:`XarrayAssetsExtension` on an
     :class:`~pystac.Asset` that extends the Asset fields to include properties defined
     in the :stac-ext:`XarrayAssets Extension <xarray>`.
 
     This class should generally not be instantiated directly. Instead, call
     :meth:`XarrayAssetsExtension.ext` on an :class:`~pystac.Asset` to extend it.
     """
 
     asset: pystac.Asset
-    properties: Dict[str, Any]
-    additional_read_properties: Optional[List[Dict[str, Any]]] = None
+    properties: dict[str, Any]
+    additional_read_properties: list[dict[str, Any]] | None = None
 
     def __init__(self, asset: pystac.Asset):
         self.asset = asset
         self.properties = asset.extra_fields
         if asset.owner and isinstance(asset.owner, pystac.Item):
             self.additional_read_properties = [asset.owner.properties]
 
     @property
-    def storage_options(self) -> Optional[Dict[str, Any]]:
+    def storage_options(self) -> dict[str, Any] | None:
         """Additional keywords for accessing the dataset from remote storage"""
         return self.properties.get(STORAGE_OPTIONS_PROP)
 
     @storage_options.setter
-    def storage_options(self, v: Optional[Dict[str, Any]]) -> Any:
+    def storage_options(self, v: dict[str, Any] | None) -> Any:
         if v is None:
             self.properties.pop(STORAGE_OPTIONS_PROP, None)
         else:
             self.properties[STORAGE_OPTIONS_PROP] = v
 
     @property
-    def open_kwargs(self) -> Optional[Dict[str, Any]]:
+    def open_kwargs(self) -> dict[str, Any] | None:
         """Additional keywords for opening the dataset"""
         return self.properties.get(OPEN_KWARGS_PROP)
 
     @open_kwargs.setter
-    def open_kwargs(self, v: Optional[Dict[str, Any]]) -> Any:
+    def open_kwargs(self, v: dict[str, Any] | None) -> Any:
         if v is None:
             self.properties.pop(OPEN_KWARGS_PROP, None)
         else:
             self.properties[OPEN_KWARGS_PROP] = v
 
     def __repr__(self) -> str:
-        return "<AssetXarrayAssetsExtension Asset href={}>".format(self.asset.href)
+        return f"<AssetXarrayAssetsExtension Asset href={self.asset.href}>"
 
 
 class XarrayAssetsExtensionHooks(ExtensionHooks):
     schema_uri: str = SCHEMA_URI
     prev_extension_ids = {"xarray"}
     stac_object_types = {pystac.STACObjectType.COLLECTION, pystac.STACObjectType.ITEM}
```

### Comparing `pystac-1.8.4/pystac/html/JSON.jinja2` & `pystac-1.9.0/pystac/html/JSON.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/html/Macros.jinja2` & `pystac-1.9.0/pystac/html/Macros.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/item.py` & `pystac-1.9.0/pystac/item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import warnings
 from copy import copy, deepcopy
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, TypeVar, cast
 
 import pystac
 from pystac import RelType, STACError, STACObjectType
-from pystac.asset import Asset
+from pystac.asset import Asset, Assets
 from pystac.catalog import Catalog
 from pystac.collection import Collection
 from pystac.errors import DeprecatedWarning, ExtensionNotImplemented
 from pystac.link import Link
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
@@ -27,16 +27,18 @@
 
 T = TypeVar("T", bound="Item")
 
 if TYPE_CHECKING:
     # avoids conflicts since there are also kwargs and attrs called `datetime`
     from datetime import datetime as Datetime
 
+    from pystac.extensions.ext import ItemExt
 
-class Item(STACObject):
+
+class Item(STACObject, Assets):
     """An Item is the core granular entity in a STAC, containing the core metadata
     that enables any client to search or crawl online catalogs of spatial 'assets' -
     satellite imagery, derived data, DEM's, etc.
 
     Args:
         id : Provider identifier. Must be unique within the STAC.
         geometry : Defines the full footprint of the asset represented by this
@@ -61,86 +63,86 @@
         extra_fields : Extra fields that are part of the top-level JSON
             properties of the Item.
         assets : A dictionary mapping string keys to :class:`~pystac.Asset` objects. All
             :class:`~pystac.Asset` values in the dictionary will have their
             :attr:`~pystac.Asset.owner` attribute set to the created Item.
     """
 
-    assets: Dict[str, Asset]
+    assets: dict[str, Asset]
     """Dictionary of :class:`~pystac.Asset` objects, each with a unique key."""
 
-    bbox: Optional[List[float]]
+    bbox: list[float] | None
     """Bounding Box of the asset represented by this item using either 2D or 3D
     geometries. The length of the array is 2*n where n is the number of dimensions.
     Could also be None in the case of a null geometry."""
 
-    collection: Optional[Collection]
+    collection: Collection | None
     """:class:`~pystac.Collection` to which this Item belongs, if any."""
 
-    collection_id: Optional[str]
+    collection_id: str | None
     """The Collection ID that this item belongs to, if any."""
 
-    datetime: Optional[Datetime]
+    datetime: Datetime | None
     """Datetime associated with this item. If ``None``, then
     :attr:`~pystac.CommonMetadata.start_datetime` and
     :attr:`~pystac.CommonMetadata.end_datetime` in :attr:`~pystac.Item.common_metadata`
     will supply the datetime range of the Item."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Extra fields that are part of the top-level JSON fields the Item."""
 
-    geometry: Optional[Dict[str, Any]]
+    geometry: dict[str, Any] | None
     """Defines the full footprint of the asset represented by this item, formatted
     according to `RFC 7946, section 3.1 (GeoJSON)
     <https://tools.ietf.org/html/rfc7946>`_."""
 
     id: str
     """Provider identifier. Unique within the STAC."""
 
-    links: List[Link]
+    links: list[Link]
     """A list of :class:`~pystac.Link` objects representing all links associated with
     this Item."""
 
-    properties: Dict[str, Any]
+    properties: dict[str, Any]
     """A dictionary of additional metadata for the Item."""
 
-    stac_extensions: List[str]
+    stac_extensions: list[str]
     """List of extensions the Item implements."""
 
     STAC_OBJECT_TYPE = STACObjectType.ITEM
 
     def __init__(
         self,
         id: str,
-        geometry: Optional[Dict[str, Any]],
-        bbox: Optional[List[float]],
-        datetime: Optional[Datetime],
-        properties: Dict[str, Any],
-        start_datetime: Optional[Datetime] = None,
-        end_datetime: Optional[Datetime] = None,
-        stac_extensions: Optional[List[str]] = None,
-        href: Optional[str] = None,
-        collection: Optional[Union[str, Collection]] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
-        assets: Optional[Dict[str, Asset]] = None,
+        geometry: dict[str, Any] | None,
+        bbox: list[float] | None,
+        datetime: Datetime | None,
+        properties: dict[str, Any],
+        start_datetime: Datetime | None = None,
+        end_datetime: Datetime | None = None,
+        stac_extensions: list[str] | None = None,
+        href: str | None = None,
+        collection: str | Collection | None = None,
+        extra_fields: dict[str, Any] | None = None,
+        assets: dict[str, Asset] | None = None,
     ):
         super().__init__(stac_extensions or [])
 
         self.id = id
         self.geometry = geometry
         self.bbox = bbox
         self.properties = properties
         if extra_fields is None:
             self.extra_fields = {}
         else:
             self.extra_fields = extra_fields
 
-        self.assets: Dict[str, Asset] = {}
+        self.assets: dict[str, Asset] = {}
 
-        self.datetime: Optional[Datetime] = None
+        self.datetime: Datetime | None = None
         if start_datetime:
             properties["start_datetime"] = datetime_to_str(start_datetime)
         if end_datetime:
             properties["end_datetime"] = datetime_to_str(end_datetime)
         if datetime is None:
             if "start_datetime" not in properties or "end_datetime" not in properties:
                 raise STACError(
@@ -151,30 +153,30 @@
             self.datetime = None
         else:
             self.datetime = datetime
 
         if href is not None:
             self.set_self_href(href)
 
-        self.collection_id: Optional[str] = None
+        self.collection_id: str | None = None
         if collection is not None:
             if isinstance(collection, Collection):
                 self.set_collection(collection)
             else:
                 self.collection_id = collection
 
         self.assets = {}
         if assets is not None:
             for k, asset in assets.items():
                 self.add_asset(k, asset)
 
     def __repr__(self) -> str:
-        return "<Item id={}>".format(self.id)
+        return f"<Item id={self.id}>"
 
-    def set_self_href(self, href: Optional[str]) -> None:
+    def set_self_href(self, href: str | None) -> None:
         """Sets the absolute HREF that is represented by the ``rel == 'self'``
         :class:`~pystac.Link`.
 
         Changing the self HREF of the item will ensure that all asset HREFs
         remain valid. If asset HREFs are relative, the HREFs will change
         to point to the same location based on the new item self HREF,
         either by making them relative to the new location or making them
@@ -196,15 +198,15 @@
             for asset in self.assets.values():
                 asset_href = asset.href
                 if not is_absolute_href(asset_href):
                     abs_href = make_absolute_href(asset_href, prev_href)
                     new_relative_href = make_relative_href(abs_href, new_href)
                     asset.href = new_relative_href
 
-    def get_datetime(self, asset: Optional[Asset] = None) -> Optional[Datetime]:
+    def get_datetime(self, asset: Asset | None = None) -> Datetime | None:
         """Gets an Item or an Asset datetime.
 
         If an Asset is supplied and the Item property exists on the Asset,
         returns the Asset's value. Otherwise returns the Item's value.
 
         Returns:
             datetime or None
@@ -214,114 +216,26 @@
         else:
             asset_dt = asset.extra_fields.get("datetime")
             if asset_dt is None:
                 return None
             else:
                 return str_to_datetime(asset_dt)
 
-    def set_datetime(self, datetime: Datetime, asset: Optional[Asset] = None) -> None:
+    def set_datetime(self, datetime: Datetime, asset: Asset | None = None) -> None:
         """Set an Item or an Asset datetime.
 
         If an Asset is supplied, sets the property on the Asset.
         Otherwise sets the Item's value.
         """
         if asset is None:
             self.datetime = datetime
         else:
             asset.extra_fields["datetime"] = datetime_to_str(datetime)
 
-    def get_assets(
-        self,
-        media_type: Optional[Union[str, pystac.MediaType]] = None,
-        role: Optional[str] = None,
-    ) -> Dict[str, Asset]:
-        """Get this item's assets.
-
-        Args:
-            media_type: If set, filter the assets such that only those with a
-                matching ``media_type`` are returned.
-            role: If set, filter the assets such that only those with a matching
-                ``role`` are returned.
-
-        Returns:
-            Dict[str, Asset]: A dictionary of assets that match ``media_type``
-                and/or ``role`` if set or else all of this item's assets.
-        """
-        return {
-            k: deepcopy(v)
-            for k, v in self.assets.items()
-            if (media_type is None or v.media_type == media_type)
-            and (role is None or v.has_role(role))
-        }
-
-    def add_asset(self, key: str, asset: Asset) -> None:
-        """Adds an Asset to this item.
-
-        Args:
-            key : The unique key of this asset.
-            asset : The Asset to add.
-        """
-        asset.set_owner(self)
-        self.assets[key] = asset
-
-    def delete_asset(self, key: str) -> None:
-        """Deletes the asset at the given key, and removes the asset's data
-        file from the local filesystem.
-
-        It is an error to attempt to delete an asset's file if it is on a
-        remote filesystem.
-
-        To delete the asset without removing the file, use `del item.assets["key"]`.
-
-        Args:
-            key: The unique key of this asset.
-        """
-        asset = self.assets[key]
-        asset.set_owner(self)
-        asset.delete()
-
-        del self.assets[key]
-
-    def make_asset_hrefs_relative(self) -> Item:
-        """Modify each asset's HREF to be relative to this item's self HREF.
-
-        Returns:
-            Item: self
-        """
-        self_href = self.get_self_href()
-        for asset in self.assets.values():
-            if is_absolute_href(asset.href):
-                if self_href is None:
-                    raise STACError(
-                        "Cannot make asset HREFs relative " "if no self_href is set."
-                    )
-                asset.href = make_relative_href(asset.href, self_href)
-        return self
-
-    def make_asset_hrefs_absolute(self) -> Item:
-        """Modify each asset's HREF to be absolute.
-
-        Any asset HREFs that are relative will be modified to absolute based on this
-        item's self HREF.
-
-        Returns:
-            Item: self
-        """
-        self_href = self.get_self_href()
-        for asset in self.assets.values():
-            if not is_absolute_href(asset.href):
-                if self_href is None:
-                    raise STACError(
-                        "Cannot make relative asset HREFs absolute "
-                        "if no self_href is set."
-                    )
-                asset.href = make_absolute_href(asset.href, self_href)
-        return self
-
-    def set_collection(self, collection: Optional[Collection]) -> Item:
+    def set_collection(self, collection: Collection | None) -> Item:
         """Set the collection of this item.
 
         This method will replace any existing Collection link and attribute for
         this item.
 
         Args:
             collection : The collection to set as this
@@ -334,30 +248,30 @@
         self.collection_id = None
         if collection is not None:
             self.add_link(Link.collection(collection))
             self.collection_id = collection.id
 
         return self
 
-    def get_collection(self) -> Optional[Collection]:
+    def get_collection(self) -> Collection | None:
         """Gets the collection of this item, if one exists.
 
         Returns:
             Collection or None: If this item belongs to a collection, returns
             a reference to the collection. Otherwise returns None.
         """
         collection_link = self.get_single_link(pystac.RelType.COLLECTION)
         if collection_link is None:
             return None
         else:
             return cast(
                 Collection, collection_link.resolve_stac_object(self.get_root()).target
             )
 
-    def add_derived_from(self, *items: Union[Item, str]) -> Item:
+    def add_derived_from(self, *items: Item | str) -> Item:
         """Add one or more items that this is derived from.
 
         This method will add to any existing "derived_from" links.
 
         Args:
             items : Items (or href of items) to add to derived_from links.
 
@@ -372,15 +286,15 @@
         """Remove an item that this is derived from.
 
         This method will remove from existing "derived_from" links.
 
         Args:
             item_id : ID of item to remove from derived_from links.
         """
-        new_links: List[pystac.Link] = []
+        new_links: list[pystac.Link] = []
 
         for link in self.links:
             if link.rel != pystac.RelType.DERIVED_FROM:
                 new_links.append(link)
             else:
                 try:
                     item = cast(Item, link.resolve_stac_object().target)
@@ -388,15 +302,15 @@
                     raise pystac.STACError(
                         "Link failed to resolve. Use remove_links instead."
                     ) from e
                 if item.id != item_id:
                     new_links.append(link)
         self.links = new_links
 
-    def get_derived_from(self) -> List[Item]:
+    def get_derived_from(self) -> list[Item]:
         """Get the items that this is derived from.
 
         Returns:
             List[Item]: Returns a reference to the derived_from items.
         """
         links = self.get_links(pystac.RelType.DERIVED_FROM)
         try:
@@ -404,27 +318,27 @@
         except Exception as e:
             raise pystac.STACError(
                 "Link failed to resolve. Use get_links instead."
             ) from e
 
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         links = self.links
         if not include_self_link:
             links = [x for x in links if x.rel != pystac.RelType.SELF]
 
         assets = {k: v.to_dict() for k, v in self.assets.items()}
 
         if self.datetime is not None:
             self.properties["datetime"] = datetime_to_str(self.datetime)
         else:
             self.properties["datetime"] = None
 
-        d: Dict[str, Any] = {
+        d: dict[str, Any] = {
             "type": "Feature",
             "stac_version": pystac.get_stac_version(),
             "id": self.id,
             "properties": self.properties,
             "geometry": self.geometry,
             "links": [link.to_dict(transform_href=transform_hrefs) for link in links],
             "assets": assets,
@@ -457,26 +371,26 @@
             assets={k: asset.clone() for k, asset in self.assets.items()},
         )
         for link in self.links:
             clone.add_link(link.clone())
 
         return clone
 
-    def _object_links(self) -> List[Union[str, pystac.RelType]]:
+    def _object_links(self) -> list[str | pystac.RelType]:
         return [
             pystac.RelType.COLLECTION,
             *pystac.EXTENSION_HOOKS.get_extended_object_links(self),
         ]
 
     @classmethod
     def from_dict(
-        cls: Type[T],
-        d: Dict[str, Any],
-        href: Optional[str] = None,
-        root: Optional[Catalog] = None,
+        cls: type[T],
+        d: dict[str, Any],
+        href: str | None = None,
+        root: Catalog | None = None,
         migrate: bool = False,
         preserve_dict: bool = True,
     ) -> T:
         from pystac.extensions.version import ItemVersionExtension
 
         if preserve_dict:
             d = deepcopy(d)
@@ -548,30 +462,42 @@
     @property
     def common_metadata(self) -> pystac.CommonMetadata:
         """Access the item's common metadata fields as a
         :class:`~pystac.CommonMetadata` object."""
         return pystac.CommonMetadata(self)
 
     def full_copy(
-        self, root: Optional[Catalog] = None, parent: Optional[Catalog] = None
+        self, root: Catalog | None = None, parent: Catalog | None = None
     ) -> Item:
         return cast(Item, super().full_copy(root, parent))
 
     @classmethod
-    def matches_object_type(cls, d: Dict[str, Any]) -> bool:
+    def matches_object_type(cls, d: dict[str, Any]) -> bool:
         for field in ("type", "stac_version"):
             if field not in d:
                 raise pystac.STACTypeError(d, cls, f"'{field}' is missing.")
         return identify_stac_object_type(d) == STACObjectType.ITEM
 
     @property
-    def __geo_interface__(self) -> Dict[str, Any]:
+    def __geo_interface__(self) -> dict[str, Any]:
         """Returns this item as a dictionary.
 
         This just calls `to_dict` without self links or transforming any hrefs.
 
         https://gist.github.com/sgillies/2217756
 
         Returns:
             Dict[str, Any]: This item as a dictionary.
         """
         return self.to_dict(include_self_link=False, transform_hrefs=False)
+
+    @property
+    def ext(self) -> ItemExt:
+        """Accessor for extension classes on this item
+
+        Example::
+
+            item.ext.proj.epsg = 4326
+        """
+        from pystac.extensions.ext import ItemExt
+
+        return ItemExt(stac_object=self)
```

### Comparing `pystac-1.8.4/pystac/item_collection.py` & `pystac-1.9.0/pystac/item_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from __future__ import annotations
 
+from collections.abc import Collection, Iterable, Iterator
 from copy import deepcopy
 from html import escape
 from typing import (
     Any,
-    Collection,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Type,
     TypeVar,
     Union,
 )
 
 import pystac
 from pystac.errors import STACTypeError
 from pystac.html.jinja_env import get_jinja_env
 from pystac.serialization.identify import identify_stac_object_type
-from pystac.utils import is_absolute_href, make_absolute_href
+from pystac.utils import HREF, is_absolute_href, make_absolute_href, make_posix_style
 
-ItemLike = Union[pystac.Item, Dict[str, Any]]
+ItemLike = Union[pystac.Item, dict[str, Any]]
 
 C = TypeVar("C", bound="ItemCollection")
 
 
 class ItemCollection(Collection[pystac.Item]):
     """Implementation of a GeoJSON FeatureCollection whose features are all STAC
     Items.
@@ -82,25 +76,25 @@
         >>> item_collection_1 = ItemCollection(items=[item_1, item_2])
         >>> item_collection_2 = ItemCollection(items=[item_2, item_3])
         >>> combined = item_collection_1 + item_collection_2
         >>> assert len(combined) == 4
         # If an item is present in both ItemCollections it will occur twice
     """
 
-    items: List[pystac.Item]
+    items: list[pystac.Item]
     """List of :class:`pystac.Item` instances contained in this ``ItemCollection``."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Dictionary of additional top-level fields for the GeoJSON
     FeatureCollection."""
 
     def __init__(
         self,
         items: Iterable[ItemLike],
-        extra_fields: Optional[Dict[str, Any]] = None,
+        extra_fields: dict[str, Any] | None = None,
         clone_items: bool = True,
     ):
         def map_item(item_or_dict: ItemLike) -> pystac.Item:
             # Converts dicts to pystac.Items and clones if necessary
             if isinstance(item_or_dict, pystac.Item):
                 return item_or_dict.clone() if clone_items else item_or_dict
             else:
@@ -117,22 +111,22 @@
 
     def __len__(self) -> int:
         return len(self.items)
 
     def __contains__(self, __x: object) -> bool:
         return __x in self.items
 
-    def __add__(self, other: object) -> "ItemCollection":
+    def __add__(self, other: object) -> ItemCollection:
         if not isinstance(other, ItemCollection):
             return NotImplemented
 
         combined = [*self.items, *other.items]
         return ItemCollection(items=combined)
 
-    def to_dict(self, transform_hrefs: bool = False) -> Dict[str, Any]:
+    def to_dict(self, transform_hrefs: bool = False) -> dict[str, Any]:
         """Serializes an :class:`ItemCollection` instance to a dictionary.
 
         Args:
             transform_hrefs: If True, transform the HREF of hierarchical links
                 of Items based on the type of catalog the Item belongs to (if any).
                 I.e. if the item belongs to a root catalog that is
                 RELATIVE_PUBLISHED or SELF_CONTAINED,
@@ -163,18 +157,18 @@
         return self.__class__(
             items=[item.clone() for item in self.items],
             extra_fields=deepcopy(self.extra_fields),
         )
 
     @classmethod
     def from_dict(
-        cls: Type[C],
-        d: Dict[str, Any],
+        cls: type[C],
+        d: dict[str, Any],
         preserve_dict: bool = True,
-        root: Optional[pystac.Catalog] = None,
+        root: pystac.Catalog | None = None,
     ) -> C:
         """Creates a :class:`ItemCollection` instance from a dictionary.
 
         Arguments:
             d : The dictionary from which the :class:`~ItemCollection` will be created
             preserve_dict: If False, the dict parameter ``d`` may be modified
                 during this method call. Otherwise the dict is not mutated.
@@ -190,52 +184,51 @@
             for item in d.get("features", [])
         ]
         extra_fields = {k: v for k, v in d.items() if k not in ("features", "type")}
 
         return cls(items=items, extra_fields=extra_fields)
 
     @classmethod
-    def from_file(
-        cls: Type[C], href: str, stac_io: Optional[pystac.StacIO] = None
-    ) -> C:
+    def from_file(cls: type[C], href: HREF, stac_io: pystac.StacIO | None = None) -> C:
         """Reads a :class:`ItemCollection` from a JSON file.
 
         Arguments:
             href : Path to the file.
             stac_io : A :class:`~pystac.StacIO` instance to use for file I/O
         """
         if stac_io is None:
             stac_io = pystac.StacIO.default()
 
+        href = make_posix_style(href)
         if not is_absolute_href(href):
             href = make_absolute_href(href)
 
         d = stac_io.read_json(href)
 
         return cls.from_dict(d, preserve_dict=False)
 
     def save_object(
         self,
         dest_href: str,
-        stac_io: Optional[pystac.StacIO] = None,
+        stac_io: pystac.StacIO | None = None,
     ) -> None:
         """Saves this instance to the ``dest_href`` location.
 
         Args:
             dest_href : Location to which the file will be saved.
             stac_io: Optional :class:`~pystac.StacIO` instance to use. If not provided,
                 will use the default instance.
         """
         if stac_io is None:
             stac_io = pystac.StacIO.default()
 
         stac_io.save_json(dest_href, self.to_dict())
 
     @staticmethod
-    def is_item_collection(d: Dict[str, Any]) -> bool:
+    def is_item_collection(d: dict[str, Any]) -> bool:
         """Checks if the given dictionary represents a valid :class:`ItemCollection`.
 
         Args:
             d : Dictionary to check
         """
         typ = d.get("type")
```

### Comparing `pystac-1.8.4/pystac/layout.py` & `pystac-1.9.0/pystac/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import posixpath
 import warnings
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from string import Formatter
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable
 
 import pystac
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
     from pystac.collection import Collection
     from pystac.item import Item
@@ -91,37 +91,35 @@
         defaults : A dictionary of template vars to values. These values
             will be used in case a value cannot be derived from a stac object.
     """
 
     template: str
     """The template string to use."""
 
-    defaults: Dict[str, str]
+    defaults: dict[str, str]
     """A dictionary of template vars to values. These values will be used in case a
     value cannot be derived from a stac object."""
 
-    template_vars: List[str]
+    template_vars: list[str]
     """List of template vars to use when templating."""
 
     # Special template vars specific to Items
     ITEM_TEMPLATE_VARS = ["date", "year", "month", "day", "collection"]
 
-    def __init__(
-        self, template: str, defaults: Optional[Dict[str, str]] = None
-    ) -> None:
+    def __init__(self, template: str, defaults: dict[str, str] | None = None) -> None:
         self.template = template
         self.defaults = defaults or {}
 
         # Generate list of template vars
         template_vars = []
         for formatter_parse_result in Formatter().parse(template):
             v = formatter_parse_result[1]
             if v is not None:
                 if formatter_parse_result[2] != "":
-                    v = "{}:{}".format(v, formatter_parse_result[2])
+                    v = f"{v}:{formatter_parse_result[2]}"
                 template_vars.append(v)
         self.template_vars = template_vars
 
     def _get_template_value(self, stac_object: STACObject, template_var: str) -> Any:
         if template_var in self.ITEM_TEMPLATE_VARS:
             if isinstance(stac_object, pystac.Item):
                 # Datetime
@@ -158,32 +156,32 @@
                     '"{}" cannot be used to template non-Item {} in {}'.format(
                         template_var, stac_object, self.template
                     )
                 )
 
         # Allow dot-notation properties for arbitrary object values.
         props = template_var.split(".")
-        prop_source: Optional[Union[pystac.STACObject, Dict[str, Any]]] = None
+        prop_source: pystac.STACObject | dict[str, Any] | None = None
         error = pystac.TemplateError(
             "Cannot find property {} on {} for template {}".format(
                 template_var, stac_object, self.template
             )
         )
 
         try:
             if hasattr(stac_object, props[0]):
                 prop_source = stac_object
 
             if prop_source is None and hasattr(stac_object, "properties"):
-                obj_props: Optional[Dict[str, Any]] = stac_object.properties
+                obj_props: dict[str, Any] | None = stac_object.properties
                 if obj_props is not None and props[0] in obj_props:
                     prop_source = obj_props
 
             if prop_source is None and hasattr(stac_object, "extra_fields"):
-                extra_fields: Optional[Dict[str, Any]] = stac_object.extra_fields
+                extra_fields: dict[str, Any] | None = stac_object.extra_fields
                 if extra_fields is not None and props[0] in extra_fields:
                     prop_source = extra_fields
 
             if prop_source is None:
                 raise error
 
             v: Any = prop_source
@@ -199,15 +197,15 @@
         except pystac.TemplateError as e:
             if template_var in self.defaults:
                 return self.defaults[template_var]
             raise e
 
         return v
 
-    def get_template_values(self, stac_object: STACObject) -> Dict[str, Any]:
+    def get_template_values(self, stac_object: STACObject) -> dict[str, Any]:
         """Gets a dictionary of template variables to values derived from
         the given stac_object. If the template vars cannot be found in the
         stac object, and defaults was supplied to this template, a default
         value is used; if there is no default then this will raise an error.
 
         Args:
             stac_object : The STACObject to derive template
@@ -246,15 +244,15 @@
                 derived from the stac object and there is no default,
                 this error will be raised.
         """
         parts = self.get_template_values(stac_object)
 
         s = self.template
         for key, value in parts.items():
-            s = s.replace("${" + "{}".format(key) + "}", "{}".format(value))
+            s = s.replace("${" + f"{key}" + "}", f"{value}")
         return s
 
 
 class HrefLayoutStrategy(ABC):
     """Base class for HREF Layout strategies."""
 
     def get_href(
@@ -263,15 +261,15 @@
         if isinstance(stac_object, pystac.Item):
             return self.get_item_href(stac_object, parent_dir)
         elif isinstance(stac_object, pystac.Collection):
             return self.get_collection_href(stac_object, parent_dir, is_root)
         elif isinstance(stac_object, pystac.Catalog):
             return self.get_catalog_href(stac_object, parent_dir, is_root)
         else:
-            raise pystac.STACError("Unknown STAC object type {}".format(stac_object))
+            raise pystac.STACError(f"Unknown STAC object type {stac_object}")
 
     @abstractmethod
     def get_catalog_href(self, cat: Catalog, parent_dir: str, is_root: bool) -> str:
         raise NotImplementedError
 
     @abstractmethod
     def get_collection_href(
@@ -301,38 +299,38 @@
             an item and a parent directory and returns the path to be used
             for the item.
         fallback_strategy : The fallback strategy to
             use if a function is not provided for a stac object type. Defaults to
             :class:`~pystac.layout.BestPracticesLayoutStrategy`
     """
 
-    catalog_func: Optional[Callable[[Catalog, str, bool], str]]
+    catalog_func: Callable[[Catalog, str, bool], str] | None
     """A function that takes a :class:`~pystac.Catalog`, a parent directory, and a
     boolean specifying whether or not this Catalog is the root. If it is the root, it
     is usually best to not create a subdirectory and put the Catalog file directly
     in the parent directory. Must return the string path."""
 
-    collection_func: Optional[Callable[[Collection, str, bool], str]]
+    collection_func: Callable[[Collection, str, bool], str] | None
     """A function that is used for collections in the same manner as
     :attr:`~catalog_func`. This takes the same parameters."""
 
     fallback_strategy: HrefLayoutStrategy
     """The fallback strategy to use if a function is not provided for a stac object
     type. Defaults to :class:`~pystac.layout.BestPracticesLayoutStrategy`."""
 
-    item_func: Optional[Callable[[Item, str], str]]
+    item_func: Callable[[Item, str], str] | None
     """An optional function that takes an :class:`~pystac.Item` and a parent directory
     and returns the path to be used for the Item."""
 
     def __init__(
         self,
-        catalog_func: Optional[Callable[[Catalog, str, bool], str]] = None,
-        collection_func: Optional[Callable[[Collection, str, bool], str]] = None,
-        item_func: Optional[Callable[[Item, str], str]] = None,
-        fallback_strategy: Optional[HrefLayoutStrategy] = None,
+        catalog_func: Callable[[Catalog, str, bool], str] | None = None,
+        collection_func: Callable[[Collection, str, bool], str] | None = None,
+        item_func: Callable[[Item, str], str] | None = None,
+        fallback_strategy: HrefLayoutStrategy | None = None,
     ):
         self.item_func = item_func
         self.collection_func = collection_func
         self.catalog_func = catalog_func
         if fallback_strategy is None:
             fallback_strategy = BestPracticesLayoutStrategy()
         self.fallback_strategy = fallback_strategy
@@ -382,36 +380,36 @@
             Must be a valid template string that can be used by
             :class:`~pystac.layout.LayoutTemplate`
         fallback_strategy : The fallback strategy to
             use if a template is not provided. Defaults to
             :class:`~pystac.layout.BestPracticesLayoutStrategy`
     """
 
-    catalog_template: Optional[LayoutTemplate]
+    catalog_template: LayoutTemplate | None
     """The template string to use for catalog paths. Must be a valid template string
     that can be used by :class:`~pystac.layout.LayoutTemplate`."""
 
-    collection_template: Optional[LayoutTemplate]
+    collection_template: LayoutTemplate | None
     """The template string to use for collection paths. Must be a valid template string
     that can be used by :class:`~pystac.layout.LayoutTemplate`."""
 
     fallback_strategy: HrefLayoutStrategy
     """The fallback strategy to use if a template is not provided. Defaults to
     :class:`~pystac.layout.BestPracticesLayoutStrategy`."""
 
-    item_template: Optional[LayoutTemplate]
+    item_template: LayoutTemplate | None
     """The template string to use for item paths. Must be a valid template string that
     can be used by :class:`~pystac.layout.LayoutTemplate`."""
 
     def __init__(
         self,
-        catalog_template: Optional[str] = None,
-        collection_template: Optional[str] = None,
-        item_template: Optional[str] = None,
-        fallback_strategy: Optional[HrefLayoutStrategy] = None,
+        catalog_template: str | None = None,
+        collection_template: str | None = None,
+        item_template: str | None = None,
+        fallback_strategy: HrefLayoutStrategy | None = None,
     ):
         self.catalog_template = (
             LayoutTemplate(catalog_template) if catalog_template is not None else None
         )
         self.collection_template = (
             LayoutTemplate(collection_template)
             if collection_template is not None
@@ -449,15 +447,15 @@
 
     def get_item_href(self, item: Item, parent_dir: str) -> str:
         if self.item_template is None:
             return self.fallback_strategy.get_item_href(item, parent_dir)
         else:
             template_path = self.item_template.substitute(item)
             if not template_path.endswith(".json"):
-                template_path = posixpath.join(template_path, "{}.json".format(item.id))
+                template_path = posixpath.join(template_path, f"{item.id}.json")
 
             return posixpath.join(parent_dir, template_path)
 
 
 class BestPracticesLayoutStrategy(HrefLayoutStrategy):
     """Layout strategy that represents the catalog layout described
     in the :stac-spec:`STAC Best Practices documentation
@@ -473,32 +471,32 @@
     All paths are appended to the parent directory.
     """
 
     def get_catalog_href(self, cat: Catalog, parent_dir: str, is_root: bool) -> str:
         if is_root:
             cat_root = parent_dir
         else:
-            cat_root = posixpath.join(parent_dir, "{}".format(cat.id))
+            cat_root = posixpath.join(parent_dir, f"{cat.id}")
 
         return posixpath.join(cat_root, cat.DEFAULT_FILE_NAME)
 
     def get_collection_href(
         self, col: Collection, parent_dir: str, is_root: bool
     ) -> str:
         if is_root:
             col_root = parent_dir
         else:
-            col_root = posixpath.join(parent_dir, "{}".format(col.id))
+            col_root = posixpath.join(parent_dir, f"{col.id}")
 
         return posixpath.join(col_root, col.DEFAULT_FILE_NAME)
 
     def get_item_href(self, item: Item, parent_dir: str) -> str:
-        item_root = posixpath.join(parent_dir, "{}".format(item.id))
+        item_root = posixpath.join(parent_dir, f"{item.id}")
 
-        return posixpath.join(item_root, "{}.json".format(item.id))
+        return posixpath.join(item_root, f"{item.id}.json")
 
 
 class AsIsLayoutStrategy(HrefLayoutStrategy):
     """Layout strategy that simply preserves the current href of all objects.
 
     If any object doesn't have a self href, a ValueError is raised.
     """
```

### Comparing `pystac-1.8.4/pystac/link.py` & `pystac-1.9.0/pystac/link.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 from copy import copy
 from html import escape
-from typing import TYPE_CHECKING, Any, Dict, Optional, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, TypeVar
 
 import pystac
 from pystac.html.jinja_env import get_jinja_env
 from pystac.utils import (
     HREF as HREF,
 )
 from pystac.utils import (
@@ -16,14 +16,15 @@
     make_posix_style,
     make_relative_href,
 )
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog
     from pystac.collection import Collection
+    from pystac.extensions.ext import LinkExt
     from pystac.item import Item
     from pystac.stac_object import STACObject
 
     PathLike = os.PathLike[str]
 
 else:
     PathLike = os.PathLike
@@ -65,42 +66,42 @@
             are preferred. See :class:`~pystac.MediaType` for common media types.
         title : Optional title for this link.
         extra_fields : Optional, additional fields for this link. This is used
             by extensions as a way to serialize and deserialize properties on link
             object JSON.
     """
 
-    rel: Union[str, pystac.RelType]
+    rel: str | pystac.RelType
     """The relation of the link (e.g. 'child', 'item'). Registered rel Types are
     preferred. See :class:`~pystac.RelType` for common media types."""
 
-    media_type: Optional[Union[str, pystac.MediaType]]
+    media_type: str | pystac.MediaType | None
     """Optional description of the media type. Registered Media Types are preferred.
     See :class:`~pystac.MediaType` for common media types."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Optional, additional fields for this link. This is used by extensions as a
     way to serialize and deserialize properties on link object JSON."""
 
-    owner: Optional[STACObject]
+    owner: STACObject | None
     """The owner of this link. The link will use its owner's root catalog
     :class:`~pystac.resolved_object_cache.ResolvedObjectCache` to resolve objects, and
     will create absolute HREFs from relative HREFs against the owner's self HREF."""
 
-    _target_href: Optional[str]
-    _target_object: Optional[STACObject]
-    _title: Optional[str]
+    _target_href: str | None
+    _target_object: STACObject | None
+    _title: str | None
 
     def __init__(
         self,
-        rel: Union[str, pystac.RelType],
-        target: Union[str, STACObject],
-        media_type: Optional[Union[str, pystac.MediaType]] = None,
-        title: Optional[str] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
+        rel: str | pystac.RelType,
+        target: str | STACObject,
+        media_type: str | pystac.MediaType | None = None,
+        title: str | None = None,
+        extra_fields: dict[str, Any] | None = None,
     ) -> None:
         self.rel = rel
         if isinstance(target, str):
             if rel == pystac.RelType.SELF:
                 self._target_href = make_absolute_href(target)
             else:
                 self._target_href = make_posix_style(target)
@@ -109,52 +110,52 @@
             self._target_href = None
             self._target_object = target
         self.media_type = media_type
         self.title = title
         self.extra_fields = extra_fields or {}
         self.owner = None
 
-    def set_owner(self, owner: Optional[STACObject]) -> Link:
+    def set_owner(self, owner: STACObject | None) -> Link:
         """Sets the owner of this link.
 
         Args:
             owner: The owner of this link. Pass None to clear.
         """
         self.owner = owner
         return self
 
     @property
-    def title(self) -> Optional[str]:
+    def title(self) -> str | None:
         """Optional title for this link. If not provided during instantiation, this will
         attempt to get the title from the STAC object that the link references."""
         if self._title is not None:
             return self._title
         if self._target_object is not None and isinstance(
             self._target_object, pystac.Catalog
         ):
             return self._target_object.title
         return None
 
     @title.setter
-    def title(self, v: Optional[str]) -> None:
+    def title(self, v: str | None) -> None:
         self._title = v
 
     @property
     def href(self) -> str:
         """Returns the HREF for this link.
 
         If the href is None, this will throw an exception.
         Use get_href if there may not be an href.
         """
         result = self.get_href()
         if result is None:
             raise ValueError(f"{self} does not have an HREF set.")
         return result
 
-    def get_href(self, transform_href: bool = True) -> Optional[str]:
+    def get_href(self, transform_href: bool = True) -> str | None:
         """Gets the HREF for this link.
 
         Args:
             transform_href: If True, transform the HREF based on the type of
                 catalog the owner belongs to (if any). I.e. if the link owner
                 belongs to a root catalog that is RELATIVE_PUBLISHED or SELF_CONTAINED,
                 the HREF will be transformed to be relative to the catalog root
@@ -201,15 +202,15 @@
         Use get_absolute_href if there may not be an href set.
         """
         result = self.get_absolute_href()
         if result is None:
             raise ValueError(f"{self} does not have an HREF set.")
         return result
 
-    def get_absolute_href(self) -> Optional[str]:
+    def get_absolute_href(self) -> str | None:
         """Gets the absolute href for this link, if possible.
 
         Returns:
             str: Returns this link's HREF. It attempts to derive an absolute HREF
             from this link; however, if the link is relative, has no owner,
             and has an unresolved target, this will return a relative HREF.
         """
@@ -220,36 +221,36 @@
 
         if href is not None and self.owner is not None:
             href = make_absolute_href(href, self.owner.get_self_href())
 
         return href
 
     @property
-    def target(self) -> Union[str, STACObject]:
+    def target(self) -> str | STACObject:
         """The target of the link. If the link is unresolved, or the link is to
         something that is not a STACObject, the target is an HREF. If resolved, the
         target is a STACObject."""
         if self._target_object:
             return self._target_object
         elif self._target_href:
             return self._target_href
         else:
             raise ValueError("No target defined for link.")
 
     @target.setter
-    def target(self, target: Union[str, STACObject]) -> None:
+    def target(self, target: str | STACObject) -> None:
         """Sets this link's target to a string or a STAC object."""
         if isinstance(target, str):
             self._target_href = target
             self._target_object = None
         else:
             self._target_href = None
             self._target_object = target
 
-    def get_target_str(self) -> Optional[str]:
+    def get_target_str(self) -> str | None:
         """Returns this link's target as a string.
 
         If a string href was provided, returns that. If not, tries to resolve
         the self link of the target object.
         """
         if self._target_href:
             return self._target_href
@@ -262,25 +263,25 @@
         """Returns true if this link has a string href in its target information."""
         return self._target_href is not None
 
     def __fspath__(self) -> str:
         return self.absolute_href
 
     def __repr__(self) -> str:
-        return "<Link rel={} target={}>".format(self.rel, self.target)
+        return f"<Link rel={self.rel} target={self.target}>"
 
     def _repr_html_(self) -> str:
         jinja_env = get_jinja_env()
         if jinja_env:
             template = jinja_env.get_template("JSON.jinja2")
             return str(template.render(dict=self.to_dict()))
         else:
             return escape(repr(self))
 
-    def resolve_stac_object(self, root: Optional[Catalog] = None) -> Link:
+    def resolve_stac_object(self, root: Catalog | None = None) -> Link:
         """Resolves a STAC object from the HREF of this link, if the link is not
         already resolved.
 
         Args:
             root : Optional root of the catalog for this link.
                 If provided, the root's resolved object cache is used to search for
                 previously resolved instances of the STAC object.
@@ -304,15 +305,15 @@
                         "Relative path {} encountered "
                         'without owner "self" link set.'.format(target_href)
                     )
 
                 target_href = make_absolute_href(target_href, start_href)
             obj = None
 
-            stac_io: Optional[pystac.StacIO] = None
+            stac_io: pystac.StacIO | None = None
 
             if root is not None:
                 obj = root._resolved_objects.get_by_href(target_href)
                 stac_io = root._stac_io
 
             if obj is None:
                 if stac_io is None:
@@ -364,28 +365,28 @@
         relation types, see :py:const:`HIERARCHICAL_LINKS`.
 
         Returns:
             bool: True if the link's rel type is hierarchical.
         """
         return self.rel in HIERARCHICAL_LINKS
 
-    def to_dict(self, transform_href: bool = True) -> Dict[str, Any]:
+    def to_dict(self, transform_href: bool = True) -> dict[str, Any]:
         """Returns this link as a dictionary.
 
         Args:
             transform_href : If ``True``, transform the HREF based on the type of
                 catalog the owner belongs to (if any). I.e. if the link owner
                 belongs to a root catalog that is RELATIVE_PUBLISHED or SELF_CONTAINED,
                 the HREF will be transformed to be relative to the catalog root
                 if this is a hierarchical link relation.
         Returns:
             dict : A serialization of the Link.
         """
 
-        d: Dict[str, Any] = {
+        d: dict[str, Any] = {
             "rel": str(self.rel),
             "href": self.get_href(transform_href=transform_href),
         }
 
         if self.media_type is not None:
             d["type"] = str(self.media_type)
 
@@ -411,15 +412,15 @@
             rel=self.rel,
             target=self.target,
             media_type=self.media_type,
             title=self.title,
         )
 
     @classmethod
-    def from_dict(cls: Type[L], d: Dict[str, Any]) -> L:
+    def from_dict(cls: type[L], d: dict[str, Any]) -> L:
         """Deserializes a Link from a dict.
 
         Args:
             d : The dict that represents the Link in JSON
 
         Returns:
             Link: Link instance constructed from the dict.
@@ -439,66 +440,76 @@
             target=href,
             media_type=media_type,
             title=title,
             extra_fields=extra_fields,
         )
 
     @classmethod
-    def root(cls: Type[L], c: Catalog) -> L:
+    def root(cls: type[L], c: Catalog) -> L:
         """Creates a link to a root Catalog or Collection."""
         return cls(pystac.RelType.ROOT, c, media_type=pystac.MediaType.JSON)
 
     @classmethod
-    def parent(cls: Type[L], c: Catalog) -> L:
+    def parent(cls: type[L], c: Catalog) -> L:
         """Creates a link to a parent Catalog or Collection."""
         return cls(pystac.RelType.PARENT, c, media_type=pystac.MediaType.JSON)
 
     @classmethod
-    def collection(cls: Type[L], c: Collection) -> L:
+    def collection(cls: type[L], c: Collection) -> L:
         """Creates a link to an item's Collection."""
         return cls(pystac.RelType.COLLECTION, c, media_type=pystac.MediaType.JSON)
 
     @classmethod
-    def self_href(cls: Type[L], href: HREF) -> L:
+    def self_href(cls: type[L], href: HREF) -> L:
         """Creates a self link to a file's location."""
         href_str = str(os.fspath(href))
         return cls(pystac.RelType.SELF, href_str, media_type=pystac.MediaType.JSON)
 
     @classmethod
-    def child(cls: Type[L], c: Catalog, title: Optional[str] = None) -> L:
+    def child(cls: type[L], c: Catalog, title: str | None = None) -> L:
         """Creates a link to a child Catalog or Collection."""
         return cls(
             pystac.RelType.CHILD, c, title=title, media_type=pystac.MediaType.JSON
         )
 
     @classmethod
-    def item(cls: Type[L], item: Item, title: Optional[str] = None) -> L:
+    def item(cls: type[L], item: Item, title: str | None = None) -> L:
         """Creates a link to an Item."""
         return cls(
             pystac.RelType.ITEM, item, title=title, media_type=pystac.MediaType.JSON
         )
 
     @classmethod
-    def derived_from(
-        cls: Type[L], item: Union[Item, str], title: Optional[str] = None
-    ) -> L:
+    def derived_from(cls: type[L], item: Item | str, title: str | None = None) -> L:
         """Creates a link to a derived_from Item."""
         return cls(
             pystac.RelType.DERIVED_FROM,
             item,
             title=title,
             media_type=pystac.MediaType.JSON,
         )
 
     @classmethod
     def canonical(
-        cls: Type[L],
-        item_or_collection: Union[Item, Collection],
-        title: Optional[str] = None,
+        cls: type[L],
+        item_or_collection: Item | Collection,
+        title: str | None = None,
     ) -> L:
         """Creates a canonical link to an Item or Collection."""
         return cls(
             pystac.RelType.CANONICAL,
             item_or_collection,
             title=title,
             media_type=pystac.MediaType.JSON,
         )
+
+    @property
+    def ext(self) -> LinkExt:
+        """Accessor for extension classes on this link
+
+        Example::
+
+            link.ext.file.size = 8675309
+        """
+        from pystac.extensions.ext import LinkExt
+
+        return LinkExt(stac_object=self)
```

### Comparing `pystac-1.8.4/pystac/media_type.py` & `pystac-1.9.0/pystac/media_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/provider.py` & `pystac-1.9.0/pystac/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from html import escape
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 from pystac.html.jinja_env import get_jinja_env
 from pystac.utils import StringEnum
 
 
 class ProviderRole(StringEnum):
     """Enumerates the allows values of the Provider "role" field."""
@@ -37,33 +37,33 @@
     """The name of the organization or the individual."""
 
     description: Optional[str]
     """Optional multi-line description to add further provider
     information such as processing details for processors and producers,
     hosting details for hosts or basic contact information."""
 
-    roles: Optional[List[ProviderRole]]
+    roles: Optional[list[ProviderRole]]
     """Optional roles of the provider. Any of
     licensor, producer, processor or host."""
 
     url: Optional[str]
     """Optional homepage on which the provider describes the dataset
     and publishes contact information."""
 
-    extra_fields: Dict[str, Any]
+    extra_fields: dict[str, Any]
     """Dictionary containing additional top-level fields defined on the Provider
     object."""
 
     def __init__(
         self,
         name: str,
         description: Optional[str] = None,
-        roles: Optional[List[ProviderRole]] = None,
+        roles: Optional[list[ProviderRole]] = None,
         url: Optional[str] = None,
-        extra_fields: Optional[Dict[str, Any]] = None,
+        extra_fields: Optional[dict[str, Any]] = None,
     ):
         self.name = name
         self.description = description
         self.roles = roles
         self.url = url
         self.extra_fields = extra_fields or {}
 
@@ -76,34 +76,34 @@
         jinja_env = get_jinja_env()
         if jinja_env:
             template = jinja_env.get_template("JSON.jinja2")
             return str(template.render(dict=self.to_dict()))
         else:
             return escape(repr(self))
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         """Returns this provider as a dictionary.
 
         Returns:
             dict: A serialization of the Provider.
         """
-        d: Dict[str, Any] = {"name": self.name}
+        d: dict[str, Any] = {"name": self.name}
         if self.description is not None:
             d["description"] = self.description
         if self.roles is not None:
             d["roles"] = self.roles
         if self.url is not None:
             d["url"] = self.url
 
         d.update(self.extra_fields)
 
         return d
 
     @staticmethod
-    def from_dict(d: Dict[str, Any]) -> "Provider":
+    def from_dict(d: dict[str, Any]) -> "Provider":
         """Constructs an Provider from a dict.
 
         Returns:
             Provider: The Provider deserialized from the JSON dict.
         """
         return Provider(
             name=d["name"],
```

### Comparing `pystac-1.8.4/pystac/rel_type.py` & `pystac-1.9.0/pystac/rel_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/serialization/common_properties.py` & `pystac-1.9.0/pystac/serialization/common_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Any, Dict, Iterable, List, Optional, Union, cast
+from collections.abc import Iterable
+from typing import Any, Optional, Union, cast
 
 import pystac
 from pystac.cache import CollectionCache
 from pystac.serialization.identify import STACVersionID
 from pystac.utils import make_absolute_href
 
 
 def merge_common_properties(
-    item_dict: Dict[str, Any],
+    item_dict: dict[str, Any],
     collection_cache: Optional[CollectionCache] = None,
     json_href: Optional[str] = None,
 ) -> bool:
     """Merges Collection properties into an Item.
 
     Note: This is only applicable to reading old STAC versions (pre 1.0.0-beta.1).
 
@@ -24,15 +25,15 @@
             to resolve relative paths.
 
     Returns:
         bool: True if Collection properties have been merged, otherwise False.
     """
     properties_merged = False
 
-    collection: Optional[Union[pystac.Collection, Dict[str, Any]]] = None
+    collection: Optional[Union[pystac.Collection, dict[str, Any]]] = None
     collection_href: Optional[str] = None
 
     stac_version = item_dict.get("stac_version")
 
     # The commons extension was removed in 1.0.0-beta.1, so if this is an earlier STAC
     # item we don't have to bother with merging.
     if stac_version is not None and STACVersionID(stac_version) > "0.9.0":
@@ -55,17 +56,17 @@
         if collection_cache is not None:
             collection = collection_cache.get_by_id(collection_id)
 
     # Next, try the collection link.
     if collection is None:
         # Account for 0.5 links, which were dicts
         if isinstance(item_dict["links"], dict):
-            links = list(cast(Iterable[Dict[str, Any]], item_dict["links"].values()))
+            links = list(cast(Iterable[dict[str, Any]], item_dict["links"].values()))
         else:
-            links = cast(List[Dict[str, Any]], item_dict["links"])
+            links = cast(list[dict[str, Any]], item_dict["links"])
 
         collection_link = next(
             (link for link in links if link["rel"] == pystac.RelType.COLLECTION), None
         )
         if collection_link is not None:
             collection_href = collection_link.get("href")
             if collection_href is not None:
@@ -74,15 +75,15 @@
                 if collection_cache is not None:
                     collection = collection_cache.get_by_href(collection_href)
 
                 if collection is None:
                     collection = pystac.StacIO.default().read_json(collection_href)
 
     if collection is not None:
-        collection_props: Optional[Dict[str, Any]] = None
+        collection_props: Optional[dict[str, Any]] = None
         if isinstance(collection, pystac.Collection):
             collection_id = collection.id
             collection_props = collection.extra_fields.get("properties")
         elif isinstance(collection, dict):
             collection_id = collection["id"]
             if "properties" in collection:
                 collection_props = collection["properties"]
```

### Comparing `pystac-1.8.4/pystac/serialization/identify.py` & `pystac-1.9.0/pystac/serialization/identify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from enum import Enum
 from functools import total_ordering
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 import pystac
 from pystac.version import STACVersion
 
 if TYPE_CHECKING:
     from pystac.stac_object import STACObjectType
 
@@ -37,15 +37,15 @@
 class STACVersionID:
     """Defines STAC versions in an object that is orderable based on version number.
     For instance, ``1.0.0-beta.2 < 1.0.0``
     """
 
     version_string: str
     version_core: str
-    version_prerelease: Optional[str]
+    version_prerelease: str | None
 
     def __init__(self, version_string: str) -> None:
         self.version_string = version_string
 
         # Account for RC or beta releases in version
         version_parts = version_string.split("-")
         self.version_core = version_parts[0]
@@ -83,16 +83,16 @@
     """Defines a range of STAC versions."""
 
     min_version: STACVersionID
     max_version: STACVersionID
 
     def __init__(
         self,
-        min_version: Union[str, STACVersionID] = "0.8.0",
-        max_version: Optional[Union[str, STACVersionID]] = None,
+        min_version: str | STACVersionID = "0.8.0",
+        max_version: str | STACVersionID | None = None,
     ):
         if isinstance(min_version, str):
             self.min_version = STACVersionID(min_version)
         else:
             self.min_version = min_version
 
         if max_version is None:
@@ -120,34 +120,34 @@
     def set_to_single(self, v: STACVersionID) -> None:
         self.set_min(v)
         self.set_max(v)
 
     def latest_valid_version(self) -> STACVersionID:
         return self.max_version
 
-    def contains(self, v: Union[str, STACVersionID]) -> bool:
+    def contains(self, v: str | STACVersionID) -> bool:
         if isinstance(v, str):
             v = STACVersionID(v)
         return self.min_version <= v <= self.max_version
 
     def is_single_version(self) -> bool:
         return self.min_version >= self.max_version
 
-    def is_earlier_than(self, v: Union[str, STACVersionID]) -> bool:
+    def is_earlier_than(self, v: str | STACVersionID) -> bool:
         if isinstance(v, str):
             v = STACVersionID(v)
         return self.max_version < v
 
-    def is_later_than(self, v: Union[str, STACVersionID]) -> bool:
+    def is_later_than(self, v: str | STACVersionID) -> bool:
         if isinstance(v, str):
             v = STACVersionID(v)
         return v < self.min_version
 
     def __repr__(self) -> str:
-        return "<VERSIONS {}-{}>".format(self.min_version, self.max_version)
+        return f"<VERSIONS {self.min_version}-{self.max_version}>"
 
 
 class STACJSONDescription:
     """Describes the STAC object information for a STAC object represented in JSON
 
     Attributes:
         object_type : Describes the STAC object type. One of
@@ -156,33 +156,33 @@
             has been identified as potential valid versions of the stac object.
         extensions : List of extension schema URIs for extensions this
             object implements
     """
 
     object_type: STACObjectType
     version_range: STACVersionRange
-    extensions: List[str]
+    extensions: list[str]
 
     def __init__(
         self,
         object_type: STACObjectType,
         version_range: STACVersionRange,
-        extensions: List[str],
+        extensions: list[str],
     ) -> None:
         self.object_type = object_type
         self.version_range = version_range
         self.extensions = extensions
 
     def __repr__(self) -> str:
         return "<{} {} ext={}>".format(
             self.object_type, self.version_range, ",".join(self.extensions)
         )
 
 
-def identify_stac_object_type(json_dict: Dict[str, Any]) -> Optional[STACObjectType]:
+def identify_stac_object_type(json_dict: dict[str, Any]) -> STACObjectType | None:
     """Determines the STACObjectType of the provided JSON dict. If the JSON dict does
     not represent a STAC object, returns ``None``.
 
     Will first try to identify the object using ``"type"`` field as described in the
     guidelines in :stac-spec:`How to Differentiate STAC Files
     <best-practices.md#how-to-differentiate-stac-files>`. If this fails, will fall back
     to using the pre-1.0 heuristic described in `this issue
@@ -231,15 +231,15 @@
         # Everything else that has a stac_version is a Catalog
         else:
             return pystac.STACObjectType.CATALOG
 
     return None
 
 
-def identify_stac_object(json_dict: Dict[str, Any]) -> STACJSONDescription:
+def identify_stac_object(json_dict: dict[str, Any]) -> STACJSONDescription:
     """Determines the STACJSONDescription of the provided JSON dict.
 
     Args:
         json_dict : The dict of STAC JSON to identify.
 
     Returns:
         STACJSONDescription: The description of the STAC object serialized in the
```

### Comparing `pystac-1.8.4/pystac/serialization/migrate.py` & `pystac-1.9.0/pystac/serialization/migrate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple
+from typing import TYPE_CHECKING, Any, Callable
 
 import pystac
 from pystac.serialization.identify import (
     OldExtensionShortIDs,
     STACJSONDescription,
     STACVersionID,
 )
 from pystac.version import STACVersion
 
 if TYPE_CHECKING:
     from pystac import STACObjectType
 
 
 def _migrate_catalog(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
 ) -> None:
     d["type"] = pystac.STACObjectType.CATALOG
 
 
 def _migrate_collection_summaries(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
 ) -> None:
     if version < "1.0.0-rc.1":
         for prop, summary in d.get("summaries", {}).items():
             if isinstance(summary, dict) and "min" in summary and "max" in summary:
                 d["summaries"][prop] = {
                     "minimum": summary["min"],
                     "maximum": summary["max"],
                 }
 
 
 def _migrate_collection(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
 ) -> None:
     d["type"] = pystac.STACObjectType.COLLECTION
     _migrate_collection_summaries(d, version, info)
 
 
 def _migrate_item(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
 ) -> None:
     # No migrations necessary for supported STAC versions (>=0.8)
     pass
 
 
 # Extensions
 def _migrate_item_assets(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
-) -> Optional[Set[str]]:
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
+) -> set[str] | None:
     if version < "1.0.0-beta.2":
         if info.object_type == pystac.STACObjectType.COLLECTION:
             if "assets" in d:
                 d["item_assets"] = d["assets"]
                 del d["assets"]
     return None
 
 
 def _migrate_datetime_range(
-    d: Dict[str, Any], version: STACVersionID, info: STACJSONDescription
-) -> Optional[Set[str]]:
+    d: dict[str, Any], version: STACVersionID, info: STACJSONDescription
+) -> set[str] | None:
     if version < "0.9":
         # Datetime range was removed
         if (
             "dtr:start_datetime" in d["properties"]
             and "start_datetime" not in d["properties"]
         ):
             d["properties"]["start_datetime"] = d["properties"]["dtr:start_datetime"]
@@ -78,34 +78,35 @@
             d["properties"]["end_datetime"] = d["properties"]["dtr:end_datetime"]
             del d["properties"]["dtr:end_datetime"]
 
     return None
 
 
 def _get_object_migrations() -> (
-    Dict[str, Callable[[Dict[str, Any], STACVersionID, STACJSONDescription], None]]
+    dict[str, Callable[[dict[str, Any], STACVersionID, STACJSONDescription], None]]
 ):
     return {
         pystac.STACObjectType.CATALOG: _migrate_catalog,
         pystac.STACObjectType.COLLECTION: _migrate_collection,
         pystac.STACObjectType.ITEM: _migrate_item,
     }
 
 
 def _get_removed_extension_migrations() -> (
-    Dict[
+    dict[
         str,
-        Tuple[
-            Optional[List[STACObjectType]],
-            Optional[
+        tuple[
+            list[STACObjectType] | None,
+            None
+            | (
                 Callable[
-                    [Dict[str, Any], STACVersionID, STACJSONDescription],
-                    Optional[Set[str]],
+                    [dict[str, Any], STACVersionID, STACJSONDescription],
+                    set[str] | None,
                 ]
-            ],
+            ),
         ],
     ]
 ):
     """Handles removed extensions.
 
     This does not handle renamed extension or extensions that were absorbed
     by other extensions; for instance the FileExtensions handles the migration of
@@ -153,21 +154,21 @@
         "dtr": (None, _migrate_datetime_range),
         "datetime-range": (None, _migrate_datetime_range),
         "commons": (None, None),
     }
 
 
 # TODO: Item Assets
-def _get_extension_renames() -> Dict[str, str]:
+def _get_extension_renames() -> dict[str, str]:
     return {"asset": "item-assets"}
 
 
 def migrate_to_latest(
-    json_dict: Dict[str, Any], info: STACJSONDescription
-) -> Dict[str, Any]:
+    json_dict: dict[str, Any], info: STACJSONDescription
+) -> dict[str, Any]:
     """Migrates the STAC JSON to the latest version
 
     Args:
         json_dict : The dict of STAC JSON to identify.
         info : The info from
             :func:`~pystac.serialization.identify.identify_stac_object` that describes
             the STAC object contained in the JSON dict.
```

### Comparing `pystac-1.8.4/pystac/stac_io.py` & `pystac-1.9.0/pystac/stac_io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable
 from urllib.error import HTTPError
 from urllib.request import Request, urlopen
 
 import pystac
 from pystac.serialization import (
     identify_stac_object,
     identify_stac_object_type,
@@ -36,17 +36,17 @@
     from pystac.stac_object import STACObject
 
 
 logger = logging.getLogger(__name__)
 
 
 class StacIO(ABC):
-    _default_io: Optional[Callable[[], StacIO]] = None
+    _default_io: Callable[[], StacIO] | None = None
 
-    def __init__(self, headers: Optional[Dict[str, str]] = None):
+    def __init__(self, headers: dict[str, str] | None = None):
         self.headers = headers or {}
 
     @abstractmethod
     def read_text(self, source: HREF, *args: Any, **kwargs: Any) -> str:
         """Read text from the given URI.
 
         The source to read from can be specified as a string or :class:`os.PathLike`
@@ -86,35 +86,35 @@
 
         Args:
             dest : The destination to write to.
             txt : The text to write.
         """
         raise NotImplementedError
 
-    def json_loads(self, txt: str, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    def json_loads(self, txt: str, *args: Any, **kwargs: Any) -> dict[str, Any]:
         """Method used internally by :class:`StacIO` instances to deserialize a
         dictionary from a JSON string.
 
         This method may be overwritten in :class:`StacIO` sub-classes to provide custom
         deserialization logic. The method accepts arbitrary keyword arguments. These are
         not used by the default implementation, but may be used by sub-class
         implementations.
 
         Args:
 
             txt : The JSON string to deserialize to a dictionary.
         """
-        result: Dict[str, Any]
+        result: dict[str, Any]
         if orjson is not None:
             result = orjson.loads(txt)
         else:
             result = json.loads(txt, *args, **kwargs)
         return result
 
-    def json_dumps(self, json_dict: Dict[str, Any], *args: Any, **kwargs: Any) -> str:
+    def json_dumps(self, json_dict: dict[str, Any], *args: Any, **kwargs: Any) -> str:
         """Method used internally by :class:`StacIO` instances to serialize a dictionary
         to a JSON string.
 
         This method may be overwritten in :class:`StacIO` sub-classes to provide custom
         serialization logic. The method accepts arbitrary keyword arguments. These are
         not used by the default implementation, but may be used by sub-class
         implementations.
@@ -128,17 +128,17 @@
                 "utf-8"
             )
         else:
             return json.dumps(json_dict, *args, indent=2, **kwargs)
 
     def stac_object_from_dict(
         self,
-        d: Dict[str, Any],
-        href: Optional[HREF] = None,
-        root: Optional[Catalog] = None,
+        d: dict[str, Any],
+        href: HREF | None = None,
+        root: Catalog | None = None,
         preserve_dict: bool = True,
     ) -> STACObject:
         """Deserializes a :class:`~pystac.STACObject` sub-class instance from a
         dictionary.
 
         Args:
 
@@ -181,15 +181,15 @@
         if info.object_type == pystac.STACObjectType.ITEM:
             return pystac.Item.from_dict(
                 d, href=href_str, root=root, migrate=False, preserve_dict=preserve_dict
             )
 
         raise ValueError(f"Unknown STAC object type {info.object_type}")
 
-    def read_json(self, source: HREF, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    def read_json(self, source: HREF, *args: Any, **kwargs: Any) -> dict[str, Any]:
         """Read a dict from the given source.
 
         See :func:`StacIO.read_text <pystac.StacIO.read_text>` for usage of
         str vs Link as a parameter.
 
         Args:
             source : The source from which to read.
@@ -204,15 +204,15 @@
         """
         txt = self.read_text(source, *args, **kwargs)
         return self.json_loads(txt)
 
     def read_stac_object(
         self,
         source: HREF,
-        root: Optional[Catalog] = None,
+        root: Catalog | None = None,
         *args: Any,
         **kwargs: Any,
     ) -> STACObject:
         """Read a STACObject from a JSON file at the given source.
 
         See :func:`StacIO.read_text <pystac.StacIO.read_text>` for usage of
         str vs Link as a parameter.
@@ -235,15 +235,15 @@
         return self.stac_object_from_dict(
             d, href=source, root=root, preserve_dict=False
         )
 
     def save_json(
         self,
         dest: HREF,
-        json_dict: Dict[str, Any],
+        json_dict: dict[str, Any],
         *args: Any,
         **kwargs: Any,
     ) -> None:
         """Write a dict to the given URI as JSON.
 
         See :func:`StacIO.write_text <pystac.StacIO.write_text>` for usage of
         str vs Link as a parameter.
@@ -296,15 +296,15 @@
         if _is_url(href):
             try:
                 logger.debug(f"GET {href} Headers: {self.headers}")
                 req = Request(href, headers=self.headers)
                 with urlopen(req) as f:
                     href_contents = f.read().decode("utf-8")
             except HTTPError as e:
-                raise Exception("Could not read uri {}".format(href)) from e
+                raise Exception(f"Could not read uri {href}") from e
         else:
             with open(href, encoding="utf-8") as f:
                 href_contents = f.read()
         return href_contents
 
     def write_text(self, dest: HREF, txt: str, *_: Any, **__: Any) -> None:
         """A concrete implementation of :meth:`StacIO.write_text
@@ -338,29 +338,29 @@
 class DuplicateKeyReportingMixin(StacIO):
     """A mixin for :class:`pystac.StacIO` implementations that will report
     on duplicate keys in the JSON being read in.
 
     See https://github.com/stac-utils/pystac/issues/313
     """
 
-    def json_loads(self, txt: str, *_: Any, **__: Any) -> Dict[str, Any]:
+    def json_loads(self, txt: str, *_: Any, **__: Any) -> dict[str, Any]:
         """Overwrites :meth:`StacIO.json_loads <pystac.StacIO.json_loads>` as the
         internal method used by :class:`DuplicateKeyReportingMixin` for deserializing
         a JSON string to a dictionary while checking for duplicate object keys.
 
         Raises:
 
             pystac.DuplicateObjectKeyError : If a duplicate object key is found.
         """
-        result: Dict[str, Any] = json.loads(
+        result: dict[str, Any] = json.loads(
             txt, object_pairs_hook=self._report_duplicate_object_names
         )
         return result
 
-    def read_json(self, source: HREF, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    def read_json(self, source: HREF, *args: Any, **kwargs: Any) -> dict[str, Any]:
         """Overwrites :meth:`StacIO.read_json <pystac.StacIO.read_json>` for
         deserializing a JSON file to a dictionary while checking for duplicate object
         keys.
 
         Raises:
 
             pystac.DuplicateObjectKeyError : If a duplicate object key is found.
@@ -371,17 +371,17 @@
         except pystac.DuplicateObjectKeyError as e:
             url = str(os.fspath(source))
             msg = str(e) + f" in {url}"
             raise pystac.DuplicateObjectKeyError(msg)
 
     @staticmethod
     def _report_duplicate_object_names(
-        object_pairs: List[Tuple[str, Any]]
-    ) -> Dict[str, Any]:
-        result: Dict[str, Any] = {}
+        object_pairs: list[tuple[str, Any]]
+    ) -> dict[str, Any]:
+        result: dict[str, Any] = {}
         for key, value in object_pairs:
             if key in result:
                 raise pystac.DuplicateObjectKeyError(
                     f'Found duplicate object name "{key}"'
                 )
             else:
                 result[key] = value
@@ -416,16 +416,16 @@
 
         retry: Retry
         """The :py:class:`urllib3.util.retry.Retry` to use with all reading network
         requests."""
 
         def __init__(
             self,
-            headers: Optional[Dict[str, str]] = None,
-            retry: Optional[Retry] = None,
+            headers: dict[str, str] | None = None,
+            retry: Retry | None = None,
         ):
             super().__init__(headers)
             self.retry = retry or Retry()
 
         def read_text_from_href(self, href: str) -> str:
             """Reads file as a UTF-8 string, with retry support.
 
@@ -438,10 +438,10 @@
                 http = PoolManager()
                 try:
                     response = http.request(
                         "GET", href, retries=self.retry  # type: ignore
                     )
                     return cast(str, response.data.decode("utf-8"))
                 except HTTPError as e:
-                    raise Exception("Could not read uri {}".format(href)) from e
+                    raise Exception(f"Could not read uri {href}") from e
             else:
                 return super().read_text_from_href(href)
```

### Comparing `pystac-1.8.4/pystac/stac_object.py` & `pystac-1.9.0/pystac/stac_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 from html import escape
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Type,
     TypeVar,
-    Union,
     cast,
 )
 
 import pystac
 from pystac import STACError
 from pystac.html.jinja_env import get_jinja_env
 from pystac.link import Link
 from pystac.utils import (
+    HREF,
     StringEnum,
     is_absolute_href,
     make_absolute_href,
     make_posix_style,
 )
 
 if TYPE_CHECKING:
@@ -46,31 +41,31 @@
     and writing files. You shouldn't use STACObject directly, but instead access this
     functionality through the implementing classes.
     """
 
     id: str
     """The ID of the STAC Object."""
 
-    links: List[Link]
+    links: list[Link]
     """A list of :class:`~pystac.Link` objects representing all links associated with
     this STAC Object."""
 
-    stac_extensions: List[str]
+    stac_extensions: list[str]
     """A list of schema URIs for STAC Extensions implemented by this STAC Object."""
 
     STAC_OBJECT_TYPE: STACObjectType
 
     _allow_parent_to_override_href: bool = True
     """Private attribute for whether parent objects should override on normalization"""
 
-    def __init__(self, stac_extensions: List[str]) -> None:
+    def __init__(self, stac_extensions: list[str]) -> None:
         self.links = []
         self.stac_extensions = stac_extensions
 
-    def validate(self) -> List[Any]:
+    def validate(self) -> list[Any]:
         """Validate this STACObject.
 
         Returns a list of validation results, which depends on the validation
         implementation. For JSON Schema validation, this will be a list
         of schema URIs that were used during validation.
 
         Raises:
@@ -85,34 +80,34 @@
 
         Args:
              link : The link to add.
         """
         link.set_owner(self)
         self.links.append(link)
 
-    def add_links(self, links: List[Link]) -> None:
+    def add_links(self, links: list[Link]) -> None:
         """Add links to this object's set of links.
 
         Args:
              links : The links to add.
         """
 
         for link in links:
             self.add_link(link)
 
-    def remove_links(self, rel: Union[str, pystac.RelType]) -> None:
+    def remove_links(self, rel: str | pystac.RelType) -> None:
         """Remove links to this object's set of links that match the given ``rel``.
 
         Args:
              rel : The :class:`~pystac.Link` ``rel`` to match on.
         """
 
         self.links = [link for link in self.links if link.rel != rel]
 
-    def remove_hierarchical_links(self, add_canonical: bool = False) -> List[Link]:
+    def remove_hierarchical_links(self, add_canonical: bool = False) -> list[Link]:
         """Removes all hierarchical links from this object.
 
         See :py:const:`pystac.link.HIERARCHICAL_LINKS` for a list of all
         hierarchical links. If the object has a ``self`` href and
         ``add_canonical`` is True, a link with ``rel="canonical"`` is added.
 
         Args:
@@ -133,29 +128,27 @@
             if link.is_hierarchical():
                 remove.append(link)
             else:
                 keep.append(link)
         self.links = keep
         return remove
 
-    def target_in_hierarchy(self, target: Union[str, STACObject]) -> bool:
+    def target_in_hierarchy(self, target: str | STACObject) -> bool:
         """Determine if target is somewhere in the hierarchical link tree of
         a STACObject.
 
         Args:
             target: A string or STACObject to search for
 
         Returns:
             bool: Returns True if the target was found in the hierarchical link tree
                 for the current STACObject
         """
 
-        def traverse(
-            obj: Union[str, STACObject], visited: Set[Union[str, STACObject]]
-        ) -> bool:
+        def traverse(obj: str | STACObject, visited: set[str | STACObject]) -> bool:
             if obj == target:
                 return True
             if isinstance(obj, str):
                 return False
 
             new_targets = [
                 link.target
@@ -168,21 +161,21 @@
             for subtree in new_targets:
                 visited.add(subtree)
                 if traverse(subtree, visited):
                     return True
 
             return False
 
-        return traverse(self, set([self]))
+        return traverse(self, {self})
 
     def get_single_link(
         self,
-        rel: Optional[Union[str, pystac.RelType]] = None,
-        media_type: Optional[Union[str, pystac.MediaType]] = None,
-    ) -> Optional[Link]:
+        rel: str | pystac.RelType | None = None,
+        media_type: str | pystac.MediaType | None = None,
+    ) -> Link | None:
         """Get a single :class:`~pystac.Link` instance associated with this
         object.
 
         Args:
             rel : If set, filter links such that only those
                 matching this relationship are returned.
             media_type: If set, filter the links such that only
@@ -203,17 +196,17 @@
                 and (media_type is None or link.media_type == media_type)
             ),
             None,
         )
 
     def get_links(
         self,
-        rel: Optional[Union[str, pystac.RelType]] = None,
-        media_type: Optional[Union[str, pystac.MediaType]] = None,
-    ) -> List[Link]:
+        rel: str | pystac.RelType | None = None,
+        media_type: str | pystac.MediaType | None = None,
+    ) -> list[Link]:
         """Gets the :class:`~pystac.Link` instances associated with this object.
 
         Args:
             rel : If set, filter links such that only those
                 matching this relationship are returned.
             media_type: If set, filter the links such that only
                 those matching media_type are returned
@@ -229,26 +222,26 @@
             return [
                 link
                 for link in self.links
                 if (rel is None or link.rel == rel)
                 and (media_type is None or link.media_type == media_type)
             ]
 
-    def clear_links(self, rel: Optional[Union[str, pystac.RelType]] = None) -> None:
+    def clear_links(self, rel: str | pystac.RelType | None = None) -> None:
         """Clears all :class:`~pystac.Link` instances associated with this object.
 
         Args:
             rel : If set, only clear links that match this relationship.
         """
         if rel is not None:
             self.links = [link for link in self.links if link.rel != rel]
         else:
             self.links = []
 
-    def get_root_link(self) -> Optional[Link]:
+    def get_root_link(self) -> Link | None:
         """Get the :class:`~pystac.Link` representing
         the root for this object.
 
         Returns:
             :class:`~pystac.Link` or None: The root link for this object,
             or ``None`` if no root link is set.
         """
@@ -264,15 +257,15 @@
                 a ValueError. Use get_self_href if there may not be an href set.
         """
         result = self.get_self_href()
         if result is None:
             raise ValueError(f"{self} does not have a self_href set.")
         return result
 
-    def get_self_href(self) -> Optional[str]:
+    def get_self_href(self) -> str | None:
         """Gets the absolute HREF that is represented by the ``rel == 'self'``
         :class:`~pystac.Link`.
 
         Returns:
             str or None: The absolute HREF of this object, or ``None`` if
             there is no self link defined.
 
@@ -285,15 +278,15 @@
         """
         self_link = self.get_single_link(pystac.RelType.SELF)
         if self_link and self_link.has_target_href():
             return self_link.get_target_str()
         else:
             return None
 
-    def set_self_href(self, href: Optional[str]) -> None:
+    def set_self_href(self, href: str | None) -> None:
         """Sets the absolute HREF that is represented by the ``rel == 'self'``
         :class:`~pystac.Link`.
 
         Args:
             href : The absolute HREF of this object. If the given HREF
                 is not absolute, it will be transformed to an absolute
                 HREF based on the current working directory. If this is None
@@ -306,15 +299,15 @@
         self.remove_links(pystac.RelType.SELF)
         if href is not None:
             self.add_link(Link.self_href(href))
 
         if root_link is not None and root_link.is_resolved():
             cast(pystac.Catalog, root_link.target)._resolved_objects.cache(self)
 
-    def get_root(self) -> Optional[Catalog]:
+    def get_root(self) -> Catalog | None:
         """Get the :class:`~pystac.Catalog` or :class:`~pystac.Collection` to
         the root for this object. The root is represented by a
         :class:`~pystac.Link` with ``rel == 'root'``.
 
         Returns:
             Catalog, Collection, or None:
             The root object for this object, or ``None`` if no root link is set.
@@ -325,15 +318,15 @@
                 root_link.resolve_stac_object()
                 # Use set_root, so Catalogs can merge ResolvedObjectCache instances.
                 self.set_root(cast(pystac.Catalog, root_link.target))
             return cast(pystac.Catalog, root_link.target)
         else:
             return None
 
-    def set_root(self, root: Optional[Catalog]) -> None:
+    def set_root(self, root: Catalog | None) -> None:
         """Sets the root :class:`~pystac.Catalog` or :class:`~pystac.Collection`
         for this object.
 
         Args:
             root : The root
                 object to set. Passing in None will clear the root.
         """
@@ -361,15 +354,15 @@
             if root_link_index is not None:
                 self.links[root_link_index] = new_root_link
                 new_root_link.set_owner(self)
             else:
                 self.add_link(new_root_link)
             root._resolved_objects.cache(self)
 
-    def get_parent(self) -> Optional[Catalog]:
+    def get_parent(self) -> Catalog | None:
         """Get the :class:`~pystac.Catalog` or :class:`~pystac.Collection` to
         the parent for this object. The root is represented by a
         :class:`~pystac.Link` with ``rel == 'parent'``.
 
         Returns:
             Catalog, Collection, or None:
                 The parent object for this object,
@@ -377,32 +370,32 @@
         """
         parent_link = self.get_single_link(pystac.RelType.PARENT)
         if parent_link:
             return cast(pystac.Catalog, parent_link.resolve_stac_object().target)
         else:
             return None
 
-    def set_parent(self, parent: Optional[Catalog]) -> None:
+    def set_parent(self, parent: Catalog | None) -> None:
         """Sets the parent :class:`~pystac.Catalog` or :class:`~pystac.Collection`
         for this object.
 
         Args:
             parent : The parent
                 object to set. Passing in None will clear the parent.
         """
 
         self.remove_links(pystac.RelType.PARENT)
         if parent is not None:
             self.add_link(Link.parent(parent))
 
     def get_stac_objects(
         self,
-        rel: Union[str, pystac.RelType],
-        typ: Optional[Type[STACObject]] = None,
-        modify_links: Optional[Callable[[List[Link]], List[Link]]] = None,
+        rel: str | pystac.RelType,
+        typ: type[STACObject] | None = None,
+        modify_links: Callable[[list[Link]], list[Link]] | None = None,
     ) -> Iterable[STACObject]:
         """Gets the :class:`~pystac.STACObject` instances that are linked to
         by links with their ``rel`` property matching the passed in argument.
 
         Args:
             rel : The relation to match each :class:`~pystac.Link`'s
                 ``rel`` property against.
@@ -427,16 +420,16 @@
                 link.resolve_stac_object(root=self.get_root())
                 if typ is None or isinstance(link.target, typ):
                     yield cast(STACObject, link.target)
 
     def save_object(
         self,
         include_self_link: bool = True,
-        dest_href: Optional[str] = None,
-        stac_io: Optional[pystac.StacIO] = None,
+        dest_href: str | None = None,
+        stac_io: pystac.StacIO | None = None,
     ) -> None:
         """Saves this STAC Object to it's 'self' HREF.
 
         Args:
             include_self_link : If this is true, include the 'self' link with
                 this object. Otherwise, leave out the self link.
             dest_href : Optional HREF to save the file to. If None, the object
@@ -473,16 +466,16 @@
                 )
             dest_href = self_href
 
         stac_io.save_json(dest_href, self.to_dict(include_self_link=include_self_link))
 
     def full_copy(
         self,
-        root: Optional[Catalog] = None,
-        parent: Optional[Catalog] = None,
+        root: Catalog | None = None,
+        parent: Catalog | None = None,
     ) -> STACObject:
         """Create a full copy of this STAC object and any stac objects linked to by
         this object.
 
         Args:
             root : Optional root to set as the root of the copied object,
                 and any other copies that are contained by this object.
@@ -548,25 +541,25 @@
 
         for link in self.links:
             if link.rel in link_rels:
                 if not link.is_resolved():
                     link.resolve_stac_object(root=self.get_root())
 
     @abstractmethod
-    def _object_links(self) -> List[str]:
+    def _object_links(self) -> list[str]:
         """Inherited classes return a list of link 'rel' types that represent
         STACObjects linked to by this object (not including root, parent or self).
         This can include optional relations (which may not be present).
         """
         raise NotImplementedError
 
     @abstractmethod
     def to_dict(
         self, include_self_link: bool = True, transform_hrefs: bool = True
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         """Returns this object as a dictionary.
 
         Args:
             include_self_link : If True, the dict will contain a self link
                 to this object. If False, the self link will be omitted.
             transform_hrefs: If True, transform the HREF of hierarchical links
                 based on the type of catalog this object belongs to (if any).
@@ -598,17 +591,15 @@
 
         Returns:
             STACObject: The clone of this object.
         """
         raise NotImplementedError
 
     @classmethod
-    def from_file(
-        cls: Type[S], href: str, stac_io: Optional[pystac.StacIO] = None
-    ) -> S:
+    def from_file(cls: type[S], href: HREF, stac_io: pystac.StacIO | None = None) -> S:
         """Reads a STACObject implementation from a file.
 
         Args:
             href : The HREF to read the object from.
             stac_io: Optional instance of StacIO to use. If not provided, will use the
                 default instance.
 
@@ -637,18 +628,18 @@
                 if root_link.get_absolute_href() == href:
                     o.set_root(cast(pystac.Catalog, o))
         return o
 
     @classmethod
     @abstractmethod
     def from_dict(
-        cls: Type[S],
-        d: Dict[str, Any],
-        href: Optional[str] = None,
-        root: Optional[Catalog] = None,
+        cls: type[S],
+        d: dict[str, Any],
+        href: str | None = None,
+        root: Catalog | None = None,
         migrate: bool = False,
         preserve_dict: bool = True,
     ) -> S:
         """Parses this STACObject from the passed in dictionary.
 
         Args:
             d : The dict to parse.
@@ -668,15 +659,15 @@
         Returns:
             STACObject: The STACObject parsed from this dict.
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def matches_object_type(cls, d: Dict[str, Any]) -> bool:
+    def matches_object_type(cls, d: dict[str, Any]) -> bool:
         """Returns a boolean indicating whether the given dictionary represents a valid
         instance of this :class:`~STACObject` sub-class.
 
         Args:
             d : A dictionary to identify
         """
         raise NotImplementedError
```

### Comparing `pystac-1.8.4/pystac/static/fields-normalized.json` & `pystac-1.9.0/pystac/static/fields-normalized.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/summaries.py` & `pystac-1.9.0/pystac/summaries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from __future__ import annotations
 
+import importlib.resources
 import json
 import numbers
-import sys
 from abc import abstractmethod
+from collections.abc import Iterable
 from copy import deepcopy
 from enum import Enum
 from functools import lru_cache
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
     Generic,
-    Iterable,
-    List,
-    Optional,
     Protocol,
     TypeVar,
     Union,
 )
 
-if sys.version_info[:2] < (3, 9):
-    from importlib_resources import files as importlib_resources_files
-else:
-    from importlib.resources import files as importlib_resources_files
-
 import pystac
 from pystac.utils import get_required
 
 if TYPE_CHECKING:
     from pystac.collection import Collection
     from pystac.item import Item
 
@@ -52,50 +44,50 @@
     """Protocol for annotating comparable types.
 
     For matching __lt__ that takes an 'x' parameter
     (e.g. float)
     """
 
     @abstractmethod
-    def __lt__(self: "T", x: "T") -> bool:
+    def __lt__(self: T, x: T) -> bool:
         return NotImplemented
 
 
 class _Comparable_other(Protocol):
     """Protocol for annotating comparable types.
 
     For matching __lt___ that takes an 'other' parameter
     (e.g. datetime)
     """
 
     @abstractmethod
-    def __lt__(self: "T", other: "T") -> bool:
+    def __lt__(self: T, other: T) -> bool:
         return NotImplemented
 
 
 T = TypeVar("T", bound=Union[_Comparable_x, _Comparable_other])
 
 
 class RangeSummary(Generic[T]):
     minimum: T
     maximum: T
 
     def __init__(self, minimum: T, maximum: T):
         self.minimum = minimum
         self.maximum = maximum
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {"minimum": self.minimum, "maximum": self.maximum}
 
     def update_with_value(self, v: T) -> None:
         self.minimum = min(self.minimum, v)
         self.maximum = max(self.maximum, v)
 
     @classmethod
-    def from_dict(cls, d: Dict[str, Any]) -> RangeSummary[T]:
+    def from_dict(cls, d: dict[str, Any]) -> RangeSummary[T]:
         minimum: T = get_required(d.get("minimum"), "RangeSummary", "minimum")
         maximum: T = get_required(d.get("maximum"), "RangeSummary", "maximum")
         return cls(minimum=minimum, maximum=maximum)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, RangeSummary):
             return NotImplemented
@@ -103,20 +95,20 @@
         return self.to_dict() == o.to_dict()
 
     def __repr__(self) -> str:
         return self.to_dict().__repr__()
 
 
 @lru_cache(maxsize=None)
-def _get_fields_json(url: Optional[str]) -> Dict[str, Any]:
+def _get_fields_json(url: str | None) -> dict[str, Any]:
     if url is None:
         # Every time pystac is released this file gets pulled from
         # https://cdn.jsdelivr.net/npm/@radiantearth/stac-fields/fields-normalized.json
-        jsonfields: Dict[str, Any] = json.loads(
-            importlib_resources_files("pystac.static")
+        jsonfields: dict[str, Any] = json.loads(
+            importlib.resources.files("pystac.static")
             .joinpath("fields-normalized.json")
             .read_text()
         )
         return jsonfields
     return pystac.StacIO.default().read_json(url)
 
 
@@ -149,24 +141,24 @@
     Args:
         fields: A string containing the path to the json file with field descriptions.
             Alternatively, a dict with the field names as keys and SummaryStrategys
             as values.
             If nothing is passed, a default file with field descriptions will be used.
     """
 
-    summaryfields: Dict[str, SummaryStrategy]
+    summaryfields: dict[str, SummaryStrategy]
 
-    def __init__(self, fields: Optional[Union[str, Dict[str, SummaryStrategy]]] = None):
+    def __init__(self, fields: str | dict[str, SummaryStrategy] | None = None):
         if isinstance(fields, dict):
             self._set_field_definitions(fields)
         else:
             jsonfields = _get_fields_json(fields)
             self._set_field_definitions(jsonfields["metadata"])
 
-    def _set_field_definitions(self, fields: Dict[str, Any]) -> None:
+    def _set_field_definitions(self, fields: dict[str, Any]) -> None:
         self.summaryfields = {}
         for name, desc in fields.items():
             strategy: SummaryStrategy = SummaryStrategy.DEFAULT
             if isinstance(desc, SummaryStrategy):
                 strategy = desc
             elif isinstance(desc, dict):
                 strategy_value = desc.get("summary", True)
@@ -183,36 +175,36 @@
             if k in self.summaryfields:
                 strategy = self.summaryfields[k]
                 if strategy == SummaryStrategy.RANGE or (
                     strategy == SummaryStrategy.DEFAULT
                     and isinstance(v, numbers.Number)
                     and not isinstance(v, bool)
                 ):
-                    rangesummary: Optional[RangeSummary[Any]] = summaries.get_range(k)
+                    rangesummary: RangeSummary[Any] | None = summaries.get_range(k)
                     if rangesummary is None:
                         summaries.add(k, RangeSummary(v, v))
                     else:
                         rangesummary.update_with_value(v)
                 elif strategy == SummaryStrategy.ARRAY or (
                     strategy == SummaryStrategy.DEFAULT and isinstance(v, list)
                 ):
-                    listsummary: List[Any] = summaries.get_list(k) or []
+                    listsummary: list[Any] = summaries.get_list(k) or []
                     if not isinstance(v, list):
                         v = [v]
                     for element in v:
                         if element not in listsummary:
                             listsummary.append(element)
                     summaries.add(k, listsummary)
                 else:
-                    summary: List[Any] = summaries.get_list(k) or []
+                    summary: list[Any] = summaries.get_list(k) or []
                     if v not in summary:
                         summary.append(v)
                     summaries.add(k, summary)
 
-    def summarize(self, source: Union[Collection, Iterable[Item]]) -> Summaries:
+    def summarize(self, source: Collection | Iterable[Item]) -> Summaries:
         """Creates summaries from items"""
         summaries = Summaries.empty()
         if isinstance(source, pystac.Collection):
             for item in source.get_items(recursive=True):
                 self._update_with_item(summaries, item)
         else:
             for item in source:
@@ -221,49 +213,49 @@
         return summaries
 
 
 DEFAULT_MAXCOUNT = 25
 
 
 class Summaries:
-    _summaries: Dict[str, Any]
+    _summaries: dict[str, Any]
 
-    lists: Dict[str, List[Any]]
-    other: Dict[str, Any]
-    ranges: Dict[str, RangeSummary[Any]]
-    schemas: Dict[str, Dict[str, Any]]
+    lists: dict[str, list[Any]]
+    other: dict[str, Any]
+    ranges: dict[str, RangeSummary[Any]]
+    schemas: dict[str, dict[str, Any]]
     maxcount: int
 
     def __init__(
-        self, summaries: Dict[str, Any], maxcount: int = DEFAULT_MAXCOUNT
+        self, summaries: dict[str, Any], maxcount: int = DEFAULT_MAXCOUNT
     ) -> None:
         self._summaries = summaries
         self.maxcount = maxcount
 
         self.lists = {}
         self.ranges = {}
         self.schemas = {}
         self.other = {}
 
         for prop_key, summary in summaries.items():
             self.add(prop_key, summary)
 
-    def get_list(self, prop: str) -> Optional[List[Any]]:
+    def get_list(self, prop: str) -> list[Any] | None:
         return self.lists.get(prop)
 
-    def get_range(self, prop: str) -> Optional[RangeSummary[Any]]:
+    def get_range(self, prop: str) -> RangeSummary[Any] | None:
         return self.ranges.get(prop)
 
-    def get_schema(self, prop: str) -> Optional[Dict[str, Any]]:
+    def get_schema(self, prop: str) -> dict[str, Any] | None:
         return self.schemas.get(prop)
 
     def add(
         self,
         prop_key: str,
-        summary: Union[List[Any], RangeSummary[Any], Dict[str, Any]],
+        summary: list[Any] | RangeSummary[Any] | dict[str, Any],
     ) -> None:
         if isinstance(summary, list):
             self.lists[prop_key] = summary
         elif isinstance(summary, dict):
             if "minimum" in summary:
                 self.ranges[prop_key] = RangeSummary[Any].from_dict(summary)
             else:
@@ -323,15 +315,15 @@
         summaries = cls(summaries=deepcopy(self._summaries), maxcount=self.maxcount)
         summaries.lists = deepcopy(self.lists)
         summaries.other = deepcopy(self.other)
         summaries.ranges = deepcopy(self.ranges)
         summaries.schemas = deepcopy(self.schemas)
         return summaries
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             **{k: v for k, v in self.lists.items() if len(v) < self.maxcount},
             **{k: v.to_dict() for k, v in self.ranges.items()},
             **self.schemas,
             **self.other,
         }
```

### Comparing `pystac-1.8.4/pystac/utils.py` & `pystac-1.9.0/pystac/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import warnings
 from datetime import datetime, timezone
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    Dict,
-    List,
     Optional,
     TypeVar,
     Union,
     cast,
 )
 from urllib.parse import ParseResult as URLParseResult
 from urllib.parse import urljoin, urlparse, urlunparse
@@ -55,18 +53,18 @@
         href (str) : The HREF to parse. May be a local file path or URL.
 
     Returns:
         urllib.parse.ParseResult : The named tuple representing the parsed HREF.
     """
     parsed = urlparse(href)
     if parsed.scheme != "" and (
-        href.lower().startswith("{}:\\".format(parsed.scheme))
+        href.lower().startswith(f"{parsed.scheme}:\\")
         or (
-            href.lower().startswith("{}:/".format(parsed.scheme))
-            and not href.lower().startswith("{}://".format(parsed.scheme))
+            href.lower().startswith(f"{parsed.scheme}:/")
+            and not href.lower().startswith(f"{parsed.scheme}://")
         )
     ):
         return URLParseResult(
             scheme="",
             netloc="",
             path="{}:{}".format(
                 # We use this more complicated formulation because parsed.scheme
@@ -82,14 +80,17 @@
         return parsed
 
 
 class StringEnum(str, Enum):
     """Base :class:`enum.Enum` class for string enums that will serialize as the string
     value."""
 
+    def __repr__(self) -> str:
+        return str(self.value)
+
     def __str__(self) -> str:
         return cast(str, self.value)
 
 
 class JoinType(StringEnum):
     """DEPRECATED.
 
@@ -389,15 +390,15 @@
     """
     if dt.tzinfo is None:
         dt = dt.replace(tzinfo=timezone.utc)
 
     timestamp = dt.isoformat(timespec=timespec)
     zulu = "+00:00"
     if timestamp.endswith(zulu):
-        timestamp = "{}Z".format(timestamp[: -len(zulu)])
+        timestamp = f"{timestamp[: -len(zulu)]}Z"
 
     return timestamp
 
 
 def str_to_datetime(s: str) -> datetime:
     """Converts a string timestamp to a :class:`datetime.datetime` instance using
     :meth:`dateutil.parser.parse` under the hood. The input string may be in any
@@ -419,30 +420,30 @@
 
 
 def now_to_rfc3339_str() -> str:
     """Returns an RFC 3339 string representing now"""
     return datetime_to_str(now_in_utc())
 
 
-def geometry_to_bbox(geometry: Dict[str, Any]) -> List[float]:
+def geometry_to_bbox(geometry: dict[str, Any]) -> list[float]:
     """Extract the bounding box from a geojson geometry
 
     Args:
         geometry : GeoJSON geometry dict
 
     Returns:
         list: Bounding box of geojson geometry, formatted according to:
         https://tools.ietf.org/html/rfc7946#section-5
     """
     coords = geometry["coordinates"]
 
-    lats: List[float] = []
-    lons: List[float] = []
+    lats: list[float] = []
+    lons: list[float] = []
 
-    def extract_coords(coords: List[Union[List[float], List[List[Any]]]]) -> None:
+    def extract_coords(coords: list[Union[list[float], list[list[Any]]]]) -> None:
         for x in coords:
             # This handles points
             if isinstance(x, float):
                 assert isinstance(
                     coords[0], float
                 ), f"Type mismatch: {coords[0]} is not a float"
                 assert isinstance(
```

### Comparing `pystac-1.8.4/pystac/validation/__init__.py` & `pystac-1.9.0/pystac/validation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
+import warnings
+from collections.abc import Iterable, Mapping
+from typing import TYPE_CHECKING, Any, cast
 
 import pystac
 from pystac.serialization.identify import STACVersionID, identify_stac_object
 from pystac.stac_object import STACObjectType
 from pystac.utils import make_absolute_href
 from pystac.validation.schema_uri_map import OldExtensionSchemaUriMap
+from pystac.validation.stac_validator import GetSchemaError
 
 if TYPE_CHECKING:
     from pystac.stac_object import STACObject
 
 
 # Import after above class definition
 from pystac.validation.stac_validator import JsonSchemaSTACValidator, STACValidator
 
 
-def validate(stac_object: STACObject) -> List[Any]:
+def validate(stac_object: STACObject) -> list[Any]:
     """Validates a :class:`~pystac.STACObject`.
 
     Args:
         stac_object : The stac object to validate.
 
     Returns:
         List[Object]: List of return values from the validation calls for the
@@ -36,20 +39,20 @@
         stac_version=pystac.get_stac_version(),
         extensions=stac_object.stac_extensions,
         href=stac_object.get_self_href(),
     )
 
 
 def validate_dict(
-    stac_dict: Dict[str, Any],
-    stac_object_type: Optional[STACObjectType] = None,
-    stac_version: Optional[str] = None,
-    extensions: Optional[List[str]] = None,
-    href: Optional[str] = None,
-) -> List[Any]:
+    stac_dict: dict[str, Any],
+    stac_object_type: STACObjectType | None = None,
+    stac_version: str | None = None,
+    extensions: list[str] | None = None,
+    href: str | None = None,
+) -> list[Any]:
     """Validate a stac object serialized as JSON into a dict.
 
     This method delegates to the call to
     :meth:`pystac.validation.STACValidator.validate` for the STACValidator registered
     via :meth:`~pystac.validation.set_validator` or
     :class:`~pystac.validation.JsonSchemaSTACValidator` by default.
 
@@ -88,47 +91,100 @@
 
     stac_version_id = STACVersionID(stac_version)
 
     # If the version is before 1.0.0-rc.2, substitute extension short IDs for
     # their schemas.
     if stac_version_id < "1.0.0-rc.2":
 
-        def _get_uri(ext: str) -> Optional[str]:
+        def _get_uri(ext: str) -> str | None:
             return OldExtensionSchemaUriMap.get_extension_schema_uri(
                 ext,
                 stac_object_type,
                 stac_version_id,
             )
 
         extensions = [uri for uri in map(_get_uri, extensions) if uri is not None]
 
     return RegisteredValidator.get_validator().validate(
         stac_dict, stac_object_type, stac_version, extensions, href
     )
 
 
 def validate_all(
-    stac_dict: Dict[str, Any], href: str, stac_io: Optional[pystac.StacIO] = None
+    stac_object: STACObject | dict[str, Any],
+    href: str | None = None,
+    stac_io: pystac.StacIO | None = None,
 ) -> None:
-    """Validate STAC JSON and all contained catalogs, collections and items.
+    """Validate a :class:`~pystac.STACObject`, or a STAC object serialized as
+    JSON into a dict.
 
-    If this stac_dict represents a catalog or collection, this method will
-    recursively be called for each child link and all contained items.
+    If the STAC object represents a catalog or collection, this function will be
+    called recursively for each child link and all contained items.
 
     Args:
+        stac_object : STAC object to validate
+        href : HREF of the STAC object being validated. Used for error
+            reporting and resolving relative links.
+        stac_io : Optional StacIO instance to use for reading hrefs. If None,
+            the StacIO.default() instance is used.
+
+    Raises:
+        STACValidationError: if the STAC object or any contained catalog, collection,
+            or item has a validation error
+        ValueError: if stac_object is a STACObject and href is not None, or if
+            stacl_object is a dict and href is None
+    """
+    if stac_io is None:
+        stac_io = pystac.StacIO.default()
+
+    if isinstance(stac_object, dict):
+        warnings.warn(
+            "validating a STAC object as a dict is deprecated;"
+            " use validate_all_dict instead",
+            DeprecationWarning,
+        )
+
+        if href is None:
+            raise ValueError(
+                "href must be set if stac_object is a dict; it will be removed"
+                " once support for validating a STAC object as a dict is removed from"
+                " validate_all, due to the introduction of validate_all_dict"
+            )
 
+        validate_all_dict(stac_object, href, stac_io)
+    elif href is not None:
+        raise ValueError(
+            "href must be None if stac_object is a STACObject; it will be removed"
+            " once support for validating a STAC object as a dict is removed from"
+            " validate_all, due to the introduction of validate_all_dict"
+        )
+    else:
+        validate_all_dict(stac_object.to_dict(), stac_object.get_self_href(), stac_io)
+
+
+def validate_all_dict(
+    stac_dict: dict[str, Any],
+    href: str | None,
+    stac_io: pystac.StacIO | None = None,
+) -> None:
+    """Validate a stac object serialized as JSON into a dict.
+
+    If the STAC object represents a catalog or collection, this function will be
+    called recursively for each child link and all contained items.
+
+    Args:
         stac_dict : Dictionary that is the STAC json of the object.
         href : HREF of the STAC object being validated. Used for error
             reporting and resolving relative links.
-        stac_io: Optional StacIO instance to use for reading hrefs. If None,
+        stac_io : Optional StacIO instance to use for reading hrefs. If None,
             the StacIO.default() instance is used.
 
     Raises:
-        STACValidationError: This will raise a STACValidationError if this or any
-            contained catalog, collection or item has a validation error.
+        STACValidationError: if the STAC object or any contained catalog, collection,
+        or item has a validation error
     """
     if stac_io is None:
         stac_io = pystac.StacIO.default()
 
     info = identify_stac_object(stac_dict)
 
     # Validate this object
@@ -136,34 +192,32 @@
         stac_dict,
         stac_object_type=info.object_type,
         stac_version=str(info.version_range.latest_valid_version()),
         extensions=list(info.extensions),
         href=href,
     )
 
-    if info.object_type != pystac.STACObjectType.ITEM:
-        if "links" in stac_dict:
+    if info.object_type != pystac.STACObjectType.ITEM and "links" in stac_dict:
+        links = (
             # Account for 0.6 links
-            if isinstance(stac_dict["links"], dict):
-                links: List[Dict[str, Any]] = list(stac_dict["links"].values())
-            else:
-                links = cast(List[Dict[str, Any]], stac_dict.get("links"))
-            for link in links:
-                rel = link.get("rel")
-                if rel in [pystac.RelType.ITEM, pystac.RelType.CHILD]:
-                    link_href = make_absolute_href(
-                        cast(str, link.get("href")), start_href=href
-                    )
-                    if link_href is not None:
-                        d = stac_io.read_json(link_href)
-                        validate_all(d, link_href)
+            stac_dict["links"].values()
+            if isinstance(stac_dict["links"], dict)
+            else stac_dict.get("links")
+        )
+
+        for link in cast(Iterable[Mapping[str, Any]], links):
+            if link.get("rel") in [pystac.RelType.ITEM, pystac.RelType.CHILD]:
+                link_href = make_absolute_href(
+                    cast(str, link.get("href")), start_href=href
+                )
+                validate_all_dict(stac_io.read_json(link_href), link_href, stac_io)
 
 
 class RegisteredValidator:
-    _validator: Optional[STACValidator] = None
+    _validator: STACValidator | None = None
 
     @classmethod
     def get_validator(cls) -> STACValidator:
         if cls._validator is None:
             try:
                 import jsonschema as _  # noqa
             except ImportError:
@@ -176,19 +230,22 @@
             cls._validator = JsonSchemaSTACValidator()
 
         return cls._validator
 
     @classmethod
     def set_validator(cls, validator: STACValidator) -> None:
         if not issubclass(type(validator), STACValidator):
-            raise Exception("Validator must be a subclass of {}".format(STACValidator))
+            raise Exception(f"Validator must be a subclass of {STACValidator}")
         cls._validator = validator
 
 
 def set_validator(validator: STACValidator) -> None:
     """Sets the STACValidator to use in PySTAC.
 
     Args:
         validator : The STACValidator implementation to use for
             validation.
     """
     RegisteredValidator.set_validator(validator)
+
+
+__all__ = ["GetSchemaError"]
```

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/geojson/Feature.json` & `pystac-1.9.0/pystac/validation/jsonschemas/geojson/Feature.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/geojson/Geometry.json` & `pystac-1.9.0/pystac/validation/jsonschemas/geojson/Geometry.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json` & `pystac-1.9.0/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.4/pystac/validation/local_validator.py` & `pystac-1.9.0/pystac/validation/local_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,29 @@
+import importlib.resources
 import json
-import sys
 import warnings
-from typing import Any, Dict, List, cast
+from typing import Any, cast
 
 from jsonschema import Draft7Validator, ValidationError
 from referencing import Registry, Resource
 
 from pystac.errors import STACLocalValidationError
 from pystac.version import STACVersion
 
-if sys.version_info[:2] < (3, 9):
-    from importlib_resources import files as importlib_resources_files
-else:
-    from importlib.resources import files as importlib_resources_files
-
 VERSION = STACVersion.DEFAULT_STAC_VERSION
 
 
-def _read_schema(file_name: str) -> Dict[str, Any]:
-    with importlib_resources_files("pystac.validation.jsonschemas").joinpath(
+def _read_schema(file_name: str) -> dict[str, Any]:
+    with importlib.resources.files("pystac.validation.jsonschemas").joinpath(
         file_name
     ).open("r") as f:
-        return cast(Dict[str, Any], json.load(f))
+        return cast(dict[str, Any], json.load(f))
 
 
-def get_local_schema_cache() -> Dict[str, Dict[str, Any]]:
+def get_local_schema_cache() -> dict[str, dict[str, Any]]:
     return {
         **{
             (
                 f"https://schemas.stacspec.org/v{VERSION}/"
                 f"{name}-spec/json-schema/{name}.json"
             ): _read_schema(f"stac-spec/v{VERSION}/{name}.json")
             for name in ("item", "catalog", "collection")
@@ -91,31 +86,31 @@
         return Registry().with_resources(
             [
                 (k, Resource.from_contents(v)) for k, v in self.schema_cache.items()
             ]  # type: ignore
         )
 
     def _validate_from_local(
-        self, schema_uri: str, stac_dict: Dict[str, Any]
-    ) -> List[ValidationError]:
+        self, schema_uri: str, stac_dict: dict[str, Any]
+    ) -> list[ValidationError]:
         if schema_uri == _deprecated_ITEM_SCHEMA_URI:
             validator = self.item_validator(VERSION)
         elif schema_uri == _deprecated_COLLECTION_SCHEMA_URI:
             validator = self.collection_validator(VERSION)
         elif schema_uri == _deprecated_CATALOG_SCHEMA_URI:
             validator = self.catalog_validator(VERSION)
         else:
             raise STACLocalValidationError(
                 f"Schema not available locally: {schema_uri}"
             )
         return list(validator.iter_errors(stac_dict))
 
     def _validator(self, stac_type: str, version: str) -> Draft7Validator:
         schema = _read_schema(f"stac-spec/v{version}/{stac_type}.json")
-        return Draft7Validator(schema, registry=self.registry)
+        return Draft7Validator(schema, registry=self.registry())
 
     def catalog_validator(self, version: str = VERSION) -> Draft7Validator:
         return self._validator("catalog", version)
 
     def collection_validator(self, version: str = VERSION) -> Draft7Validator:
         return self._validator("collection", version)
```

### Comparing `pystac-1.8.4/pystac/validation/schema_uri_map.py` & `pystac-1.9.0/pystac/validation/schema_uri_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from functools import lru_cache
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Callable, Optional
 
 import pystac
 from pystac.serialization import STACVersionRange
 from pystac.serialization.identify import OldExtensionShortIDs, STACVersionID
 from pystac.stac_object import STACObjectType
 
 
@@ -39,18 +39,18 @@
     """
 
     # BASE_URIS contains a list of tuples, the first element is a version range and the
     # second being the base URI for schemas for that range. The schema URI of a STAC
     # for a particular version uses the base URI associated with the version range which
     # contains it. If the version it outside of any VersionRange, there is no URI for
     # the schema.
-    BASE_URIS: List[Tuple[STACVersionRange, Callable[[str], str]]] = [
+    BASE_URIS: list[tuple[STACVersionRange, Callable[[str], str]]] = [
         (
             STACVersionRange(min_version="1.0.0-beta.2"),
-            lambda version: "https://schemas.stacspec.org/v{}".format(version),
+            lambda version: f"https://schemas.stacspec.org/v{version}",
         ),
         (
             STACVersionRange(min_version="0.8.0", max_version="1.0.0-beta.1"),
             lambda version: (
                 f"https://raw.githubusercontent.com/radiantearth/stac-spec/v{version}"
             ),
         ),
@@ -60,15 +60,15 @@
     # URIs based on the stac object type and the stac version, using a similar
     # technique as BASE_URIS. Uris are contained in a tuple whose first element
     # represents the URI of the latest version, so that a search through version
     # ranges is avoided if the STAC being validated
     # is the latest version. If it's a previous version, the stac_version that matches
     # the listed version range is used, or else the URI from the latest version is used
     # if there are no overrides for previous versions.
-    DEFAULT_SCHEMA_MAP: Dict[str, Any] = {
+    DEFAULT_SCHEMA_MAP: dict[str, Any] = {
         STACObjectType.CATALOG: ("catalog-spec/json-schema/catalog.json", None),
         STACObjectType.COLLECTION: (
             "collection-spec/json-schema/collection.json",
             None,
         ),
         STACObjectType.ITEM: ("item-spec/json-schema/item.json", None),
     }
@@ -76,28 +76,28 @@
     @classmethod
     def _append_base_uri_if_needed(cls, uri: str, stac_version: str) -> Optional[str]:
         # Only append the base URI if it's not already an absolute URI
         if "://" not in uri:
             for version_range, f in cls.BASE_URIS:
                 if version_range.contains(stac_version):
                     base_uri = f(stac_version)
-                    return "{}/{}".format(base_uri, uri)
+                    return f"{base_uri}/{uri}"
 
             # We don't have JSON schema validation for this version of PySTAC
             return None
         else:
             return uri
 
     def get_object_schema_uri(
         self, object_type: STACObjectType, stac_version: str
     ) -> Optional[str]:
         is_latest = stac_version == pystac.get_stac_version()
 
         if object_type not in self.DEFAULT_SCHEMA_MAP:
-            raise KeyError("Unknown STAC object type {}".format(object_type))
+            raise KeyError(f"Unknown STAC object type {object_type}")
         uri = self.DEFAULT_SCHEMA_MAP[object_type][0]
         if not is_latest:
             if self.DEFAULT_SCHEMA_MAP[object_type][1]:
                 for version_range, range_uri in self.DEFAULT_SCHEMA_MAP[object_type][1]:
                     if version_range.contains(stac_version):
                         uri = range_uri
                         break
@@ -114,18 +114,18 @@
 
     # BASE_URIS contains a list of tuples, the first element is a version range and the
     # second being the base URI for schemas for that range. The schema URI of a STAC
     # for a particular version uses the base URI associated with the version range which
     # contains it. If the version it outside of any VersionRange, there is no URI for
     # the schema.
     @classmethod
-    @lru_cache()
+    @lru_cache
     def get_base_uris(
         cls,
-    ) -> List[Tuple[STACVersionRange, Callable[[STACVersionID], str]]]:
+    ) -> list[tuple[STACVersionRange, Callable[[STACVersionID], str]]]:
         return [
             (
                 STACVersionRange(min_version="1.0.0-beta.2"),
                 lambda version: f"https://schemas.stacspec.org/v{version}",
             ),
             (
                 STACVersionRange(min_version="0.8.0", max_version="1.0.0-beta.1"),
@@ -140,16 +140,16 @@
     # based on the stac object type, extension ID and the stac version.
     # Uris are contained in a tuple whose first element represents the URI of the latest
     # version, so that a search through version ranges is avoided if the STAC being
     # validated is the latest version. If it's a previous version, the stac_version
     # that matches the listed version range is used, or else the URI from the latest
     # version is used if there are no overrides for previous versions.
     @classmethod
-    @lru_cache()
-    def get_schema_map(cls) -> Dict[str, Any]:
+    @lru_cache
+    def get_schema_map(cls) -> dict[str, Any]:
         return {
             OldExtensionShortIDs.CHECKSUM.value: (
                 {
                     pystac.STACObjectType.CATALOG: (
                         "extensions/checksum/json-schema/schema.json"
                     ),
                     pystac.STACObjectType.COLLECTION: (
@@ -312,15 +312,15 @@
         cls, uri: str, stac_version: STACVersionID
     ) -> Optional[str]:
         # Only append the base URI if it's not already an absolute URI
         if "://" not in uri:
             for version_range, f in cls.get_base_uris():
                 if version_range.contains(stac_version):
                     base_uri = f(stac_version)
-                    return "{}/{}".format(base_uri, uri)
+                    return f"{base_uri}/{uri}"
 
             # No JSON Schema for the old extension
             return None
         else:
             return uri
 
     @classmethod
```

### Comparing `pystac-1.8.4/pystac/validation/stac_validator.py` & `pystac-1.9.0/pystac/validation/stac_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 import warnings
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Optional
 
 import pystac
 import pystac.utils
 from pystac.errors import STACValidationError
 from pystac.stac_object import STACObjectType
 from pystac.validation.schema_uri_map import DefaultSchemaUriMap, SchemaUriMap
 
@@ -21,26 +21,33 @@
     HAS_JSONSCHEMA = True
 except ImportError:
     HAS_JSONSCHEMA = False
 
 logger = logging.getLogger(__name__)
 
 
+class GetSchemaError(Exception):
+    """Raised when unable to fetch a schema."""
+
+    def __init__(self, href: str, error: Exception) -> None:
+        super().__init__(f"Error when fetching schema {href}: {error}")
+
+
 class STACValidator(ABC):
     """STACValidator defines methods for validating STAC
     JSON. Implementations define methods for validating core objects and extension.
     By default the JsonSchemaSTACValidator is used by PySTAC; users can define their own
     STACValidator implementation and set that validator to be used by
     pystac by using the :func:`~pystac.validation.set_validator` method.
     """
 
     @abstractmethod
     def validate_core(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         href: Optional[str] = None,
     ) -> Any:
         """Validate a core stac object.
 
         Return value can be None or specific to the implementation.
@@ -53,15 +60,15 @@
             href : Optional HREF of the STAC object being validated.
         """
         raise NotImplementedError
 
     @abstractmethod
     def validate_extension(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         extension_id: str,
         href: Optional[str] = None,
     ) -> Any:
         """Validate an extension stac object.
 
@@ -75,20 +82,20 @@
             extension_id : The extension ID of the extension to validate against.
             href : Optional HREF of the STAC object being validated.
         """
         raise NotImplementedError
 
     def validate(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
-        extensions: List[str],
+        extensions: list[str],
         href: Optional[str] = None,
-    ) -> List[Any]:
+    ) -> list[Any]:
         """Validate a STAC object JSON.
 
         Args:
             stac_dict : Dictionary that is the STAC json of the object.
             stac_object_type : The stac object type of the object encoded in
                 stac_dict. One of :class:`~pystac.STACObjectType`.
             stac_version : The version of STAC to validate the object against.
@@ -96,15 +103,15 @@
             href : Optional href of the STAC object being validated.
 
         Returns:
             List[Any]: List of return values from the validation calls for the
                core object and any extensions. Element type is specific to the
                STACValidator implementation.
         """
-        results: List[Any] = []
+        results: list[Any] = []
 
         # Pass the dict through JSON serialization and parsing, otherwise
         # some valid properties can be marked as invalid (e.g. tuples in
         # coordinate sequences for geometries).
         json_dict = json.loads(json.dumps(stac_dict))
         core_result = self.validate_core(
             json_dict, stac_object_type, stac_version, href
@@ -136,58 +143,61 @@
             :class:`~pystac.validation.schema_uri_map.DefaultSchemaUriMap`
 
     Note:
     This class requires the ``jsonschema`` library to be installed.
     """
 
     schema_uri_map: SchemaUriMap
-    schema_cache: Dict[str, Dict[str, Any]]
+    schema_cache: dict[str, dict[str, Any]]
 
     def __init__(self, schema_uri_map: Optional[SchemaUriMap] = None) -> None:
         if not HAS_JSONSCHEMA:
             raise ImportError("Cannot instantiate, requires jsonschema package")
 
         if schema_uri_map is not None:
             self.schema_uri_map = schema_uri_map
         else:
             self.schema_uri_map = DefaultSchemaUriMap()
 
         self.schema_cache = get_local_schema_cache()
 
-    def _get_schema(self, schema_uri: str) -> Dict[str, Any]:
+    def _get_schema(self, schema_uri: str) -> dict[str, Any]:
         if schema_uri not in self.schema_cache:
-            s = json.loads(pystac.StacIO.default().read_text(schema_uri))
+            try:
+                s = json.loads(pystac.StacIO.default().read_text(schema_uri))
+            except Exception as error:
+                raise GetSchemaError(schema_uri, error) from error
             self.schema_cache[schema_uri] = s
             id_field = "$id" if "$id" in s else "id"
             if not s[id_field].startswith("http"):
                 s[id_field] = schema_uri
         return self.schema_cache[schema_uri]
 
     @property
     def registry(self) -> Any:
-        def retrieve(schema_uri: str) -> Resource[Dict[str, Any]]:
+        def retrieve(schema_uri: str) -> Resource[dict[str, Any]]:
             return Resource.from_contents(self._get_schema(schema_uri))
 
         return Registry(retrieve=retrieve).with_resources(  # type: ignore
             [
                 (k, Resource.from_contents(v)) for k, v in self.schema_cache.items()
             ]  # type: ignore
         )
 
-    def get_schema_from_uri(self, schema_uri: str) -> Tuple[Dict[str, Any], Any]:
+    def get_schema_from_uri(self, schema_uri: str) -> tuple[dict[str, Any], Any]:
         """DEPRECATED"""
         warnings.warn(
             "get_schema_from_uri is deprecated and will be removed in v2.",
             DeprecationWarning,
         )
         return self._get_schema(schema_uri), self.registry
 
     def _validate_from_uri(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         schema_uri: str,
         href: Optional[str] = None,
     ) -> None:
         try:
             schema = self._get_schema(schema_uri)
             # This block is cribbed (w/ change in error handling) from
@@ -206,19 +216,21 @@
             if href is not None:
                 msg += f"at {href} "
             if stac_id is not None:
                 msg += f"with ID {stac_id} "
             msg += f"against schema at {schema_uri}"
 
             best = jsonschema.exceptions.best_match(errors)
+            if best:
+                msg += "\n" + str(best)
             raise STACValidationError(msg, source=errors) from best
 
     def validate_core(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         href: Optional[str] = None,
     ) -> Optional[str]:
         """Validate a core stac object.
 
         Return value can be None or specific to the implementation.
@@ -249,15 +261,15 @@
 
         self._validate_from_uri(stac_dict, stac_object_type, schema_uri, href=href)
 
         return schema_uri
 
     def validate_extension(
         self,
-        stac_dict: Dict[str, Any],
+        stac_dict: dict[str, Any],
         stac_object_type: STACObjectType,
         stac_version: str,
         extension_id: str,
         href: Optional[str] = None,
     ) -> Optional[str]:
         """Validate an extension stac object.
```

### Comparing `pystac-1.8.4/pystac/version.py` & `pystac-1.9.0/pystac/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-__version__ = "1.8.4"
+__version__ = "1.9.0"
 """Library version"""
 
 
 class STACVersion:
     DEFAULT_STAC_VERSION = "1.0.0"
     """Latest STAC version supported by PySTAC"""
```

### Comparing `pystac-1.8.4/pystac.egg-info/PKG-INFO` & `pystac-1.9.0/pystac.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/stac-utils/pystac
 Project-URL: Documentation, https://pystac.readthedocs.io
 Project-URL: Repository, https://github.com/stac-utils/pystac.git
@@ -12,34 +12,35 @@
 Project-URL: Discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
 Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: importlib-resources>=5.12.0; python_version < "3.9"
 Requires-Dist: python-dateutil>=2.7.0
 Provides-Extra: bench
 Requires-Dist: asv~=0.6.0; extra == "bench"
 Requires-Dist: packaging~=23.1; extra == "bench"
 Requires-Dist: virtualenv~=20.22; extra == "bench"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.2; extra == "docs"
+Requires-Dist: boto3~=1.28; extra == "docs"
 Requires-Dist: ipython~=8.12; extra == "docs"
 Requires-Dist: jinja2<4.0; extra == "docs"
 Requires-Dist: jupyter~=1.0; extra == "docs"
 Requires-Dist: nbsphinx~=0.9.0; extra == "docs"
 Requires-Dist: pydata-sphinx-theme~=0.13; extra == "docs"
+Requires-Dist: rasterio~=1.3; extra == "docs"
+Requires-Dist: shapely~=2.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
 Requires-Dist: sphinx-design~=0.5.0; extra == "docs"
 Requires-Dist: sphinxcontrib-fulltoc~=1.2; extra == "docs"
 Provides-Extra: jinja2
 Requires-Dist: jinja2<4.0; extra == "jinja2"
 Provides-Extra: orjson
 Requires-Dist: orjson>=3.5; extra == "orjson"
@@ -54,17 +55,19 @@
 Requires-Dist: mypy~=1.2; extra == "test"
 Requires-Dist: orjson~=3.8; extra == "test"
 Requires-Dist: pre-commit~=3.2; extra == "test"
 Requires-Dist: pytest-cov~=4.0; extra == "test"
 Requires-Dist: pytest-mock~=3.10; extra == "test"
 Requires-Dist: pytest-recording~=0.13.0; extra == "test"
 Requires-Dist: pytest~=7.3; extra == "test"
-Requires-Dist: ruff==0.0.291; extra == "test"
+Requires-Dist: requests-mock~=1.11; extra == "test"
+Requires-Dist: ruff==0.1.1; extra == "test"
 Requires-Dist: types-html5lib~=1.1; extra == "test"
 Requires-Dist: types-orjson~=3.6; extra == "test"
+Requires-Dist: types-jsonschema~=4.18; extra == "test"
 Requires-Dist: types-python-dateutil~=2.8; extra == "test"
 Requires-Dist: types-urllib3~=1.26; extra == "test"
 Provides-Extra: urllib3
 Requires-Dist: urllib3>=1.26; extra == "urllib3"
 Provides-Extra: validation
 Requires-Dist: jsonschema~=4.18; extra == "validation"
```

### Comparing `pystac-1.8.4/pystac.egg-info/SOURCES.txt` & `pystac-1.9.0/pystac.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pystac.egg-info/requires.txt
 pystac.egg-info/top_level.txt
 pystac/extensions/__init__.py
 pystac/extensions/base.py
 pystac/extensions/classification.py
 pystac/extensions/datacube.py
 pystac/extensions/eo.py
+pystac/extensions/ext.py
 pystac/extensions/file.py
 pystac/extensions/grid.py
 pystac/extensions/hooks.py
 pystac/extensions/item_assets.py
 pystac/extensions/label.py
 pystac/extensions/mgrs.py
 pystac/extensions/pointcloud.py
```

### Comparing `pystac-1.8.4/pystac.egg-info/requires.txt` & `pystac-1.9.0/pystac.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 python-dateutil>=2.7.0
 
-[:python_version < "3.9"]
-importlib-resources>=5.12.0
-
 [bench]
 asv~=0.6.0
 packaging~=23.1
 virtualenv~=20.22
 
 [docs]
 Sphinx~=6.2
+boto3~=1.28
 ipython~=8.12
 jinja2<4.0
 jupyter~=1.0
 nbsphinx~=0.9.0
 pydata-sphinx-theme~=0.13
+rasterio~=1.3
+shapely~=2.0
 sphinx-autobuild==2021.3.14
 sphinx-design~=0.5.0
 sphinxcontrib-fulltoc~=1.2
 
 [jinja2]
 jinja2<4.0
 
@@ -36,17 +36,19 @@
 mypy~=1.2
 orjson~=3.8
 pre-commit~=3.2
 pytest-cov~=4.0
 pytest-mock~=3.10
 pytest-recording~=0.13.0
 pytest~=7.3
-ruff==0.0.291
+requests-mock~=1.11
+ruff==0.1.1
 types-html5lib~=1.1
 types-orjson~=3.6
+types-jsonschema~=4.18
 types-python-dateutil~=2.8
 types-urllib3~=1.26
 
 [urllib3]
 urllib3>=1.26
 
 [validation]
```

