# Comparing `tmp/hidebound-0.9.2.tar.gz` & `tmp/hidebound-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hidebound-0.9.2.tar", last modified: Sat Oct  3 04:49:49 2020, max compression
+gzip compressed data, was "dist/hidebound-0.9.7.tar", last modified: Wed Mar 24 07:45:04 2021, max compression
```

## Comparing `hidebound-0.9.2.tar` & `hidebound-0.9.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/
--rw-r--r--   0 root         (0) root         (0)      115 2020-10-03 04:49:48.000000 hidebound-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    20535 2020-10-03 04:49:49.000000 hidebound-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16538 2020-10-03 04:49:48.000000 hidebound-0.9.2/README.md
--rw-r--r--   0 root         (0) root         (0)      368 2020-10-03 04:49:48.000000 hidebound-0.9.2/dev_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound/core/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5001 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/config.py
--rw-r--r--   0 root         (0) root         (0)    12651 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/database.py
--rw-r--r--   0 root         (0) root         (0)    12939 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/database_tools.py
--rw-r--r--   0 root         (0) root         (0)    11498 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/parser.py
--rw-r--r--   0 root         (0) root         (0)    11621 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/specification_base.py
--rw-r--r--   0 root         (0) root         (0)     3734 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/specifications.py
--rw-r--r--   0 root         (0) root         (0)     4584 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/tools.py
--rw-r--r--   0 root         (0) root         (0)     1900 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/traits.py
--rw-r--r--   0 root         (0) root         (0)    12382 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/core/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound/exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/exporters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3000 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/exporters/exporter_base.py
--rw-r--r--   0 root         (0) root         (0)     7243 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/exporters/girder_exporter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound/server/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11022 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/server/api.py
--rw-r--r--   0 root         (0) root         (0)     8787 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/server/app.py
--rw-r--r--   0 root         (0) root         (0)    16299 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/server/components.py
--rw-r--r--   0 root         (0) root         (0)     5728 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/server/server_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound/templates/
--rw-r--r--   0 root         (0) root         (0)    13867 2020-10-03 04:49:48.000000 hidebound-0.9.2/hidebound/templates/style.css.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20535 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      616 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2020-10-03 04:49:49.000000 hidebound-0.9.2/hidebound.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      241 2020-10-03 04:49:48.000000 hidebound-0.9.2/prod_requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2020-10-03 04:49:49.000000 hidebound-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1587 2020-10-03 04:49:48.000000 hidebound-0.9.2/setup.py
--rw-r--r--   0 root         (0) root         (0)        6 2020-10-03 04:49:48.000000 hidebound-0.9.2/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/
+-rw-r--r--   0 root         (0) root         (0)      115 2021-03-24 07:45:03.000000 hidebound-0.9.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21548 2021-03-24 07:45:04.000000 hidebound-0.9.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17465 2021-03-24 07:45:03.000000 hidebound-0.9.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      368 2021-03-24 07:45:03.000000 hidebound-0.9.7/dev_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5004 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    12844 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/database.py
+-rw-r--r--   0 root         (0) root         (0)    12958 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/database_tools.py
+-rw-r--r--   0 root         (0) root         (0)    11502 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/parser.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/specification_base.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/specifications.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/traits.py
+-rw-r--r--   0 root         (0) root         (0)    12382 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/core/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound/exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/exporters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/exporters/exporter_base.py
+-rw-r--r--   0 root         (0) root         (0)     7341 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/exporters/girder_exporter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/server/api.py
+-rw-r--r--   0 root         (0) root         (0)     8992 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/server/app.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/server/components.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/server/server_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound/templates/
+-rw-r--r--   0 root         (0) root         (0)    13894 2021-03-24 07:45:03.000000 hidebound-0.9.7/hidebound/templates/style.css.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21548 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      628 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-03-24 07:45:04.000000 hidebound-0.9.7/hidebound.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      253 2021-03-24 07:45:03.000000 hidebound-0.9.7/prod_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2021-03-24 07:45:04.000000 hidebound-0.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2021-03-24 07:45:03.000000 hidebound-0.9.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)        6 2021-03-24 07:45:03.000000 hidebound-0.9.7/version.txt
```

### Comparing `hidebound-0.9.2/PKG-INFO` & `hidebound-0.9.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hidebound
-Version: 0.9.2
+Version: 0.9.7
 Summary: A local database service for converting directories of arbitrary files into validated assets and derived JSON metadata.
 Home-page: https://github.com/theNewFlesh/hidebound
 Author: Alex Braun
 Author-email: Alexander.G.Braun@gmail.com
 License: MIT
