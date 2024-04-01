# Comparing `tmp/deep_agent-1.1.0.tar.gz` & `tmp/deep_agent-1.1.1.tar.gz`

## Comparing `deep_agent-1.1.0.tar` & `deep_agent-1.1.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/thread_local.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/utils.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/version.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/__init__.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/deep.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/types.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/attributes/__init__.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/auth/__init__.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/__init__.py
--rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/otel.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/python.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/metric/__init__.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/metric/otel_metrics.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/metric/prometheus_metrics.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/plugin/span/__init__.py
--rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/resource/__init__.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/tracepoint/__init__.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/tracepoint/constants.py
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/tracepoint/eventsnapshot.py
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/tracepoint/tracepoint_config.py
--rw-r--r--   0        0        0    21053 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/api/tracepoint/trigger.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/config/__init__.py
--rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/config/config_service.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/config/tracepoint_config.py
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/grpc/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/grpc/grpc_service.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/logging/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/logging/logging.conf
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/poll/__init__.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/poll/poll.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/__init__.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/frame_collector.py
--rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/frame_config.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/trigger_handler.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/variable_processor.py
--rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/variable_set_processor.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/bfs/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/__init__.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/action_context.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/action_results.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/callback_context.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/log_action.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/metric_action.py
--rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/snapshot_action.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/span_action.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/processor/context/trigger_context.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/push/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/push/push_service.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 deep_agent-1.1.0/src/deep/task/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/test_utils.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/utils.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/it_tests/__init__.py
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/it_tests/it_utils.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/it_tests/test_it_basic.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/it_tests/test_target.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/test_deep.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/test_target.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/test_utils.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/__init__.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/attributes/__init__.py
--rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/attributes/test_attributes.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/plugin/test_otel.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/plugin/test_plugin.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/plugin/test_python.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/plugin/metrics/test_otel_metrics.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/plugin/metrics/test_prometheus_metrics.py
--rw-r--r--   0        0        0    15573 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/api/resource/test_resource.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/auth/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/auth/test_auth.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/config/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/config/test_config.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/config/test_config_service.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/config/test_tracepoint_config.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/grpc/__init__.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/grpc/test_grpc.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/poll/test_poll.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/__init__.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/test_log_messages.py
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/test_trigger_handler.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/test_variable_processor.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/context/__init__.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/context/test_log_action.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/processor/context/test_metric_action.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/push/test_push.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/push/test_push_service.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/task/test_task.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/tracepoint/__init__.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/tracepoint/test_tracepoint_config.py
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deep_agent-1.1.0/tests/unit_tests/tracepoint/test_trigger.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 deep_agent-1.1.0/.gitignore
--rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 deep_agent-1.1.0/LICENSE
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 deep_agent-1.1.0/README.md
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 deep_agent-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 deep_agent-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/thread_local.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/utils.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/version.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/__init__.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/deep.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/types.py
+-rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/attributes/__init__.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/auth/__init__.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/__init__.py
+-rw-r--r--   0        0        0     6085 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/otel.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/python.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/metric/__init__.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/metric/otel_metrics.py
+-rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/metric/prometheus_metrics.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/plugin/span/__init__.py
+-rw-r--r--   0        0        0    11403 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/resource/__init__.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/tracepoint/__init__.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/tracepoint/constants.py
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/tracepoint/eventsnapshot.py
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/tracepoint/tracepoint_config.py
+-rw-r--r--   0        0        0    21053 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/api/tracepoint/trigger.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/config/__init__.py
+-rw-r--r--   0        0        0     7122 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/config/config_service.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/config/tracepoint_config.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/grpc/__init__.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/grpc/grpc_service.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/logging/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/logging/logging.conf
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/poll/__init__.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/poll/poll.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/__init__.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/frame_collector.py
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/frame_config.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/trigger_handler.py
+-rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/variable_processor.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/variable_set_processor.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/bfs/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/__init__.py
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/action_context.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/action_results.py
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/callback_context.py
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/log_action.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/metric_action.py
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/snapshot_action.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/span_action.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/processor/context/trigger_context.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/push/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/push/push_service.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 deep_agent-1.1.1/src/deep/task/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/utils.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/it_tests/__init__.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/it_tests/it_utils.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/it_tests/test_it_basic.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/it_tests/test_target.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/test_deep.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/test_target.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/test_utils.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/attributes/__init__.py
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/attributes/test_attributes.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/plugin/test_otel.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/plugin/test_plugin.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/plugin/test_python.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/plugin/metrics/test_otel_metrics.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/plugin/metrics/test_prometheus_metrics.py
+-rw-r--r--   0        0        0    15963 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/api/resource/test_resource.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/auth/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/auth/test_auth.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/config/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/config/test_config.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/config/test_config_service.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/config/test_tracepoint_config.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/grpc/__init__.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/grpc/test_grpc.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/poll/test_poll.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/__init__.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/test_log_messages.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/test_trigger_handler.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/test_variable_processor.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/context/__init__.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/context/test_log_action.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/processor/context/test_metric_action.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/push/test_push.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/push/test_push_service.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/task/test_task.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/tracepoint/__init__.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/tracepoint/test_tracepoint_config.py
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deep_agent-1.1.1/tests/unit_tests/tracepoint/test_trigger.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 deep_agent-1.1.1/.gitignore
+-rw-r--r--   0        0        0    34522 2020-02-02 00:00:00.000000 deep_agent-1.1.1/LICENSE
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 deep_agent-1.1.1/README.md
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 deep_agent-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 deep_agent-1.1.1/PKG-INFO
```

### Comparing `deep_agent-1.1.0/src/deep/__init__.py` & `deep_agent-1.1.1/src/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/thread_local.py` & `deep_agent-1.1.1/src/deep/thread_local.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/utils.py` & `deep_agent-1.1.1/src/deep/utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/version.py` & `deep_agent-1.1.1/src/deep/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """Version information about deep."""
 
-__version__ = "1.1.0"  # this version is set by the build, but not updated in the code.
+__version__ = "1.1.1"  # this version is set by the build, but not updated in the code.
 """The version of the agent that is running."""
```

### Comparing `deep_agent-1.1.0/src/deep/api/__init__.py` & `deep_agent-1.1.1/src/deep/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/deep.py` & `deep_agent-1.1.1/src/deep/api/deep.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/types.py` & `deep_agent-1.1.1/src/deep/api/types.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/attributes/__init__.py` & `deep_agent-1.1.1/src/deep/api/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/auth/__init__.py` & `deep_agent-1.1.1/src/deep/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/__init__.py` & `deep_agent-1.1.1/src/deep/api/plugin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,18 +144,19 @@
         pass
 
 
 class SnapshotDecorator(Plugin, abc.ABC):
     """Implement this to decorate collected snapshots with attributes."""
 
     @abc.abstractmethod
-    def decorate(self, context: ActionContext) -> Optional[BoundedAttributes]:
+    def decorate(self, snapshot_id: str, context: ActionContext) -> Optional[BoundedAttributes]:
         """
         Decorate a snapshot with additional data.
 
+        :param snapshot_id: the id of the collected snapshot
         :param context: the action context for this action
 
         :return: the additional attributes to attach
         """
         pass
