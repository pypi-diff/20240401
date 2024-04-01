# Comparing `tmp/openedx-events-9.5.2.tar.gz` & `tmp/openedx-events-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-9.5.2.tar", last modified: Mon Feb 19 12:59:28 2024, max compression
+gzip compressed data, was "openedx-events-9.6.0.tar", last modified: Mon Apr  1 12:59:12 2024, max compression
```

## Comparing `openedx-events-9.5.2.tar` & `openedx-events-9.6.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-02-19 12:59:23.000000 openedx-events-9.5.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-19 12:59:23.000000 openedx-events-9.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-19 12:59:23.000000 openedx-events-9.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-02-19 12:59:28.186075 openedx-events-9.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-19 12:59:23.000000 openedx-events-9.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.182075 openedx-events-9.5.2/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.182075 openedx-events-9.5.2/openedx_events/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/analytics/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/analytics/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.182075 openedx-events-9.5.2/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.182075 openedx-events-9.5.2/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/test_producer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-19 12:59:23.000000 openedx-events-9.5.2/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-19 12:59:28.000000 openedx-events-9.5.2/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-19 12:59:23.000000 openedx-events-9.5.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-19 12:59:23.000000 openedx-events-9.5.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-19 12:59:28.190075 openedx-events-9.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-19 12:59:23.000000 openedx-events-9.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 12:59:28.186075 openedx-events-9.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-19 12:59:23.000000 openedx-events-9.5.2/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-01 12:59:09.000000 openedx-events-9.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 12:59:09.000000 openedx-events-9.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-01 12:59:09.000000 openedx-events-9.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-04-01 12:59:12.792969 openedx-events-9.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-01 12:59:09.000000 openedx-events-9.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/analytics/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.788969 openedx-events-9.6.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_producer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-01 12:59:09.000000 openedx-events-9.6.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 12:59:12.000000 openedx-events-9.6.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 12:59:09.000000 openedx-events-9.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-01 12:59:09.000000 openedx-events-9.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-01 12:59:12.796969 openedx-events-9.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-01 12:59:09.000000 openedx-events-9.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:59:12.792969 openedx-events-9.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 12:59:09.000000 openedx-events-9.6.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-9.5.2/CHANGELOG.rst` & `openedx-events-9.6.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+Added
+~~~~~
+* Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.5.2/LICENSE.txt` & `openedx-events-9.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/PKG-INFO` & `openedx-events-9.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.5.2
+Version: 9.6.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,14 +163,17 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+Added
+~~~~~
+* Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.5.2/README.rst` & `openedx-events-9.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/analytics/data.py` & `openedx-events-9.6.0/openedx_events/analytics/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/analytics/signals.py` & `openedx-events-9.6.0/openedx_events/analytics/signals.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 from openedx_events.analytics.data import TrackingLogData
 from openedx_events.tooling import OpenEdxPublicSignal
 
 # .. event_type: org.openedx.analytics.tracking.event.emitted.v1
 # .. event_name: TRACKING_EVENT_EMITTED
