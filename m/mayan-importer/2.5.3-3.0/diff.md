# Comparing `tmp/mayan-importer-2.5.3.tar.gz` & `tmp/mayan-importer-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-2.5.3.tar", last modified: Thu Feb 22 23:55:24 2024, max compression
+gzip compressed data, was "mayan-importer-3.0.tar", last modified: Mon Apr  1 10:02:43 2024, max compression
```

## Comparing `mayan-importer-2.5.3.tar` & `mayan-importer-3.0.tar`

### file list

```diff
@@ -1,78 +1,73 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5855 2024-02-22 17:57:51.000000 mayan-importer-2.5.3/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/MANIFEST.in
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8716 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.395018 mayan-importer-2.5.3/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      835 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4601 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8633 2024-02-13 00:40:50.000000 mayan-importer-2.5.3/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    10581 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      237 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1563 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      214 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/exceptions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4144 2024-02-22 17:47:30.000000 mayan-importer-2.5.3/importer/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1973 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4374 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/import_setup_actions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7776 2024-02-20 15:50:11.000000 mayan-importer-2.5.3/importer/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6328 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      737 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.395018 mayan-importer-2.5.3/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.395018 mayan-importer-2.5.3/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      141 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2400 2023-06-12 09:35:45.000000 mayan-importer-2.5.3/importer/models/import_setup_action_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6490 2024-02-22 17:45:24.000000 mayan-importer-2.5.3/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8841 2024-02-22 17:56:46.000000 mayan-importer-2.5.3/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1997 2024-02-22 23:54:22.000000 mayan-importer-2.5.3/importer/models/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1114 2020-10-02 10:42:37.000000 mayan-importer-2.5.3/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1141 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3471 2024-02-15 20:51:27.000000 mayan-importer-2.5.3/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2295 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.395018 mayan-importer-2.5.3/importer/templatetags/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/templatetags/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2966 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/templatetags/templating_tags.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       64 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      270 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/import_setup_actions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1553 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      643 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    11061 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7199 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/test_import_setup_action_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7870 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12228 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6415 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6686 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-2.5.3/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6683 2024-02-22 17:51:03.000000 mayan-importer-2.5.3/importer/views/import_setup_action_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16162 2024-02-22 17:53:06.000000 mayan-importer-2.5.3/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6223 2024-02-22 17:54:21.000000 mayan-importer-2.5.3/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/mayan_importer.egg-info/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8716 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2268 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-02-22 23:55:24.000000 mayan-importer-2.5.3/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-02-22 23:55:24.399018 mayan-importer-2.5.3/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-02-22 23:54:42.000000 mayan-importer-2.5.3/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.330866 mayan-importer-3.0/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9231 2024-04-01 10:02:43.330866 mayan-importer-3.0/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.324866 mayan-importer-3.0/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7228 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/exceptions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.327866 mayan-importer-3.0/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.328866 mayan-importer-3.0/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.329866 mayan-importer-3.0/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.329866 mayan-importer-3.0/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.330866 mayan-importer-3.0/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9231 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2148 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-01 10:02:43.331866 mayan-importer-3.0/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-04-01 10:00:07.000000 mayan-importer-3.0/setup.py
```

### Comparing `mayan-importer-2.5.3/HISTORY.rst` & `mayan-importer-3.0/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+3.0 (2024-04-01)
+================
+- Refactor app.
+- Remove import setup action.
+- Use source metadata to store import metadata.
+- Don't deserialize import item source column.
+- Use upstream backend, dynamic forms, credentials mixins, model mixins,
+  error log.
+- Use fieldsets.
+- Bring code standards up to series 4.5.
+- Support processing and deleting individual setup item entries.
+- Improve import setup and import setup item state handling.
+- Improve navigation, add return links.
+
 2.5.2 (2024-02-22)
 ==================
 - Fix credential `get_backend` usage.
 - Code styles updates.
 - Add view icons.
 
 2.5.1 (2024-02-20)
```

### Comparing `mayan-importer-2.5.3/LICENSE` & `mayan-importer-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/PKG-INFO` & `mayan-importer-3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 2.5.3
+Version: 3.0
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Communications :: File Sharing
 Requires-Python: !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 License-File: LICENSE
+Requires-Dist: dropbox==10.4.1
 
 ===========
 Description
 ===========
 
 Mayan EDMS app to migrate files from external sources.
 
@@ -92,14 +93,28 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.0 (2024-04-01)
+================
+- Refactor app.
+- Remove import setup action.
+- Use source metadata to store import metadata.
+- Don't deserialize import item source column.
+- Use upstream backend, dynamic forms, credentials mixins, model mixins,
+  error log.
+- Use fieldsets.
+- Bring code standards up to series 4.5.
+- Support processing and deleting individual setup item entries.
+- Improve import setup and import setup item state handling.
+- Improve navigation, add return links.
+
 2.5.2 (2024-02-22)
 ==================
 - Fix credential `get_backend` usage.
 - Code styles updates.
 - Add view icons.
 
 2.5.1 (2024-02-20)
```

### Comparing `mayan-importer-2.5.3/README.rst` & `mayan-importer-3.0/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/api_views.py` & `mayan-importer-3.0/importer/api_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,29 @@
     """
     post: Delete all the items of the specified import setup.
     """
     lookup_url_kwarg = 'import_setup_id'
     mayan_object_permissions = {
         'POST': (permission_import_setup_process,)
     }
-    queryset = ImportSetup.objects.all()
+    source_queryset = ImportSetup.objects.all()
 
     def object_action(self, request, serializer):
         self.object.clear()
 
 
 class APIImportSetupPopulateView(generics.ObjectActionAPIView):
     """
     post: Populate all the items of the specified import setup.
     """
     lookup_url_kwarg = 'import_setup_id'
     mayan_object_permissions = {
         'POST': (permission_import_setup_process,)
     }
-    queryset = ImportSetup.objects.all()
+    source_queryset = ImportSetup.objects.all()
 
     def object_action(self, request, serializer):
         task_import_setup_populate.apply_async(
             kwargs={'import_setup_id': self.object.pk}
         )
 
 
@@ -46,15 +46,15 @@
     """
     post: Process all the items of the specified import setup.
     """
     lookup_url_kwarg = 'import_setup_id'
     mayan_object_permissions = {
         'POST': (permission_import_setup_process,)
     }
-    queryset = ImportSetup.objects.all()
+    source_queryset = ImportSetup.objects.all()
 
     def object_action(self, request, serializer):
         task_import_setup_process.apply_async(
             kwargs={'import_setup_id': self.object.pk}
         )
 
 
@@ -68,15 +68,15 @@
     lookup_url_kwarg = 'import_setup_id'
     mayan_object_permissions = {
         'DELETE': (permission_import_setup_delete,),
         'GET': (permission_import_setup_view,),
         'PATCH': (permission_import_setup_edit,),
         'PUT': (permission_import_setup_edit,)
     }
-    queryset = ImportSetup.objects.all()
+    source_queryset = ImportSetup.objects.all()
     serializer_class = ImportSetupSerializer
 
     def get_serializer(self, *args, **kwargs):
         if not self.request:
             return None
 
         return super().get_serializer(*args, **kwargs)
@@ -85,16 +85,16 @@
 class APIImportSetupListView(generics.ListCreateAPIView):
     """
     get: Returns a list of all the import setups.
     post: Create a new import setup.
     """
     mayan_object_permissions = {'GET': (permission_import_setup_view,)}
     mayan_view_permissions = {'POST': (permission_import_setup_create,)}
-    queryset = ImportSetup.objects.all()
     serializer_class = ImportSetupSerializer
+    source_queryset = ImportSetup.objects.all()
 
     def get_serializer(self, *args, **kwargs):
         if not self.request:
             return None
 
         return super().get_serializer(*args, **kwargs)
 
@@ -104,15 +104,15 @@
 
 class ImportSetupParentMixin:
     def get_import_setup(self):
         return get_object_or_404(
             klass=ImportSetup, pk=self.kwargs['import_setup_id']
         )
 
-    def get_queryset(self):
+    def get_source_queryset(self):
         return self.get_import_setup().items.all()
 
 
 class APIImportSetupItemListView(ImportSetupParentMixin, generics.ListAPIView):
     """
     get: Returns a list of all the import setup items.
     """
```

### Comparing `mayan-importer-2.5.3/importer/apps.py` & `mayan-importer-3.0/importer/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import logging
 
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.acls.classes import ModelPermission
 from mayan.apps.common.apps import MayanAppConfig
 from mayan.apps.common.menus import (
-    menu_list_facet, menu_multi_item, menu_object, menu_return,
+    menu_list_facet, menu_multi_item, menu_object, menu_related, menu_return,
     menu_secondary, menu_setup
 )
+from mayan.apps.credentials.links import link_credential_list
 from mayan.apps.events.classes import EventModelRegistry, ModelEventType
+from mayan.apps.logging.classes import ErrorLog
 from mayan.apps.navigation.classes import SourceColumn
-from mayan.apps.views.column_widgets import TwoStateWidget
 
-from .classes import ImportSetupActionBackend, ImportSetupBackend, ModelFiler
+from .classes import ImportSetupBackend, ModelFiler
 from .events import (
-    event_import_setup_edited, event_import_setup_item_completed,
+    event_import_setup_edited, event_import_setup_item_finished,
     event_import_setup_item_deleted, event_import_setup_item_edited,
-    event_import_setup_process_ended, event_import_setup_process_started,
-    event_import_setup_populate_ended, event_import_setup_populate_started
+    event_import_setup_process_finished, event_import_setup_process_started,
+    event_import_setup_populate_finished, event_import_setup_populate_started
 )
 from .links import (
     link_import_setup_backend_selection, link_import_setup_delete,
     link_import_setup_clear, link_import_setup_edit,
-    link_import_setup_item_edit, link_import_setup_item_multiple_delete,
+    link_import_setup_item_delete, link_import_setup_item_edit,
+    link_import_setup_item_multiple_delete,
     link_import_setup_item_document_list,
     link_import_setup_item_multiple_process, link_import_setup_item_list,
-    link_import_setup_logs, link_import_setup_multiple_clear,
+    link_import_setup_item_process, link_import_setup_multiple_clear,
     link_import_setup_multiple_populate, link_import_setup_multiple_process,
     link_import_setup_populate, link_import_setup_process,
     link_import_setup_list, link_import_setup_setup, link_model_filer_load,
     link_model_filer_save
 )
-from .links import (
-    link_import_setup_action_backend_selection,
-    link_import_setup_action_delete, link_import_setup_action_edit,
-    link_import_setup_action_list
-)
 from .permissions import (
     permission_import_setup_delete, permission_import_setup_edit,
     permission_import_setup_process, permission_import_setup_view,
     permission_model_filer_load, permission_model_filer_save
 )
 
 logger = logging.getLogger(name=__name__)
@@ -47,43 +44,43 @@
 
 class ImporterApp(MayanAppConfig):
     app_namespace = 'importer'
     app_url = 'importer'
     has_rest_api = True
     has_tests = True
     name = 'importer'
-    verbose_name = _('Importer')
+    verbose_name = _(message='Importer')
 
     def ready(self):
         super().ready()
 
-        ImportSetupActionBackend.load_modules()
         ImportSetupBackend.load_modules()
 
         ImportSetup = self.get_model(model_name='ImportSetup')
-        ImportSetupAction = self.get_model(model_name='ImportSetupAction')
         ImportSetupItem = self.get_model(model_name='ImportSetupItem')
-        ImportSetupLog = self.get_model(model_name='ImportSetupLog')
+
+        error_log = ErrorLog(app_config=self)
+        error_log.register_model(model=ImportSetup, register_permission=True)
+        error_log.register_model(model=ImportSetupItem)
 
         EventModelRegistry.register(model=ImportSetup)
-        EventModelRegistry.register(model=ImportSetupAction)
         EventModelRegistry.register(model=ImportSetupItem)
 
         ModelEventType.register(
             model=ImportSetup, event_types=(
                 event_import_setup_edited, event_import_setup_item_deleted,
-                event_import_setup_populate_ended,
+                event_import_setup_populate_finished,
                 event_import_setup_populate_started,
-                event_import_setup_process_ended,
+                event_import_setup_process_finished,
                 event_import_setup_process_started
             )
         )
         ModelEventType.register(
             model=ImportSetupItem, event_types=(
-                event_import_setup_item_completed,
+                event_import_setup_item_finished,
                 event_import_setup_item_edited
             )
         )
 
         ModelFiler(model=ImportSetupItem)
 
         ModelPermission.register(
@@ -92,106 +89,93 @@
                 permission_import_setup_process,
                 permission_import_setup_view, permission_model_filer_load,
                 permission_model_filer_save
             )
         )
 
         ModelPermission.register_inheritance(
-            model=ImportSetupAction, related='import_setup',
-        )
-        ModelPermission.register_inheritance(
             model=ImportSetupItem, related='import_setup',
         )
 
