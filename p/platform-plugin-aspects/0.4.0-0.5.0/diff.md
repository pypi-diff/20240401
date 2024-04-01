# Comparing `tmp/platform-plugin-aspects-0.4.0.tar.gz` & `tmp/platform-plugin-aspects-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platform-plugin-aspects-0.4.0.tar", last modified: Wed Mar 20 15:20:24 2024, max compression
+gzip compressed data, was "platform-plugin-aspects-0.5.0.tar", last modified: Mon Apr  1 16:46:20 2024, max compression
```

## Comparing `platform-plugin-aspects-0.4.0.tar` & `platform-plugin-aspects-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/extensions/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/base_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/course_overview_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/external_id_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/user_profile_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/user_retire_sink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.345160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/css/superset.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.349160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/html/superset.html
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/html/superset_student.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/embed_dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/install_required.js
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/superset.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.345160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/platform_plugin_aspects/templates/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/waffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects/xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5229 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 15:20:24.000000 platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 15:20:24.353160 platform-plugin-aspects-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-03-20 15:20:18.000000 platform-plugin-aspects-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/load_test_tracking_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.770943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/base_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/course_overview_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/external_id_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_profile_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_retire_sink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.766943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/superset.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset_student.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/embed_dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/install_required.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/superset.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.766943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects/xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 16:46:20.000000 platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 16:46:20.774943 platform-plugin-aspects-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6977 2024-04-01 16:46:17.000000 platform-plugin-aspects-0.5.0/setup.py
```

### Comparing `platform-plugin-aspects-0.4.0/CHANGELOG.rst` & `platform-plugin-aspects-0.5.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.5.0 - 2024-04-01
+******************
+
+Added
+=====
+
+* Load testing and test monitoring scripts.
+
+
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
```

### Comparing `platform-plugin-aspects-0.4.0/LICENSE` & `platform-plugin-aspects-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/PKG-INFO` & `platform-plugin-aspects-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.4.0
+Version: 0.5.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,15 @@
 Requires-Dist: django-rest-framework
 Requires-Dist: django_crum
 Requires-Dist: edx-django-utils
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles
 Requires-Dist: openedx-atlas
 Requires-Dist: openedx-filters
+Requires-Dist: redis
 Requires-Dist: requests
 Requires-Dist: superset-api-client
 Requires-Dist: web_fragments
 
 Platform Plugin Aspects
 #######################
 
@@ -145,14 +146,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.5.0 - 2024-04-01
+******************
+
+Added
+=====
+
+* Load testing and test monitoring scripts.
+
+
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
```

### Comparing `platform-plugin-aspects-0.4.0/README.rst` & `platform-plugin-aspects-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/apps.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/apps.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/extensions/filters.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/extensions/filters.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/common.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/common.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/settings/production.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/settings/production.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/signals.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/signals.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/base_sink.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/base_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/course_overview_sink.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/course_overview_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/external_id_sink.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/external_id_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/serializers.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/user_profile_sink.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_profile_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/sinks/user_retire_sink.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/sinks/user_retire_sink.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/css/superset.css` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/css/superset.css`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/html/superset.html` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/html/superset.html`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/embed_dashboard.js` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/embed_dashboard.js`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/static/js/superset.js` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/static/js/superset.js`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/tasks.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/tasks.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/templates/instructor_dashboard/aspects.html`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/utils.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from django.conf import settings
 from supersetapiclient.client import SupersetClient
 from xblock.reference.user_service import XBlockUser
 
 logger = logging.getLogger(__name__)
 
-if settings.DEBUG:
+if settings.DEBUG:  # pragma: no cover
     os.environ["OAUTHLIB_INSECURE_TRANSPORT"] = "1"
 
 
 def _(text):
     """
     Define a dummy `gettext` replacement to make string extraction tools scrape strings marked for translation.
     """
```

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects/xblock.py` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects/xblock.py`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/PKG-INFO` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platform-plugin-aspects
-Version: 0.4.0
+Version: 0.5.0
 Summary: Aspects plugins for edx-platform
 Home-page: https://github.com/openedx/platform-plugin-aspects
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,15 @@
 Requires-Dist: django-rest-framework
 Requires-Dist: django_crum
 Requires-Dist: edx-django-utils
 Requires-Dist: edx-opaque-keys
 Requires-Dist: edx-toggles
 Requires-Dist: openedx-atlas
 Requires-Dist: openedx-filters
+Requires-Dist: redis
 Requires-Dist: requests
 Requires-Dist: superset-api-client
 Requires-Dist: web_fragments
 
 Platform Plugin Aspects
 #######################
 
@@ -145,14 +146,23 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+0.5.0 - 2024-04-01
+******************
+
+Added
+=====
+
+* Load testing and test monitoring scripts.
+
+
 0.4.0 - 2024-03-18
 ******************
 
 Added
 =====
 
 * Embed multiple Superset Dashboards.
```

### Comparing `platform-plugin-aspects-0.4.0/platform_plugin_aspects.egg-info/SOURCES.txt` & `platform-plugin-aspects-0.5.0/platform_plugin_aspects.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 platform_plugin_aspects.egg-info/requires.txt
 platform_plugin_aspects.egg-info/top_level.txt
 platform_plugin_aspects/extensions/__init__.py
 platform_plugin_aspects/extensions/filters.py
 platform_plugin_aspects/management/__init__.py
 platform_plugin_aspects/management/commands/__init__.py
 platform_plugin_aspects/management/commands/dump_data_to_clickhouse.py
+platform_plugin_aspects/management/commands/load_test_tracking_events.py
+platform_plugin_aspects/management/commands/monitor_load_test_tracking.py
 platform_plugin_aspects/settings/__init__.py
 platform_plugin_aspects/settings/common.py
 platform_plugin_aspects/settings/production.py
 platform_plugin_aspects/sinks/__init__.py
 platform_plugin_aspects/sinks/base_sink.py
 platform_plugin_aspects/sinks/course_overview_sink.py
 platform_plugin_aspects/sinks/external_id_sink.py
```

### Comparing `platform-plugin-aspects-0.4.0/requirements/constraints.txt` & `platform-plugin-aspects-0.5.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `platform-plugin-aspects-0.4.0/setup.py` & `platform-plugin-aspects-0.5.0/setup.py`

 * *Files identical despite different names*

