# Comparing `tmp/dataflows-0.5.4.tar.gz` & `tmp/dataflows-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows-0.5.4.tar", last modified: Fri Mar 22 17:13:35 2024, max compression
+gzip compressed data, was "dataflows-0.5.5.tar", last modified: Mon Apr  1 19:51:52 2024, max compression
```

## Comparing `dataflows-0.5.4.tar` & `dataflows-0.5.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.720297 dataflows-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-22 17:13:29.000000 dataflows-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 17:13:29.000000 dataflows-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-22 17:13:29.000000 dataflows-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-22 17:13:35.720297 dataflows-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-03-22 17:13:29.000000 dataflows-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.708297 dataflows-0.5.4/dataflows/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.712297 dataflows-0.5.4/dataflows/base/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/datastream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/datastream_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/package_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/resource_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/base/schema_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.712297 dataflows-0.5.4/dataflows/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/datapackage_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/extended_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/iterable_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/resource_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/resources_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/row_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/helpers/rows_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.716297 dataflows-0.5.4/dataflows/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/add_computed_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/add_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/delete_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/delete_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.720297 dataflows-0.5.4/dataflows/processors/dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/dumper_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/file_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.720297 dataflows-0.5.4/dataflows/processors/dumpers/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/format_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/format_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/format_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/formats/format_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/to_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/to_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/dumpers/to_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/filter_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/finalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/find_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parallelize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.720297 dataflows-0.5.4/dataflows/processors/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parsers/excel_xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parsers/geojson_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parsers/sql_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/parsers/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/rename_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/select_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/set_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/set_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/sort_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/unpivot.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/unstream.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/update_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/update_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/update_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/processors/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.720297 dataflows-0.5.4/dataflows/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-22 17:13:29.000000 dataflows-0.5.4/dataflows/templates/main.tpl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:13:35.712297 dataflows-0.5.4/dataflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 17:13:35.000000 dataflows-0.5.4/dataflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 17:13:35.720297 dataflows-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-22 17:13:29.000000 dataflows-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.449082 dataflows-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-01 19:51:46.000000 dataflows-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 19:51:46.000000 dataflows-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 19:51:46.000000 dataflows-0.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-01 19:51:52.449082 dataflows-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-01 19:51:46.000000 dataflows-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.437082 dataflows-0.5.5/dataflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.441082 dataflows-0.5.5/dataflows/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/datastream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/package_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/resource_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/base/schema_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.441082 dataflows-0.5.5/dataflows/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/datapackage_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/extended_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/iterable_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/resource_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/resources_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/row_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/helpers/rows_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.445082 dataflows-0.5.5/dataflows/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/add_computed_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/add_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/delete_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/delete_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.445082 dataflows-0.5.5/dataflows/processors/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/dumper_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/file_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.449082 dataflows-0.5.5/dataflows/processors/dumpers/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/format_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/format_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/format_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/formats/format_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/to_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/to_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/dumpers/to_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/filter_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/finalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/find_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parallelize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.449082 dataflows-0.5.5/dataflows/processors/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parsers/excel_xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parsers/geojson_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parsers/sql_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/parsers/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/rename_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/select_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/set_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/set_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/sort_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/unpivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/unstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/update_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/update_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/update_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/processors/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.449082 dataflows-0.5.5/dataflows/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-01 19:51:46.000000 dataflows-0.5.5/dataflows/templates/main.tpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:51:52.441082 dataflows-0.5.5/dataflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 19:51:52.000000 dataflows-0.5.5/dataflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 19:51:52.449082 dataflows-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-01 19:51:46.000000 dataflows-0.5.5/setup.py
```

### Comparing `dataflows-0.5.4/LICENSE` & `dataflows-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/Makefile` & `dataflows-0.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/PKG-INFO` & `dataflows-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows
-Version: 0.5.4
+Version: 0.5.5
 Summary: A nifty data processing framework, based on data packages
 Home-page: https://github.com/datahq/dataflows
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # ![logo](logo-s.png) DataFlows
```

### Comparing `dataflows-0.5.4/README.md` & `dataflows-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/base/datastream_processor.py` & `dataflows-0.5.5/dataflows/base/datastream_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datapackage import Package
 from tableschema.exceptions import CastError, UniqueKeyError
 
 from . import exceptions
 from .datastream import DataStream
 from .resource_wrapper import ResourceWrapper
-from .schema_validator import schema_validator, raise_exception
+from .schema_validator import schema_validator
 
 
 class LazyIterator:
 
     def __init__(self, get_iterator):
         self.get_iterator = get_iterator
 
@@ -92,23 +92,26 @@
                 processor_name=self.__class__.__name__,
                 processor_object=self,
                 processor_position=self.position
             )
             raise error from cause
         raise cause
 