+        # Import setup
+
         SourceColumn(
             attribute='label', is_identifier=True, is_sortable=True,
             source=ImportSetup
         )
         SourceColumn(
-            attribute='get_backend_label', include_label=True,
+            attribute='get_backend_class_label', include_label=True,
             source=ImportSetup
         )
         SourceColumn(
-            attribute='item_count_percent', empty_value=_('0%'),
+            attribute='item_count_percent', empty_value=_(message='0%'),
             include_label=True, source=ImportSetup
         )
         SourceColumn(
             attribute='get_state_label', include_label=True,
             is_sortable=True, sort_field='state', source=ImportSetup
         )
 
-        SourceColumn(
-            attribute='datetime', is_sortable=True, is_identifier=True,
-            source=ImportSetupLog
-        )
-        SourceColumn(
-            attribute='text', source=ImportSetupLog,
-        )
-
-        # Import Setup Action
-
-        SourceColumn(
-            attribute='label', is_identifier=True, is_sortable=True,
-            source=ImportSetupAction
-        )
-        SourceColumn(
-            attribute='enabled', include_label=True, is_sortable=True,
-            source=ImportSetupAction, widget=TwoStateWidget
-        )
-        SourceColumn(
-            attribute='order', include_label=True, is_sortable=True,
-            source=ImportSetupAction
-        )
-        SourceColumn(
-            attribute='get_backend_label', include_label=True,
-            label=_('Action type'), source=ImportSetupAction
-        )
-
-        # Import Setup Item
+        # Import setup item
 
         SourceColumn(
             attribute='identifier', is_identifier=True, is_sortable=True,
             source=ImportSetupItem
         )
         SourceColumn(
-            attribute='get_data_display', source=ImportSetupItem
+            attribute='serialized_data', include_label=True,
+            source=ImportSetupItem
         )
         SourceColumn(
-            attribute='get_state_label', is_sortable=True,
+            attribute='get_state_label', include_label=True, is_sortable=True,
             sort_field='state', source=ImportSetupItem
         )
-        SourceColumn(
-            attribute='state_data', source=ImportSetupItem
-        )
 
-        # ImportSetup
+        # Import setup
 
         menu_list_facet.bind_links(
-            links=(
-                link_import_setup_item_list, link_import_setup_logs
-            ), sources=(ImportSetup,)
+            links=(link_import_setup_item_list,), sources=(ImportSetup,)
         )
 
         menu_multi_item.bind_links(
             links=(
                 link_import_setup_multiple_clear,
                 link_import_setup_multiple_populate,
                 link_import_setup_multiple_process
             ), sources=(ImportSetup,)
         )
+
         menu_object.bind_links(
             links=(
                 link_import_setup_delete, link_import_setup_edit,
                 link_import_setup_process
             ), sources=(ImportSetup,)
         )
+
+        menu_related.bind_links(
+            links=(link_credential_list,),
+            sources=(
+                ImportSetup, ImportSetupItem,
+                'importer:import_setup_backend_selection',
+                'importer:import_setup_create',
+                'importer:import_setup_list'
+            )
+        )
+
+        menu_return.bind_links(
+            links=(link_import_setup_list,), sources=(
+                ImportSetup, ImportSetupItem,
+                'importer:import_setup_backend_selection',
+                'importer:import_setup_create',
+                'importer:import_setup_list'
+            )
+        )
+
         menu_secondary.bind_links(
-            links=(
-                link_import_setup_backend_selection,
-            ),
+            links=(link_import_setup_backend_selection,),
             sources=(
                 ImportSetup, 'importer:import_setup_items_list',
                 'importer:import_setup_create', 'importer:import_setup_list'
             )
         )
 
         menu_secondary.bind_links(
@@ -203,56 +187,30 @@
                 'importer:import_setup_load',
                 'importer:import_setup_items_list',
                 'importer:import_setup_populate',
                 'importer:import_setup_save'
             )
         )
 
-        menu_return.bind_links(
-            links=(
-                link_import_setup_list,
-            ),
-            sources=(
-                ImportSetup, ImportSetupAction, ImportSetupItem
-            )
-        )
-
         menu_setup.bind_links(
             links=(link_import_setup_setup,)
         )
 
-        # Import setup action
-
-        menu_list_facet.bind_links(
-            links=(
-                link_import_setup_action_list,
-            ), sources=(ImportSetup,)
-        )
-
-        menu_object.bind_links(
-            links=(
-                link_import_setup_action_delete,
-                link_import_setup_action_edit,
-            ), sources=(ImportSetupAction,)
-        )
-        menu_secondary.bind_links(
-            links=(
-                link_import_setup_action_backend_selection,
-            ), sources=(
-                ImportSetup,
-            )
-        )
-
         # Import setup item
 
         menu_list_facet.bind_links(
             links=(
                 link_import_setup_item_document_list,
                 link_import_setup_item_edit
             ), sources=(ImportSetupItem,)
         )
         menu_multi_item.bind_links(
             links=(
                 link_import_setup_item_multiple_delete,
                 link_import_setup_item_multiple_process
             ), sources=(ImportSetupItem,)
         )
+        menu_object.bind_links(
+            links=(
+                link_import_setup_item_delete, link_import_setup_item_process,
+            ), sources=(ImportSetupItem,)
+        )
```

### Comparing `mayan-importer-2.5.3/importer/classes.py` & `mayan-importer-3.0/importer/classes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,200 +1,82 @@
 import csv
 import io
-import json
 import logging
 import shutil
 
 from furl import furl
 
 from django.apps import apps
 from django.db import models
 from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 
-from mayan.apps.common.class_mixins import AppsModuleLoaderMixin
+from mayan.apps.backends.class_mixins import DynamicFormBackendMixin
+from mayan.apps.backends.classes import ModelBaseBackend
 from mayan.apps.locales.utils import to_language
 from mayan.apps.storage.utils import NamedTemporaryFile
-from mayan.apps.templating.classes import Template
 
-from .exceptions import ImportSetupActionError
 from .permissions import permission_import_setup_view
 
 logger = logging.getLogger(name=__name__)
 
-__all__ = ('ImportSetupActionBackend', 'ImportSetupBackend',)
+__all__ = ('ImportSetupBackend',)
 MESSAGE_MODEL_FILER_SAVE_BODY = _(
     'The model data from object type %(save_file_title)s has been '
     'exported and is available for download using the '
     'link: %(download_url)s or from '
     'the downloads area (%(download_list_url)s).'
 )
 MESSAGE_MODEL_FILER_SAVE_SUBJECT = _('Model data export.')
 
 
-class ImportSetupActionBackendMetaclass(type):
-    _registry = {}
-
-    def __new__(mcs, name, bases, attrs):
-        new_class = super().__new__(
-            mcs, name, bases, attrs
-        )
-
-        if not new_class.__module__ == __name__:
-            mcs._registry[
-                '{}.{}'.format(new_class.__module__, name)
-            ] = new_class
-
-        return new_class
-
-
-class ImportSetupActionBackend(
-    AppsModuleLoaderMixin, metaclass=ImportSetupActionBackendMetaclass
-):
-    _loader_module_name = 'import_setup_actions'
-    fields = ()
-
-    @classmethod
-    def clean(cls, request, cleaned_data, dynamic_form_data):
-        cleaned_data['backend_data'] = json.dumps(obj=dynamic_form_data)
-        return cleaned_data
-
-    @classmethod
-    def get(cls, name):
-        return cls._registry[name]
-
-    @classmethod
-    def get_all(cls):
-        return sorted(cls._registry.values(), key=lambda x: x.label)
+class ImportSetupBackend(DynamicFormBackendMixin, ModelBaseBackend):
+    _backend_app_label = 'importer'
+    _backend_model_name = 'ImportSetup'
+    _loader_module_name = 'importers'
 
     @classmethod
-    def get_choices(cls):
-        apps_name_map = {
-            app.name: app for app in apps.get_app_configs()
-        }
-
-        # Match each import_setup action to an app
-        apps_import_setup_action_map = {}
-
-        for klass in cls.get_all():
-            for app_name, app in apps_name_map.items():
-                if klass.__module__.startswith(app_name):
-                    apps_import_setup_action_map.setdefault(app, [])
-                    apps_import_setup_action_map[app].append(
-                        (klass.id(), klass.label)
-                    )
-
-        result = [
-            (app.verbose_name, import_setup_actions) for app, import_setup_actions in apps_import_setup_action_map.items()
-        ]
-
-        # Sort by app, then by import_setup action
-        return sorted(result, key=lambda x: (x[0], x[1]))
+    def callback_document_file(
+        cls, document_file, mayan_import_setup_item_id, source_metadata
+    ):
+        DocumentFileSourceMetadata = apps.get_model(
+            app_label='sources', model_name='DocumentFileSourceMetadata'
+        )
 
-    @classmethod
-    def id(cls):
-        return '{}.{}'.format(cls.__module__, cls.__name__)
+        coroutine = DocumentFileSourceMetadata.objects.create_bulk()
+        next(coroutine)
 