-Download-URL: https://github.com/theNewFlesh/hidebound/archive/0.9.2.tar.gz
+Download-URL: https://github.com/theNewFlesh/hidebound/archive/0.9.7.tar.gz
 Description: # Introduction
         A local database service for converting directories of arbitrary files into
         validated assets and derived metadata for export to databases like AWS S3 and
         MongoDB.
         
         See [documentation](https://thenewflesh.github.io/hidebound/) for details.
         
@@ -46,14 +46,30 @@
         for consumption by databases like the aforementioned.
         
         Hidebound is framework for validating, and extracting metadata from files and
         directories according, to user defined specifications. Assets are placed into a
         root directory (typically one reserved for Hidebound projects) and then
         discovered, validated, extracted, and copied or moved by Hidebound.
         
+        # Dataflow
+        ![](resources/screenshots/data_flow.png)
+        
+        Data begins as files on disk. Hidebound creates a JSON-compatible dict from
+        their name traits and file traits and then constructs an internal database table
+        from them, one dict per row. All the rows are then aggregated by asset, and
+        converted into a JSON blobs. Those blobs are then validated according to their
+        respective specifications. Files from valid assets are then copied or moved into
+        Hidebound's data directory, according to their same directory structure and
+        naming. Metadata is written to JSON files inside Hidebound's metadata directory.
+        Each file's metadata is written as a JSON file in /hidebound/metadata/file, and
+        each asset's metadata (the aggregate of its file metadata) is written to
+        /hidebound/metadata/asset. From their exporters, can export the valid
+        asset data and its accompanying metadata to various locations, like an AWS S3
+        bucket.
+        
         # Workflow
         The acronynm to remember for workflows is **CRUDES**: create, read, update,
         delete, export and search. Those operations constitue the main functionality
         that Hidebound supports.
         
         ### *Create Asset*
         For example, an asset could be an image sequence, such as a directory full of
@@ -96,17 +112,17 @@
         see in the height and width columns, that it's 1024 by 1024 and the channels
         column says it has three.
         
         ### *Create*
         Next we click the create button. For each valid asset, Hidebound generates file
         and asset metadata as JSON files within the hidebound/metadata directory.
         Hidebound also copies or moves, depending on the config write mode, valid files
-        and directories into the hidebound/data directory. Thus we now have a hidebound
-        directory that looks like this (unmentioned assets are collapsed behind the
-        ellipses):
+        and directories into the hidebound/content directory. Thus we now have a
+        hidebound directory that looks like this (unmentioned assets are collapsed
+        behind the ellipses):
         ```
         /tmp/hidebound
         ├── hidebound_config.json
         │
         ├── specifications
         │   └── specifications.py
         │
@@ -140,22 +156,22 @@
         the "exporters" key. Below we can see the results of an export to Girder in the
         Girder web app.
         
         ![](resources/screenshots/girder.png)
         
         ### *Delete*
         Once this export process is complete, we may click the delete button. Hidebound
-        deletes the hidebound/data and hidebound/metdata directories and all their
+        deletes the hidebound/content and hidebound/metdata directories and all their
         contents. If write_mode in the Hidebound configuration is set to "copy", then
         this step will merely delete data created by Hidebound. If it is set to "move",
         then Hidebound will presumably delete, the only existing copy of out asset data
         on the host machine.
         
         # Naming Convention
-        Hidebound is a highly opionated framework that relies upon a strict but
+        Hidebound is a highly opinionated framework that relies upon a strict but
         composable naming convention in order to extract metadata from filenames. All
         files and directories that are part of assets must conform to a naming
         convention defined within that asset's specification.
         
         In an over-simplified sense; sentences are constructions of words. Syntax
         concerns how each word is formed, grammar concerns how to form words into a
         sentence, and semantics concerns what each word means. Similarly, filenames can
@@ -185,15 +201,16 @@
         | ---------------- | --------------------------------------------------- |
         | Field indicator  | determines metadata key                             |
         | Field token      | a set of 1+ characters that define the field's data |
         
         ---
         ### **Example Diagrams**
         In our example filename:
-        `p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will be:
+        `p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will
+        be:
         ```
         {
             'project': 'cat001',
             'specification': 'spec001',
             'descriptor': 'running-cat',
             'version': 1,
             'coordinate': [0, 5],
@@ -219,15 +236,15 @@
         | Field            | s-spec001                |
         | Field indicator  | s-                       |
         | Field token      | spec001                  |
         | Derived metadata | {specification: spec001} |
         
         ### *Special Field Syntax*
         
-        - Projects begin with 3 or 4 letters followed by 1 or 3 numbers
+        - Projects begin with 3 or 4 letters followed by 1 to 4 numbers
         - Specifications begin with 3 or 4 letters followed by 3 numbers
         - Descriptors begin with a letter or number and may also contain hyphens
         - Descriptors may not begin with the words master, final or last
         - Versions are triple-padded with zeros and must be greater than 0
         - Coordinates may contain up to 3 quadruple-padded numbers, separated by hyphens
         - Coordinates are always evaluated in XYZ order. For example: `c0001-0002-0003`
           produces `{x: 1, y: 2, z: 3}`.
@@ -350,17 +367,17 @@
         
         Its functions are as follows:
         
         * Search - Search the updated database's data via SQL
         * Dropdown - Groups search results by file or asset
         * Init - Initialized the database with the current config
         * Update - Initializes and updates the database with the current config
-        * Create - Copies or moves valid assets to hidebound/data directory and creates
-                   JSON files in hidebound/metadata directory
-        * Delete - Deletes hidebound/data and hidebound/metadata directories
+        * Create - Copies or moves valid assets to hidebound/content directory and
+                   creates JSON files in hidebound/metadata directory
+        * Delete - Deletes hidebound/content and hidebound/metadata directories
         
         Prior to calling update, the application will look like this:
         
         ![](resources/screenshots/pre_update.png)
         
         ### Graph
         The graph tab is used for visualizing the state of all the assets within a root
@@ -406,11 +423,10 @@
         
 Keywords: asset,project,data,json,database,datastore,flask,service
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `hidebound-0.9.2/README.md` & `hidebound-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,30 @@
 for consumption by databases like the aforementioned.
 
 Hidebound is framework for validating, and extracting metadata from files and
 directories according, to user defined specifications. Assets are placed into a
 root directory (typically one reserved for Hidebound projects) and then
 discovered, validated, extracted, and copied or moved by Hidebound.
 
+# Dataflow
+![](resources/screenshots/data_flow.png)
+
+Data begins as files on disk. Hidebound creates a JSON-compatible dict from
+their name traits and file traits and then constructs an internal database table
+from them, one dict per row. All the rows are then aggregated by asset, and
+converted into a JSON blobs. Those blobs are then validated according to their
+respective specifications. Files from valid assets are then copied or moved into
+Hidebound's data directory, according to their same directory structure and
+naming. Metadata is written to JSON files inside Hidebound's metadata directory.
+Each file's metadata is written as a JSON file in /hidebound/metadata/file, and
+each asset's metadata (the aggregate of its file metadata) is written to
+/hidebound/metadata/asset. From their exporters, can export the valid
+asset data and its accompanying metadata to various locations, like an AWS S3
+bucket.
+
 # Workflow
 The acronynm to remember for workflows is **CRUDES**: create, read, update,
 delete, export and search. Those operations constitue the main functionality
 that Hidebound supports.
 
 ### *Create Asset*
 For example, an asset could be an image sequence, such as a directory full of
@@ -87,17 +103,17 @@
 see in the height and width columns, that it's 1024 by 1024 and the channels
 column says it has three.
 
 ### *Create*
 Next we click the create button. For each valid asset, Hidebound generates file
 and asset metadata as JSON files within the hidebound/metadata directory.
 Hidebound also copies or moves, depending on the config write mode, valid files
-and directories into the hidebound/data directory. Thus we now have a hidebound
-directory that looks like this (unmentioned assets are collapsed behind the
-ellipses):
+and directories into the hidebound/content directory. Thus we now have a
+hidebound directory that looks like this (unmentioned assets are collapsed
+behind the ellipses):
 ```
 /tmp/hidebound
 ├── hidebound_config.json
 │
 ├── specifications
 │   └── specifications.py
 │
@@ -131,22 +147,22 @@
 the "exporters" key. Below we can see the results of an export to Girder in the
 Girder web app.
 
 ![](resources/screenshots/girder.png)
 
 ### *Delete*
 Once this export process is complete, we may click the delete button. Hidebound
-deletes the hidebound/data and hidebound/metdata directories and all their
+deletes the hidebound/content and hidebound/metdata directories and all their
 contents. If write_mode in the Hidebound configuration is set to "copy", then
 this step will merely delete data created by Hidebound. If it is set to "move",
 then Hidebound will presumably delete, the only existing copy of out asset data
 on the host machine.
 
 # Naming Convention
-Hidebound is a highly opionated framework that relies upon a strict but
+Hidebound is a highly opinionated framework that relies upon a strict but
 composable naming convention in order to extract metadata from filenames. All
 files and directories that are part of assets must conform to a naming
 convention defined within that asset's specification.
 
 In an over-simplified sense; sentences are constructions of words. Syntax
 concerns how each word is formed, grammar concerns how to form words into a
 sentence, and semantics concerns what each word means. Similarly, filenames can
@@ -176,15 +192,16 @@
 | ---------------- | --------------------------------------------------- |
 | Field indicator  | determines metadata key                             |
 | Field token      | a set of 1+ characters that define the field's data |
 
 ---
 ### **Example Diagrams**
 In our example filename:
-`p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will be:
+`p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will
+be:
 ```
 {
     'project': 'cat001',
     'specification': 'spec001',
     'descriptor': 'running-cat',
     'version': 1,
     'coordinate': [0, 5],
@@ -210,15 +227,15 @@
 | Field            | s-spec001                |
 | Field indicator  | s-                       |
 | Field token      | spec001                  |
 | Derived metadata | {specification: spec001} |
 
 ### *Special Field Syntax*
 
-- Projects begin with 3 or 4 letters followed by 1 or 3 numbers
+- Projects begin with 3 or 4 letters followed by 1 to 4 numbers
 - Specifications begin with 3 or 4 letters followed by 3 numbers
 - Descriptors begin with a letter or number and may also contain hyphens
 - Descriptors may not begin with the words master, final or last
 - Versions are triple-padded with zeros and must be greater than 0
 - Coordinates may contain up to 3 quadruple-padded numbers, separated by hyphens
 - Coordinates are always evaluated in XYZ order. For example: `c0001-0002-0003`
   produces `{x: 1, y: 2, z: 3}`.
@@ -341,17 +358,17 @@
 
 Its functions are as follows:
 
 * Search - Search the updated database's data via SQL
 * Dropdown - Groups search results by file or asset
 * Init - Initialized the database with the current config
 * Update - Initializes and updates the database with the current config
-* Create - Copies or moves valid assets to hidebound/data directory and creates
-           JSON files in hidebound/metadata directory
-* Delete - Deletes hidebound/data and hidebound/metadata directories
+* Create - Copies or moves valid assets to hidebound/content directory and
+           creates JSON files in hidebound/metadata directory
+* Delete - Deletes hidebound/content and hidebound/metadata directories
 
 Prior to calling update, the application will look like this:
 
 ![](resources/screenshots/pre_update.png)
 
 ### Graph
 The graph tab is used for visualizing the state of all the assets within a root
```

### Comparing `hidebound-0.9.2/hidebound/core/config.py` & `hidebound-0.9.7/hidebound/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         specification_files (list[str], optional): List of asset specification
             files. Default: [].
         include_regex (str, optional): Include filenames that match this regex.
             Default: ''.
         exclude_regex (str, optional): Exclude filenames that match this regex.
             Default: '\.DS_Store'.
         write_mode (str, optional): How assets will be extracted to
-            hidebound/data directory. Default: copy.
+            hidebound/content directory. Default: copy.
         exporters (dict, optional): Dictionary of exporter configs, where the
             key is the exporter name and the value is its config. Default: {}.
     '''
     root_directory = StringType(
         required=True, validators=[vd.is_directory]
     )  # type: StringType
     hidebound_directory = StringType(
```

### Comparing `hidebound-0.9.2/hidebound/core/database.py` & `hidebound-0.9.7/hidebound/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from pathlib import Path
 import json
 import os
 import shutil
 import sys
 
 from pandas import DataFrame
-import pandasql
+import jsoncomment as jsonc
 import numpy as np
+import pandasql
 
 from hidebound.core.config import Config
 from hidebound.core.specification_base import SpecificationBase
 from hidebound.exporters.girder_exporter import GirderExporter
 import hidebound.core.database_tools as db_tools
 import hidebound.core.tools as tools
 # ------------------------------------------------------------------------------
@@ -78,15 +79,15 @@
         Args:
             filepath (str or Path): Filepath of json config file.
 
         Returns:
             Database: Database instance.
         '''
         with open(filepath) as f:
-            config = json.load(f)
+            config = jsonc.JsonComment().load(f)
         return Database.from_config(config)
 
     def __init__(
         self,
         root_dir,
         hidebound_dir,
         specifications=[],
@@ -106,15 +107,15 @@
             specifications (list[SpecificationBase], optional): List of asset
                 specifications. Default: [].
             include_regex (str, optional): Include filenames that match this
                 regex. Default: None.
             exclude_regex (str, optional): Exclude filenames that match this
                 regex. Default: '\.DS_Store'.
             write_mode (str, optional): How assets will be extracted to
-                hidebound/data directory. Default: copy.
+                hidebound/content directory. Default: copy.
             exporters (dict, optional): Dictionary of exporter configs, where
                 the key is the exporter name and the value is its config.
                 Default: {}.
 
         Raises:
             TypeError: If specifications contains a non-SpecificationBase
                 object.
@@ -174,15 +175,16 @@
         # type: () -> "Database"
         '''
         Extract valid assets as data and metadata within the hidebound
         directory.
 
         Writes:
 
-            * file data to hb_parent/hidebound/data - under same directory structure
+            * file content to hb_parent/hidebound/content - under same directory
+                                                            structure
             * file metadata as json to hb_parent/hidebound/metadata/file
             * asset metadata as json to hb_parent/hidebound/metadata/asset
 
         Raises:
             RunTimeError: If data has not been initialized.
 
         Returns:
@@ -266,17 +268,20 @@
 
             mask = traits[col].notnull()
             data.loc[mask, col] = traits.loc[mask, col]
 
         # find columns by legal type
         cols = self.data.columns.tolist()
         if len(self.data) > 0:
-            cols = data.applymap(type).apply(lambda x: set(x.unique()))
+            cols = data \
+                .applymap(type) \
+                .apply(lambda x: [x.unique().tolist()]) \
+                .loc[0]
             legal_cols = set([int, float, str, bool, None])
-            mask = cols.apply(lambda x: x.difference(legal_cols) == set())
+            mask = cols.apply(lambda x: set(x).difference(legal_cols) == set())
             cols = cols[mask].index.tolist()
 
         # nicely order columns
         head_cols = [
             'project',
             'specification',
             'descriptor',
@@ -331,21 +336,21 @@
         data = db_tools._cleanup(data)
         self.data = data
         return self
 
     def delete(self):
         # type: () -> "Database"
         '''
-        Deletes hidebound/data and hidebound/metadata directories and all their
+        Deletes hidebound/content and hidebound/metadata directories and all their
         contents.
 
         Returns:
             Database: self.
         '''
-        data_dir = Path(self._hb_root, 'data')
+        data_dir = Path(self._hb_root, 'content')
         if data_dir.exists():
             shutil.rmtree(data_dir)
 
         meta_dir = Path(self._hb_root, 'metadata')
         if meta_dir.exists():
             shutil.rmtree(meta_dir)
```

### Comparing `hidebound-0.9.2/hidebound/core/database_tools.py` & `hidebound-0.9.7/hidebound/core/database_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,22 +330,22 @@
     data = data[data.asset_valid]
 
     # return if there is no valid asset data
     if len(data) == 0:
         return None
 
     source_dir = Path(source_dir).absolute().as_posix()
-    data_dir = Path(target_dir, 'data').absolute().as_posix()
+    data_dir = Path(target_dir, 'content').absolute().as_posix()
     meta_dir = Path(target_dir, 'metadata').absolute().as_posix()
 
     # add asset id
     keys = data.asset_path.unique().tolist()
     vals = [str(uuid.uuid4()) for x in keys]
     lut = dict(zip(keys, vals))
-    lut = defaultdict(lambda: np.nan, lut)
+    lut = defaultdict(lambda: np.nan, lut)  # type: ignore
     data['asset_id'] = data.asset_path.apply(lambda x: lut[x])
 
     # create file id and metadata
     data['file_id'] = data.asset_name.apply(lambda x: str(uuid.uuid4()))
     data['metadata'] = data.apply(
         lambda x: dict(
             asset_id=x.asset_id,
```

### Comparing `hidebound-0.9.2/hidebound/core/parser.py` & `hidebound-0.9.7/hidebound/core/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         # type: () -> Dict[str, Any]
         '''
         Create parser grammar dictionary.
 
         Returns:
             dict: Grammar.
         '''
-        project = Regex(r'[a-z]{3,4}\d{1,3}')\
+        project = Regex(r'[a-z]{3,4}\d\d?\d?\d?')\
             .setResultsName('project')\
             .setFailAction(AssetNameParser._raise_field_error('project', 'token'))
 
         specification = Regex(r'[a-z]{3,4}\d\d\d')\
             .setResultsName('specification')\
             .setFailAction(AssetNameParser._raise_field_error('specification', 'token'))
```

### Comparing `hidebound-0.9.2/hidebound/core/specification_base.py` & `hidebound-0.9.7/hidebound/core/specification_base.py`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound/core/specifications.py` & `hidebound-0.9.7/hidebound/core/specifications.py`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound/core/tools.py` & `hidebound-0.9.7/hidebound/core/tools.py`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound/core/traits.py` & `hidebound-0.9.7/hidebound/core/traits.py`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound/core/validators.py` & `hidebound-0.9.7/hidebound/core/validators.py`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound/exporters/exporter_base.py` & `hidebound-0.9.7/hidebound/exporters/exporter_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Union
 
 from pathlib import Path
-import json
 import os
+
+import jsoncomment as jsonc
 # ------------------------------------------------------------------------------
 
 
 class ExporterBase:
     '''
     Abstract base class for hidebound exporters.
     '''
@@ -21,15 +22,15 @@
 
         Args:
             hidebound_dir (Path or str): Hidebound directory.
 
         Raises:
             FileNotFoundError: If any of the directories have not been found.
         '''
-        data = Path(hidebound_dir, 'data')
+        data = Path(hidebound_dir, 'content')
         meta = Path(hidebound_dir, 'metadata')
         asset_dir = Path(meta, 'asset')
         file_dir = Path(meta, 'file')
         for path in [data, meta, asset_dir, file_dir]:
             if not path.is_dir():
                 msg = f'{path.as_posix()} directory does not exist.'
                 raise FileNotFoundError(msg)
@@ -47,24 +48,24 @@
         asset_dir = Path(hidebound_dir, 'metadata', 'asset')
         file_dir = Path(hidebound_dir, 'metadata', 'file')
         for asset in os.listdir(asset_dir):  # type: Union[str, Path]
 
             # export asset
             asset = Path(asset_dir, asset)
             with open(asset) as f:
-                asset_meta = json.load(f)
+                asset_meta = jsonc.JsonComment().load(f)
             self._export_asset(asset_meta)
 
             # export files
             filepaths = asset_meta['file_ids']
             filepaths = [Path(file_dir, f'{x}.json') for x in filepaths]
             for filepath in filepaths:
                 filepath = Path(file_dir, filepath)
                 with open(filepath) as f:
-                    file_meta = json.load(f)
+                    file_meta = jsonc.JsonComment().load(f)
                 self._export_file(file_meta)
 
     def _export_asset(self, metadata):
         # type: (Dict) -> None
         '''
         Exports metadata from single JSON file in hidebound/metadata/asset.
```

### Comparing `hidebound-0.9.2/hidebound/exporters/girder_exporter.py` & `hidebound-0.9.7/hidebound/exporters/girder_exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, Union
 
 from pathlib import Path
 
 from girder_client import HttpError
 from schematics import Model
-from schematics.types import IntType, StringType, IPv4Type
+from schematics.types import IntType, StringType, URLType
 import girder_client
 
 from hidebound.exporters.exporter_base import ExporterBase
 import hidebound.core.validators as vd
 # ------------------------------------------------------------------------------
 
 
@@ -18,25 +18,25 @@
 
     Attributes:
         api_key (str): Girder API key.
         root_id (str): ID of folder or collection under which all data will
             be exported.
         root_type (str, optional): Root entity type. Default: collection.
             Options: folder, collection
-        host (str, optional): Docker host IP address. Default: 0.0.0.0.
+        host (str, optional): Docker host URL address. Default: http://0.0.0.0
         port (int, optional): Docker host port. Default: 8080.
     '''
     api_key = StringType(required=True)  # type: StringType
     root_id = StringType(required=True)  # type: StringType
     root_type = StringType(
         required=True,
         default='collection',
         validators=[lambda x: vd.is_in([x], ['collection', 'folder'])]
     )  # type: StringType
-    host = IPv4Type(required=True, default='0.0.0.0')  # type: IPv4Type
+    host = URLType(required=True, default='http://0.0.0.0')  # type: URLType
     port = IntType(
         required=True,
         default=8080,
         validators=[
             lambda x: vd.is_lt(x, 65536),
             lambda x: vd.is_gt(x, 1023),
         ]
@@ -67,29 +67,30 @@
         return GirderExporter(client=client, **config)
 
     def __init__(
         self,
         api_key,
         root_id,
         root_type='collection',
-        host='0.0.0.0',
+        host='http://0.0.0.0',
         port=8080,
         client=None,
     ):
         # type: (str, str, str, str, int, Any) -> None
         '''
         Constructs a GirderExporter instances and creates a Girder client.
 
         Args:
             api_key (str): Girder API key.
             root_id (str): ID of folder or collection under which all data will
                 be exported.
             root_type (str, optional): Root entity type. Default: collection.
                 Options: folder, collection
-            host (str, optional): Docker host IP address. Default: 0.0.0.0.
+            host (str, optional): Docker host URL address.
+                Default: http://0.0.0.0.
             port (int, optional): Docker host port. Default: 8080.
             client (object, optional): Client instance, for testing.
                 Default: None.
 
         Raises:
             DataError: If config is invalid.
         '''
@@ -99,17 +100,19 @@
         config = dict(
             api_key=api_key,
             root_id=root_id,
             root_type=root_type,
             host=host,
             port=port,
         )
-        GirderConfig(config).validate()
+        config = GirderConfig(config)
+        config.validate()
+        config = config.to_primitive()
 
-        self._url = f'http://{host}:{port}/api/v1'  # type: str
+        self._url = f'{host}:{port}/api/v1'  # type: str
 
         if client is None:
             client = girder_client.GirderClient(apiUrl=self._url)  # pragma: no cover
             client.authenticate(apiKey=api_key)  # pragma: no cover
         self._client = client  # type: Any
 
         self._root_id = root_id  # type: str
```

### Comparing `hidebound-0.9.2/hidebound/server/api.py` & `hidebound-0.9.7/hidebound/server/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             description='Exclude filenames that match this regex.',
             required=False,
             default=r'\.DS_Store',
         ),
         dict(
             name='write_mode',
             type='string',
-            description='How assets will be extracted to hidebound/data directory.',
+            description='How assets will be extracted to hidebound/content directory.',
             required=False,
             default='copy',
             enum=['copy', 'move'],
         )
     ],
     responses={
         200: dict(
```

### Comparing `hidebound-0.9.2/hidebound/server/app.py` & `hidebound-0.9.7/hidebound/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 '''
 Hidebound service used for displaying and interacting with Hidebound database.
 '''
 
 
-APP = flask.Flask(__name__)  # type: Union[flask.Flask, dash.Dash]
+APP = flask.Flask('hidebound')  # type: Union[flask.Flask, dash.Dash]
 swg.Swagger(APP)
 APP.register_blueprint(api.API)
 APP = components.get_dash_app(APP)
 CONFIG_PATH = None  # type: Union[str, Path, None]
 
 
 @APP.server.route('/static/<stylesheet>')
@@ -101,19 +101,23 @@
     if inputs_['dropdown'] == 'asset':
         grp = True
     inputs_['dropdown'] = grp
 
     input_id = context.triggered[0]['prop_id'].split('.')[0]
 
     if input_id == 'init-button':
-        APP.server.test_client().post('/api/initialize', json=conf)
+        response = APP.server.test_client().post('/api/initialize', json=conf).json
+        if 'error' in response.keys():
+            store['/api/read'] = response
 
     elif input_id == 'update-button':
         if api.DATABASE is None:
-            APP.server.test_client().post('/api/initialize', json=conf)
+            response = APP.server.test_client().post('/api/initialize', json=conf).json
+            if 'error' in response.keys():
+                store['/api/read'] = response
 
         APP.server.test_client().post('/api/update')
 
         params = json.dumps({'group_by_asset': grp})
         response = APP.server.test_client().post('/api/read', json=params).json
         store['/api/read'] = response
```

### Comparing `hidebound-0.9.2/hidebound/server/components.py` & `hidebound-0.9.7/hidebound/server/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     store = dcc.Store(id='store', storage_type=storage_type)
 
     tab_style = {
         'padding': '4px',
         'background': COLOR_SCHEME['bg'],
         'color': COLOR_SCHEME['light1'],
         'border': '0px',
-        'min-width': '200px',
     }
     tab_selected_style = {
         'padding': '4px',
         'background': COLOR_SCHEME['grey1'],
         'color': COLOR_SCHEME['cyan2'],
         'border': '0px',
     }
@@ -132,17 +131,18 @@
                 selected_style=tab_selected_style,
             )
         ],
     )
     content = html.Div(id='content', className='content')
 
     app = dash.Dash(
-        __name__,
+        name='hidebound',
+        title='Hidebound',
         server=server,
-        external_stylesheets=['http://0.0.0.0:5000/static/style.css'],
+        external_stylesheets=['/static/style.css'],
     )
     app.layout = html.Div(id='layout', children=[store, tabs, content])
     app.config['suppress_callback_exceptions'] = True
 
     return app
 
 
@@ -259,15 +259,15 @@
         html.Div(className='dummy', id='write-button', n_clicks=None),
     ]
 
 
 def get_configbar(config):
     # type: (Dict) -> html.Div
     '''
-    Get a row of elements used for configuring hidebound.core.
+    Get a row of elements used for configuring Hidebound.
 
     Args:
         config (dict): Configuration to be displayed.
 
     Returns:
         Div: Div with buttons and JSON editor.
     '''
