# Comparing `tmp/edx-event-routing-backends-8.3.0.tar.gz` & `tmp/edx-event-routing-backends-8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-8.3.0.tar", last modified: Fri Mar 22 20:20:27 2024, max compression
+gzip compressed data, was "edx-event-routing-backends-8.3.1.tar", last modified: Mon Apr  1 19:55:33 2024, max compression
```

## Comparing `edx-event-routing-backends-8.3.0.tar` & `edx-event-routing-backends-8.3.1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 20:20:27.000000 edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.307797 edx-event-routing-backends-8.3.0/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.307797 edx-event-routing-backends-8.3.0/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/async_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    12518 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/sync_events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.307797 edx-event-routing-backends-8.3.0/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44356 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.307797 edx-event-routing-backends-8.3.0/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.307797 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/queued_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/recover_failed_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.311797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.315797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.319797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.319797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.319797 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.303797 edx-event-routing-backends-8.3.0/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.303797 edx-event-routing-backends-8.3.0/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.303797 edx-event-routing-backends-8.3.0/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-22 20:20:27.323797 edx-event-routing-backends-8.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-22 20:20:24.000000 edx-event-routing-backends-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 19:55:33.000000 edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/async_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/sync_events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44356 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/queued_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/recover_failed_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_recover_failed_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.370018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.374018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/completion_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/exam_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/grading_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16362 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.378018 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.366018 edx-event-routing-backends-8.3.1/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-01 19:55:33.382018 edx-event-routing-backends-8.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-01 19:55:29.000000 edx-event-routing-backends-8.3.1/setup.py
```

### Comparing `edx-event-routing-backends-8.3.0/CHANGELOG.rst` & `edx-event-routing-backends-8.3.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/LICENSE.txt` & `edx-event-routing-backends-8.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/PKG-INFO` & `edx-event-routing-backends-8.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 8.3.0
+Version: 8.3.1
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-8.3.0/README.rst` & `edx-event-routing-backends-8.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 8.3.0
+Version: 8.3.1
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `edx-event-routing-backends-8.3.0/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-8.3.1/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/admin.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/admin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/apps.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/backends/async_events_router.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/backends/async_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/backends/events_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,27 +221,40 @@
         """
         event["timestamp"] = event["timestamp"].isoformat()
         queue_size = redis.lpush(self.queue_name, json.dumps(event, cls=DateTimeJSONEncoder))
         logger.info(f'Event {event["name"]} has been queued for batching. Queue size: {queue_size}')
 
         if queue_size >= settings.EVENT_ROUTING_BACKEND_BATCH_SIZE or self.time_to_send(redis):
             batch = redis.rpop(self.queue_name, queue_size)
+
+            orig_size = len(batch)
+            # Deduplicate list, in some misconfigured cases tracking events can be emitted to the
+            # bus twice, causing them to be processed twice, which LRSs will reject.
+            # See: https://github.com/openedx/event-routing-backends/issues/410
+            batch = [i for n, i in enumerate(batch) if i not in batch[n + 1:]]
+            final_size = len(batch)
+
+            if final_size != orig_size:  # pragma: no cover
+                logger.warning(f"{orig_size - final_size} duplicate events in event-routing-backends batch queue! "
+                               f"This is a likely due to misconfiguration of EVENT_TRACKING_BACKENDS.")
             return batch
 
         return None
 
     def time_to_send(self, redis):
         """
         Check if it is time to send the batched events.
         """
         last_sent = redis.get(self.last_sent_key)
         if not last_sent:
             return True
         time_passed = (datetime.now() - datetime.fromisoformat(last_sent.decode('utf-8')))
-        return time_passed > timedelta(seconds=settings.EVENT_ROUTING_BACKEND_BATCH_INTERVAL)
+        ready = time_passed > timedelta(seconds=settings.EVENT_ROUTING_BACKEND_BATCH_INTERVAL)
+
+        return ready
 
     def process_event(self, event):
         """
         Process the event through this router's processors.
 
         This single event may produce multiple processed events, and so we return a list of events here.
```

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/backends/sync_events_router.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/backends/sync_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/backends/tests/test_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/helpers.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/recover_failed_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/recover_failed_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/tests/test_recover_failed_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_recover_failed_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/models.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Test the caliper processor.
 """
 import json
 
 from django.test import SimpleTestCase
 from django.test.utils import override_settings
-from eventtracking.processors.exceptions import EventEmissionExit, NoBackendEnabled
 from mock import MagicMock, call, patch, sentinel
 
 from event_routing_backends.processors.caliper.transformer_processor import CaliperProcessor
 
 
 @override_settings(CALIPER_EVENTS_ENABLED=True)
 class TestCaliperProcessor(SimpleTestCase):
@@ -25,21 +24,19 @@
             '1': MagicMock(),
         }
 
         self.processor = CaliperProcessor()
 
     @override_settings(CALIPER_EVENTS_ENABLED=False)
     def test_skip_event_when_disabled(self):
-        with self.assertRaises(NoBackendEnabled):
-            self.processor(self.sample_event)
+        self.assertFalse(self.processor(self.sample_event))
 
     @patch('event_routing_backends.processors.mixins.base_transformer_processor.logger')
     def test_send_method_with_no_transformer_implemented(self, mocked_logger):
-        with self.assertRaises(EventEmissionExit):
-            self.processor([self.sample_event])
+        self.assertFalse(self.processor([self.sample_event]))
 
         mocked_logger.error.assert_called_once_with(
             'Could not get transformer for %s event.',
             self.sample_event.get('name')
         )
 
     @patch(
@@ -126,10 +123,9 @@
             mocked_caliper_logger.info.mock_calls
         )
 
     @patch('event_routing_backends.processors.mixins.base_transformer_processor.logger')
     def test_with_no_registry(self, mocked_logger):
         backend = CaliperProcessor()
         backend.registry = None
-        with self.assertRaises(EventEmissionExit):
-            self.assertIsNone(backend([self.sample_event]))
+        self.assertFalse(backend([self.sample_event]))
         mocked_logger.exception.assert_called_once()
```

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,17 +171,15 @@
         else:
             result = BaseTransformerMixin.find_nested(self.event, key)
 
         if result != 0 and not result:
             result = None
 
         if result is None:
-            if not required:
-                logger.warning('Could not get value for %s in event "%s"', key, self.event.get('name', None))
-            else:
+            if required:
                 raise ValueError(
                     'Could not get value for {} in event "{}"'.format(key, self.event.get('name', None))
                 )
 
         return result
 
     def del_none(self, source_dict):
```

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Base Processor Mixin for transformer processors.
 """
 from logging import getLogger
 