-    def __init__(self, **kwargs):
-        # Set the values of the dynamic fields
-        for class_field in getattr(self, 'class_fields', ()):
-            setattr(self, class_field, kwargs.pop(class_field, None))
-
-        # Set the values of the persistent backend attributes
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    def get_form_schema(self, request=None):
-        result = {
-            'fields': self.fields or {},
-            'media': getattr(self, 'media', {}),
-            'widgets': getattr(self, 'widgets', {}),
-        }
-
-        if hasattr(self, 'field_order'):
-            result['field_order'] = self.field_order
-
-        return result
-
-    def render_field(self, field_name, context):
-        try:
-            result = Template(
-                template_string=getattr(self, field_name, '')
-            ).render(
-                context=context
-            )
-        except Exception as exception:
-            raise ImportSetupActionError(
-                _('%(field_name)s template error: %(exception)s') % {
-                    'field_name': field_name, 'exception': exception
+        for key, value in source_metadata.items():
+            coroutine.send(
+                {
+                    'document_file': document_file, 'key': key, 'value': value
                 }
             )
 
-        logger.debug('%s template result: %s', field_name, result)
-
-        return result
-
-
-class ImportSetupBackendMetaclass(type):
-    _registry = {}
-
-    def __new__(mcs, name, bases, attrs):
-        new_class = super().__new__(
-            mcs, name, bases, attrs
-        )
-        if not new_class.__module__ == 'importer.classes':
-            mcs._registry[
-                '{}.{}'.format(new_class.__module__, name)
-            ] = new_class
-
-        return new_class
-
-
-class ImportSetupBackend(
-    AppsModuleLoaderMixin, metaclass=ImportSetupBackendMetaclass
-):
-    _loader_module_name = 'importers'
-    fields = {}
-
-    @classmethod
-    def get(cls, name):
-        return cls._registry[name]
+        coroutine.close()
 
     @classmethod
-    def get_all(cls):
-        return cls._registry
-
-    @classmethod
-    def get_choices(cls):
-        return sorted(
-            [
-                (
-                    key, backend.label
-                ) for key, backend in cls.get_all().items()
-            ], key=lambda x: x[1]
+    def get_form_fieldsets(cls):
+        fieldsets = (
+            (
+                _('General'), {
+                    'fields': ('label', 'document_type')
+                }
+            ), (
+                _(message='Processing'), {
+                    'fields': ('item_time_buffer', 'process_size')
+                }
+            ),
         )
 
-    @classmethod
-    def get_class_fields(cls):
-        backend_field_list = getattr(cls, 'fields', {}).keys()
-        return getattr(cls, 'class_fields', backend_field_list)
-
-    def __init__(self, **kwargs):
-        for class_field in getattr(self, 'class_fields', ()):
-            setattr(self, class_field, kwargs.get(class_field, None))
-
-        self.credential_class = kwargs.get('credential_class', None)
-        self.credential_data = kwargs.get('credential_data', None)
-
-    def check_valid(self, identifier, data):
-        return True
+        return fieldsets
 
 
 class NullBackend(ImportSetupBackend):
-    label = _('Null backend')
+    label = _(message='Null backend')
 
 
 class ModelFiler:
     _registry = {}
 
     @staticmethod
     def get_field_names(model):
@@ -248,15 +130,17 @@
 
                 if self.bulk_size:
                     bulk_list = []
                     bulk_count = 0
 
                     for row in reader:
                         row.update(**field_defaults)
-                        bulk_list.append(self.model(**row))
+                        bulk_list.append(
+                            self.model(**row)
+                        )
                         bulk_count += 1
 
                         if bulk_count > self.bulk_size:
                             manager.bulk_create(bulk_list)
                             bulk_list = []
                             bulk_count = 0
 
@@ -280,24 +164,30 @@
         if not filter_kwargs:
             filter_kwargs = {}
 
         field_names = ModelFiler.get_field_names(model=self.model)
 
         queryset = self.model._meta.default_manager.filter(**filter_kwargs)
 
+        filename = '{}-export.csv'.format(
+            self.get_model_full_name()
+        )
+
         download_file = DownloadFile(
-            content_object=queryset.first(), filename='{}-export.csv'.format(self.get_model_full_name()),
-            label=_('Export of %s to CSV') % save_file_title,
+            content_object=queryset.first(), filename=filename,
+            label=_(message='Export of %s to CSV') % save_file_title,
             permission=permission_import_setup_view.stored_permission
         )
         download_file._event_actor = user
         download_file.save()
 
         with NamedTemporaryFile(mode='r+') as temporary_file_object:
-            writer = csv.DictWriter(f=temporary_file_object, fieldnames=field_names)
+            writer = csv.DictWriter(
+                f=temporary_file_object, fieldnames=field_names
+            )
 
             writer.writeheader()
             for item in queryset.values(*field_names):
                 writer.writerow(item)
 
             temporary_file_object.seek(0)
```

### Comparing `mayan-importer-2.5.3/importer/events.py` & `mayan-importer-3.0/importer/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.events.classes import EventTypeNamespace
 
-namespace = EventTypeNamespace(label=_('Importer'), name='importer')
+namespace = EventTypeNamespace(
+    label=_(message='Importer'), name='importer'
+)
+
+# Import setup
 
 event_import_setup_created = namespace.add_event_type(
-    label=_('Import setup created'), name='import_setup_created'
+    label=_(message='Import setup created'), name='import_setup_created'
 )
 event_import_setup_edited = namespace.add_event_type(
-    label=_('Import setup edited'), name='import_setup_edited'
+    label=_(message='Import setup edited'), name='import_setup_edited'
 )
-event_import_setup_item_created = namespace.add_event_type(
-    label=_('Import setup item created'), name='import_setup_item_created'
-)
-event_import_setup_item_deleted = namespace.add_event_type(
-    label=_('Import setup item deleted'), name='import_setup_item_deleted'
+event_import_setup_populate_finished = namespace.add_event_type(
+    label=_(message='Import setup populate ended'),
+    name='import_setup_populate_finished'
 )
-event_import_setup_item_edited = namespace.add_event_type(
-    label=_('Import setup item edited'), name='import_setup_item_edited'
-)
-event_import_setup_item_completed = namespace.add_event_type(
-    label=_('Import setup item completed'), name='import_setup_item_completed'
+event_import_setup_populate_started = namespace.add_event_type(
+    label=_(message='Import setup populate started'),
+    name='import_setup_populate_started'
 )
-event_import_setup_process_ended = namespace.add_event_type(
-    label=_('Import setup process ended'), name='import_setup_process_ended'
+event_import_setup_process_finished = namespace.add_event_type(
+    label=_(message='Import setup process ended'),
+    name='import_setup_process_finished'
 )
 event_import_setup_process_started = namespace.add_event_type(
-    label=_('Import setup process started'),
+    label=_(message='Import setup process started'),
     name='import_setup_process_started'
 )
-event_import_setup_populate_ended = namespace.add_event_type(
-    label=_('Import setup populate ended'), name='import_setup_populate_ended'
+
+# Import setup item
+
+event_import_setup_item_created = namespace.add_event_type(
+    label=_(message='Import setup item created'),
+    name='import_setup_item_created'
 )
-event_import_setup_populate_started = namespace.add_event_type(
-    label=_('Import setup populate started'),
-    name='import_setup_populate_started'
+event_import_setup_item_deleted = namespace.add_event_type(
+    label=_(message='Import setup item deleted'),
+    name='import_setup_item_deleted'
+)
+event_import_setup_item_edited = namespace.add_event_type(
+    label=_(message='Import setup item edited'),
+    name='import_setup_item_edited'
+)
+event_import_setup_item_finished = namespace.add_event_type(
+    label=_(message='Import setup item completed'),
+    name='import_setup_item_finished'
 )
```

### Comparing `mayan-importer-2.5.3/importer/icons.py` & `mayan-importer-3.0/importer/icons.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,40 +7,18 @@
 )
 icon_import_setup_clear = Icon(
     driver_name='fontawesome', symbol='eraser'
 )
 icon_import_setup_delete = Icon(driver_name='fontawesome', symbol='times')
 
 icon_import_setup_edit = Icon(driver_name='fontawesome', symbol='pencil-alt')
-icon_import_setup_log_list = Icon(
-    driver_name='fontawesome', symbol='exclamation-triangle'
-)
 icon_import_setup_process = Icon(
     driver_name='fontawesome', symbol='play'
 )
 
-# Import setup actions
-
-icon_import_setup_action = Icon(
-    driver_name='fontawesome', symbol='code'
-)
-icon_import_setup_action_delete = Icon(
-    driver_name='fontawesome', symbol='times'
-)
-icon_import_setup_action_edit = Icon(
-    driver_name='fontawesome', symbol='pencil-alt'
-)
-icon_import_setup_action_list = Icon(
-    driver_name='fontawesome', symbol='code'
-)
-icon_import_setup_action_backend_selection = Icon(
-    driver_name='fontawesome-dual', primary_symbol='code',
-    secondary_symbol='plus'
-)
-
 # Import setup items
 
 icon_import_setup_item_delete = Icon(
     driver_name='fontawesome', symbol='times'
 )
 icon_import_setup_item_edit = Icon(
     driver_name='fontawesome', symbol='pencil-alt'
```

### Comparing `mayan-importer-2.5.3/importer/importers.py` & `mayan-importer-3.0/importer/importers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,167 @@
 from collections import namedtuple
 import re
 import shutil
 
 import dropbox
 
 from django.core.files import File
-from django.core.exceptions import ImproperlyConfigured
 from django.utils.functional import cached_property
 from django.utils.translation import ugettext_lazy as _
 
-from mayan.apps.credentials.credential_backends import CredentialBackendAccessToken
+from mayan.apps.credentials.class_mixins import BackendMixinCredentials
 from mayan.apps.storage.models import SharedUploadedFile
 from mayan.apps.storage.utils import NamedTemporaryFile
 
 from .classes import ImportSetupBackend
+from .exceptions import ImportSetupException
 
 
-class ImporterDropbox(ImportSetupBackend):
-    class_fields = (
-        'as_team_admin', 'team_admin_id', 'filename_regex', 'folder_regex'
-    )
-    field_order = (
-        'as_team_admin', 'team_admin_id', 'filename_regex', 'folder_regex'
-    )
-    fields = {
-        'as_team_admin': {
-            'label': _('Login as Team administrator'),
-            'class': 'django.forms.BooleanField', 'default': '',
-            'help_text': _(
-                'Access the API as a Team administrator in order to access '
-                'the entire set of files on a Dropbox Team/Business account. '
-                'If a Team administrator API ID is not specified, it will '
-                'be determined by using the Team API at the cost of an '
-                'extra request per item to process.'
-            ),
-            'required': False
-        },
-        'team_admin_id': {
-            'label': _('Team administrator API ID'),
-            'class': 'django.forms.CharField', 'default': '',
-            'help_text': _(
-                'An optional Team administrator API to avoid a request '
-                'per item to import.'
-            ),
-            'kwargs': {
-                'max_length': 248
-            }, 'required': False
-        },
-        'filename_regex': {
-            'label': _('Filename regular expression'),
-            'class': 'django.forms.CharField', 'default': '',
-            'help_text': _(
-                'An optional regular expression used to filter which files '
-                'to import. The regular expression will be matched against '
-                'the filename.'
-            ),
-            'kwargs': {
-                'max_length': 248
-            }, 'required': False
-        },
-        'folder_regex': {
-            'label': _('Folder regular expression'),
-            'class': 'django.forms.CharField', 'default': '',
-            'help_text': _(
-                'An optional regular expression used to filter which files '
-                'to import. The regular expression will be matched against '
-                'the file folder path.'
-            ),
-            'kwargs': {
-                'max_length': 248
-            }, 'required': False
-        },
-    }
-    label = _('Dropbox')
+class ImporterDropbox(BackendMixinCredentials, ImportSetupBackend):
+    label = _(message='Dropbox')
     item_identifier = 'id'  # Dropbox file unique identifier.
     item_label = 'name'  # Dropbox file field corresponding to the filename.
 
+    @classmethod
+    def get_form_fields(cls):
+        fields = super().get_form_fields()
+
+        fields.update(
+            {
+                'as_team_admin': {
+                    'label': _(message='Login as Team administrator'),
+                    'class': 'django.forms.BooleanField', 'default': '',
+                    'help_text': _(
+                        message='Access the API as a Team administrator in order to access '
+                        'the entire set of files on a Dropbox Team/Business account. '
+                        'If a Team administrator API ID is not specified, it will '
+                        'be determined by using the Team API at the cost of an '
+                        'extra request per item to process.'
+                    ),
+                    'required': False
+                },
+                'team_admin_id': {
+                    'label': _(message='Team administrator API ID'),
+                    'class': 'django.forms.CharField', 'default': '',
+                    'help_text': _(
+                        message='An optional Team administrator API to avoid a request '
+                        'per item to import.'
+                    ),
+                    'kwargs': {
+                        'max_length': 248
+                    }, 'required': False
+                },
+                'filename_regex': {
+                    'label': _(message='Filename regular expression'),
+                    'class': 'django.forms.CharField', 'default': '',
+                    'help_text': _(
+                        message='An optional regular expression used to filter which files '
+                        'to import. The regular expression will be matched against '
+                        'the filename.'
+                    ),
+                    'kwargs': {
+                        'max_length': 248
+                    }, 'required': False
+                },
+                'folder_regex': {
+                    'label': _(message='Folder regular expression'),
+                    'class': 'django.forms.CharField', 'default': '',
+                    'help_text': _(
+                        message='An optional regular expression used to filter which files '
+                        'to import. The regular expression will be matched against '
+                        'the file folder path.'
+                    ),
+                    'kwargs': {
+                        'max_length': 248
+                    }, 'required': False
+                },
+            }
+        )
+
+        return fields
+
+    @classmethod
+    def get_form_fieldsets(cls):
+        fieldsets = super().get_form_fieldsets()
+
+        fieldsets += (
+            (
+                _(message='API'), {
+                    'fields': ('as_team_admin', 'team_admin_id')
+                }
+            ), (
+                _(message='Content filtering'), {
+                    'fields': ('filename_regex', 'folder_regex')
+                }
+            ),
+        )
+
+        return fieldsets
+
     def get_client_base_kwargs(self):
-        if issubclass(self.credential_class, CredentialBackendAccessToken):
+        credential = self.get_credential()
+
+        try:
             kwargs = {
-                'oauth2_access_token': self.credential_data['token']
+                'oauth2_access_token': credential['token']
             }
-        else:
-            raise ImproperlyConfigured(
-                'Unknown credential class `{}`.'.format(
-                    self.credential_class.label
-                )
+        except KeyError:
+            raise ImportSetupException(
+                'Incompatible credential class. The credential must provide '
+                'an access token.'
             )
-
-        return kwargs
+        else:
+            return kwargs
 
     @cached_property
     def admin_profile_team_id(self):
         if self.team_admin_id:
             return self.team_admin_id
         else:
-            kwargs = self.get_client_base_kwargs()
-            client_team = dropbox.DropboxTeam(**kwargs)
+            client_kwargs = self.get_client_base_kwargs()
+            client_team = dropbox.DropboxTeam(**client_kwargs)
             token_get_authenticated_admin_result = client_team.team_token_get_authenticated_admin()
             return token_get_authenticated_admin_result.admin_profile.team_member_id
 
     def check_valid(self, identifier, data):
         entry = self.get_entry(identifier=identifier, data=data)
 
         return self.match_filename_factory(entry=entry) and self.match_folder_factory(entry=entry)
 
     def get_client(self):
         """
         Return an instance of the Dropbox API client.
         """
         kwargs = self.get_client_base_kwargs()
 
-        if self.as_team_admin:
+        as_team_admin = self.kwargs['as_team_admin']
+
+        if as_team_admin:
             headers = kwargs.get(
                 'headers', {}
             )
             headers.update(
                 {
-                    'Dropbox-API-Select-User': self.admin_profile_team_id
+                    'Dropbox-API-Select-User': self.kwargs['admin_profile_team_id']
                 }
             )
             kwargs['headers'] = headers
 
         return dropbox.Dropbox(**kwargs)
 
     def get_entry(self, identifier, data):
         Entry = namedtuple(
             typename='Entry', field_names=data.keys()
         )
         return Entry(**data)
 
-    def item_process(self, identifier, data):
-        entry = self.get_entry(identifier=identifier, data=data)
-
-        if self.match_filename_factory(entry=entry) and self.match_folder_factory(entry=entry):
-            client = self.get_client()
-
-            data, response = client.files_download(
-                path=identifier
-            )
-
-            response.raise_for_status()
-
-            # Copy the Dropbox file to a temporary location using streaming
-            # download.
-            # The create a shared upload instance from the temporary file.
-            with NamedTemporaryFile() as file_object:
-                shutil.copyfileobj(fsrc=response.raw, fdst=file_object)
-
-                file_object.seek(0)
-
-                return SharedUploadedFile.objects.create(
-                    file=File(file_object),
-                )
-
     def get_item_list(self):
         """
         Crawl the folders and add all the items that are actual files as
-        ImportSetupItem instances for later processing.
+        `ImportSetupItem` instances for later processing.
         """
         client = self.get_client()
         response = client.files_list_folder(
             include_non_downloadable_files=False, path='', recursive=True
         )
 
         while True:
@@ -181,22 +181,47 @@
             if not response.has_more:
                 break
             else:
                 response = client.files_list_folder_continue(
                     cursor=response.cursor
                 )
 
+    def item_process(self, identifier, data):
+        entry = self.get_entry(identifier=identifier, data=data)
+
+        if self.match_filename_factory(entry=entry) and self.match_folder_factory(entry=entry):
+            client = self.get_client()
+
+            data, response = client.files_download(
+                path=identifier
+            )
+
+            response.raise_for_status()
+
+            # Copy the Dropbox file to a temporary location using streaming
+            # download.
+            # The create a shared upload instance from the temporary file.
+            with NamedTemporaryFile() as file_object:
+                shutil.copyfileobj(fsrc=response.raw, fdst=file_object)
+
+                file_object.seek(0)
+
+                file = File(file_object)
+
+                return SharedUploadedFile.objects.create(file=file)
+
     @cached_property
     def match_filename_factory(self):
         """
         Perform a regular expression of and entry's filename.
         Returns True if there is a regular expression match or if there is no
         regular expression set.
         """
-        pattern = self.filename_regex
+        pattern = self.kwargs['filename_regex']
+
         if pattern:
             regex = re.compile(pattern=pattern)
 
             def match_function(entry):
                 return regex.match(string=entry.name)
         else:
             def match_function(entry):
@@ -207,15 +232,16 @@
     @cached_property
     def match_folder_factory(self):
         """
         Perform a regular expression of and entry's path.
         Returns True if there is a regular expression match or if there is no
         regular expression set.
         """
-        pattern = self.folder_regex
+        pattern = self.kwargs['folder_regex']
+
         if pattern:
             regex = re.compile(pattern=pattern)
 
             def match_function(entry):
                 return regex.match(string=entry.path_lower)
         else:
             def match_function(entry):
```

### Comparing `mayan-importer-2.5.3/importer/links.py` & `mayan-importer-3.0/importer/links.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,154 @@
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.navigation.classes import Link
 from mayan.apps.navigation.utils import factory_condition_queryset_access
 
 from .icons import (
-    icon_import_setup_action_delete, icon_import_setup_action_edit,
-    icon_import_setup_action_list,
-    icon_import_setup_action_backend_selection,
     icon_import_setup_backend_selection, icon_import_setup_delete,
-    icon_import_setup_edit, icon_import_setup_log_list,
-    icon_import_setup_process, icon_import_setup_item_delete,
-    icon_import_setup_item_document_list, icon_import_setup_item_edit,
-    icon_import_setup_item_process, icon_import_setup_clear,
-    icon_import_setup_items_list, icon_import_setup_list,
-    icon_import_setup_populate, icon_model_filer_load, icon_model_filer_save
+    icon_import_setup_edit, icon_import_setup_process,
+    icon_import_setup_item_delete, icon_import_setup_item_document_list,
+    icon_import_setup_item_edit, icon_import_setup_item_process,
+    icon_import_setup_clear, icon_import_setup_items_list,
+    icon_import_setup_list, icon_import_setup_populate, icon_model_filer_load,
+    icon_model_filer_save
 )
 from .permissions import (
     permission_import_setup_create, permission_import_setup_delete,
     permission_import_setup_edit, permission_import_setup_process,
     permission_import_setup_view, permission_model_filer_load,
     permission_model_filer_save
 )
 
 
 def conditional_disable_import_has_items(context):
     return context['resolved_object'].items.count() == 0
 
 
+def conditional_import_setup_item_process_allowed(context):
+    return not context['resolved_object'].get_process_allowed()
+
+
 # Import setup
 
 link_import_setup_backend_selection = Link(
     icon=icon_import_setup_backend_selection,
     permissions=(permission_import_setup_create,),
-    text=_('Create import setup'),
+    text=_(message='Create import setup'),
     view='importer:import_setup_backend_selection',
 )
 link_import_setup_clear = Link(
     args='resolved_object.pk', conditional_disable=conditional_disable_import_has_items,
     icon=icon_import_setup_clear,
-    permissions=(permission_import_setup_process,), text=_('Clear items'),
+    permissions=(permission_import_setup_process,), text=_(message='Clear items'),
     view='importer:import_setup_clear'
 )
 link_import_setup_delete = Link(
     args='resolved_object.pk',
     icon=icon_import_setup_delete,
     permissions=(permission_import_setup_delete,),
-    tags='dangerous', text=_('Delete'), view='importer:import_setup_delete'
+    tags='dangerous', text=_(message='Delete'), view='importer:import_setup_delete'
 )
 link_import_setup_edit = Link(
     args='resolved_object.pk',
     icon=icon_import_setup_edit,
-    permissions=(permission_import_setup_edit,), text=_('Edit'),
+    permissions=(permission_import_setup_edit,), text=_(message='Edit'),
     view='importer:import_setup_edit'
 )
 link_import_setup_list = Link(
     icon=icon_import_setup_list,
-    text=_('Import setup list'),
+    text=_(message='Import setup list'),
     view='importer:import_setup_list'
 )
-link_import_setup_logs = Link(
-    args=('resolved_object.pk',), icon=icon_import_setup_log_list,
-    permissions=(permission_import_setup_view,), text=_('Logs'),
-    view='importer:import_setup_log_list'
-)
 link_import_setup_multiple_clear = Link(
-    icon=icon_import_setup_clear, text=_('Clear items'),
+    icon=icon_import_setup_clear, text=_(message='Clear items'),
     view='importer:import_setup_multiple_clear'
 )
 link_import_setup_multiple_populate = Link(
-    icon=icon_import_setup_populate, text=_('Populate items'),
+    icon=icon_import_setup_populate, text=_(message='Populate items'),
     view='importer:import_setup_multiple_populate'
 )
 link_import_setup_multiple_process = Link(
-    icon=icon_import_setup_process, text=_('Process'),
+    icon=icon_import_setup_process, text=_(message='Process'),
     view='importer:import_setup_multiple_process'
 )
 link_import_setup_populate = Link(
     args='resolved_object.pk',
     icon=icon_import_setup_populate,
-    permissions=(permission_import_setup_process,), text=_('Populate items'),
+    permissions=(permission_import_setup_process,),
+    text=_(message='Populate items'),
     view='importer:import_setup_populate'
 )
 link_import_setup_process = Link(
     args='resolved_object.pk',
     conditional_disable=conditional_disable_import_has_items,
     icon=icon_import_setup_process,
-    permissions=(permission_import_setup_process,), text=_('Process'),
+    permissions=(permission_import_setup_process,), text=_(message='Process'),
     view='importer:import_setup_process'
 )
 link_import_setup_setup = Link(
     condition=factory_condition_queryset_access(
         app_label='importer', model_name='ImportSetup',
         object_permission=permission_import_setup_view,
         view_permission=permission_import_setup_create,
     ), icon=icon_import_setup_list,
-    text=_('Importer'),
+    text=_(message='Importer'),
     view='importer:import_setup_list'
 )
 
-
-# Import setup actions
-
-
-link_import_setup_action_delete = Link(
-    args='resolved_object.pk',
-    icon=icon_import_setup_action_delete,
-    permissions=(permission_import_setup_edit,),
-    tags='dangerous', text=_('Delete'),
-    view='importer:import_setup_action_delete',
-)
-link_import_setup_action_edit = Link(
-    args='resolved_object.pk',
-    icon=icon_import_setup_action_edit,
-    permissions=(permission_import_setup_edit,),
-    text=_('Edit'), view='importer:import_setup_action_edit',
-)
-link_import_setup_action_list = Link(
-    args='resolved_object.pk',
-    icon=icon_import_setup_action_list,
-    permissions=(permission_import_setup_view,), text=_('Actions'),
-    view='importer:import_setup_action_list'
-)
-link_import_setup_action_backend_selection = Link(
-    args='resolved_object.pk',
-    icon=icon_import_setup_action_backend_selection,
-    permissions=(permission_import_setup_edit,), text=_('Create action'),
-    view='importer:import_setup_action_backend_selection',
-)
-
 # Import setup item
 
-
 link_import_setup_item_document_list = Link(
     args='resolved_object.pk',
     icon=icon_import_setup_item_document_list,
-    permissions=(permission_import_setup_view,), text=_('Documents'),
+    permissions=(permission_import_setup_view,), text=_(message='Documents'),
     view='importer:import_setup_item_document_list'
 )
+link_import_setup_item_delete = Link(
+    args='resolved_object.pk', icon=icon_import_setup_item_delete,
+    permissions=(permission_import_setup_edit,),
+    tags='dangerous', text=_(message='Delete'),
+    view='importer:import_setup_item_delete'
+)
 link_import_setup_item_edit = Link(
     args='resolved_object.pk', icon=icon_import_setup_item_edit,
-    permissions=(permission_import_setup_edit,), text=_('Edit'),
+    permissions=(permission_import_setup_edit,), text=_(message='Edit'),
     view='importer:import_setup_item_edit'
 )
 link_import_setup_item_list = Link(
     args='resolved_object.pk',
     icon=icon_import_setup_items_list,
-    permissions=(permission_import_setup_view,), text=_('Items'),
+    permissions=(permission_import_setup_view,), text=_(message='Items'),
     view='importer:import_setup_items_list'
 )
 link_import_setup_item_multiple_delete = Link(
     icon=icon_import_setup_item_delete,
     permissions=(permission_import_setup_edit,),
-    tags='dangerous', text=_('Delete'),
+    tags='dangerous', text=_(message='Delete'),
     view='importer:import_setup_item_multiple_delete'
 )
 link_import_setup_item_multiple_process = Link(
     icon=icon_import_setup_item_process,
     permissions=(permission_import_setup_edit,),
-    text=_('Process'), view='importer:import_setup_item_multiple_process'
+    text=_(message='Process'),
+    view='importer:import_setup_item_multiple_process'
+)
+link_import_setup_item_process = Link(
+    args='resolved_object.pk',
+    conditional_disable=conditional_import_setup_item_process_allowed,
+    icon=icon_import_setup_item_process,
+    permissions=(permission_import_setup_edit,),
+    text=_(message='Process'), view='importer:import_setup_item_process'
 )
 
 # Model filer
 
 link_model_filer_load = Link(
     args='resolved_object.pk', icon=icon_model_filer_load,
     permissions=(permission_model_filer_load,),
-    text=_('Load items'), view='importer:import_setup_load'
+    text=_(message='Load items'), view='importer:import_setup_load'
 )
 link_model_filer_save = Link(
     args='resolved_object.pk', icon=icon_model_filer_save,
     permissions=(permission_model_filer_save,),
-    text=_('Save items'), view='importer:import_setup_save'
+    text=_(message='Save items'), view='importer:import_setup_save'
 )
```

### Comparing `mayan-importer-2.5.3/importer/literals.py` & `mayan-importer-3.0/importer/literals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from django.utils.translation import ugettext_lazy as _
 
 DEFAULT_ITEM_TIME_BUFFER = 100
 DEFAULT_PROCESS_SIZE = 2
 
-ITEM_STATE_NONE = 1
-ITEM_STATE_ERROR = 2
-ITEM_STATE_QUEUED = 3
-ITEM_STATE_DOWNLOADED = 4
-ITEM_STATE_COMPLETE = 5
-
-ITEM_STATE_CHOICES = (
-    (ITEM_STATE_NONE, _('None')),
-    (ITEM_STATE_ERROR, _('Error')),
-    (ITEM_STATE_QUEUED, _('Queued')),
-    (ITEM_STATE_DOWNLOADED, _('Downloaded')),
-    (ITEM_STATE_COMPLETE, _('Complete')),
+ENABLE_STATE_CHANGE = False
+
+SETUP_ITEM_STATE_NONE = 1
+SETUP_ITEM_STATE_ERROR = 2
+SETUP_ITEM_STATE_QUEUED = 3
+SETUP_ITEM_STATE_COMPLETE = 5
+SETUP_ITEM_STATE_PROCESSING = 6
+
+SETUP_ITEM_STATE_CHOICES = (
+    (SETUP_ITEM_STATE_NONE, _(message='None')),
+    (SETUP_ITEM_STATE_ERROR, _(message='Error')),
+    (SETUP_ITEM_STATE_QUEUED, _(message='Queued')),
+    (SETUP_ITEM_STATE_COMPLETE, _(message='Complete')),
+    (SETUP_ITEM_STATE_PROCESSING, _(message='Processing')),
 )
 
 SETUP_STATE_NONE = 1
 SETUP_STATE_ERROR = 2
 SETUP_STATE_POPULATING = 3
 SETUP_STATE_EXECUTING = 4
 
 SETUP_STATE_CHOICES = (
-    (SETUP_STATE_NONE, _('None')),
-    (SETUP_STATE_ERROR, _('Error')),
-    (SETUP_STATE_POPULATING, _('Populating')),
-    (SETUP_STATE_EXECUTING, _('Executing')),
+    (SETUP_STATE_NONE, _(message='None')),
+    (SETUP_STATE_ERROR, _(message='Error')),
+    (SETUP_STATE_POPULATING, _(message='Populating')),
+    (SETUP_STATE_EXECUTING, _(message='Executing')),
 )
```

### Comparing `mayan-importer-2.5.3/importer/migrations/0001_initial.py` & `mayan-importer-3.0/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.0/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.0/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.0/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.0/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.0/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.0/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.0/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.0/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.0/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.0/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.0/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/models/import_setup_action_models.py` & `mayan-importer-3.0/importer/models/import_setup_item_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 from django.db import models
-from django.db.models import Max
+from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 
-try:
-    from mayan.apps.events.classes import EventManagerSave
-except ImportError:
-    from mayan.apps.events.event_managers import EventManagerSave
-
+from mayan.apps.documents.models.document_models import Document
 from mayan.apps.events.decorators import method_event
+from mayan.apps.events.event_managers import (
+    EventManagerMethodAfter, EventManagerSave
+)
+
+from ..events import (
+    event_import_setup_item_created, event_import_setup_item_deleted,
+    event_import_setup_item_edited
+)
+from ..literals import SETUP_ITEM_STATE_CHOICES, SETUP_ITEM_STATE_NONE
 
-from ..events import event_import_setup_edited
-
+from .import_setup_item_model_mixins import ImportSetupItemBusinessLogicMixin
 from .import_setup_models import ImportSetup
-from .mixins import BackendModelMixin
 
 
-class ImportSetupAction(BackendModelMixin, models.Model):
+class ImportSetupItem(ImportSetupItemBusinessLogicMixin, models.Model):
     import_setup = models.ForeignKey(
-        on_delete=models.CASCADE, related_name='actions', to=ImportSetup,
-        verbose_name=_('Import Setup')
+        on_delete=models.CASCADE, related_name='items',
+        to=ImportSetup, verbose_name=_(message='Import setup')
+    )
+    identifier = models.CharField(
+        db_index=True, help_text=_(
+            message='Source data element that uniquely identifies a file to '
+            'import.'
+        ), max_length=64, verbose_name=_(message='Identifier')
     )
-    label = models.CharField(
-        max_length=255, help_text=_('A short text describing the action.'),
-        verbose_name=_('Label')
-    )
-    enabled = models.BooleanField(default=True, verbose_name=_('Enabled'))
-    order = models.PositiveIntegerField(
-        blank=True, db_index=True, default=0, help_text=_(
-            'Order in which the action will be executed. If left '
-            'unchanged, an automatic order value will be assigned.'
-        ), verbose_name=_('Order')
+    serialized_data = models.TextField(
+        blank=True, default='{}', help_text=_(
+            message='Source data corresponding to a file to import.'
+        ), verbose_name=_(message='Serialized data')
+    )
+    state = models.IntegerField(
+        db_index=True, choices=SETUP_ITEM_STATE_CHOICES,
+        default=SETUP_ITEM_STATE_NONE, verbose_name=_(message='State')
+    )
+    documents = models.ManyToManyField(
+        blank=True, related_name='import_items', to=Document,
+        verbose_name=_(message='Document')
     )
 
     class Meta:
-        ordering = ('order', 'label')
-        unique_together = (
-            ('import_setup', 'order'), ('import_setup', 'label')
-        )
-        verbose_name = _('Import setup action')
-        verbose_name_plural = _('Import setup actions')
+        ordering = ('import_setup', 'identifier')
+        verbose_name = _(message='Import setup item')
+        verbose_name_plural = _(message='Import setup items')
 
     def __str__(self):
-        return self.label
+        return self.identifier
 
-    def execute(self, context=None):
-        if not context:
-            context = {}
-
-        return self.get_backend_instance().execute(context=context)
-
-    def get_next_order(self):
-        last_order = self.import_setup.actions.aggregate(
-            Max('order')
-        )['order__max']
-
-        if last_order is not None:
-            return last_order + 1
-        else:
-            return 0
+    def get_absolute_url(self):
+        return reverse(
+            viewname='importer:import_setup_items_list', kwargs={
+                'import_setup_id': self.import_setup.pk
+            }
+        )
+
+    @method_event(
+        event_manager_class=EventManagerMethodAfter,
+        event=event_import_setup_item_deleted,
+        action_object='self',
+        target='import_setup'
+    )
+    def delete(self):
+        return super().delete()
 
     @method_event(
         event_manager_class=EventManagerSave,
         created={
-            'action_object': 'self',
-            'event': event_import_setup_edited,
-            'target': 'import_setup'
+            'action_object': 'import_setup',
+            'event': event_import_setup_item_created,
+            'target': 'self'
         },
         edited={
-            'action_object': 'self',
-            'event': event_import_setup_edited,
-            'target': 'import_setup'
+            'action_object': 'import_setup',
+            'event': event_import_setup_item_edited,
+            'target': 'self'
         }
     )
     def save(self, *args, **kwargs):
-        if not self.order:
-            self.order = self.get_next_order()
+        if not self.state:
+            self.state = SETUP_ITEM_STATE_NONE
+
         super().save(*args, **kwargs)
```

### Comparing `mayan-importer-2.5.3/importer/permissions.py` & `mayan-importer-3.0/importer/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 from django.utils.translation import ugettext_lazy as _
 
 from mayan.apps.permissions import PermissionNamespace
 
-namespace = PermissionNamespace(label=_('Importer'), name='importer')
+namespace = PermissionNamespace(
+    label=_(message='Importer'), name='importer'
+)
+
+# Documents
+
+permission_import_setup_metadata_view = namespace.add_permission(
+    label=_('View document import setup metadata'),
+    name='import_setup_metadata_view'
+)
+
+# Import setup
 
 permission_import_setup_create = namespace.add_permission(
-    label=_('Create import setups'), name='import_setup_create'
+    label=_(message='Create import setups'), name='import_setup_create'
 )
 permission_import_setup_delete = namespace.add_permission(
-    label=_('Delete import setups'), name='import_setup_delete'
+    label=_(message='Delete import setups'), name='import_setup_delete'
 )
 permission_import_setup_edit = namespace.add_permission(
-    label=_('Edit import setups'), name='import_setup_edit'
+    label=_(message='Edit import setups'), name='import_setup_edit'
 )
 permission_import_setup_process = namespace.add_permission(
-    label=_('Process import setups'), name='import_setup_process'
+    label=_(message='Process import setups'), name='import_setup_process'
 )
 permission_import_setup_view = namespace.add_permission(
-    label=_('View import setups'), name='import_setup_view'
+    label=_(message='View import setups'), name='import_setup_view'
 )
 
-namespace = PermissionNamespace(label=_('Model filer'), name='model_filer')
+namespace = PermissionNamespace(
+    label=_(message='Model filer'), name='model_filer'
+)
 
 permission_model_filer_load = namespace.add_permission(
-    label=_('Save models to load'), name='model_filer_load'
+    label=_(message='Save models to load'), name='model_filer_load'
 )
 permission_model_filer_save = namespace.add_permission(
-    label=_('Save models to file'), name='model_filer_save'
+    label=_(message='Save models to file'), name='model_filer_save'
 )
```

### Comparing `mayan-importer-2.5.3/importer/queues.py` & `mayan-importer-3.0/importer/queues.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 
 worker_importer = Worker(
     maximum_memory_per_child=300000, maximum_tasks_per_child=100,
     name='worker_importer'
 )
 
 queue_importer = CeleryQueue(
-    label=_('Importer'), name='importer', worker=worker_importer
+    label=_(message='Importer'), name='importer', worker=worker_importer
 )
 queue_model_filer = CeleryQueue(
-    label=_('Model filer'), name='filer', worker=worker_importer
+    label=_(message='Model filer'), name='filer', worker=worker_importer
 )
 
 queue_importer.add_task_type(
-    label=_('Process an import setup'),
+    label=_(message='Process an import setup'),
     dotted_path='importer.tasks.task_import_setup_process'
 )
 queue_importer.add_task_type(
-    label=_('Process an import setup item'),
+    label=_(message='Process an import setup item'),
     dotted_path='importer.tasks.task_import_setup_item_process'
 )
 queue_importer.add_task_type(
-    label=_('Populate the items of an import setup'),
+    label=_(message='Populate the items of an import setup'),
     dotted_path='importer.tasks.task_import_setup_populate'
 )
 
 queue_model_filer.add_task_type(
-    label=_('Generates CSV files from a model'),
+    label=_(message='Generates CSV files from a model'),
     dotted_path='importer.tasks.task_model_filer_save'
 )
 queue_model_filer.add_task_type(
-    label=_('Loads CSV files and created models'),
+    label=_(message='Loads CSV files and created models'),
     dotted_path='importer.tasks.task_model_filer_load'
 )
```

### Comparing `mayan-importer-2.5.3/importer/serializers.py` & `mayan-importer-3.0/importer/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from .models import ImportSetup, ImportSetupItem
 
 
 class ImportSetupSerializer(serializers.HyperlinkedModelSerializer):
     clear_url = serializers.SerializerMethodField()
     credential = StoredCredentialSerializer(read_only=True)
     credential_id = serializers.IntegerField(
-        label=_('Credential ID'), required=False, write_only=True
+        label=_(message='Credential ID'), required=False, write_only=True
     )
     document_type = DocumentTypeSerializer(read_only=True)
     document_type_id = serializers.IntegerField(
-        label=_('Document type ID'), write_only=True
+        label=_(message='Document type ID'), write_only=True
     )
     item_list_url = serializers.SerializerMethodField()
     populate_url = serializers.SerializerMethodField()
     process_url = serializers.SerializerMethodField()
 
     class Meta:
         extra_kwargs = {
@@ -70,15 +70,15 @@
 class ImportSetupItemSerializer(serializers.HyperlinkedModelSerializer):
     import_setup_url = serializers.SerializerMethodField()
     url = serializers.SerializerMethodField()
 
     class Meta:
         fields = (
             'import_setup_url', 'id', 'identifier', 'serialized_data',
-            'state', 'state_data', 'url'
+            'state', 'url'
         )
         model = ImportSetupItem
 
     def get_import_setup_url(self, instance):
         return reverse(
             'rest_api:importsetup-detail', kwargs={
                 'import_setup_id': instance.import_setup_id,
```

### Comparing `mayan-importer-2.5.3/importer/tasks.py` & `mayan-importer-3.0/importer/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from django.apps import apps
 from django.contrib.auth import get_user_model
 
 from mayan.celery import app
 
 from .classes import ModelFiler
+from .literals import SETUP_ITEM_STATE_QUEUED
 
 logger = logging.getLogger(name=__name__)
 
 
 @app.task(ignore_result=True)
 def task_import_setup_process(import_setup_id):
     ImportSetup = apps.get_model(
@@ -23,15 +24,30 @@
 @app.task(ignore_result=True)
 def task_import_setup_item_process(import_setup_item_id):
     ImportSetupItem = apps.get_model(
         app_label='importer', model_name='ImportSetupItem'
     )
 
     import_setup_item = ImportSetupItem.objects.get(pk=import_setup_item_id)
-    import_setup_item.process()
+    import_setup_item.process(force=True)
+
+
+def task_import_setup_item_process_apply_async(**kwargs):
+    task_code_kwargs = kwargs['kwargs']
+    import_setup_item_id = task_code_kwargs['import_setup_item_id']
+
+    ImportSetupItem = apps.get_model(
+        app_label='importer', model_name='ImportSetupItem'
+    )
+
+    ImportSetupItem.objects.filter(pk=import_setup_item_id).update(
+        state=SETUP_ITEM_STATE_QUEUED
+    )
+
+    task_import_setup_item_process.apply_async(**kwargs)
 
 
 @app.task(ignore_result=True)
 def task_import_setup_populate(import_setup_id):
     ImportSetup = apps.get_model(
         app_label='importer', model_name='ImportSetup'
     )
```

### Comparing `mayan-importer-2.5.3/importer/tests/importers.py` & `mayan-importer-3.0/importer/tests/importers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 import shutil
 
 from django.core.files import File
 from django.utils.translation import ugettext_lazy as _
 
-from mayan.apps.documents.tests.literals import TEST_SMALL_DOCUMENT_PATH
+from mayan.apps.documents.tests.literals import TEST_FILE_SMALL_PATH
 from mayan.apps.storage.models import SharedUploadedFile
 from mayan.apps.storage.utils import NamedTemporaryFile
 
 from ..classes import ImportSetupBackend
 
 from .literals import (
     TEST_IMPORT_SETUP_ITEM_IDENTIFIER, TEST_IMPORT_SETUP_ITEM_NAME
@@ -27,25 +27,26 @@
     @staticmethod
     def get_test_item():
         return TestImporterItem(
             id=TEST_IMPORT_SETUP_ITEM_IDENTIFIER,
             name=TEST_IMPORT_SETUP_ITEM_NAME
         )
 
+    @staticmethod
+    def get_item_list():
+        return [TestImporter.get_test_item()]
+
     def item_process(self, identifier, data):
         # Copy the Dropbox file to a temporary location using streaming
         # download.
         # The create a shared upload instance from the temporary file.
-        with open(TEST_SMALL_DOCUMENT_PATH, mode='rb') as document_file_object:
+        with open(TEST_FILE_SMALL_PATH, mode='rb') as document_file_object:
             with NamedTemporaryFile() as file_object:
                 shutil.copyfileobj(
                     fsrc=document_file_object, fdst=file_object
                 )
 
                 file_object.seek(0)
 
                 return SharedUploadedFile.objects.create(
                     file=File(file_object),
                 )
-
-    def get_item_list(self):
-        return [TestImporter.get_test_item()]
```

### Comparing `mayan-importer-2.5.3/importer/tests/mixins.py` & `mayan-importer-3.0/importer/tests/mixins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from django.db.models import Q
 
-from ..models import ImportSetup, ImportSetupAction
+from ..models import ImportSetup
 
 from .literals import (
-    TEST_IMPORT_SETUP_ACTION_BACKEND_PATH, TEST_IMPORT_SETUP_ACTION_LABEL,
-    TEST_IMPORT_SETUP_ACTION_LABEL_EDITED,
     TEST_IMPORT_SETUP_ITEM_IDENTIFIER_EDITED,
     TEST_IMPORT_SETUP_ITEM_TIME_BUFFER, TEST_IMPORT_SETUP_LABEL,
     TEST_IMPORT_SETUP_LABEL_EDITED, TEST_IMPORT_SETUP_PROCESS_SIZE,
     TEST_IMPORTER_BACKEND_PATH
 )
 from .importers import TestImporter
 
 
 class ImportSetupAPIViewTestMixin:
     def _request_test_import_setup_create_api_view(self):
-        pk_list = list(ImportSetup.objects.values_list('pk', flat=True))
+        pk_list = list(
+            ImportSetup.objects.values_list('pk', flat=True)
+        )
 
         response = self.post(
             viewname='rest_api:importsetup-list', data={
                 'label': TEST_IMPORT_SETUP_LABEL,
                 'backend_path': TEST_IMPORTER_BACKEND_PATH,
-                'document_type_id': self.test_document_type.pk
+                'document_type_id': self._test_document_type.pk
             }
         )
 
         try:
             self.test_import_setup = ImportSetup.objects.get(
                 ~Q(pk__in=pk_list)
             )
@@ -67,77 +67,14 @@
             }
         )
 
     def _request_test_import_setup_list_api_view(self):
         return self.get(viewname='rest_api:importsetup-list')
 
 
-class ImportSetupActionTestMixin:
-    def _create_test_import_setup_action(self):
-        self.test_import_setup_action = self.test_import_setup.actions.create(
-            backend_path=TEST_IMPORT_SETUP_ACTION_BACKEND_PATH,
-            label=TEST_IMPORT_SETUP_ACTION_LABEL,
-        )
-
-
-class ImportSetupActionViewTestMixin:
-    def _request_test_import_setup_action_backend_selection_view(self):
-        return self.post(
-            viewname='importer:import_setup_action_backend_selection', kwargs={
-                'import_setup_id': self.test_import_setup.pk
-            }, data={
-                'class_path': TEST_IMPORT_SETUP_ACTION_BACKEND_PATH,
-            }
-        )
-
-    def _request_test_import_setup_action_create_view(self):
-        pk_list = list(ImportSetupAction.objects.values_list('pk', flat=True))
-
-        response = self.post(
-            viewname='importer:import_setup_action_create', kwargs={
-                'import_setup_id': self.test_import_setup.pk,
-                'class_path': TEST_IMPORT_SETUP_ACTION_BACKEND_PATH
-            }, data={
-                'label': TEST_IMPORT_SETUP_ACTION_LABEL,
-            }
-        )
-
-        try:
-            self.test_import_setup_action = ImportSetupAction.objects.get(
-                ~Q(pk__in=pk_list)
-            )
-        except ImportSetupAction.DoesNotExist:
-            self.test_import_setup_action = None
-
-        return response
-
-    def _request_test_import_setup_action_delete_view(self):
-        return self.post(
-            viewname='importer:import_setup_action_delete', kwargs={
-                'import_setup_action_id': self.test_import_setup_action.pk
-            }
-        )
-
-    def _request_test_import_setup_action_edit_view(self):
-        return self.post(
-            viewname='importer:import_setup_action_edit', kwargs={
-                'import_setup_action_id': self.test_import_setup_action.pk
-            }, data={
-                'label': TEST_IMPORT_SETUP_ACTION_LABEL_EDITED,
-            }
-        )
-
-    def _request_test_import_setup_action_list_view(self):
-        return self.get(
-            viewname='importer:import_setup_action_list', kwargs={
-                'import_setup_id': self.test_import_setup.pk
-            }
-        )
-
-
 class ImportSetupItemAPIViewTestMixin:
     def _request_test_import_setup_clear_api_view(self):
         return self.post(
             viewname='rest_api:importsetup-clear', kwargs={
                 'import_setup_id': self.test_import_setup.pk
             }
         )
@@ -201,42 +138,45 @@
 
 
 class ImportSetupTestMixin:
     def _create_test_import_setup(self):
         self.test_import_setup = ImportSetup.objects.create(
             backend_path=TEST_IMPORTER_BACKEND_PATH,
             label=TEST_IMPORT_SETUP_LABEL,
-            document_type=self.test_document_type
+            document_type=self._test_document_type
         )
 
 
 class ImportSetupItemTestMixin:
     def _create_test_import_setup_item(self):
-        test_item_list = TestImporter().get_item_list()
+        test_item_list = TestImporter.get_item_list()
+
         self.test_import_setup_item = self.test_import_setup.items.create(
             identifier=test_item_list[0].id
         )
 
 
 class ImportSetupViewTestMixin:
     def _request_test_import_setup_backend_selection_view(self):
         return self.post(
             viewname='importer:import_setup_backend_selection', data={
                 'backend': TEST_IMPORTER_BACKEND_PATH,
             }
         )
 
     def _request_test_import_setup_create_view(self):
-        pk_list = list(ImportSetup.objects.values_list('pk', flat=True))
+        pk_list = list(
+            ImportSetup.objects.values_list('pk', flat=True)
+        )
 
         repsonse = self.post(
             viewname='importer:import_setup_create', kwargs={
-                'class_path': TEST_IMPORTER_BACKEND_PATH
+                'backend_path': TEST_IMPORTER_BACKEND_PATH
             }, data={
-                'document_type': self.test_document_type.pk,
+                'document_type': self._test_document_type.pk,
                 'label': TEST_IMPORT_SETUP_LABEL,
                 'item_time_buffer': TEST_IMPORT_SETUP_ITEM_TIME_BUFFER,
                 'process_size': TEST_IMPORT_SETUP_PROCESS_SIZE
             }
         )
 
         try:
@@ -256,16 +196,16 @@
         )
 
     def _request_test_import_setup_edit_view(self):
         return self.post(
             viewname='importer:import_setup_edit', kwargs={
                 'import_setup_id': self.test_import_setup.pk
             }, data={
-                'credential': self.test_stored_credential.pk,
-                'document_type': self.test_document_type.pk,
+                'credential': self._test_stored_credential.pk,
+                'document_type': self._test_document_type.pk,
                 'item_time_buffer': TEST_IMPORT_SETUP_ITEM_TIME_BUFFER,
                 'label': TEST_IMPORT_SETUP_LABEL_EDITED,
                 'process_size': TEST_IMPORT_SETUP_PROCESS_SIZE
             }
         )
 
     def _request_test_import_setup_list_view(self):
```

### Comparing `mayan-importer-2.5.3/importer/tests/test_import_setup_api.py` & `mayan-importer-3.0/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-2.5.3/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.0/importer/tests/test_import_setup_item_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rest_framework import status
 
-from credentials.tests.mixins import StoredCredentialTestMixin
+from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.tests.mixins.document_mixins import DocumentTestMixin
 from mayan.apps.rest_api.tests.base import BaseAPITestCase
 
 from ..events import (
     event_import_setup_item_edited, event_import_setup_item_deleted
 )
 from ..permissions import (
```

### Comparing `mayan-importer-2.5.3/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.0/importer/tests/test_import_setup_item_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
+from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.events import (
     event_document_created, event_document_file_created,
     event_document_file_edited, event_document_version_created,
     event_document_version_page_created
 )
 from mayan.apps.documents.models.document_models import Document
 from mayan.apps.documents.tests.base import GenericDocumentViewTestCase
 
-from credentials.tests.mixins import StoredCredentialTestMixin
-
 from ..events import (
-    event_import_setup_item_completed, event_import_setup_item_created,
+    event_import_setup_item_finished, event_import_setup_item_created,
     event_import_setup_item_deleted, event_import_setup_item_edited,
-    event_import_setup_populate_ended, event_import_setup_populate_started,
-    event_import_setup_process_ended, event_import_setup_process_started
+    event_import_setup_populate_finished, event_import_setup_populate_started,
+    event_import_setup_process_finished, event_import_setup_process_started
 )
 from ..permissions import (
     permission_import_setup_edit, permission_import_setup_process
 )
 
 from .mixins import (
     ImportSetupTestMixin, ImportSetupItemTestMixin,
@@ -227,50 +226,50 @@
             events[2].verb, event_import_setup_item_edited.id
         )
 
         self.assertEqual(events[3].action_object, None)
         self.assertEqual(events[3].actor, self.test_import_setup)
         self.assertEqual(events[3].target, self.test_import_setup)
         self.assertEqual(
-            events[3].verb, event_import_setup_populate_ended.id
+            events[3].verb, event_import_setup_populate_finished.id
         )
 
     def test_import_setup_process_view_no_permission(self):
         self._create_test_import_setup_item()
 
-        document_count = self.test_document_type.documents.count()
+        document_count = self._test_document_type.documents.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_process_view()
         self.assertEqual(response.status_code, 404)
 
         self.assertEqual(
-            self.test_document_type.documents.count(), document_count
+            self._test_document_type.documents.count(), document_count
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 0)
 
     def test_import_setup_process_view_with_access(self):
         self._create_test_import_setup_item()
 
         self.grant_access(
             obj=self.test_import_setup,
             permission=permission_import_setup_process
         )
-        document_count = self.test_document_type.documents.count()
+        document_count = self._test_document_type.documents.count()
 
         self._clear_events()
 
         response = self._request_test_import_setup_process_view()
         self.assertEqual(response.status_code, 302)
 
         self.assertEqual(
-            self.test_document_type.documents.count(), document_count + 1
+            self._test_document_type.documents.count(), document_count + 1
         )
 
         events = self._get_test_events()
         self.assertEqual(events.count(), 10)
 
         test_document = Document.objects.last()
         test_document_file = test_document.file_latest
@@ -287,15 +286,15 @@
         )
 
         self.assertEqual(events[1].action_object, self.test_import_setup)
         self.assertEqual(events[1].actor, test_import_setup_item)
         self.assertEqual(events[1].target, test_import_setup_item)
         self.assertEqual(events[1].verb, event_import_setup_item_edited.id)
 
-        self.assertEqual(events[2].action_object, self.test_document_type)
+        self.assertEqual(events[2].action_object, self._test_document_type)
         self.assertEqual(events[2].actor, test_document)
         self.assertEqual(events[2].target, test_document)
         self.assertEqual(events[2].verb, event_document_created.id)
 
         self.assertEqual(events[3].action_object, self.test_import_setup)
         self.assertEqual(events[3].actor, test_import_setup_item)
         self.assertEqual(events[3].target, test_import_setup_item)
@@ -323,14 +322,14 @@
             events[7].verb, event_document_version_page_created.id
         )
 
         self.assertEqual(events[8].action_object, self.test_import_setup)
         self.assertEqual(events[8].actor, self.test_import_setup_item)
         self.assertEqual(events[8].target, self.test_import_setup_item)
         self.assertEqual(
-            events[8].verb, event_import_setup_item_completed.id
+            events[8].verb, event_import_setup_item_finished.id
         )
 
         self.assertEqual(events[9].action_object, None)
         self.assertEqual(events[9].actor, self.test_import_setup)
         self.assertEqual(events[9].target, self.test_import_setup)
-        self.assertEqual(events[9].verb, event_import_setup_process_ended.id)
+        self.assertEqual(events[9].verb, event_import_setup_process_finished.id)
```

### Comparing `mayan-importer-2.5.3/importer/tests/test_import_setup_views.py` & `mayan-importer-3.0/importer/tests/test_import_setup_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+from mayan.apps.credentials.tests.mixins import StoredCredentialTestMixin
 from mayan.apps.documents.tests.base import GenericDocumentViewTestCase
 
-from credentials.tests.mixins import StoredCredentialTestMixin
-
 from ..events import event_import_setup_created, event_import_setup_edited
 from ..models import ImportSetup
 from ..permissions import (
     permission_import_setup_create, permission_import_setup_delete,
     permission_import_setup_edit, permission_import_setup_view
 )
```

### Comparing `mayan-importer-2.5.3/importer/urls.py` & `mayan-importer-3.0/importer/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,86 +2,50 @@
 
 from .api_views import (
     APIImportSetupClearView, APIImportSetupDetailView,
     APIImportSetupListView, APIImportSetupPopulateView,
     APIImportSetupProcessView, APIImportSetupItemDetailView,
     APIImportSetupItemListView
 )
-from .views.import_setup_action_views import (
-    ImportSetupActionCreateView, ImportSetupActionDeleteView,
-    ImportSetupActionEditView, ImportSetupActionListView,
-    ImportSetupActionBackendSelectionView
-)
 from .views.import_setup_item_views import (
     ImportSetupClearView, ImportSetupItemDeleteView,
     ImportSetupItemDocumentListView, ImportSetupItemEditView,
     ImportSetupItemListView, ImportSetupItemLoadView,
     ImportSetupItemProcessView, ImportSetupItemSaveConfirmView,
     ImportSetupPopulateView, ImportSetupProcessView
 )
 from .views.import_setup_views import (
     ImportSetupBackendSelectionView,
     ImportSetupCreateView, ImportSetupDeleteView, ImportSetupEditView,
-    ImportSetupLogListView, ImportSetupListView
+    ImportSetupListView
 )
 
+
 urlpatterns_import_setup = [
     url(
         regex=r'^import_setups/$', name='import_setup_list',
         view=ImportSetupListView.as_view()
     ),
     url(
         regex=r'^import_setups/backend/selection/$',
         name='import_setup_backend_selection',
         view=ImportSetupBackendSelectionView.as_view()
     ),
     url(
-        regex=r'^import_setups/(?P<class_path>[a-zA-Z0-9_.]+)/create/$',
+        regex=r'^import_setups/(?P<backend_path>[a-zA-Z0-9_.]+)/create/$',
         name='import_setup_create',
         view=ImportSetupCreateView.as_view()
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/delete/$',
         name='import_setup_delete', view=ImportSetupDeleteView.as_view()
     ),
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/edit/$',
         name='import_setup_edit', view=ImportSetupEditView.as_view()
-    ),
-    url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/logs/$',
-        name='import_setup_log_list', view=ImportSetupLogListView.as_view()
-    )
-]
-
-urlpatterns_import_setup_actions = [
-    url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/actions/$',
-        name='import_setup_action_list',
-        view=ImportSetupActionListView.as_view()
-    ),
-    url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/actions/(?P<class_path>[a-zA-Z0-9_.]+)/create/$',
-        name='import_setup_action_create',
-        view=ImportSetupActionCreateView.as_view()
-    ),
-    url(
-        regex=r'^import_setups/actions/(?P<import_setup_action_id>\d+)/delete/$',
-        name='import_setup_action_delete',
-        view=ImportSetupActionDeleteView.as_view()
-    ),
-    url(
-        regex=r'^import_setups/actions/(?P<import_setup_action_id>\d+)/edit/$',
-        name='import_setup_action_edit',
-        view=ImportSetupActionEditView.as_view()
-    ),
-    url(
-        regex=r'^import_setups/(?P<import_setup_id>\d+)/actions/selection/$',
-        name='import_setup_action_backend_selection',
-        view=ImportSetupActionBackendSelectionView.as_view()
     )
 ]
 
 urlpatterns_import_setup_items = [
     url(
         regex=r'^import_setups/(?P<import_setup_id>\d+)/clear/$',
         name='import_setup_clear',
@@ -135,28 +99,37 @@
     ),
     url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/documents/$',
         name='import_setup_item_document_list',
         view=ImportSetupItemDocumentListView.as_view()
     ),
     url(
+        regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/delete/$',
+        name='import_setup_item_delete',
+        view=ImportSetupItemDeleteView.as_view()
+    ),
+    url(
         regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/edit/$',
         name='import_setup_item_edit',
         view=ImportSetupItemEditView.as_view()
     ),
     url(
         regex=r'^import_setups/items/multiple/process/$',
         name='import_setup_item_multiple_process',
         view=ImportSetupItemProcessView.as_view()
-    )
+    ),
+    url(
+        regex=r'^import_setups/items/(?P<import_setup_item_id>\d+)/process/$',
+        name='import_setup_item_process',
+        view=ImportSetupItemProcessView.as_view()
+    ),
 ]
 
 urlpatterns = []
 urlpatterns.extend(urlpatterns_import_setup)
-urlpatterns.extend(urlpatterns_import_setup_actions)
 urlpatterns.extend(urlpatterns_import_setup_items)
 
 api_urls = [
     url(
         regex=r'^import_setups/$', name='importsetup-list',
         view=APIImportSetupListView.as_view()
     ),
```

### Comparing `mayan-importer-2.5.3/importer/views/import_setup_item_views.py` & `mayan-importer-3.0/importer/views/import_setup_item_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 from ..models import ImportSetup, ImportSetupItem
 from ..permissions import (
     permission_import_setup_edit, permission_import_setup_process,
     permission_import_setup_view, permission_model_filer_load,
     permission_model_filer_save
 )
 from ..tasks import (
-    task_import_setup_item_process, task_import_setup_populate,
+    task_import_setup_item_process_apply_async, task_import_setup_populate,
     task_import_setup_process, task_model_filer_load, task_model_filer_save
 )
 
 logger = logging.getLogger(name=__name__)
 
 
 class ImportSetupClearView(MultipleObjectConfirmActionView):
     model = ImportSetup
     object_permission = permission_import_setup_process
     pk_url_kwarg = 'import_setup_id'
-    success_message = _('%(count)d import setup cleared.')
-    success_message_plural = _('%(count)d import setups cleared.')
+    success_message = _(message='%(count)d import setup cleared.')
+    success_message_plural = _(message='%(count)d import setups cleared.')
     view_icon = icon_import_setup_clear
 
     def get_extra_context(self):
         queryset = self.object_list
 
         result = {
             'title': ungettext(
@@ -59,60 +59,64 @@
             )
         }
 
         if queryset.count() == 1:
             result.update(
                 {
                     'object': queryset.first(),
-                    'title': _('Clear import setup: %s') % queryset.first()
+                    'title': _(
+                        message='Clear import setup: %s'
+                    ) % queryset.first()
                 }
             )
 
         return result
 
     def get_instance_extra_data(self):
-        return {
-            '_event_actor': self.request.user,
-        }
+        return {'_event_actor': self.request.user}
 
     def object_action(self, instance, form=None):
         instance.clear()
 
 
 class ImportSetupItemDeleteView(MultipleObjectConfirmActionView):
     model = ImportSetupItem
     object_permission = permission_import_setup_edit
     pk_url_kwarg = 'import_setup_item_id'
-    success_message = _('%(count)d import setup item deleted.')
-    success_message_plural = _('%(count)d import setup items deleted.')
+    success_message = _(message='%(count)d import setup item deleted.')
+    success_message_plural = _(
+        message='%(count)d import setup items deleted.'
+    )
     view_icon = icon_import_setup_item_delete
 
     def get_extra_context(self):
         queryset = self.object_list
 
         result = {
             'delete_view': True,
             'import_setup': self.object_list.first().import_setup,
             'message': _(
-                'You can add this item again by executing the prepare '
-                'action.'
+                message='You can add this item again by executing the '
+                'prepare action.'
             ),
             'navigation_object_list': ('import_setup', 'object'),
             'title': ungettext(
                 singular='Delete the selected import setup item?',
                 plural='Delete the selected import setup items?',
                 number=queryset.count()
             )
         }
 
         if queryset.count() == 1:
             result.update(
                 {
                     'object': queryset.first(),
-                    'title': _('Delete import setup item: %s') % queryset.first()
+                    'title': _(
+                        message='Delete import setup item: %s'
+                    ) % queryset.first()
                 }
             )
 
         return result
 
     def get_instance_extra_data(self):
         return {
@@ -128,30 +132,25 @@
         )
 
     def object_action(self, instance, form=None):
         instance.delete()
 
 
 class ImportSetupItemEditView(SingleObjectEditView):
-    fields = (
-        'identifier', 'serialized_data', 'serialized_data', 'state',
-        'state_data'
-    )
+    fields = ('identifier', 'serialized_data', 'serialized_data', 'state')
     model = ImportSetupItem
     object_permission = permission_import_setup_edit
     pk_url_kwarg = 'import_setup_item_id'
     view_icon = icon_import_setup_item_edit
 
     def get_extra_context(self):
         return {
             'import_setup': self.object.import_setup,
             'navigation_object_list': ('import_setup', 'object'),
-            'title': _(
-                'Edit import setup item: %s'
-            ) % self.object
+            'title': _(message='Edit import setup item: %s') % self.object
         }
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user
         }
 
@@ -173,22 +172,23 @@
             {
                 'import_setup': self.external_object.import_setup,
                 'import_setup_item': self.external_object,
                 'navigation_object_list': (
                     'import_setup', 'import_setup_item'
                 ),
                 'no_results_text': _(
-                    'This view will list the documents that were created '
-                    'by an import setup item.'
+                    message='This view will list the documents that were '
+                    'created by an import setup item.'
                 ),
                 'no_results_title': _(
-                    'There are no documents for this import setup item.'
+                    message='There are no documents for this import setup '
+                    'item.'
                 ),
                 'title': _(
-                    'Document created from import setup item: %s'
+                    message='Document created from import setup item: %s'
                 ) % self.external_object
             }
         )
         return context
 
 
 class ImportSetupItemListView(ExternalObjectViewMixin, SingleObjectListView):
@@ -213,32 +213,36 @@
                     context=RequestContext(
                         dict_={'object': self.external_object},
                         request=self.request
                     )
                 ),
             ),
             'no_results_text': _(
-                'Import setups items are the entries for the actual '
+                message='Import setups items are the entries for the actual '
                 'files that will be imported and converted into documents.'
             ),
-            'no_results_title': _('No import setups items available'),
+            'no_results_title': _(message='No import setups items available'),
             'object': self.external_object,
-            'title': _('Items of import setup: %s') % self.external_object
+            'title': _(
+                message='Items of import setup: %s'
+            ) % self.external_object
         }
 
     def get_source_queryset(self):
         return self.external_object.items.all()
 
 
 class ImportSetupItemProcessView(MultipleObjectConfirmActionView):
     model = ImportSetupItem
     object_permission = permission_import_setup_process
     pk_url_kwarg = 'import_setup_item_id'
-    success_message = _('%(count)d import setup item processed.')
-    success_message_plural = _('%(count)d import setup items processed.')
+    success_message = _(message='%(count)d import setup item processed.')
+    success_message_plural = _(
+        message='%(count)d import setup items processed.'
+    )
     view_icon = icon_import_setup_item_process
 
     def get_extra_context(self):
         queryset = self.object_list
 
         result = {
             'import_setup': self.object_list.first().import_setup,
@@ -250,15 +254,17 @@
             )
         }
 
         if queryset.count() == 1:
             result.update(
                 {
                     'object': queryset.first(),
-                    'title': _('Process import setup item: %s') % queryset.first()
+                    'title': _(
+                        message='Process import setup item: %s'
+                    ) % queryset.first()
                 }
             )
 
         return result
 
     def get_instance_extra_data(self):
         return {
@@ -270,18 +276,16 @@
         return reverse(
             viewname='importer:import_setup_items_list', kwargs={
                 'import_setup_id': self.object_list[0].import_setup.pk
             }
         )
 
     def object_action(self, instance, form=None):
-        task_import_setup_item_process.apply_async(
-            kwargs={
-                'import_setup_item_id': instance.pk
-            }
+        task_import_setup_item_process_apply_async(
+            kwargs={'import_setup_item_id': instance.pk}
         )
 
 
 class ImportSetupItemLoadView(ExternalObjectViewMixin, FormView):
     external_object_class = ImportSetup
     external_object_object_permission = permission_model_filer_load
     external_object_pk_url_kwarg = 'import_setup_id'
@@ -302,26 +306,27 @@
                 'field_defaults': {'import_setup_id': self.external_object.pk},
                 'full_model_name': full_model_name,
                 'shared_upload_file_id': shared_upload_file.pk
             }
         )
 
         messages.success(
-            message=_('File uploaded and queued for loading as models.'),
-            request=self.request
+            message=_(
+                message='File uploaded and queued for loading as models.'
+            ), request=self.request
         )
         return HttpResponseRedirect(
             redirect_to=reverse(viewname='importer:import_setup_list')
         )
 
     def get_extra_context(self):
         return {
             'object': self.external_object,
             'title': _(
-                'Load the items of import setup: %s'
+                message='Load the items of import setup: %s'
             ) % self.external_object
         }
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user,
         }