+# .. event_key_field: tracking_log.name
 # .. event_description: emitted when a tracking log is created.
 # .. event_data: TrackingLogData
 TRACKING_EVENT_EMITTED = OpenEdxPublicSignal(
     event_type="org.openedx.analytics.tracking.event.emitted.v1",
     data={
         "tracking_log": TrackingLogData,
     }
```

### Comparing `openedx-events-9.5.2/openedx_events/apps.py` & `openedx-events-9.6.0/openedx_events/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/content_authoring/data.py` & `openedx-events-9.6.0/openedx_events/content_authoring/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,7 +176,21 @@
     Arguments:
         library_key (LibraryLocatorV2): a key that represents a Blockstore-based content library.
         usage_key (LibraryUsageLocatorV2): a key that represents a XBlock in a Blockstore-based content library.
     """
 
     library_key = attr.ib(type=LibraryLocatorV2)
     usage_key = attr.ib(type=LibraryUsageLocatorV2)
+
+
+@attr.s(frozen=True)
+class ContentObjectData:
+    """
+    Data about changed content object
+
+    Arguments:
+        object_id (str): identifier of the Content object. This represents the id of the course or library block
+        as a string. For example:
+        block-v1:SampleTaxonomyOrg2+STC1+2023_1+type@vertical+block@f8de78f0897049ce997777a3a31b6ea0
+    """
+
+    object_id = attr.ib(type=str)
```

### Comparing `openedx-events-9.5.2/openedx_events/content_authoring/signals.py` & `openedx-events-9.6.0/openedx_events/content_authoring/signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,57 +6,62 @@
 
 They also must comply with the payload definition specified in
 docs/decisions/0003-events-payload.rst
 """
 from openedx_events.content_authoring.data import (
     CertificateConfigData,
     ContentLibraryData,
+    ContentObjectData,
     CourseCatalogData,
     CourseData,
     DuplicatedXBlockData,
     LibraryBlockData,
     XBlockData,
 )
 from openedx_events.tooling import OpenEdxPublicSignal
 
 # .. event_type: org.openedx.content_authoring.course.catalog_info.changed.v1
 # .. event_name: COURSE_CATALOG_INFO_CHANGED
+# .. event_key_field: catalog_info.course_key
 # .. event_description: Fired when a course changes in Studio in a way that is relevant for catalog consumers.
 # .. event_data: CourseCatalogData
 COURSE_CATALOG_INFO_CHANGED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.course.catalog_info.changed.v1",
     data={
         "catalog_info": CourseCatalogData,
     }
 )
 
 # .. event_type: org.openedx.content_authoring.xblock.created.v1
 # .. event_name: XBLOCK_CREATED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock is created.
 # .. event_data: XBlockData
 XBLOCK_CREATED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.xblock.created.v1",
     data={
         "xblock_info": XBlockData,
     }
 )
 
 # .. event_type: org.openedx.content_authoring.xblock.updated.v1
 # .. event_name: XBLOCK_UPDATED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock is updated.
 # .. event_data: XBlockData
 XBLOCK_UPDATED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.xblock.updated.v1",
     data={
         "xblock_info": XBlockData,
     }
 )
 
 # .. event_type: org.openedx.content_authoring.xblock.published.v1
 # .. event_name: XBLOCK_PUBLISHED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock is published. If a parent block
 #       with changes in one or more child blocks is published, only a single
 #       XBLOCK_PUBLISHED event is fired with parent block details.
 #       For example: If a section is published with changes in multiple units,
 #       only a single event is fired with section details like :
 #       `XBlockData(usage_key="section-usage-key", block_type="chapter")`
 # .. event_data: XBlockData
@@ -66,26 +71,28 @@
         "xblock_info": XBlockData,
     }
 )
 
 
 # .. event_type: org.openedx.content_authoring.xblock.deleted.v1
 # .. event_name: XBLOCK_DELETED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock is deleted.
 # .. event_data: XBlockData
 XBLOCK_DELETED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.xblock.deleted.v1",
     data={
         "xblock_info": XBlockData,
     }
 )
 
 
 # .. event_type: org.openedx.content_authoring.xblock.duplicated.v1
 # .. event_name: XBLOCK_DUPLICATED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock is duplicated in Studio.
 # .. event_data: DuplicatedXBlockData
 XBLOCK_DUPLICATED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.xblock.duplicated.v1",
     data={
         "xblock_info": DuplicatedXBlockData,
     }
@@ -188,7 +195,18 @@
 # .. event_data: LibraryBlockData
 LIBRARY_BLOCK_DELETED = OpenEdxPublicSignal(
     event_type="org.openedx.content_authoring.library_block.deleted.v1",
     data={
         "library_block": LibraryBlockData,
     }
 )
+
+# .. event_type: org.openedx.content_authoring.content.object.tags.changed.v1
+# .. event_name: CONTENT_OBJECT_TAGS_CHANGED
+# .. event_description: emitted when an object's tags are changed
+# .. event_data: ContentObjectData
+CONTENT_OBJECT_TAGS_CHANGED = OpenEdxPublicSignal(
+    event_type="org.openedx.content_authoring.content.object.tags.changed.v1",
+    data={
+        "content_object": ContentObjectData
+    }
+)
```

### Comparing `openedx-events-9.5.2/openedx_events/data.py` & `openedx-events-9.6.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/__init__.py` & `openedx-events-9.6.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/schema.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/serializer.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-9.6.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-9.6.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/exceptions.py` & `openedx-events-9.6.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/learning/data.py` & `openedx-events-9.6.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/learning/signals.py` & `openedx-events-9.6.0/openedx_events/learning/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "user": UserData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.auth.session.login.completed.v1
 # .. event_name: SESSION_LOGIN_COMPLETED
+# .. event_key_field: user.pii.username
 # .. event_description: emitted when the user's login process in the LMS is completed.
 # .. event_data: UserData
 SESSION_LOGIN_COMPLETED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.auth.session.login.completed.v1",
     data={
         "user": UserData,
     }
@@ -71,37 +72,40 @@
         "enrollment": CourseEnrollmentData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.course.unenrollment.completed.v1
 # .. event_name: COURSE_UNENROLLMENT_COMPLETED