-    def safe_process(self, on_error=None):
+    def safe_process(self, return_results=False, on_error=None):
         results = []
         try:
             ds = self._process()
             for res in ds.res_iter:
-                if on_error is not None:
-                    results.append(list(
-                        schema_validator(res.res, res, on_error=on_error)
-                    ))
+                if return_results:
+                    if on_error is not None:
+                        results.append(list(
+                            schema_validator(res.res, res, on_error=on_error)
+                        ))
+                    else:
+                        results.append(list(res))
                 else:
                     collections.deque(res, maxlen=0)
         except UniqueKeyError as e:
             self.raise_exception(e)
         except CastError as e:
             for err in e.errors:
                 logging.error('%s', err)
@@ -117,11 +120,9 @@
         return ds, results
 
     def process(self):
         ds, _ = self.safe_process()
         return ds.dp, ds.merge_stats()
 
     def results(self, on_error=None):
-        if on_error is None:
-            on_error = raise_exception
-        ds, results = self.safe_process(on_error=on_error)
+        ds, results = self.safe_process(return_results=True, on_error=on_error)
         return results, ds.dp, ds.merge_stats()
```

### Comparing `dataflows-0.5.4/dataflows/base/exceptions.py` & `dataflows-0.5.5/dataflows/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/base/flow.py` & `dataflows-0.5.5/dataflows/base/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from inspect import isfunction, signature
 from collections.abc import Iterable
 
 from .datastream_processor import DataStreamProcessor
+from .schema_validator import raise_exception
 
 
 class Flow:
     def __init__(self, *args):
         self.chain = args
 
-    def results(self, on_error=None):
+    def results(self, on_error=raise_exception):
         return self._chain().results(on_error=on_error)
 
     def process(self):
         return self._chain().process()
 
     def datastream(self, ds=None):
         return self._chain(ds)._process()
```

### Comparing `dataflows-0.5.4/dataflows/base/schema_validator.py` & `dataflows-0.5.5/dataflows/base/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/cli.py` & `dataflows-0.5.5/dataflows/cli.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/helpers/datapackage_processor.py` & `dataflows-0.5.5/dataflows/helpers/datapackage_processor.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/helpers/extended_json.py` & `dataflows-0.5.5/dataflows/helpers/extended_json.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/helpers/iterable_loader.py` & `dataflows-0.5.5/dataflows/helpers/iterable_loader.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/helpers/resource_matcher.py` & `dataflows-0.5.5/dataflows/helpers/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/__init__.py` & `dataflows-0.5.5/dataflows/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/add_computed_field.py` & `dataflows-0.5.5/dataflows/processors/add_computed_field.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/checkpoint.py` & `dataflows-0.5.5/dataflows/processors/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/concatenate.py` & `dataflows-0.5.5/dataflows/processors/concatenate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/deduplicate.py` & `dataflows-0.5.5/dataflows/processors/deduplicate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/delete_fields.py` & `dataflows-0.5.5/dataflows/processors/delete_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/delete_resource.py` & `dataflows-0.5.5/dataflows/processors/delete_resource.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/dumper_base.py` & `dataflows-0.5.5/dataflows/processors/dumpers/dumper_base.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/file_dumper.py` & `dataflows-0.5.5/dataflows/processors/dumpers/file_dumper.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/formats/base.py` & `dataflows-0.5.5/dataflows/processors/dumpers/formats/base.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/formats/format_csv.py` & `dataflows-0.5.5/dataflows/processors/dumpers/formats/format_csv.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/formats/format_excel.py` & `dataflows-0.5.5/dataflows/processors/dumpers/formats/format_excel.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/formats/format_geojson.py` & `dataflows-0.5.5/dataflows/processors/dumpers/formats/format_geojson.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/formats/format_json.py` & `dataflows-0.5.5/dataflows/processors/dumpers/formats/format_json.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/to_path.py` & `dataflows-0.5.5/dataflows/processors/dumpers/to_path.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/to_sql.py` & `dataflows-0.5.5/dataflows/processors/dumpers/to_sql.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/dumpers/to_zip.py` & `dataflows-0.5.5/dataflows/processors/dumpers/to_zip.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/duplicate.py` & `dataflows-0.5.5/dataflows/processors/duplicate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/filter_rows.py` & `dataflows-0.5.5/dataflows/processors/filter_rows.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/finalizer.py` & `dataflows-0.5.5/dataflows/processors/finalizer.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/find_replace.py` & `dataflows-0.5.5/dataflows/processors/find_replace.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/join.py` & `dataflows-0.5.5/dataflows/processors/join.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/load.py` & `dataflows-0.5.5/dataflows/processors/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,18 @@
                                   profile='tabular-data-resource')
                 self.resource_descriptors.append(descriptor)
                 descriptor['name'] = self.name or path
                 if 'encoding' in self.options:
                     descriptor['encoding'] = self.options['encoding']
                 self.options['custom_parsers'] = self.get_custom_parsers(self.options.get('custom_parsers'))
                 self.options.setdefault('ignore_blank_headers', True)