@@ -333,15 +338,15 @@
     external_object_pk_url_kwarg = 'import_setup_id'
     view_icon = icon_model_filer_save
 
     def get_extra_context(self):
         return {
             'object': self.external_object,
             'title': _(
-                'Save the items of import setup: %s'
+                message='Save the items of import setup: %s'
             ) % self.external_object
         }
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user,
         }
@@ -352,15 +357,15 @@
         )
 
         task_model_filer_save.apply_async(
             kwargs={
                 'filter_kwargs': {'import_setup': self.external_object.pk},
                 'full_model_name': full_model_name,
                 'save_file_title': str(
-                    _('Import setup "%s"') % self.external_object
+                    _(message='Import setup "%s"') % self.external_object
                 ),
                 'organization_installation_url': get_organization_installation_url(
                     request=self.request
                 ),
                 'user_id': self.request.user.pk
             }
         )
@@ -369,25 +374,29 @@
 class ImportSetupPopulateView(MultipleObjectConfirmActionView):
     model = ImportSetup
     object_permission = permission_import_setup_process
     pk_url_kwarg = 'import_setup_id'
     post_action_redirect = reverse_lazy(
         viewname='importer:import_setup_list'
     )
-    success_message = _('%(count)d import setup item population queued.')
-    success_message_plural = _('%(count)d import setups item population queued.')
+    success_message = _(
+        message='%(count)d import setup item population queued.'
+    )
+    success_message_plural = _(
+        message='%(count)d import setups item population queued.'
+    )
     view_icon = icon_import_setup_populate
 
     def get_extra_context(self):
         queryset = self.object_list
 
         result = {
             'message': _(
-                'This process will populate the items to import by querying '
-                'the source repository. The process will run in the '
+                message='This process will populate the items to import by '
+                'querying the source repository. The process will run in the '
                 'background and once starter, cannot be stopped from the '
                 'user interface. The time to completion will depend on the '
                 'number of files that match the import setup criteria, the '
                 'import backend, the size of the source repository, and '
                 'the bandwidth between Mayan EDMS and the source '
                 'repository. The completion may take between a few minutes '
                 'to a few days to complete.'
@@ -399,15 +408,17 @@
             )
         }
 
         if queryset.count() == 1:
             result.update(
                 {
                     'object': queryset.first(),
-                    'title': _('Prepare import setup: %s') % queryset.first()
+                    'title': _(
+                        message='Prepare import setup: %s'
+                    ) % queryset.first()
                 }
             )
 
         return result
 
     def get_instance_extra_data(self):
         return {
@@ -423,16 +434,18 @@
 class ImportSetupProcessView(MultipleObjectConfirmActionView):
     model = ImportSetup
     object_permission = permission_import_setup_process
     pk_url_kwarg = 'import_setup_id'
     post_action_redirect = reverse_lazy(
         viewname='importer:import_setup_list'
     )
-    success_message = _('%(count)d import setup processing queued.')
-    success_message_plural = _('%(count)d import setups processing queued.')
+    success_message = _(message='%(count)d import setup processing queued.')
+    success_message_plural = _(
+        message='%(count)d import setups processing queued.'
+    )
     view_icon = icon_import_setup_process
 
     def get_extra_context(self):
         queryset = self.object_list
 
         result = {
             'title': ungettext(
@@ -442,31 +455,33 @@
             )
         }
 
         if queryset.count() == 1:
             result.update(
                 {
                     'object': queryset.first(),
-                    'title': _('Process import setup: %s') % queryset.first()
+                    'title': _(
+                        message='Process import setup: %s'
+                    ) % queryset.first()
                 }
             )
 
         return result
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user,
         }
 
     def object_action(self, instance, form=None):
         if instance.items.count() == 0:
             messages.warning(
                 message=_(
-                    'Import setup "%s" does not have any item to process. '
-                    'Use the prepare action first.'
+                    message='Import setup "%s" does not have any item to '
+                    'process. Use the prepare action first.'
                 ) % instance, request=self.request
             )
         else:
             task_import_setup_process.apply_async(
                 kwargs={
                     'import_setup_id': instance.pk
                 }
```

### Comparing `mayan-importer-2.5.3/importer/views/import_setup_views.py` & `mayan-importer-3.0/importer/views/import_setup_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import logging
 
-from django.http import Http404, HttpResponseRedirect
+from django.http import HttpResponseRedirect
 from django.template import RequestContext
 from django.urls import reverse, reverse_lazy
 from django.utils.translation import ugettext_lazy as _
 
+from mayan.apps.backends.views import (
+    ViewSingleObjectDynamicFormModelBackendCreate,
+    ViewSingleObjectDynamicFormModelBackendEdit
+)
 from mayan.apps.views.generics import (
-    FormView, SingleObjectDeleteView, SingleObjectDynamicFormCreateView,
-    SingleObjectDynamicFormEditView, SingleObjectListView
+    FormView, SingleObjectDeleteView, SingleObjectListView
 )
-from mayan.apps.views.view_mixins import ExternalObjectViewMixin
 
 from ..classes import ImportSetupBackend
 from ..forms import (
     ImportSetupBackendSelectionForm, ImportSetupBackendDynamicForm
 )
 from ..icons import (
     icon_import_setup_backend_selection, icon_import_setup_delete,
-    icon_import_setup_edit, icon_import_setup_list,
-    icon_import_setup_log_list
+    icon_import_setup_edit, icon_import_setup_list
 )
 from ..links import link_import_setup_backend_selection
 from ..models import ImportSetup
 from ..permissions import (
     permission_import_setup_create, permission_import_setup_delete,
     permission_import_setup_edit, permission_import_setup_view
 )
@@ -35,69 +36,45 @@
         'title': _('New import backend selection')
     }
     form_class = ImportSetupBackendSelectionForm
     view_icon = icon_import_setup_backend_selection
     view_permission = permission_import_setup_create
 
     def form_valid(self, form):
