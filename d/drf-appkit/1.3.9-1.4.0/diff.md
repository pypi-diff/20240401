# Comparing `tmp/drf-appkit-1.3.9.tar.gz` & `tmp/drf-appkit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-appkit-1.3.9.tar", last modified: Sun Mar 31 15:43:20 2024, max compression
+gzip compressed data, was "drf-appkit-1.4.0.tar", last modified: Mon Apr  1 17:38:09 2024, max compression
```

## Comparing `drf-appkit-1.3.9.tar` & `drf-appkit-1.4.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.747287 drf-appkit-1.3.9/
--rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf-appkit-1.3.9/LICENSE
--rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf-appkit-1.3.9/MANIFEST.in
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-31 15:43:20.747217 drf-appkit-1.3.9/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf-appkit-1.3.9/README.md
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.719505 drf-appkit-1.3.9/appkit/
--rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 15:40:37.000000 drf-appkit-1.3.9/appkit/__init__.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.722024 drf-appkit-1.3.9/appkit/api/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf-appkit-1.3.9/appkit/api/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/pagination.py
--rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/relations.py
--rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/renderers.py
--rw-r--r--   0 allan      (501) staff       (20)    14953 2024-03-20 23:00:29.000000 drf-appkit-1.3.9/appkit/api/serializers.py
--rw-r--r--   0 allan      (501) staff       (20)     8538 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/api/tests.py
--rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf-appkit-1.3.9/appkit/api/views.py
--rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 15:40:37.000000 drf-appkit-1.3.9/appkit/apps.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.724341 drf-appkit-1.3.9/appkit/auth/
--rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/auth/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/auth/backends.py
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/auth/decorators.py
--rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/auth/email.py
--rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/auth/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/debug.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.730077 drf-appkit-1.3.9/appkit/drf/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf-appkit-1.3.9/appkit/drf/adapters.py
--rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/authentication.py
--rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/backends.py
--rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf-appkit-1.3.9/appkit/drf/endpoints.py
--rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/exceptions.py
--rw-r--r--   0 allan      (501) staff       (20)     3714 2024-03-24 18:40:59.000000 drf-appkit-1.3.9/appkit/drf/fields.py
--rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf-appkit-1.3.9/appkit/drf/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/drf/serializers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.733059 drf-appkit-1.3.9/appkit/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf-appkit-1.3.9/appkit/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf-appkit-1.3.9/appkit/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf-appkit-1.3.9/appkit/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf-appkit-1.3.9/appkit/drf_appkit.egg-info/top_level.txt
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.733741 drf-appkit-1.3.9/appkit/forms/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/forms/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     1133 2024-03-27 20:11:11.000000 drf-appkit-1.3.9/appkit/forms/widgets.py
--rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 15:42:54.000000 drf-appkit-1.3.9/appkit/handlers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.714067 drf-appkit-1.3.9/appkit/jinja2/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.714126 drf-appkit-1.3.9/appkit/jinja2/appkit/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.714193 drf-appkit-1.3.9/appkit/jinja2/appkit/forms/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.734006 drf-appkit-1.3.9/appkit/jinja2/appkit/forms/widgets/
--rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/jinja2/appkit/forms/widgets/money_widget.html
--rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/managers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.746112 drf-appkit-1.3.9/appkit/migrations/
--rw-r--r--   0 allan      (501) staff       (20)     9145 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0001_initial.py
--rw-r--r--   0 allan      (501) staff       (20)      395 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0002_arrangement_tags.py
--rw-r--r--   0 allan      (501) staff       (20)      575 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0003_auto_20210221_0852.py
--rw-r--r--   0 allan      (501) staff       (20)      400 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0004_auto_20210309_0655.py
--rw-r--r--   0 allan      (501) staff       (20)     1973 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0005_auto_20210324_1046.py
--rw-r--r--   0 allan      (501) staff       (20)      762 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0006_sitealias.py
--rw-r--r--   0 allan      (501) staff       (20)      393 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0007_auto_20211021_1901.py
--rw-r--r--   0 allan      (501) staff       (20)     1831 2024-03-10 01:08:12.000000 drf-appkit-1.3.9/appkit/migrations/0008_update_autofields.py
--rw-r--r--   0 allan      (501) staff       (20)     1000 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      459 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0010_arrangement_name.py
--rw-r--r--   0 allan      (501) staff       (20)      362 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0011_alter_sitealias_options.py
--rw-r--r--   0 allan      (501) staff       (20)      543 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0012_alter_sitealias_site.py
--rw-r--r--   0 allan      (501) staff       (20)     1480 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0013_usergroup.py
--rw-r--r--   0 allan      (501) staff       (20)      802 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      810 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      846 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      609 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0017_alter_imageattachment_image.py
--rw-r--r--   0 allan      (501) staff       (20)      972 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0018_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      465 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/0019_alter_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      684 2024-03-17 13:15:12.000000 drf-appkit-1.3.9/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
--rw-r--r--   0 allan      (501) staff       (20)      407 2024-03-18 02:51:42.000000 drf-appkit-1.3.9/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
--rw-r--r--   0 allan      (501) staff       (20)      655 2024-03-20 16:14:15.000000 drf-appkit-1.3.9/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/migrations/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)    12786 2024-03-31 15:42:54.000000 drf-appkit-1.3.9/appkit/models.py
--rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 03:08:40.000000 drf-appkit-1.3.9/appkit/notification.py
--rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/settings.py
--rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 03:05:20.000000 drf-appkit-1.3.9/appkit/shortcuts.py
--rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/storages.py
--rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf-appkit-1.3.9/appkit/tasks.py
--rw-r--r--   0 allan      (501) staff       (20)      690 2023-10-23 02:15:00.000000 drf-appkit-1.3.9/appkit/tests.py
--rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf-appkit-1.3.9/appkit/transformers.py
--rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 02:55:32.000000 drf-appkit-1.3.9/appkit/util.py
--rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf-appkit-1.3.9/appkit/views.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-03-31 15:43:20.746908 drf-appkit-1.3.9/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-31 15:43:20.000000 drf-appkit-1.3.9/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     2513 2024-03-31 15:43:20.000000 drf-appkit-1.3.9/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-31 15:43:20.000000 drf-appkit-1.3.9/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-31 15:43:20.000000 drf-appkit-1.3.9/drf_appkit.egg-info/top_level.txt
--rw-r--r--   0 allan      (501) staff       (20)      790 2024-03-31 15:43:20.747608 drf-appkit-1.3.9/setup.cfg
--rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf-appkit-1.3.9/setup.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.204831 drf-appkit-1.4.0/
+-rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf-appkit-1.4.0/LICENSE
+-rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf-appkit-1.4.0/MANIFEST.in
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-01 17:38:09.204760 drf-appkit-1.4.0/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf-appkit-1.4.0/README.md
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.179122 drf-appkit-1.4.0/appkit/
+-rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 16:07:10.000000 drf-appkit-1.4.0/appkit/__init__.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.181503 drf-appkit-1.4.0/appkit/api/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/api/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf-appkit-1.4.0/appkit/api/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/api/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/api/pagination.py
+-rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/api/relations.py
+-rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/api/renderers.py
+-rw-r--r--   0 allan      (501) staff       (20)    14953 2024-03-20 23:00:29.000000 drf-appkit-1.4.0/appkit/api/serializers.py
+-rw-r--r--   0 allan      (501) staff       (20)     5428 2024-04-01 16:02:52.000000 drf-appkit-1.4.0/appkit/api/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf-appkit-1.4.0/appkit/api/views.py
+-rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 16:07:10.000000 drf-appkit-1.4.0/appkit/apps.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.183461 drf-appkit-1.4.0/appkit/auth/
+-rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/auth/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/auth/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/auth/decorators.py
+-rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/auth/email.py
+-rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/auth/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/debug.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.187146 drf-appkit-1.4.0/appkit/drf/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf-appkit-1.4.0/appkit/drf/adapters.py
+-rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/authentication.py
+-rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf-appkit-1.4.0/appkit/drf/endpoints.py
+-rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/exceptions.py
+-rw-r--r--   0 allan      (501) staff       (20)     3714 2024-03-24 18:40:59.000000 drf-appkit-1.4.0/appkit/drf/fields.py
+-rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf-appkit-1.4.0/appkit/drf/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/drf/serializers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.189735 drf-appkit-1.4.0/appkit/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf-appkit-1.4.0/appkit/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf-appkit-1.4.0/appkit/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf-appkit-1.4.0/appkit/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf-appkit-1.4.0/appkit/drf_appkit.egg-info/top_level.txt
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.190113 drf-appkit-1.4.0/appkit/forms/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/forms/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     1133 2024-03-27 20:11:11.000000 drf-appkit-1.4.0/appkit/forms/widgets.py
+-rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 16:07:10.000000 drf-appkit-1.4.0/appkit/handlers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.172061 drf-appkit-1.4.0/appkit/jinja2/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.172121 drf-appkit-1.4.0/appkit/jinja2/appkit/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.172182 drf-appkit-1.4.0/appkit/jinja2/appkit/forms/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.190623 drf-appkit-1.4.0/appkit/jinja2/appkit/forms/widgets/
+-rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/jinja2/appkit/forms/widgets/money_widget.html
+-rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/managers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.203791 drf-appkit-1.4.0/appkit/migrations/
+-rw-r--r--   0 allan      (501) staff       (20)     9145 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0001_initial.py
+-rw-r--r--   0 allan      (501) staff       (20)      395 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0002_arrangement_tags.py
+-rw-r--r--   0 allan      (501) staff       (20)      575 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0003_auto_20210221_0852.py
+-rw-r--r--   0 allan      (501) staff       (20)      400 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0004_auto_20210309_0655.py
+-rw-r--r--   0 allan      (501) staff       (20)     1973 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0005_auto_20210324_1046.py
+-rw-r--r--   0 allan      (501) staff       (20)      762 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0006_sitealias.py
+-rw-r--r--   0 allan      (501) staff       (20)      393 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0007_auto_20211021_1901.py
+-rw-r--r--   0 allan      (501) staff       (20)     1831 2024-03-10 01:08:12.000000 drf-appkit-1.4.0/appkit/migrations/0008_update_autofields.py
+-rw-r--r--   0 allan      (501) staff       (20)     1000 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      459 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0010_arrangement_name.py
+-rw-r--r--   0 allan      (501) staff       (20)      362 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0011_alter_sitealias_options.py
+-rw-r--r--   0 allan      (501) staff       (20)      543 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0012_alter_sitealias_site.py
+-rw-r--r--   0 allan      (501) staff       (20)     1480 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0013_usergroup.py
+-rw-r--r--   0 allan      (501) staff       (20)      802 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      810 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      846 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      609 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0017_alter_imageattachment_image.py
+-rw-r--r--   0 allan      (501) staff       (20)      972 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0018_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      465 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/0019_alter_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      684 2024-03-17 13:15:12.000000 drf-appkit-1.4.0/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      407 2024-03-18 02:51:42.000000 drf-appkit-1.4.0/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      655 2024-03-20 16:14:15.000000 drf-appkit-1.4.0/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/migrations/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)    13102 2024-04-01 17:31:05.000000 drf-appkit-1.4.0/appkit/models.py
+-rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 20:07:19.000000 drf-appkit-1.4.0/appkit/notification.py
+-rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/settings.py
+-rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 16:07:10.000000 drf-appkit-1.4.0/appkit/shortcuts.py
+-rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/storages.py
+-rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf-appkit-1.4.0/appkit/tasks.py
+-rw-r--r--   0 allan      (501) staff       (20)     4829 2024-04-01 17:37:52.000000 drf-appkit-1.4.0/appkit/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf-appkit-1.4.0/appkit/transformers.py
+-rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 16:07:10.000000 drf-appkit-1.4.0/appkit/util.py
+-rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf-appkit-1.4.0/appkit/views.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-01 17:38:09.204511 drf-appkit-1.4.0/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-01 17:38:09.000000 drf-appkit-1.4.0/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     2513 2024-04-01 17:38:09.000000 drf-appkit-1.4.0/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-04-01 17:38:09.000000 drf-appkit-1.4.0/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-04-01 17:38:09.000000 drf-appkit-1.4.0/drf_appkit.egg-info/top_level.txt
+-rw-r--r--   0 allan      (501) staff       (20)      790 2024-04-01 17:38:09.205124 drf-appkit-1.4.0/setup.cfg
+-rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf-appkit-1.4.0/setup.py
```

### Comparing `drf-appkit-1.3.9/LICENSE` & `drf-appkit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/PKG-INFO` & `drf-appkit-1.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.3.9
+Version: 1.4.0
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.3.9/appkit/api/filters.py` & `drf-appkit-1.4.0/appkit/api/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/api/mixins.py` & `drf-appkit-1.4.0/appkit/api/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/api/pagination.py` & `drf-appkit-1.4.0/appkit/api/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/api/renderers.py` & `drf-appkit-1.4.0/appkit/api/renderers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/api/serializers.py` & `drf-appkit-1.4.0/appkit/api/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/api/views.py` & `drf-appkit-1.4.0/appkit/api/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/auth/__init__.py` & `drf-appkit-1.4.0/appkit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/auth/backends.py` & `drf-appkit-1.4.0/appkit/auth/backends.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/auth/decorators.py` & `drf-appkit-1.4.0/appkit/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/auth/email.py` & `drf-appkit-1.4.0/appkit/auth/email.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/auth/permissions.py` & `drf-appkit-1.4.0/appkit/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/debug.py` & `drf-appkit-1.4.0/appkit/debug.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/authentication.py` & `drf-appkit-1.4.0/appkit/drf/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/endpoints.py` & `drf-appkit-1.4.0/appkit/drf/endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/fields.py` & `drf-appkit-1.4.0/appkit/drf/fields.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/filters.py` & `drf-appkit-1.4.0/appkit/drf/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/mixins.py` & `drf-appkit-1.4.0/appkit/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf/serializers.py` & `drf-appkit-1.4.0/appkit/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf_appkit.egg-info/PKG-INFO` & `drf-appkit-1.4.0/appkit/drf_appkit.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/drf_appkit.egg-info/SOURCES.txt` & `drf-appkit-1.4.0/appkit/drf_appkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/forms/widgets.py` & `drf-appkit-1.4.0/appkit/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/jinja2/appkit/forms/widgets/money_widget.html` & `drf-appkit-1.4.0/appkit/jinja2/appkit/forms/widgets/money_widget.html`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/managers.py` & `drf-appkit-1.4.0/appkit/managers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0001_initial.py` & `drf-appkit-1.4.0/appkit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0003_auto_20210221_0852.py` & `drf-appkit-1.4.0/appkit/migrations/0003_auto_20210221_0852.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0005_auto_20210324_1046.py` & `drf-appkit-1.4.0/appkit/migrations/0005_auto_20210324_1046.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0006_sitealias.py` & `drf-appkit-1.4.0/appkit/migrations/0006_sitealias.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0008_update_autofields.py` & `drf-appkit-1.4.0/appkit/migrations/0008_update_autofields.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py` & `drf-appkit-1.4.0/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0012_alter_sitealias_site.py` & `drf-appkit-1.4.0/appkit/migrations/0012_alter_sitealias_site.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0013_usergroup.py` & `drf-appkit-1.4.0/appkit/migrations/0013_usergroup.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py` & `drf-appkit-1.4.0/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py` & `drf-appkit-1.4.0/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py` & `drf-appkit-1.4.0/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0017_alter_imageattachment_image.py` & `drf-appkit-1.4.0/appkit/migrations/0017_alter_imageattachment_image.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0018_place_geoposition.py` & `drf-appkit-1.4.0/appkit/migrations/0018_place_geoposition.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py` & `drf-appkit-1.4.0/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py` & `drf-appkit-1.4.0/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/models.py` & `drf-appkit-1.4.0/appkit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 
 from .settings import appkit_settings
 
 
 class ModelBase(models.Model):
     notification_classes = {}
 
+    @classmethod
+    def include_related_users_as_notification_subscribers(cls, recipients, notification_name, sender):
+        """
+         Implicitly include a document's assigned recipients in the set of notification subscribers
+        """
+        if sender:
+            recipients.update(sender.related_users)
+
     class Meta:
         abstract = True
 
     def get_detail_url_name(self):
         if hasattr(self, 'detail_url_name'):
             return getattr(self, 'detail_url_name')
```

### Comparing `drf-appkit-1.3.9/appkit/notification.py` & `drf-appkit-1.4.0/appkit/notification.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/settings.py` & `drf-appkit-1.4.0/appkit/settings.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/shortcuts.py` & `drf-appkit-1.4.0/appkit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/tasks.py` & `drf-appkit-1.4.0/appkit/tasks.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/transformers.py` & `drf-appkit-1.4.0/appkit/transformers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/util.py` & `drf-appkit-1.4.0/appkit/util.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/appkit/views.py` & `drf-appkit-1.4.0/appkit/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/drf_appkit.egg-info/PKG-INFO` & `drf-appkit-1.4.0/drf_appkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.3.9
+Version: 1.4.0
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.3.9/drf_appkit.egg-info/SOURCES.txt` & `drf-appkit-1.4.0/drf_appkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.3.9/setup.cfg` & `drf-appkit-1.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-appkit
-version = 1.3.9
+version = 1.4.0
 description = A Django app providing generic CRUD functionality
 license = BSD
 long_description = file: README.md
 author = Allan Hart
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