```

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/otel.py` & `deep_agent-1.1.1/src/deep/api/plugin/otel.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,14 +63,24 @@
         Add an attribute to the span.
 
         :param key: the attribute key
         :param value: the attribute value
         """
         self.proxy.set_attribute(key, value)
 
+    def add_event(self, name, attributes=None):
+        """
+        Add an event to the span.
+
+        :param name: the event name
+        :param attributes: the event attributes
+        :return:
+        """
+        self.proxy.add_event(name, attributes=attributes)
+
     def close(self):
         """Close the span."""
         if not self.proxy.end_time:
             try:
                 self.proxy.end()
             except Exception:
                 deep.logging.exception("failed to close span")
@@ -87,22 +97,30 @@
 class OTelPlugin(ResourceProvider, SnapshotDecorator, SpanProcessor):
     """
     Deep Otel plugin.
 
     Provide span and trace information to the snapshot.
     """
 
-    def create_span(self, name: str) -> Optional['Span']:
+    def create_span(self, name: str, context_id: str, tracepoint_id: str) -> Optional['Span']:
         """
         Create and return a new span.
 
         :param name: the name of the span to create
+        :param context_id: the id of the context
+        :param tracepoint_id: the id of thr tracepoint
         :return: the created span
         """
-        span = trace.get_tracer("deep").start_as_current_span(name, end_on_exit=False, attributes={'dynamic': 'deep'})
+        span = trace.get_tracer("deep").start_as_current_span(name,
+                                                              end_on_exit=False,
+                                                              attributes={'dynamic': 'deep',
+                                                                          'context': context_id,
+                                                                          "tracepoint": tracepoint_id
+                                                                          },
+                                                              )
         if span:
             # noinspection PyUnresolvedReferences
             # this is a generator contextlib._GeneratorContextManager
             current = span.__enter__()
             if isinstance(current, _Span):
                 return _OtelSpan(current)
         return None
@@ -125,27 +143,32 @@
         :return: the provided resource
         """
         provider = trace.get_tracer_provider()
         if isinstance(provider, TracerProvider):
             # noinspection PyUnresolvedReferences
             resource = provider.resource
             attributes = dict(resource.attributes)
-            return Resource.create(attributes=attributes)
+            return Resource(attributes=attributes)
         return None
 
-    def decorate(self, context: ActionContext) -> Optional[BoundedAttributes]:
+    def decorate(self, snapshot_id: str, context: ActionContext) -> Optional[BoundedAttributes]:
         """
         Decorate a snapshot with additional data.
 
+        :param snapshot_id: the id of the collected snapshot
         :param context: the action context for this action
 
         :return: the additional attributes to attach
         """
         span = self.current_span()
         if span is not None:
+            span.add_event(context.location_action.location.name,
+                           attributes={"snapshot": snapshot_id,
+                                       "tracepoint": context.location_action.id,
+                                       "context": context.trigger_context.id})
             return BoundedAttributes(attributes={
                 "span_name": span.name,
                 "trace_id": span.trace_id,
                 "span_id": span.span_id
             })
         return None
```

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/python.py` & `deep_agent-1.1.1/src/deep/api/plugin/python.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 class PythonPlugin(ResourceProvider, SnapshotDecorator, TracepointLogger):
     """
     Deep python plugin.
 
     This plugin provides the python version to the resource, and the thread name to the attributes.
     """
 
