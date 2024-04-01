# Comparing `tmp/sentry-kafka-schemas-0.1.8.tar.gz` & `tmp/sentry-kafka-schemas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.8.tar", last modified: Tue May 16 18:12:30 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.9.tar", last modified: Sat May 20 00:27:12 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.8.tar` & `sentry-kafka-schemas-0.1.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.163201 sentry-kafka-schemas-0.1.8/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.163201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.167201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.155201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.171201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.171201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    59601 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24745 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.167201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_codeowner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_sentry_kafka_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_valid_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_valid_topic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.563357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.567358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.571358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.575358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.559357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.575358 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.579359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59601 2023-05-20 00:27:07.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:10.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-20 00:27:07.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 00:27:08.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25054 2023-05-20 00:27:09.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.579359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38689 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.583359 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.563357 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 00:27:12.000000 sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:27:12.587360 sentry-kafka-schemas-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-20 00:26:59.000000 sentry-kafka-schemas-0.1.9/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.8/LICENSE` & `sentry-kafka-schemas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/README.md` & `sentry-kafka-schemas-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/__init__.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/json.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/msgpack.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, TypedDict, Dict, List, Literal
+from typing import TypedDict, List, Dict, Any, Literal
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Union, Dict, TypedDict, Tuple, List
+from typing import TypedDict, Any, Tuple, Dict, Union, Literal, List
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Literal, List, TypedDict, Any
+from typing import TypedDict, Any, Dict, Literal, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, TypedDict, Literal, Union
+from typing import List, Union, TypedDict, Dict, Literal
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """ counter_metric_value. """
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, TypedDict, Literal, Any
+from typing import TypedDict, Any, Union, Literal
 from typing_extensions import Required
 
 
 class ReplayRecording(TypedDict, total=False):
     """
     replay_recording.
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Any, Literal, TypedDict, Dict
+from typing import Literal, Dict, Any, TypedDict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, TypedDict, Literal, List, Dict
+from typing import List, Dict, TypedDict, Literal, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Literal, Union, Any, TypedDict
+from typing import List, TypedDict, Dict, Literal, Union, Any
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """ counter_metric_value. """
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Literal, Dict, TypedDict, Any
+from typing import Literal, Any, TypedDict, List, Union, Dict
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """ counter_metric_value. """
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, TypedDict, Any, List, Union
+from typing import List, TypedDict, Union, Any, Dict
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
     """ clickhouse_query_profile. """
 
     time_range: Required[Union[int, None]]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Literal, Any, Dict, List
+from typing import TypedDict, Dict, Literal, Any, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """ payload_v3. """
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Union, TypedDict, Dict, Tuple, Any, List
+from typing import Literal, Union, List, TypedDict, Dict, Any, Tuple
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -261,15 +261,21 @@
      { "environment": "production" }
      ```
     """
 
     contexts: Required["_Contexts"]
     """ Required property """
 
-    tags: List[List[Union[None, str]]]
+    tags: Union["_Tags", None]
+    """
+     Custom tags for this event.
+
+     A map or list of tags for this event. Each tag must be less than 200 characters.
+    """
+
     extra: "_Extra"
     sdk: "ClientSdkInfo"
     project: int
     spans: Required[List["_Span"]]
     """ Required property """
 
     measurements: "_Measurements"
@@ -851,14 +857,27 @@
 _SPANSTATUS_DATA_LOSS: Literal["data_loss"] = "data_loss"
 """The values for the 'Trace status' enum"""
 _SPANSTATUS_UNAUTHENTICATED: Literal["unauthenticated"] = "unauthenticated"
 """The values for the 'Trace status' enum"""
 
 
 
+_TagEntryAnyof0 = Tuple[Union[str, None], Union[str, None]]
+"""
+maxItems: 2
+minItems: 2
+"""
+
+
+
+_Tags = List[Union["_TagEntryAnyof0", None]]
+"""  Manual key/value tag pairs. """
+
+
+
 _TraceContext = Union["_TraceContextAnyof0"]
 """  Trace context """
 
 
 
 class _TraceContextAnyof0(TypedDict, total=False):
     client_sample_rate: Union[Union[int, float], None]
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928512687969925%*

 * *Differences: {"'definitions'": "{'Data': {'properties': {'tags': {replace: OrderedDict([('description', ' "*

 * *                  'Custom tags for this event.\\n\\n A map or list of tags for this event. Each '*

 * *                  "tag must be less than 200 characters.'), ('anyOf', [OrderedDict([('$ref', "*

 * *                  "'#/definitions/Tags')]), OrderedDict([('type', 'null')])])])}}}, 'TagEntry': "*

 * *                  "OrderedDict([('anyOf', [OrderedDict([('type', 'array'), ('items', "*

 * *                  "[OrderedDict([('type […]*

```diff
@@ -375,28 +375,23 @@
                     },
                     "type": "array"
                 },
                 "start_timestamp": {
                     "type": "number"
                 },
                 "tags": {
-                    "items": {
-                        "items": {
-                            "anyOf": [
-                                {
-                                    "type": "null"
-                                },
-                                {
-                                    "type": "string"
-                                }
-                            ]
+                    "anyOf": [
+                        {
+                            "$ref": "#/definitions/Tags"
                         },
-                        "type": "array"
-                    },
-                    "type": "array"
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "description": " Custom tags for this event.\n\n A map or list of tags for this event. Each tag must be less than 200 characters."
                 },
                 "timestamp": {
                     "type": "number"
                 },
                 "title": {
                     "type": "string"
                 },
@@ -1236,14 +1231,47 @@
                 "internal_error",
                 "unavailable",
                 "data_loss",
                 "unauthenticated"
             ],
             "type": "string"
         },
+        "TagEntry": {
+            "anyOf": [
+                {
+                    "items": [
+                        {
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        },
+                        {
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        }
+                    ],
+                    "maxItems": 2,
+                    "minItems": 2,
+                    "type": "array"
+                },
+                {
+                    "type": "null"
+                }
+            ]
+        },
+        "Tags": {
+            "description": " Manual key/value tag pairs.",
+            "items": {
+                "$ref": "#/definitions/TagEntry"
+            },
+            "type": "array"
+        },
         "TraceContext": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
                         "client_sample_rate": {
                             "description": " The client-side sample rate as reported in the envelope's `trace.sample_rate` header.\n\n The server takes this field from envelope headers and writes it back into the event. Clients\n should not ever send this value.",
```

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.9/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/tests/test_codecs.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/tests/test_codeowner.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_codeowner.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/tests/test_examples.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/tests/test_valid_schemas.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_valid_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/python/tests/test_valid_topic_data.py` & `sentry-kafka-schemas-0.1.9/python/tests/test_valid_topic_data.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.8/setup.py` & `sentry-kafka-schemas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.8",
+    version="0.1.9",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=find_packages(where="python/", exclude=["generate_python_types.py", "tests/"]),
```