-from eventtracking.processors.exceptions import EventEmissionExit, NoTransformerImplemented
+from eventtracking.processors.exceptions import NoBackendEnabled, NoTransformerImplemented
 
 logger = getLogger(__name__)
 
 
 class BaseTransformerProcessorMixin:
     """
     Base Processor Mixin for transformer processors.
@@ -30,21 +30,26 @@
 
         Raises:
             EventEmissionExit except.on:  if no transformer is registered for an event.
             ANY exception: if raised.
         """
         returned_events = []
         for event in events:
-            transformed_event = self.transform_event(event)
-            if not transformed_event:
-                raise EventEmissionExit
-            if isinstance(transformed_event, list):
-                returned_events += transformed_event
-            else:
-                returned_events.append(transformed_event)
+            try:
+                transformed_event = self.transform_event(event)
+                if not transformed_event:
+                    pass
+                elif isinstance(transformed_event, list):
+                    returned_events += transformed_event
+                else:
+                    returned_events.append(transformed_event)
+
+            # If the backend isn't enabled at all, early out
+            except NoBackendEnabled:
+                break
         return returned_events
 
     def transform_event(self, event):
         """
         Transform the event.
 
         Transformer method can return transformed events in any data structure format
@@ -56,15 +61,14 @@
         Returns:
             ANY:           transformed event
         """
         event_name = event.get('name')
 
         try:
             transformed_event = self.get_transformed_event(event)