-    def decorate(self, context: ActionContext) -> Optional[BoundedAttributes]:
+    def decorate(self, snapshot_id: str, context: ActionContext) -> Optional[BoundedAttributes]:
         """
         Decorate a snapshot with additional data.
 
+        :param snapshot_id: the id of the collected snapshot
         :param context: the action context for this action
 
         :return: the additional attributes to attach
         """
         thread = threading.current_thread()
 
         return BoundedAttributes(attributes={
@@ -51,15 +52,15 @@
 
     def resource(self) -> Optional[Resource]:
         """
         Provide resource.
 
         :return: the provided resource
         """
-        return Resource.create({
+        return Resource({
             "python_version": platform.python_version(),
         })
 
     def log_tracepoint(self, log_msg: str, tp_id: str, ctx_id: str):
         """
         Log the dynamic log message.
```

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/metric/__init__.py` & `deep_agent-1.1.1/src/deep/api/plugin/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/metric/otel_metrics.py` & `deep_agent-1.1.1/src/deep/api/plugin/metric/otel_metrics.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/metric/prometheus_metrics.py` & `deep_agent-1.1.1/src/deep/api/plugin/metric/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/plugin/span/__init__.py` & `deep_agent-1.1.1/src/deep/api/plugin/span/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 from deep.api.plugin import Plugin
 
 
 class SpanProcessor(Plugin, abc.ABC):
     """Span processor connects Deep to a span provider."""
 
     @abc.abstractmethod
-    def create_span(self, name: str) -> Optional['Span']:
+    def create_span(self, name: str, context_id: str, tracepoint_id: str) -> Optional['Span']:
         """
         Create and return a new span.
 
         :param name: the name of the span to create
+        :param context_id: the id of the context
+        :param tracepoint_id: the id of thr tracepoint
         :return: the created span
         """
     pass
 
     @abc.abstractmethod
     def current_span(self) -> Optional['Span']:
         """
@@ -76,10 +78,21 @@
 
         :param key: the attribute key
         :param value: the attribute value
         """
         pass
 
     @abc.abstractmethod
+    def add_event(self, name, attributes=None):
+        """
+        Add an event to the span.
+
+        :param name: the event name
+        :param attributes: the event attributes
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
     def close(self):
         """Close the span."""
         pass
```

### Comparing `deep_agent-1.1.0/src/deep/api/resource/__init__.py` & `deep_agent-1.1.1/src/deep/api/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/tracepoint/__init__.py` & `deep_agent-1.1.1/src/deep/api/tracepoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/tracepoint/constants.py` & `deep_agent-1.1.1/src/deep/api/tracepoint/constants.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/tracepoint/eventsnapshot.py` & `deep_agent-1.1.1/src/deep/api/tracepoint/eventsnapshot.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,53 +41,48 @@
         self._var_lookup: Dict[str, 'Variable'] = var_lookup
         self._ts_nanos = ts
         self._frames = frames
         self._watches = []
         self._attributes = BoundedAttributes(immutable=False)
         self._duration_nanos = 0
         self._resource = Resource.get_empty().merge(resource)
-        self._open = True
         self._log = None
 
     def complete(self):
         """Close and complete the snapshot."""
-        if not self._open:
-            return
         self._duration_nanos = time_ns() - self._ts_nanos
-        self._open = False
-
-    def is_open(self):
-        """Is this snapshot still open."""
-        return self._open
 
     def add_watch_result(self, watch_result: 'WatchResult'):
         """
         Append a watch result to the snapshot.
 
         :param watch_result: the result to append.
         :return:
         """
-        if self.is_open():
-            self.watches.append(watch_result)
+        self.watches.append(watch_result)
 
     def merge_var_lookup(self, lookup: Dict[str, 'Variable']):
         """
         Merge additional variables into the var lookup.
 
         :param lookup:  the values to merge
         """
-        if self.is_open():
-            self._var_lookup.update(lookup)
+        self._var_lookup.update(lookup)
 
     @property
     def id(self):
         """The id of this snapshot."""
         return self._id
 
     @property
+    def id_str(self):
+        """The id of this snapshot."""
+        return format(self._id, "032x")
+
+    @property
     def tracepoint(self):
         """The tracepoint that triggered this snapshot."""
         return self._tracepoint
 
     @property
     def var_lookup(self):
         """The captured var lookup."""
@@ -387,32 +382,45 @@
 
         if id(o) == id(self):
             return True
 
         return o._vid == self._vid and o._name == self._name and o._modifiers == self._modifiers
 
 
+WATCH_SOURCE_WATCH = "WATCH"
+"""Watch source for user watch statements."""
+WATCH_SOURCE_LOG = "LOG"
+"""Watch source for log expressions."""
+WATCH_SOURCE_METRIC = "METRIC"
+"""Watch source for metric expressions."""
+WATCH_SOURCE_CAPTURE = "CAPTURE"
+"""Watch source for captured data."""
+
+
 class WatchResult:
     """This is the result of a watch expression."""
 
     def __init__(self,
+                 source: str,
                  expression: str,
                  result: Optional['VariableId'],
-                 error: Optional[str] = None
+                 error: Optional[str] = None,
                  ):
         """
         Create new watch result.
 
+        :param source: the watch source
         :param expression: the expression used
         :param result: the result of the expression
         :param error: the error captured during execution
         """
         self._expression = expression
         self._result = result
         self._error = error
+        self.__source = source
 
     @property
     def expression(self) -> str:
         """The watch expression."""
         return self._expression
 
     @property
@@ -420,7 +428,12 @@
         """The good result."""
         return self._result
 
     @property
     def error(self) -> Optional[str]:
         """The error."""
         return self._error
+
+    @property
+    def source(self):
+        """The watch source."""
+        return self.__source
```

### Comparing `deep_agent-1.1.0/src/deep/api/tracepoint/tracepoint_config.py` & `deep_agent-1.1.1/src/deep/api/tracepoint/tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/api/tracepoint/trigger.py` & `deep_agent-1.1.1/src/deep/api/tracepoint/trigger.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/config/__init__.py` & `deep_agent-1.1.1/src/deep/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/config/config_service.py` & `deep_agent-1.1.1/src/deep/config/config_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/config/tracepoint_config.py` & `deep_agent-1.1.1/src/deep/config/tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/grpc/__init__.py` & `deep_agent-1.1.1/src/deep/grpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     :return: the converted expression
     """
     return [LabelExpression(label.key, __convert_static_value(label), label.expression) for
             label in label_expressions]
 
 
 def __convert_metric_definition(metrics):
-    return [MetricDefinition(m.name, MetricType.Name(metrics[0].type), convert_label_expressions(m.labelExpressions),
+    return [MetricDefinition(m.name, MetricType.Name(m.type), convert_label_expressions(m.labelExpressions),
                              m.expression, m.namespace, m.help, m.unit) for m in metrics]
 
 
 def convert_response(response) -> List[Trigger]:
     """
     Convert a response from GRPC to internal types.
```

### Comparing `deep_agent-1.1.0/src/deep/grpc/grpc_service.py` & `deep_agent-1.1.1/src/deep/grpc/grpc_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/logging/__init__.py` & `deep_agent-1.1.1/src/deep/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/poll/__init__.py` & `deep_agent-1.1.1/src/deep/poll/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/poll/poll.py` & `deep_agent-1.1.1/src/deep/poll/poll.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/__init__.py` & `deep_agent-1.1.1/src/deep/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/frame_collector.py` & `deep_agent-1.1.1/src/deep/processor/frame_collector.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/frame_config.py` & `deep_agent-1.1.1/src/deep/processor/frame_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/trigger_handler.py` & `deep_agent-1.1.1/src/deep/processor/trigger_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,26 +132,27 @@
 
         :param frame: the current frame
         :param event: the event 'line', 'call', etc. That we are processing.
         :param arg: the args
         :return: None to ignore other calls, or our self to continue
         """
         event, file, line, function = self.location_from_event(event, frame)
+        trigger_context = TriggerContext(self._config, self._push_service, frame, event, arg)
+
         if event in ["line", "return", "exception"] and self._callbacks.is_set:
-            self.__process_call_backs(arg, frame, event, file, line, function)
+            self.__process_call_backs(trigger_context, arg, frame, event, file, line, function)
 
         # return if we do not have any tracepoints
         if len(self._tp_config) == 0:
             return None
 
         actions = self.__actions_for_location(event, file, line, function, frame)
         if len(actions) == 0:
             return self.trace_call
 
-        trigger_context = TriggerContext(self._config, self._push_service, frame, event)
         try:
             with trigger_context:
                 for action in actions:
                     try:
                         ctx: ActionContext
                         with trigger_context.action_context(action) as ctx:
                             if ctx.can_trigger():
@@ -172,21 +173,22 @@
     def __actions_for_location(self, event, file, line, function, frame):
         actions = []
         for trigger in self._tp_config:
             if trigger.at_location(event, file, line, function, frame):
                 actions += trigger.actions
         return actions
 
-    def __process_call_backs(self, arg: any, frame: FrameType, event: str, file: str, line: int, function_name: str):
+    def __process_call_backs(self, ctx: 'TriggerContext', arg: any, frame: FrameType, event: str, file: str, line: int,
+                             function_name: str):
         # remove top context
         context: CallbackContext = self._callbacks.value.pop()
         # if it is for our location process it
         if context.at_location(event, file, line, function_name, frame):
             logging.debug("At callback location %s", context.name)
-            context.process(event, frame, arg)
+            context.process(ctx, event, frame, arg)
         else:
             logging.debug("Not at callback location %s", context.name)
             # else put the context back on the queue
             self._callbacks.value.append(context)
 
         if len(self._callbacks.value) == 0:
             logging.debug("Callbacks cleared.")
```

### Comparing `deep_agent-1.1.0/src/deep/processor/variable_processor.py` & `deep_agent-1.1.1/src/deep/processor/variable_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     'int',
     'float',
     'bool',
     'type',
     'module',
     'unicode',
     'long',
+    'NoneType',
+    'traceback'
 ]
 """A list of types that do not have child nodes, or only have child nodes we do not want to process."""
 
 LIST_LIKE_TYPES = [
     'frozenset',
     'set',
     'list',
```

### Comparing `deep_agent-1.1.0/src/deep/processor/variable_set_processor.py` & `deep_agent-1.1.1/src/deep/processor/variable_set_processor.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/bfs/__init__.py` & `deep_agent-1.1.1/src/deep/processor/bfs/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/context/__init__.py` & `deep_agent-1.1.1/src/deep/processor/context/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/context/action_context.py` & `deep_agent-1.1.1/src/deep/processor/context/action_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 """Handling for action context."""
 
 import abc
 from typing import Tuple, TYPE_CHECKING, Dict
 
 import deep.logging
+from deep.api.tracepoint.eventsnapshot import WATCH_SOURCE_CAPTURE
 from deep.logging import logging
 from deep.api.tracepoint import WatchResult, Variable
 from deep.processor.variable_set_processor import VariableSetProcessor
 from deep.utils import str2bool
 
 if TYPE_CHECKING:
     from deep.processor.context.trigger_context import TriggerContext
@@ -61,31 +62,45 @@
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         """Exit and close the context."""
         if self.has_triggered():
             self.location_action.record_triggered(self.trigger_context.ts)
 
-    def eval_watch(self, watch: str) -> Tuple[WatchResult, Dict[str, Variable], str]:
+    def eval_watch(self, watch: str, source: str) -> Tuple[WatchResult, Dict[str, Variable], str]:
         """
         Evaluate an expression in the current frame.
 
+        :param source: The watch source.
         :param watch: The watch expression to evaluate.
         :return: Tuple with WatchResult, collected variables, and the log string for the expression
         """
         var_processor = VariableSetProcessor({}, self.trigger_context.var_cache)
 
         try:
             result = self.trigger_context.evaluate_expression(watch)
             variable_id, log_str = var_processor.process_variable(watch, result)
 
-            return WatchResult(watch, variable_id), var_processor.var_lookup, log_str
+            return WatchResult(source, watch, variable_id), var_processor.var_lookup, log_str
         except BaseException as e:
             logging.exception("Error evaluating watch %s", watch)
-            return WatchResult(watch, None, str(e)), {}, str(e)
+            return WatchResult(source, watch, None, str(e)), {}, str(e)
+
+    def process_capture_variable(self, name: str, variable: any) -> Tuple[WatchResult, Dict[str, Variable], str]:
+        """
+        Process a captured variable (exception or return), into a variable set.
+
+        :param name: the name to use (raised or returned)
+        :param variable: the value to process
+        :return: Tuple with WatchResult, collected variables, and the log string for the expression
+        """
+        var_processor = VariableSetProcessor({}, self.trigger_context.var_cache)
+        variable_id, log_str = var_processor.process_variable(name, variable)
+
+        return WatchResult(WATCH_SOURCE_CAPTURE, name, variable_id), var_processor.var_lookup, log_str
 
     def process(self):
         """Process the action."""
         try:
             return self._process_action()
         finally:
             self._triggered = True
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/action_results.py` & `deep_agent-1.1.1/src/deep/processor/context/action_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,19 @@
     from deep.processor.context.trigger_context import TriggerContext
 
 
 class ActionCallback:
     """A call back to 'close' an action."""
 
     @abc.abstractmethod
-    def process(self, event: str, frame: FrameType, arg: any) -> bool:
+    def process(self, ctx: 'TriggerContext', event: str, frame: FrameType, arg: any) -> bool:
         """
         Process a callback.
 
+        :param ctx: the context for this trigger
         :param event: the event
         :param frame: the frame data
         :param arg: the arg from settrace
         :return: True, to keep this callback until next match.
         """
         pass
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/callback_context.py` & `deep_agent-1.1.1/src/deep/processor/context/callback_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """Handling for action callbacks."""
 from types import FrameType
 from typing import List
 
 from deep.api.tracepoint.trigger import Location
 
 from deep.processor.context.action_results import ActionCallback
+from deep.processor.context.trigger_context import TriggerContext
 
 
 class CallbackContext(Location, ActionCallback):
     """
     Callback Context deals with ensuring we close any pending actions created by TriggerHandler.
 
     If a span is created on a line or method, then we attach a callback that will trigger the span
@@ -55,25 +56,26 @@
             return False
 
         if self.__event == 'line':
             return self.__check_at_next_line(event, file, function_name)
         else:
             return self.__check_at_method_end(event)
 
-    def process(self, event: str, frame: FrameType, arg: any):
+    def process(self, ctx: 'TriggerContext', event: str, frame: FrameType, arg: any):
         """
         Process all callbacks.
 
+        :param ctx: the context for this trigger
         :param event: the event
         :param frame: the frame data
         :param arg: the arg from settrace
         :return: True, to keep this callback until next match.
         """
         for callback in self.__callbacks:
-            callback.process(event, frame, arg)
+            callback.process(ctx, event, frame, arg)
 
     @property
     def id(self) -> str:
         """The location id."""
         return "%s#%s" % (self.path, self.name)
 
     @property
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/log_action.py` & `deep_agent-1.1.1/src/deep/processor/context/log_action.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 """Handling for log actions."""
 
 from typing import TYPE_CHECKING, List, Dict, Optional
 
 from .action_context import ActionContext
 from .action_results import ActionResult, ActionCallback
 from ...api.tracepoint.constants import LOG_MSG
+from ...api.tracepoint.eventsnapshot import WATCH_SOURCE_LOG
 from ...api.tracepoint.trigger import LocationAction
 
 from typing import Tuple
 
 if TYPE_CHECKING:
     from ...api.tracepoint import WatchResult, Variable
     from .trigger_context import TriggerContext
@@ -79,15 +80,15 @@
 
             This type allows us to use watches within log strings and collect the watch
             as well as interpolate the values.
             """
 
             def get_field(self, field_name, args, kwargs):
                 # evaluate watch
-                watch, var_lookup, log_str = ctx_self.eval_watch(field_name)
+                watch, var_lookup, log_str = ctx_self.eval_watch(field_name, WATCH_SOURCE_LOG)
                 # collect data
                 watch_results.append(watch)
                 _var_lookup.update(var_lookup)
 
                 return log_str, field_name
 
         log_msg = "[deep] %s" % FormatExtractor().vformat(log_msg, (), FormatDict(self.trigger_context.locals))
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/metric_action.py` & `deep_agent-1.1.1/src/deep/processor/context/metric_action.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/processor/context/snapshot_action.py` & `deep_agent-1.1.1/src/deep/processor/context/snapshot_action.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """Handling for snapshot actions."""
-
+from types import FrameType
 from typing import Tuple, Optional, TYPE_CHECKING
 
 import deep.logging
 from deep.api.attributes import BoundedAttributes
 from deep.api.tracepoint import EventSnapshot
-from deep.api.tracepoint.constants import FRAME_TYPE, SINGLE_FRAME_TYPE, NO_FRAME_TYPE, ALL_FRAME_TYPE
+from deep.api.tracepoint.constants import FRAME_TYPE, SINGLE_FRAME_TYPE, NO_FRAME_TYPE, ALL_FRAME_TYPE, STAGE, \
+    LINE_CAPTURE, METHOD_CAPTURE
+from deep.api.tracepoint.eventsnapshot import WATCH_SOURCE_WATCH
 from deep.api.tracepoint.trigger import LocationAction
 from deep.processor.context.action_context import ActionContext
 from deep.processor.context.action_results import ActionResult, ActionCallback
 from deep.processor.context.log_action import LOG_MSG, LogActionContext, LogActionResult
 from deep.processor.frame_collector import FrameCollectorContext, FrameCollector
 from deep.processor.variable_set_processor import VariableProcessorConfig
 
@@ -111,15 +113,15 @@
         frames, variables = collector.collect(self.trigger_context.vars, self.trigger_context.var_cache)
 
         snapshot = EventSnapshot(self.location_action.tracepoint, self.trigger_context.ts,
                                  self.trigger_context.resource, frames, variables)
 
         # process the snapshot watches
         for watch in self.watches:
-            result, watch_lookup, _ = self.eval_watch(watch)
+            result, watch_lookup, _ = self.eval_watch(watch, WATCH_SOURCE_WATCH)
             snapshot.add_watch_result(result)
             snapshot.merge_var_lookup(watch_lookup)
 
         log_msg = self.log_msg
         if log_msg is not None:
             # create and process the log message
             context = LogActionContext(self.trigger_context, LocationAction(self.location_action.id, None, {
@@ -128,19 +130,34 @@
             log, watches, log_vars = context.process_log(log_msg)
             snapshot.log_msg = log
             for watch in watches:
                 snapshot.add_watch_result(watch)
             snapshot.merge_var_lookup(log_vars)
             self.trigger_context.attach_result(LogActionResult(context.location_action, log))
 
-        self.trigger_context.attach_result(SendSnapshotActionResult(self, snapshot))
+        if self.trigger_context.event in ['exception', 'return']:
+            watch, new_vars, _ = self.process_capture_variable(self.trigger_context.event, self.trigger_context.arg)
+            snapshot.add_watch_result(watch)
+            snapshot.merge_var_lookup(new_vars)
+
+        snapshot.complete()
+        if self._is_deferred():
+            self.trigger_context.attach_result(DeferredSnapshotActionResult(self, snapshot))
+        else:
+            self.trigger_context.attach_result(SendSnapshotActionResult(self, snapshot))
+
+    def _is_deferred(self):
+        stage = self.location_action.config.get(STAGE, None)
+        if stage is None:
+            return False
+        return stage == LINE_CAPTURE or stage == METHOD_CAPTURE
 
 
-class SendSnapshotActionResult(ActionResult):
-    """The result of a successful snapshot action."""
+class DeferredSnapshotActionResult(ActionResult):
+    """The result of a deferred snapshot action."""
 
     def __init__(self, action_context: ActionContext, snapshot: EventSnapshot):
         """
         Create a new snapshot action result.
 
         :param action_context: the action context that created this result
         :param snapshot: the snapshot result
@@ -152,19 +169,80 @@
         """
         Process this result.
 
         :param ctx: the triggering context
 
         :return: an action callback if we need to do something at the 'end', or None
         """
-        attributes = BoundedAttributes(attributes={'ctx_id': ctx.id}, immutable=False)
+        snapshot = self._decorate_snapshot(ctx)
+        return DeferredSnapshotActionCallback(self.action_context, snapshot)
+
+    def _decorate_snapshot(self, ctx):
+        attributes = BoundedAttributes(
+            attributes={'context': ctx.id, 'tracepoint': self.action_context.location_action.tracepoint.id},
+            immutable=False)
         for decorator in ctx.config.snapshot_decorators:
             try:
-                decorate = decorator.decorate(self.action_context)
+                decorate = decorator.decorate(self.snapshot.id_str, self.action_context)
                 if decorate is not None:
                     attributes.merge_in(decorate)
             except Exception:
                 deep.logging.exception("Failed to decorate snapshot: %s ", decorator)
-
         self.snapshot.attributes.merge_in(attributes)
-        ctx.push_service.push_snapshot(self.snapshot)
+        return self.snapshot
+
+
+class DeferredSnapshotActionCallback(ActionCallback):
+    """Defer the send action to the end of the line or function."""
+
+    def __init__(self, action_context: ActionContext, snapshot: EventSnapshot):
+        """
+        Create a new action callback.
+
+        :param action_context: the triggering action context
+        :param snapshot: the generated snapshot
+        """
+        self.__action_context = action_context
+        self.__snapshot = snapshot
+
+    def process(self, ctx: 'TriggerContext', event: str, frame: FrameType, arg: any) -> bool:
+        """
+        Process a callback.
+
+        :param ctx: the context for this trigger
+        :param event: the event
+        :param frame: the frame data
+        :param arg: the arg from settrace
+        :return: True, to keep this callback until next match.
+        """
+        if event in ['exception', 'return']:
+            watch, new_vars, _ = self.__action_context.process_capture_variable(event, arg)
+            self.__snapshot.add_watch_result(watch)
+            self.__snapshot.merge_var_lookup(new_vars)
+
+        ctx.push_service.push_snapshot(self.__snapshot)
+        return False
+
+
+class SendSnapshotActionResult(DeferredSnapshotActionResult):
+    """The result of a successful snapshot action."""
+
+    def __init__(self, action_context: ActionContext, snapshot: EventSnapshot):
+        """
+        Create a new snapshot action result.
+
+        :param action_context: the action context that created this result
+        :param snapshot: the snapshot result
+        """
+        super().__init__(action_context, snapshot)
+
+    def process(self, ctx: 'TriggerContext') -> Optional[ActionCallback]:
+        """
+        Process this result.
+
+        :param ctx: the triggering context
+
+        :return: an action callback if we need to do something at the 'end', or None
+        """
+        snapshot = self._decorate_snapshot(ctx)
+        ctx.push_service.push_snapshot(snapshot)
         return None
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/span_action.py` & `deep_agent-1.1.1/src/deep/processor/context/span_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 class SpanActionCallback(ActionCallback):
     """Action callback to close created spans."""
 
     def __init__(self, spans):
         """Create callback."""
         self.__spans = spans
 
-    def process(self, event: str, frame: FrameType, arg: any) -> bool:
+    def process(self, ctx: 'TriggerContext', event: str, frame: FrameType, arg: any) -> bool:
         """
         Process a callback.
 
+        :param ctx: the context for this trigger
         :param event: the event
         :param frame: the frame data
         :param arg: the arg from settrace
         :return: True, to keep this callback until next match.
         """
         for span in self.__spans:
             span.close()
@@ -81,15 +82,15 @@
         name = self._span_name
         if name is None:
             return
 
         spans = []
 
         for span_processor in self.trigger_context.config.span_processors:
-            span = span_processor.create_span(name)
+            span = span_processor.create_span(name, self.trigger_context.id, self.location_action.tracepoint.id)
             if span:
                 spans.append(span)
 
         if len(spans) > 0:
             self.trigger_context.attach_result(SpanResult(spans))
 
     @property
```

### Comparing `deep_agent-1.1.0/src/deep/processor/context/trigger_context.py` & `deep_agent-1.1.1/src/deep/processor/context/trigger_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,26 +40,28 @@
     """
     Context for a trigger.
 
     A context is created in a valid location is triggered. This context is then used to process all the actions,
     collect the data and ship of the results.
     """
 
-    def __init__(self, config: ConfigService, push_service: PushService, frame: FrameType, event: str):
+    def __init__(self, config: ConfigService, push_service: PushService, frame: FrameType, event: str, arg: any):
         """
         Create a new trigger context.
 
         :param config: the config service
         :param push_service: the push service
         :param frame: the frame data
         :param event: the trigger event
+        :param arg: the trigger arg
         """
         self.__push_service = push_service
         self.__event = event
         self.__frame = frame
+        self.__arg = arg
         self.__config = config
         self.__results: List[ActionResult] = []
         self.__ts: int = time_ns()
         self.__id: str = str(uuid.uuid4())
         self.__frame_collector: Optional[FrameCollector] = None
         self.var_cache = VariableCacheProvider()
         self.callbacks: List[ActionCallback] = []
@@ -110,14 +112,24 @@
         return self.__frame
 
     @property
     def config(self) -> ConfigService:
         """The config service."""
         return self.__config
 
+    @property
+    def arg(self):
+        """The trigger arg value."""
+        return self.__arg
+
+    @property
+    def event(self):
+        """The trigger event value."""
+        return self.__event
+
     def action_context(self, action: 'LocationAction') -> 'ActionContext':
         """
         Create an action context from this context, for the provided action.
 
         :param action: the action
         :return: the new action context.
         """
```

### Comparing `deep_agent-1.1.0/src/deep/push/__init__.py` & `deep_agent-1.1.1/src/deep/push/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import logging
 
 # noinspection PyUnresolvedReferences
 from deepproto.proto.common.v1.common_pb2 import KeyValue
 # noinspection PyUnresolvedReferences
 from deepproto.proto.tracepoint.v1.tracepoint_pb2 import Snapshot, TracePointConfig, WatchResult, Variable, \
-    VariableID, StackFrame
+    VariableID, StackFrame, WatchSource
 
 from .push_service import PushService
 
 __all__ = [PushService.__name__]
 
 from ..api.tracepoint import TracePointConfig as TrPoCo, EventSnapshot, StackFrame as StFr, WatchResult as WaRe, \
     Variable as Var, VariableId as VarId
@@ -51,17 +51,21 @@
                       app_frame=frame.app_frame,
                       transpiled_file_name=frame.transpiled_file_name,
                       transpiled_line_number=frame.transpiled_line_number,
                       transpiled_column_number=frame.transpiled_column_number,
                       )
 
 
+def __convert_watch_source(source):
+    return WatchSource.Value(source)
+
+
 def __convert_watch(watch: WaRe):
     return WatchResult(expression=watch.expression, good_result=__convert_variable_id(watch.result),
-                       error_result=watch.error)
+                       error_result=watch.error, source=__convert_watch_source(watch.source))
 
 
 def __convert_variable(variable: Var):
     return Variable(type=variable.type, value=variable.value, hash=variable.hash,
                     children=[__convert_variable_id(c) for c in variable.children], truncated=variable.truncated)
```

### Comparing `deep_agent-1.1.0/src/deep/push/push_service.py` & `deep_agent-1.1.1/src/deep/push/push_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/src/deep/task/__init__.py` & `deep_agent-1.1.1/src/deep/task/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/test_utils.py` & `deep_agent-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/utils.py` & `deep_agent-1.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/it_tests/__init__.py` & `deep_agent-1.1.1/tests/it_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/it_tests/it_utils.py` & `deep_agent-1.1.1/tests/it_tests/it_utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/it_tests/test_it_basic.py` & `deep_agent-1.1.1/tests/it_tests/test_it_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,17 @@
             _deep = deep.start(server.config({}))
             server.await_poll()
             test = BPTargetTest("name", 123)
             _ = test.name
             snapshot = server.await_snapshot()
             _deep.shutdown()
             self.assertIsNotNone(snapshot)
+
+            self.assertIsNot(0, snapshot.duration_nanos)
+
             frames = snapshot.frames
             self.assertEqual(it_tests.test_target.__file__, frames[0].file_name)
             self.assertEqual("/it_tests/test_target.py", frames[0].short_path)
             self.assertEqual(40, frames[0].line_number)
             self.assertEqual(4, len(frames[0].variables))
             self.assertEqual(6, len(snapshot.var_lookup))
 
@@ -77,14 +80,16 @@
                 test = BPTargetTest("name", 123)
                 _ = test.name
                 snapshot = server.await_snapshot()
                 _deep.shutdown()
 
                 self.assertIsNotNone(snapshot)
 
+                self.assertIsNot(0, snapshot.duration_nanos)
+
                 self.assertEqual("[deep] test log name", snapshot.log_msg)
                 self.assertIn("[deep] test log name", logs.output[0])
 
                 frames = snapshot.frames
                 self.assertEqual(it_tests.test_target.__file__, frames[0].file_name)
                 self.assertEqual("/it_tests/test_target.py", frames[0].short_path)
                 self.assertEqual(40, frames[0].line_number)
```

### Comparing `deep_agent-1.1.0/tests/it_tests/test_target.py` & `deep_agent-1.1.1/tests/it_tests/test_target.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/test_deep.py` & `deep_agent-1.1.1/tests/unit_tests/test_deep.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/test_target.py` & `deep_agent-1.1.1/tests/unit_tests/test_target.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,7 +21,11 @@
 """
 
 
 def some_test_function(arg):
     val = arg + "something"
 
     return val
+
+
+def some_test_error(arg):
+    raise Exception(some_test_function(arg))
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/test_utils.py` & `deep_agent-1.1.1/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/attributes/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/api/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/attributes/test_attributes.py` & `deep_agent-1.1.1/tests/unit_tests/api/attributes/test_attributes.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/plugin/test_otel.py` & `deep_agent-1.1.1/tests/unit_tests/api/plugin/test_otel.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import unittest
 
+import mockito
 from opentelemetry import trace
 from opentelemetry.sdk.resources import Resource, SERVICE_NAME
 from opentelemetry.sdk.trace import TracerProvider
 
 from deep.api.plugin.otel import OTelPlugin
+from deep.api.resource import TELEMETRY_SDK_NAME
 
 
 class TestOtel(unittest.TestCase):
 
     def setUp(self):
         resource = Resource(attributes={
             SERVICE_NAME: "your-service-name"
@@ -31,16 +33,36 @@
         trace.set_tracer_provider(provider)
 
     def test_load_plugin(self):
         plugin = OTelPlugin()
         load_plugin = plugin.resource()
         self.assertIsNotNone(load_plugin)
         self.assertEqual("your-service-name", load_plugin.attributes.get(SERVICE_NAME))
+        self.assertIsNone(load_plugin.attributes.get(TELEMETRY_SDK_NAME))
 
     def test_collect_attributes(self):
         with trace.get_tracer_provider().get_tracer("test").start_as_current_span("test-span"):
             plugin = OTelPlugin()
-            attributes = plugin.decorate(None)
+
+            mock = mockito.mock()
+            mock.trigger_context = mock
+            mock.trigger_context.id = "id"
+            mock.location_action = mock
+            mock.location_action.id = "id"
+            mock.location_action.location = mock
+            mock.location_action.location.name = "test"
+
+            attributes = plugin.decorate("snap_id", mock)
             self.assertIsNotNone(attributes)
             self.assertEqual("test-span", attributes.get("span_name"))
             self.assertIsNotNone(attributes.get("span_id"))
             self.assertIsNotNone(attributes.get("trace_id"))
+            self.assertEqual(plugin.current_span().proxy.events[0].name, "test")
+            self.assertEqual(plugin.current_span().proxy.events[0].attributes,
+                             {'snapshot': 'snap_id', 'tracepoint': 'id', 'context': 'id'})
+
+    def test_create_span(self):
+        plugin = OTelPlugin()
+        span = plugin.create_span("test", "ctx_id", "tp_id")
+        self.assertIsNotNone(span)
+        attributes = span.proxy.attributes
+        self.assertEqual({"dynamic": "deep", "context": "ctx_id", "tracepoint": "tp_id"}, attributes)
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/plugin/test_plugin.py` & `deep_agent-1.1.1/tests/unit_tests/api/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/plugin/test_python.py` & `deep_agent-1.1.1/tests/unit_tests/api/plugin/test_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,10 +23,10 @@
         plugin = PythonPlugin()
         load_plugin = plugin.resource()
         self.assertIsNotNone(load_plugin)
         self.assertIsNotNone(load_plugin.attributes.get('python_version'))
 
     def test_collect_attributes(self):
         plugin = PythonPlugin()
-        attributes = plugin.decorate(None)
+        attributes = plugin.decorate("", None)
         self.assertIsNotNone(attributes)
         self.assertEqual("MainThread", attributes.get("thread_name"))
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/plugin/metrics/test_otel_metrics.py` & `deep_agent-1.1.1/tests/unit_tests/api/plugin/metrics/test_otel_metrics.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/plugin/metrics/test_prometheus_metrics.py` & `deep_agent-1.1.1/tests/unit_tests/api/plugin/metrics/test_prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/api/resource/test_resource.py` & `deep_agent-1.1.1/tests/unit_tests/api/resource/test_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,23 @@
     def setUp(self) -> None:
         logging.init(ConfigService({}))
         environ[DEEP_RESOURCE_ATTRIBUTES] = ""
 
     def tearDown(self) -> None:
         environ.pop(DEEP_RESOURCE_ATTRIBUTES)
 
+    def test_merge(self):
+        create = Resource.create()
+        new_resource = Resource.create({SERVICE_NAME: 'test'})
+        self.assertEqual("unknown_service:python", create.attributes[SERVICE_NAME])
+        self.assertEqual("test", new_resource.attributes[SERVICE_NAME])
+
+        merge = create.merge(new_resource)
+        self.assertEqual("test", merge.attributes[SERVICE_NAME])
+
     def test_create(self):
         attributes = {
             "service": "ui",
             "version": 1,
             "has_bugs": True,
             "cost": 112.12,
         }
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/auth/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/auth/test_auth.py` & `deep_agent-1.1.1/tests/unit_tests/auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/config/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/config/test_config.py` & `deep_agent-1.1.1/tests/unit_tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/config/test_config_service.py` & `deep_agent-1.1.1/tests/unit_tests/config/test_config_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/config/test_tracepoint_config.py` & `deep_agent-1.1.1/tests/unit_tests/config/test_tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/grpc/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/grpc/test_grpc.py` & `deep_agent-1.1.1/tests/unit_tests/grpc/test_grpc.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/poll/test_poll.py` & `deep_agent-1.1.1/tests/unit_tests/poll/test_poll.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/test_log_messages.py` & `deep_agent-1.1.1/tests/unit_tests/processor/test_log_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         ["some log message: {person}", "[deep] some log message: {'name': 'bob'}",
          {'person': {'name': 'bob'}}, ["Size: 1"]],
         ["some log message: {person.name}", "[deep] some log message: 'dict' object has no attribute 'name'",
          {'person': {'name': 'bob'}}, ["'dict' object has no attribute 'name'"]],
         ["some log message: {person['name']}", "[deep] some log message: bob", {'person': {'name': 'bob'}}, ["bob"]],
     ])
     def test_simple_log_interpolation(self, log_msg, expected_msg, _locals, expected_watches):
-        context = LogActionContext(TriggerContext(None, None, MockFrame(_locals), "test"), None)
+        context = LogActionContext(TriggerContext(None, None, MockFrame(_locals), "test", None), None)
         log, watches, _vars = context.process_log(log_msg)
 
         self.assertEqual(expected_msg, log)
         self.assertEqual(len(expected_watches), len(watches))
         for i, watch in enumerate(watches):
             if watch.error is None:
                 self.assertEqual(_vars[watch.result.vid].value, expected_watches[i])
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/test_trigger_handler.py` & `deep_agent-1.1.1/tests/unit_tests/processor/test_trigger_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 import mockito
 
 from deep import logging
 from deep.api.plugin import TracepointLogger
 from deep.api.plugin.metric import MetricProcessor
 from deep.api.plugin.span import SpanProcessor
 from deep.api.resource import Resource
-from deep.api.tracepoint.constants import LOG_MSG, WATCHES
+from deep.api.tracepoint.constants import LOG_MSG, WATCHES, METHOD_CAPTURE, STAGE
 from deep.api.tracepoint.eventsnapshot import EventSnapshot
 from deep.api.tracepoint.tracepoint_config import MetricDefinition
 
 from deep.api.tracepoint.trigger import Location, LocationAction, LineLocation, Trigger, FunctionLocation
 from deep.config import ConfigService
 from deep.processor.trigger_handler import TriggerHandler
 from deep.push.push_service import PushService
-from unit_tests.test_target import some_test_function
+from unit_tests.test_target import some_test_function, some_test_error
 
 
 class MockPushService(PushService):
     def __init__(self, grpc, task_handler):
         super().__init__(grpc, task_handler)
         self.pushed: List[EventSnapshot] = []
 
@@ -87,38 +87,58 @@
     def __init__(self):
         self.captured_frame = None
         self.captured_event = None
         self.captured_args = None
 
     def capture_trace_call(self, location: Location):
         def trace_call(frame, event, args):
+            # print(frame, event, args)
             event, file, line, function = TriggerHandler.location_from_event(event, frame)
-            if location.at_location(event, file, line, function, frame):
+            # on raise exception we get a return immediately after,
+            # so if we have captured an exception don't capture again
+            if location.at_location(event, file, line, function, frame) and not self.captured_exception():
+                print("Capture frame:", frame, event, args)
                 self.captured_frame = frame
                 self.captured_event = event
                 self.captured_args = args
             return trace_call
 
         return trace_call
 
+    def captured_exception(self):
+        if self.captured_event == "exception":
+            return True
+        return False
+
+    def clear(self):
+        self.captured_frame = None
+        self.captured_event = None
+        self.captured_args = None
+
 
 logging.init(MockConfigService({}))
 
 
 class TestTriggerHandler(unittest.TestCase):
 
     def call_and_capture(self, location, func, args, capture):
         # here we execute the real code using a mock trace call that will capture the args to trace call
         # we cannot debug this section of the code
 
+        def func_wrap(*args):
+            try:
+                func(*args)
+            except Exception:
+                pass
+
         # we use the _trace_hook and nopt gettrace() as gettrace() is not available in all tested versions of pythong
         # noinspection PyUnresolvedReferences
         current = threading._trace_hook
         threading.settrace(capture.capture_trace_call(location))
-        thread = Thread(target=func, args=args)
+        thread = Thread(target=func_wrap, args=args)
         thread.start()
         thread.join(10)
 
         # reset the set trace to the original one
         threading.settrace(current)
 
         if capture.captured_frame is None:
@@ -232,37 +252,137 @@
         mockito.verify(mock_plugin, mockito.times(1)).counter("simple_test", {}, 'deep', None, None, 1)
 
     def test_span_action(self):
         capture = TraceCallCapture()
         config = MockConfigService({})
         mock_plugin = mockito.mock(spec=SpanProcessor)
         mock_span = mockito.mock()
-        mockito.when(mock_plugin).create_span('some_test_function').thenReturn(mock_span)
+        mockito.when(mock_plugin).create_span('some_test_function', mockito.ANY, mockito.ANY).thenReturn(mock_span)
         config.plugins = [mock_plugin]
         push = MockPushService(None, None)
         handler = TriggerHandler(config, push)
 
         location = FunctionLocation('test_target.py', "some_test_function", Location.Position.START)
         handler.new_config([Trigger(location, [
             LocationAction("tp_id", "", {},
                            LocationAction.ActionType.Span)])])
 
         self.call_and_capture(location, some_test_function, ['input'], capture)
 
         handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
 
+        capture.clear()
+
         # now extract the callback value
         pop = handler._callbacks.value
         # capture the real data that would be sent when we match this location
         self.call_and_capture(pop[0], some_test_function, ['input'], capture)
 
         # now call our trace call to check our callbacks
         handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
 
         logged = config.logger.logged
         self.assertEqual(0, len(logged))
         pushed = push.pushed
         self.assertEqual(0, len(pushed))
 
-        mockito.verify(mock_plugin, mockito.times(1)).create_span("some_test_function")
+        mockito.verify(mock_plugin, mockito.times(1)).create_span("some_test_function", mockito.ANY, mockito.ANY)
 
         mockito.verify(mock_span, mockito.times(1)).close()
+
+    def test_method_result_capture(self):
+        capture = TraceCallCapture()
+        config = MockConfigService({})
+        push = MockPushService(None, None)
+        handler = TriggerHandler(config, push)
+
+        location = FunctionLocation('test_target.py', "some_test_function", Location.Position.START)
+        handler.new_config([Trigger(location, [
+            LocationAction("tp_id", "", {STAGE: METHOD_CAPTURE}, LocationAction.ActionType.Snapshot)])])
+
+        self.call_and_capture(location, some_test_function, ['input'], capture)
+
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        capture.clear()
+
+        # now extract the callback value
+        pop = handler._callbacks.value
+        # capture the real data that would be sent when we match this location
+        self.call_and_capture(pop[0], some_test_function, ['input'], capture)
+
+        # now call our trace call to check our callbacks
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        logged = config.logger.logged
+        self.assertEqual(0, len(logged))
+        pushed = push.pushed
+        self.assertEqual(1, len(pushed))
+
+        self.assertEqual("return", pushed[0].watches[0].expression)
+        self.assertEqual("inputsomething", pushed[0].var_lookup[pushed[0].watches[0].result.vid].value)
+
+    def test_method_exception_capture(self):
+        capture = TraceCallCapture()
+        config = MockConfigService({})
+        push = MockPushService(None, None)
+        handler = TriggerHandler(config, push)
+
+        location = FunctionLocation('test_target.py', "some_test_error", Location.Position.START)
+        handler.new_config([Trigger(location, [
+            LocationAction("tp_id", "", {STAGE: METHOD_CAPTURE}, LocationAction.ActionType.Snapshot)])])
+
+        self.call_and_capture(location, some_test_error, ['input'], capture)
+
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        capture.clear()
+
+        # now extract the callback value
+        pop = handler._callbacks.value
+        # capture the real data that would be sent when we match this location
+        self.call_and_capture(pop[0], some_test_error, ['input'], capture)
+
+        # now call our trace call to check our callbacks
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        logged = config.logger.logged
+        self.assertEqual(0, len(logged))
+        pushed = push.pushed
+        self.assertEqual(1, len(pushed))
+        self.assertEqual(1, len(pushed[0].watches))
+
+        self.assertEqual("exception", pushed[0].watches[0].expression)
+        self.assertEqual("Size: 3", pushed[0].var_lookup[pushed[0].watches[0].result.vid].value)
+
+    def test_line_exception_capture(self):
+        capture = TraceCallCapture()
+        config = MockConfigService({})
+        push = MockPushService(None, None)
+        handler = TriggerHandler(config, push)
+
+        location = LineLocation('test_target.py', 31, Location.Position.START)
+        handler.new_config([Trigger(location, [
+            LocationAction("tp_id", "", {STAGE: METHOD_CAPTURE}, LocationAction.ActionType.Snapshot)])])
+
+        self.call_and_capture(location, some_test_error, ['input'], capture)
+
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        capture.clear()
+
+        # now extract the callback value
+        pop = handler._callbacks.value
+        # capture the real data that would be sent when we match this location
+        self.call_and_capture(pop[0], some_test_error, ['input'], capture)
+
+        # now call our trace call to check our callbacks
+        handler.trace_call(capture.captured_frame, capture.captured_event, capture.captured_args)
+
+        logged = config.logger.logged
+        self.assertEqual(0, len(logged))
+        pushed = push.pushed
+        self.assertEqual(1, len(pushed))
+        self.assertEqual(1, len(pushed[0].watches))
+
+        self.assertEqual("exception", pushed[0].watches[0].expression)
+        self.assertEqual("Size: 3", pushed[0].var_lookup[pushed[0].watches[0].result.vid].value)
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/test_variable_processor.py` & `deep_agent-1.1.1/tests/unit_tests/processor/test_variable_processor.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/context/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/processor/context/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/context/test_log_action.py` & `deep_agent-1.1.1/tests/unit_tests/processor/context/test_log_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         ["some log message: {person}", "[deep] some log message: {'name': 'bob'}",
          {'person': {'name': 'bob'}}, ["Size: 1"]],
         ["some log message: {person.name}", "[deep] some log message: 'dict' object has no attribute 'name'",
          {'person': {'name': 'bob'}}, ["'dict' object has no attribute 'name'"]],
         ["some log message: {person['name']}", "[deep] some log message: bob", {'person': {'name': 'bob'}}, ["bob"]],
     ])
     def test_simple_log_interpolation(self, log_msg, expected_msg, _locals, expected_watches):
-        context = LogActionContext(TriggerContext(None, None, MockFrame(_locals), "test"), None)
+        context = LogActionContext(TriggerContext(None, None, MockFrame(_locals), "test", None), None)
         log, watches, _vars = context.process_log(log_msg)
         self.assertEqual(expected_msg, log)
         self.assertEqual(len(expected_watches), len(watches))
         for i, watch in enumerate(watches):
             if watch.error is None:
                 self.assertEqual(_vars[watch.result.vid].value, expected_watches[i])
             else:
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/processor/context/test_metric_action.py` & `deep_agent-1.1.1/tests/unit_tests/processor/context/test_metric_action.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/push/test_push.py` & `deep_agent-1.1.1/tests/unit_tests/push/test_push.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from deep.api.tracepoint import WatchResult
+from deep.api.tracepoint.eventsnapshot import WATCH_SOURCE_WATCH
 from deep.push import convert_snapshot
 from utils import mock_snapshot, mock_frame, mock_variable, mock_variable_id
 
 
 def test_convert_snapshot():
     event_snapshot = mock_snapshot()
     snapshot = convert_snapshot(event_snapshot)
@@ -48,27 +49,27 @@
     assert 1 == len(snapshot.var_lookup)
 
     assert "name" == snapshot.var_lookup['vid'].value
 
 
 def test_convert_snapshot_with_watch():
     event_snapshot = mock_snapshot()
-    event_snapshot.add_watch_result(WatchResult("test", mock_variable_id()))
+    event_snapshot.add_watch_result(WatchResult(WATCH_SOURCE_WATCH, "test", mock_variable_id()))
 
     snapshot = convert_snapshot(event_snapshot)
 
     assert snapshot.watches[0].error_result == ''
     assert snapshot.watches[0].good_result is not None
     assert snapshot.watches[0].good_result.ID == "vid"
     assert "good_result" == snapshot.watches[0].WhichOneof("result")
 
 
 def test_convert_snapshot_with_error_watch():
     event_snapshot = mock_snapshot()
-    event_snapshot.add_watch_result(WatchResult("test", None, 'test error'))
+    event_snapshot.add_watch_result(WatchResult(WATCH_SOURCE_WATCH, "test", None, 'test error'))
 
     snapshot = convert_snapshot(event_snapshot)
 
     assert snapshot.watches[0].error_result == 'test error'
     assert "error_result" == snapshot.watches[0].WhichOneof("result")
```

### Comparing `deep_agent-1.1.0/tests/unit_tests/push/test_push_service.py` & `deep_agent-1.1.1/tests/unit_tests/push/test_push_service.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/task/test_task.py` & `deep_agent-1.1.1/tests/unit_tests/task/test_task.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/tracepoint/__init__.py` & `deep_agent-1.1.1/tests/unit_tests/tracepoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/tracepoint/test_tracepoint_config.py` & `deep_agent-1.1.1/tests/unit_tests/tracepoint/test_tracepoint_config.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/tests/unit_tests/tracepoint/test_trigger.py` & `deep_agent-1.1.1/tests/unit_tests/tracepoint/test_trigger.py`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/.gitignore` & `deep_agent-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/LICENSE` & `deep_agent-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/README.md` & `deep_agent-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/pyproject.toml` & `deep_agent-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deep_agent-1.1.0/PKG-INFO` & `deep_agent-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: deep-agent
-Version: 1.1.0
+Version: 1.1.1
 Summary: DEEP Python Agent
 Author-email: Intergral GmbH <support@intergral.com>, Ben Donnelly <b.w.donnelly1@gmail.com>
 License-Expression: AGPL-3.0-only
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