-        backend_class = form.cleaned_data['backend']
+        backend = form.cleaned_data['backend']
         return HttpResponseRedirect(
             redirect_to=reverse(
-                viewname='importer:import_setup_create', kwargs={
-                    'class_path': backend_class
-                }
+                kwargs={'backend_path': backend},
+                viewname='importer:import_setup_create'
             )
         )
 
 
-class ImportSetupCreateView(SingleObjectDynamicFormCreateView):
+class ImportSetupCreateView(ViewSingleObjectDynamicFormModelBackendCreate):
+    backend_class = ImportSetupBackend
     form_class = ImportSetupBackendDynamicForm
-    post_action_redirect = reverse_lazy(
-        viewname='importer:import_setup_list'
-    )
+    post_action_redirect = reverse_lazy(viewname='importer:import_setup_list')
     view_icon = icon_import_setup_backend_selection
     view_permission = permission_import_setup_create
 
-    def get_backend(self):
-        try:
-            return ImportSetupBackend.get(
-                name=self.kwargs['class_path']
-            )
-        except KeyError:
-            raise Http404(
-                '{} class not found'.format(
-                    self.kwargs['class_path']
-                )
-            )
-
     def get_extra_context(self):
         backend_class = self.get_backend_class()
         return {
             'title': _(
                 'Create a "%s" import setup'
             ) % backend_class.label
         }
 