-
         except NoTransformerImplemented:
             logger.error('Could not get transformer for %s event.', event_name)
             return None
 
         except Exception as ex:
             logger.exception(
                 'There was an error while trying to transform event "{event}" using'
```

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/decorators.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/decorators.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/openedx_filters/filters.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/openedx_filters/test_filters.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/openedx_filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/constants.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/completion_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/completion_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/exam_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/exam_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/forum_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/forum_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/grading_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/grading_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Test the xAPI processor.
 """
 import uuid
 
 from django.test import SimpleTestCase
 from django.test.utils import override_settings
-from eventtracking.processors.exceptions import EventEmissionExit, NoBackendEnabled
 from mock import MagicMock, call, patch, sentinel
 from tincan import Activity, Statement
 
 from event_routing_backends.processors.xapi.transformer_processor import XApiProcessor
 
 
 @override_settings(XAPI_EVENTS_ENABLED=True)
@@ -21,21 +20,19 @@
         self.sample_event = {
             'name': str(sentinel.name)
         }
         self.processor = XApiProcessor()
 
     @override_settings(XAPI_EVENTS_ENABLED=False)
     def test_skip_event_when_disabled(self):
-        with self.assertRaises(NoBackendEnabled):
-            self.processor(self.sample_event)
+        self.assertFalse(self.processor(self.sample_event))
 
     @patch('event_routing_backends.processors.mixins.base_transformer_processor.logger')
     def test_send_method_with_no_transformer_implemented(self, mocked_logger):
-        with self.assertRaises(EventEmissionExit):
-            self.processor([self.sample_event])
+        self.assertFalse(self.processor([self.sample_event]))
 
         mocked_logger.error.assert_called_once_with(
             'Could not get transformer for %s event.',
             self.sample_event.get('name')
         )
 
     @patch(
@@ -87,17 +84,15 @@
     @patch('event_routing_backends.processors.xapi.transformer_processor.xapi_logger')
     def test_send_method_with_invalid_object(self, mocked_logger, mocked_get_transformer):
         transformed_event = Statement()
         mocked_transformer = MagicMock()
         mocked_transformer.transform.return_value = transformed_event
         mocked_get_transformer.return_value = mocked_transformer
 
-        with self.assertRaises(EventEmissionExit):
-            self.processor([self.sample_event])
-
+        self.assertFalse(self.processor([self.sample_event]))
         self.assertNotIn(call(transformed_event.to_json()), mocked_logger.mock_calls)
 
     @override_settings(XAPI_EVENT_LOGGING_ENABLED=False)
     @patch(
         'event_routing_backends.processors.xapi.transformer_processor.XApiTransformersRegistry.get_transformer'
     )
     @patch('event_routing_backends.processors.xapi.transformer_processor.xapi_logger')
@@ -112,10 +107,9 @@
 
         self.assertNotIn(call(transformed_event.to_json()), mocked_logger.mock_calls)
 
     @patch('event_routing_backends.processors.mixins.base_transformer_processor.logger')
     def test_with_no_registry(self, mocked_logger):
         backend = XApiProcessor()
         backend.registry = None
-        with self.assertRaises(EventEmissionExit):
-            self.assertIsNone(backend([self.sample_event]))
+        self.assertFalse(backend([self.sample_event]))
         mocked_logger.exception.assert_called_once()
```

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/tests/test_xapi_event_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/settings/common.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/settings/production.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-8.3.1/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tasks.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-8.3.1/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/requirements/constraints.txt` & `edx-event-routing-backends-8.3.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-8.3.0/setup.py` & `edx-event-routing-backends-8.3.1/setup.py`

 * *Files identical despite different names*