+# .. event_key_field: enrollment.course.course_key
 # .. event_description: emitted when the user's unenrollment process is completed.
 # .. event_data: CourseEnrollmentData
 COURSE_UNENROLLMENT_COMPLETED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.course.unenrollment.completed.v1",
     data={
         "enrollment": CourseEnrollmentData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.certificate.created.v1
 # .. event_name: CERTIFICATE_CREATED
+# .. event_key_field: certificate.course.course_key
 # .. event_description: emitted when the user's certificate creation process is completed.
 # .. event_data: CertificateData
 CERTIFICATE_CREATED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.certificate.created.v1",
     data={
         "certificate": CertificateData,
     }
 )
 
 # .. event_type: org.openedx.learning.program.certificate.awarded.v1
 # .. event_name: PROGRAM_CERTIFICATE_AWARDED
+# .. event_key_field: program_certificate.program.uuid
 # .. event_description: Emit when a program certificate is awarded to a learner
 # .. event_data: ProgramCertificateData
 PROGRAM_CERTIFICATE_AWARDED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.program.certificate.awarded.v1",
     data={
         "program_certificate": ProgramCertificateData,
     }
@@ -117,25 +121,27 @@
         "certificate": CertificateData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.certificate.revoked.v1
 # .. event_name: CERTIFICATE_REVOKED
+# .. event_key_field: certificate.course.course_key
 # .. event_description: emitted when the user's certificate annulation process is completed.
 # .. event_data: CertificateData
 CERTIFICATE_REVOKED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.certificate.revoked.v1",
     data={
         "certificate": CertificateData,
     }
 )
 
 # .. event_type: org.openedx.learning.program.certificate.revoked.v1
 # .. event_name: PROGRAM_CERTIFICATE_REVOKED
+# .. event_key_field: program_certificate.program.uuid
 # .. event_description: Emit when a program certificate is revoked from a learner
 # .. event_data: ProgramCertificateData
 PROGRAM_CERTIFICATE_REVOKED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.program.certificate.revoked.v1",
     data={
         "program_certificate": ProgramCertificateData,
     }
@@ -175,14 +181,15 @@
         "grade": PersistentCourseGradeData,
     }
 )
 
 
 # .. event_type: org.openedx.learning.xblock.skill.verified.v1
 # .. event_name: XBLOCK_SKILL_VERIFIED
+# .. event_key_field: xblock_info.usage_key
 # .. event_description: Fired when an XBlock skill is verified.
 # .. event_data: XBlockSkillVerificationData
 XBLOCK_SKILL_VERIFIED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.xblock.skill.verified.v1",
     data={
         "xblock_info": XBlockSkillVerificationData,
     }
@@ -254,25 +261,27 @@
     data={
         "exam_attempt": ExamAttemptData,
     }
 )
 
 # .. event_type: org.openedx.learning.user.course_access_role.added.v1
 # .. event_name: COURSE_ACCESS_ROLE_ADDED
+# .. event_key_field: course_access_role_data.course_key
 # .. event_description: Emitted when a user is given a course access role.
 # .. event_data: CourseAccessRoleData
 COURSE_ACCESS_ROLE_ADDED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.user.course_access_role.added.v1",
     data={
         "course_access_role_data": CourseAccessRoleData,
     }
 )
 
 # .. event_type: org.openedx.learning.user.course_access_role.removed.v1
 # .. event_name: COURSE_ACCESS_ROLE_REMOVED
+# .. event_key_field: course_access_role_data.course_key
 # .. event_description: Emitted when a course access role is removed from a user.
 # .. event_data: CourseAccessRoleData
 COURSE_ACCESS_ROLE_REMOVED = OpenEdxPublicSignal(
     event_type="org.openedx.learning.user.course_access_role.removed.v1",
     data={
         "course_access_role_data": CourseAccessRoleData,
     }
```

### Comparing `openedx-events-9.5.2/openedx_events/management/commands/consume_events.py` & `openedx-events-9.6.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-9.6.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/test_consume_events_command.py` & `openedx-events-9.6.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/test_data.py` & `openedx-events-9.6.0/openedx_events/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-9.6.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/test_producer_config.py` & `openedx-events-9.6.0/openedx_events/tests/test_producer_config.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/test_tooling.py` & `openedx-events-9.6.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tests/utils.py` & `openedx-events-9.6.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/tooling.py` & `openedx-events-9.6.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events/utils.py` & `openedx-events-9.6.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/openedx_events.egg-info/PKG-INFO` & `openedx-events-9.6.0/openedx_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.5.2
+Version: 9.6.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,14 +163,17 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+Added
+~~~~~
+* Added new ``CONTENT_OBJECT_TAGGED`` events in content_authoring.
 
 [9.5.2] - 2024-02-13
 --------------------
 Removed
 ~~~~~~~
 * Remove unused ``MANAGE_STUDENTS_PERMISSION_ADDED`` and ``MANAGE_STUDENTS_PERMISSION_REMOVED`` events in learning
```

### Comparing `openedx-events-9.5.2/openedx_events.egg-info/SOURCES.txt` & `openedx-events-9.6.0/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.5.2/setup.py` & `openedx-events-9.6.0/setup.py`

 * *Files identical despite different names*