-    def get_form_schema(self):
-        backend_class = self.get_backend_class()
-        result = {
-            'fields': backend_class.fields,
-            'widgets': getattr(
-                backend_class, 'widgets', {}
-            )
-        }
-        if hasattr(backend_class, 'field_order'):
-            result['field_order'] = backend_class.field_order
-
-        return result
+    def get_form_extra_kwargs(self):
+        return {'user': self.request.user}
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user,
-            'backend_path': self.kwargs['class_path']
+            'backend_path': self.kwargs['backend_path']
         }
 
 
 class ImportSetupDeleteView(SingleObjectDeleteView):
     model = ImportSetup
     object_permission = permission_import_setup_delete
     pk_url_kwarg = 'import_setup_id'
@@ -108,39 +85,29 @@
         return {
             'import_setup': None,
             'object': self.object,
             'title': _('Delete the import setup: %s?') % self.object
         }
 
 
-class ImportSetupEditView(SingleObjectDynamicFormEditView):
+class ImportSetupEditView(ViewSingleObjectDynamicFormModelBackendEdit):
     form_class = ImportSetupBackendDynamicForm
     model = ImportSetup
     object_permission = permission_import_setup_edit
     pk_url_kwarg = 'import_setup_id'
     view_icon = icon_import_setup_edit
 
     def get_extra_context(self):
         return {
             'object': self.object,
             'title': _('Edit import setup: %s') % self.object
         }
 