+                if 'headers' not in self.options:
+                    self.options.setdefault('skip_rows', [{'type': 'preset', 'value': 'auto'}])
                 self.options.setdefault('headers', 1)
                 self.options.setdefault('sample_size', 1000)
-                self.options.setdefault('skip_rows', [{'type': 'preset', 'value': 'auto'}])
                 stream: Stream = Stream(self.load_source, **self.options).open()
                 if len(stream.headers) != len(set(stream.headers)):
                     if not self.deduplicate_headers:
                         raise ValueError(
                             'Found duplicate headers.' +
                             'Use the `deduplicate_headers` flag (found headers=%r)' % stream.headers)
                     stream.headers = self.rename_duplicate_headers(stream.headers)
@@ -211,19 +212,24 @@
                 descriptor['format'] = self.options.get('format', stream.format)
                 descriptor['path'] += '.{}'.format(stream.format)
                 self.iterators.append(stream.iter(keyed=True))
         dp.descriptor.setdefault('resources', []).extend(self.resource_descriptors)
         return dp
 
     def stripper(self, iterator):
+        whitespace = set(' \t\n\r')
         for r in iterator:
-            yield dict(
-                (k, v.strip()) if isinstance(v, str) else (k, v)
-                for k, v in r.items()
-            )
+            for k, v in r.items():
+                if v and isinstance(v, str) and (v[-1] in whitespace or v[0] in whitespace):
+                    r[k] = v.strip()
+            yield r
+            # yield dict(
+            #     (k, v.strip()) if isinstance(v, str) else (k, v)
+            #     for k, v in r.items()
+            # )
 
     def limiter(self, iterator):
         count = 0
         for row in iterator:
             yield row
             count += 1
             if count >= self.limit_rows:
```

### Comparing `dataflows-0.5.4/dataflows/processors/parallelize.py` & `dataflows-0.5.5/dataflows/processors/parallelize.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/parsers/excel_xml_parser.py` & `dataflows-0.5.5/dataflows/processors/parsers/excel_xml_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/parsers/geojson_parser.py` & `dataflows-0.5.5/dataflows/processors/parsers/geojson_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/parsers/sql_parser.py` & `dataflows-0.5.5/dataflows/processors/parsers/sql_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/parsers/xml_parser.py` & `dataflows-0.5.5/dataflows/processors/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/printer.py` & `dataflows-0.5.5/dataflows/processors/printer.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/rename_fields.py` & `dataflows-0.5.5/dataflows/processors/rename_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/select_fields.py` & `dataflows-0.5.5/dataflows/processors/select_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/set_primary_key.py` & `dataflows-0.5.5/dataflows/processors/set_primary_key.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/set_type.py` & `dataflows-0.5.5/dataflows/processors/set_type.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/sort_rows.py` & `dataflows-0.5.5/dataflows/processors/sort_rows.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/sources.py` & `dataflows-0.5.5/dataflows/processors/sources.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/stream.py` & `dataflows-0.5.5/dataflows/processors/stream.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/unpivot.py` & `dataflows-0.5.5/dataflows/processors/unpivot.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/unstream.py` & `dataflows-0.5.5/dataflows/processors/unstream.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/update_resource.py` & `dataflows-0.5.5/dataflows/processors/update_resource.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/update_schema.py` & `dataflows-0.5.5/dataflows/processors/update_schema.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/processors/validate.py` & `dataflows-0.5.5/dataflows/processors/validate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows/templates/main.tpl.py` & `dataflows-0.5.5/dataflows/templates/main.tpl.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/dataflows.egg-info/PKG-INFO` & `dataflows-0.5.5/dataflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows
-Version: 0.5.4
+Version: 0.5.5
 Summary: A nifty data processing framework, based on data packages
 Home-page: https://github.com/datahq/dataflows
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # ![logo](logo-s.png) DataFlows
```

### Comparing `dataflows-0.5.4/dataflows.egg-info/SOURCES.txt` & `dataflows-0.5.5/dataflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataflows-0.5.4/setup.py` & `dataflows-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Prepare
 PACKAGE = 'dataflows'
 NAME = PACKAGE.replace('_', '-')
 INSTALL_REQUIRES = [
     'dataflows-tabulator>=1.54.0',
     'datapackage>=1.15.4',
-    'tableschema>=1.20.10',
+    'tableschema>=1.20.11',
     'kvfile>=1.1.1',
     'click',
     'jinja2',
     'awesome-slugify',
     'inquirer',
     'tabulate',
     'tableschema-sql>=2.0.1',
```