```

### Comparing `hidebound-0.9.2/hidebound/server/server_tools.py` & `hidebound-0.9.7/hidebound/server/server_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Any, Dict, Tuple, Union
 
 from pathlib import Path
+from pprint import pformat
 import base64
 import json
 import os
 import traceback
 
 import flask
 import jinja2
+import jsoncomment as jsonc
 import lunchbox.tools as lbt
 # ------------------------------------------------------------------------------
 
 
 def render_template(filename, parameters):
     # type: (str, Dict[str, Any]) -> bytes
     '''
@@ -71,15 +73,22 @@
 
     Args:
         error (Exception): Error to be formatted.
 
     Returns:
         flask.Response: Flask response.
     '''
-    args = ['    ' + str(x) for x in error.args]  # type: Any
+    args = []  # type: Any
+    for arg in error.args:
+        if hasattr(arg, 'items'):
+            for key, val in arg.items():
+                args.append(pformat({key: pformat(val)}))
+        else:
+            args.append(str(arg))
+    args = ['    ' + x for x in args]
     args = '\n'.join(args)
     klass = error.__class__.__name__
     msg = f'{klass}(\n{args}\n)'
     return flask.Response(
         response=json.dumps(dict(
             error=error.__class__.__name__,
             args=list(map(str, error.args)),
@@ -119,15 +128,15 @@
         'specification_files': [],
         'include_regex': '',
         'exclude_regex': r'\.DS_Store',
         'write_mode': 'copy'
     }
     if config_path is not None:
         with open(config_path) as f:
-            config = json.load(f)
+            config = jsonc.JsonComment().load(f)
 
     config_path = Path(root, 'hidebound', 'hidebound_config.json')
     if not config_path.is_file():
         with open(config_path, 'w') as f:
             json.dump(config, f, indent=4, sort_keys=True)
 
     return config, config_path.as_posix()
```

### Comparing `hidebound-0.9.2/hidebound/templates/style.css.j2` & `hidebound-0.9.7/hidebound/templates/style.css.j2`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     margin: 0px;
     padding: 0px;
 }
 
 /* Logo */
 #tabs #logo,
 #tabs #logo .tab:hover {
-    width: 130px;
+    width: 150px;
     background: linear-gradient(
         100deg,
         {{ COLOR_SCHEME['bg'] }} 45%,
         {{ COLOR_SCHEME['cyan2'] }} 45%
     ) !important;
     border: 0px !important;
     font-size: large !important;
@@ -251,14 +251,15 @@
 .key-value-card-value {
     color: {{ COLOR_SCHEME['cyan2'] }};
     padding-left: 10px;
     padding-right: 10px;
     padding-top: 2px;
     flex-grow: 1000;
     word-wrap: break-word;
+    white-space: pre-wrap;
 }
 
 /* Error Card */
 #error .key-value-card-row {
     border-color: {{ COLOR_SCHEME['red2'] }};
 }
```

### Comparing `hidebound-0.9.2/hidebound.egg-info/PKG-INFO` & `hidebound-0.9.7/hidebound.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hidebound
-Version: 0.9.2
+Version: 0.9.7
 Summary: A local database service for converting directories of arbitrary files into validated assets and derived JSON metadata.
 Home-page: https://github.com/theNewFlesh/hidebound
 Author: Alex Braun
 Author-email: Alexander.G.Braun@gmail.com
 License: MIT
-Download-URL: https://github.com/theNewFlesh/hidebound/archive/0.9.2.tar.gz
+Download-URL: https://github.com/theNewFlesh/hidebound/archive/0.9.7.tar.gz
 Description: # Introduction
         A local database service for converting directories of arbitrary files into
         validated assets and derived metadata for export to databases like AWS S3 and
         MongoDB.
         
         See [documentation](https://thenewflesh.github.io/hidebound/) for details.
         
@@ -46,14 +46,30 @@
         for consumption by databases like the aforementioned.
         
         Hidebound is framework for validating, and extracting metadata from files and
         directories according, to user defined specifications. Assets are placed into a
         root directory (typically one reserved for Hidebound projects) and then
         discovered, validated, extracted, and copied or moved by Hidebound.
         
+        # Dataflow
+        ![](resources/screenshots/data_flow.png)
+        
+        Data begins as files on disk. Hidebound creates a JSON-compatible dict from
+        their name traits and file traits and then constructs an internal database table
+        from them, one dict per row. All the rows are then aggregated by asset, and
+        converted into a JSON blobs. Those blobs are then validated according to their
+        respective specifications. Files from valid assets are then copied or moved into
+        Hidebound's data directory, according to their same directory structure and
+        naming. Metadata is written to JSON files inside Hidebound's metadata directory.
+        Each file's metadata is written as a JSON file in /hidebound/metadata/file, and
+        each asset's metadata (the aggregate of its file metadata) is written to
+        /hidebound/metadata/asset. From their exporters, can export the valid
+        asset data and its accompanying metadata to various locations, like an AWS S3
+        bucket.
+        
         # Workflow
         The acronynm to remember for workflows is **CRUDES**: create, read, update,
         delete, export and search. Those operations constitue the main functionality
         that Hidebound supports.
         
         ### *Create Asset*
         For example, an asset could be an image sequence, such as a directory full of
@@ -96,17 +112,17 @@
         see in the height and width columns, that it's 1024 by 1024 and the channels
         column says it has three.
         
         ### *Create*
         Next we click the create button. For each valid asset, Hidebound generates file
         and asset metadata as JSON files within the hidebound/metadata directory.
         Hidebound also copies or moves, depending on the config write mode, valid files
-        and directories into the hidebound/data directory. Thus we now have a hidebound
-        directory that looks like this (unmentioned assets are collapsed behind the
-        ellipses):
+        and directories into the hidebound/content directory. Thus we now have a
+        hidebound directory that looks like this (unmentioned assets are collapsed
+        behind the ellipses):
         ```
         /tmp/hidebound
         ├── hidebound_config.json
         │
         ├── specifications
         │   └── specifications.py
         │
@@ -140,22 +156,22 @@
         the "exporters" key. Below we can see the results of an export to Girder in the
         Girder web app.
         
         ![](resources/screenshots/girder.png)
         
         ### *Delete*
         Once this export process is complete, we may click the delete button. Hidebound
-        deletes the hidebound/data and hidebound/metdata directories and all their
+        deletes the hidebound/content and hidebound/metdata directories and all their
         contents. If write_mode in the Hidebound configuration is set to "copy", then
         this step will merely delete data created by Hidebound. If it is set to "move",
         then Hidebound will presumably delete, the only existing copy of out asset data
         on the host machine.
         
         # Naming Convention
-        Hidebound is a highly opionated framework that relies upon a strict but
+        Hidebound is a highly opinionated framework that relies upon a strict but
         composable naming convention in order to extract metadata from filenames. All
         files and directories that are part of assets must conform to a naming
         convention defined within that asset's specification.
         
         In an over-simplified sense; sentences are constructions of words. Syntax
         concerns how each word is formed, grammar concerns how to form words into a
         sentence, and semantics concerns what each word means. Similarly, filenames can
@@ -185,15 +201,16 @@
         | ---------------- | --------------------------------------------------- |
         | Field indicator  | determines metadata key                             |
         | Field token      | a set of 1+ characters that define the field's data |
         
         ---
         ### **Example Diagrams**
         In our example filename:
-        `p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will be:
+        `p-cat001_s-spec001_d-running-cat_v001_c0000-0005_f0003.png` the metadata will
+        be:
         ```
         {
             'project': 'cat001',
             'specification': 'spec001',
             'descriptor': 'running-cat',
             'version': 1,
             'coordinate': [0, 5],
@@ -219,15 +236,15 @@
         | Field            | s-spec001                |
         | Field indicator  | s-                       |
         | Field token      | spec001                  |
         | Derived metadata | {specification: spec001} |
         
         ### *Special Field Syntax*
         
-        - Projects begin with 3 or 4 letters followed by 1 or 3 numbers
+        - Projects begin with 3 or 4 letters followed by 1 to 4 numbers
         - Specifications begin with 3 or 4 letters followed by 3 numbers
         - Descriptors begin with a letter or number and may also contain hyphens
         - Descriptors may not begin with the words master, final or last
         - Versions are triple-padded with zeros and must be greater than 0
         - Coordinates may contain up to 3 quadruple-padded numbers, separated by hyphens
         - Coordinates are always evaluated in XYZ order. For example: `c0001-0002-0003`
           produces `{x: 1, y: 2, z: 3}`.
@@ -350,17 +367,17 @@
         
         Its functions are as follows:
         
         * Search - Search the updated database's data via SQL
         * Dropdown - Groups search results by file or asset
         * Init - Initialized the database with the current config
         * Update - Initializes and updates the database with the current config
-        * Create - Copies or moves valid assets to hidebound/data directory and creates
-                   JSON files in hidebound/metadata directory
-        * Delete - Deletes hidebound/data and hidebound/metadata directories
+        * Create - Copies or moves valid assets to hidebound/content directory and
+                   creates JSON files in hidebound/metadata directory
+        * Delete - Deletes hidebound/content and hidebound/metadata directories
         
         Prior to calling update, the application will look like this:
         
         ![](resources/screenshots/pre_update.png)
         
         ### Graph
         The graph tab is used for visualizing the state of all the assets within a root
@@ -406,11 +423,10 @@
         
 Keywords: asset,project,data,json,database,datastore,flask,service
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `hidebound-0.9.2/hidebound.egg-info/SOURCES.txt` & `hidebound-0.9.7/hidebound.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidebound-0.9.2/hidebound.egg-info/requires.txt` & `hidebound-0.9.7/hidebound.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dash-html-components
 dash-table
 flasgger
 flask
 girder-client
 humanfriendly
 jinja2
+jsoncomment
 lunchbox
 marshmallow
 numpy
 OpenEXR
 pandas
 pandasql
 pyparsing
```

### Comparing `hidebound-0.9.2/setup.py` & `hidebound-0.9.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,13 @@
     ],
     install_requires=PROD_REQUIREMENTS,
     classifiers=[
       'Development Status :: 4 - Beta',
       'Intended Audience :: Developers',
       'License :: OSI Approved :: MIT License',
       'Programming Language :: Python :: 3',
-      'Programming Language :: Python :: 3.6',
       'Programming Language :: Python :: 3.7',
     ],
     extras_require={
         "dev": DEV_REQUIREMENTS
     },
 )
```