-    def get_form_schema(self):
-        backend_class = self.object.get_backend_class()
-        result = {
-            'fields': backend_class.fields,
-            'widgets': getattr(
-                backend_class, 'widgets', {}
-            )
-        }
-        if hasattr(backend_class, 'field_order'):
-            result['field_order'] = backend_class.field_order
-
-        return result
+    def get_form_extra_kwargs(self):
+        return {'user': self.request.user}
 
     def get_instance_extra_data(self):
         return {
             '_event_actor': self.request.user
         }
 
 
@@ -161,34 +128,7 @@
                 'Import setups are configuration units that will retrieve '
                 'files for external locations and create documents from '
                 'them.'
             ),
             'no_results_title': _('No import setups available'),
             'title': _('Import setups')
         }
-
-
-class ImportSetupLogListView(ExternalObjectViewMixin, SingleObjectListView):
-    external_object_class = ImportSetup
-    external_object_permission = permission_import_setup_view
-    external_object_pk_url_kwarg = 'import_setup_id'
-    view_icon = icon_import_setup_log_list
-
-    def get_extra_context(self):
-        return {
-            'hide_object': True,
-            'no_results_icon': icon_import_setup_log_list,
-            'no_results_text': _(
-                'This view displays the error log for import setups. '
-                'An empty list is a good thing.'
-            ),
-            'no_results_title': _(
-                'There are no error log entries'
-            ),
-            'object': self.external_object,
-            'title': _(
-                'Log entries for import setup: %s'
-            ) % self.external_object
-        }
-
-    def get_source_queryset(self):
-        return self.external_object.logs.all()
```

### Comparing `mayan-importer-2.5.3/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.0/mayan_importer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 2.5.3
+Version: 3.0
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Communications :: File Sharing
 Requires-Python: !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 License-File: LICENSE
+Requires-Dist: dropbox==10.4.1
 
 ===========
 Description
 ===========
 
 Mayan EDMS app to migrate files from external sources.
 
@@ -92,14 +93,28 @@
 - Generate an Access Token with no expiration.
 - Create a credential instance in the Mayan EDMS Importer app and enter the Access Token.
 - Create an Import Setup that will filter the files to fetch from Dropbox.
 - Click the "Populate" button and check that the item count is correct.
 - Click the "Process" button to start the import process.
 
 
+3.0 (2024-04-01)
+================
+- Refactor app.
+- Remove import setup action.
+- Use source metadata to store import metadata.
+- Don't deserialize import item source column.
+- Use upstream backend, dynamic forms, credentials mixins, model mixins,
+  error log.
+- Use fieldsets.
+- Bring code standards up to series 4.5.
+- Support processing and deleting individual setup item entries.
+- Improve import setup and import setup item state handling.
+- Improve navigation, add return links.
+
 2.5.2 (2024-02-22)
 ==================
 - Fix credential `get_backend` usage.
 - Code styles updates.
 - Add view icons.
 
 2.5.1 (2024-02-20)
```

### Comparing `mayan-importer-2.5.3/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.0/mayan_importer.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 importer/apps.py
 importer/classes.py
 importer/dependencies.py
 importer/events.py
 importer/exceptions.py
 importer/forms.py
 importer/icons.py
-importer/import_setup_actions.py
 importer/importers.py
 importer/links.py
 importer/literals.py
 importer/permissions.py
 importer/queues.py
 importer/serializers.py
 importer/tasks.py
@@ -35,34 +34,31 @@
 importer/migrations/0010_remove_importsetup_metadata_map.py
 importer/migrations/0011_auto_20201004_0042.py
 importer/migrations/0012_importsetupitem_documents.py
 importer/migrations/0013_auto_20201225_0155.py
 importer/migrations/0014_auto_20201227_0610.py
 importer/migrations/0015_auto_20220901_0932.py
 importer/migrations/0016_importsetup_item_time_buffer.py
+importer/migrations/0017_delete_importsetuplog.py
+importer/migrations/0018_auto_20240401_0808.py
 importer/migrations/__init__.py
 importer/models/__init__.py
-importer/models/import_setup_action_models.py
+importer/models/import_setup_item_model_mixins.py
 importer/models/import_setup_item_models.py
+importer/models/import_setup_model_mixins.py
 importer/models/import_setup_models.py
-importer/models/mixins.py
-importer/templatetags/__init__.py
-importer/templatetags/templating_tags.py
 importer/tests/__init__.py
-importer/tests/import_setup_actions.py
 importer/tests/importers.py
 importer/tests/literals.py
 importer/tests/mixins.py
-importer/tests/test_import_setup_action_views.py
 importer/tests/test_import_setup_api.py
 importer/tests/test_import_setup_item_api.py
 importer/tests/test_import_setup_item_views.py
 importer/tests/test_import_setup_views.py
 importer/views/__init__.py
-importer/views/import_setup_action_views.py
 importer/views/import_setup_item_views.py
 importer/views/import_setup_views.py
 mayan_importer.egg-info/PKG-INFO
 mayan_importer.egg-info/SOURCES.txt
 mayan_importer.egg-info/dependency_links.txt
 mayan_importer.egg-info/not-zip-safe
 mayan_importer.egg-info/requires.txt
```

### Comparing `mayan-importer-2.5.3/setup.py` & `mayan-importer-3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='2.5.3',
+    version='3.0',
     zip_safe=False,
 )
```

