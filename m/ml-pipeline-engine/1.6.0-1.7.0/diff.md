# Comparing `tmp/ml_pipeline_engine-1.6.0.tar.gz` & `tmp/ml_pipeline_engine-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_pipeline_engine-1.6.0.tar", max compression
+gzip compressed data, was "ml_pipeline_engine-1.7.0.tar", max compression
```

## Comparing `ml_pipeline_engine-1.6.0.tar` & `ml_pipeline_engine-1.7.0.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0      410 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/AUTHORS
--rw-r--r--   0        0        0     2570 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/LICENSE
--rw-r--r--   0        0        0     7578 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/README.md
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/__init__.py
--rw-r--r--   0        0        0       93 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/enums.py
--rw-r--r--   0        0        0      165 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/errors.py
--rw-r--r--   0        0        0     1726 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/serializers.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/__init__.py
--rw-r--r--   0        0        0      808 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/base.py
--rw-r--r--   0        0        0     2394 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/filesystem.py
--rw-r--r--   0        0        0      437 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/no_op.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/__init__.py
--rw-r--r--   0        0        0      400 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/datasources.py
--rw-r--r--   0        0        0      359 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/feature.py
--rw-r--r--   0        0        0      354 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/ml_model.py
--rw-r--r--   0        0        0      779 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/processors.py
--rw-r--r--   0        0        0      381 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/vectorizer.py
--rw-r--r--   0        0        0      585 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/cache.py
--rw-r--r--   0        0        0     2781 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/chart.py
--rw-r--r--   0        0        0     1403 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/cli.py
--rw-r--r--   0        0        0       34 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/const.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/__init__.py
--rw-r--r--   0        0        0     2212 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/dag.py
--rw-r--r--   0        0        0      207 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/__init__.py
--rw-r--r--   0        0        0     2378 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/dag.py
--rw-r--r--   0        0        0      444 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/enums.py
--rw-r--r--   0        0        0      325 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/graph.py
--rw-r--r--   0        0        0    22393 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/manager.py
--rw-r--r--   0        0        0      588 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/retrying.py
--rw-r--r--   0        0        0     3063 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/storage.py
--rw-r--r--   0        0        0      623 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/__init__.py
--rw-r--r--   0        0        0       31 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/__init__.py
--rw-r--r--   0        0        0    14609 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/builder.py
--rw-r--r--   0        0        0      531 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/errors.py
--rw-r--r--   0        0        0     5765 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/marks.py
--rw-r--r--   0        0        0     1796 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/decorators.py
--rw-r--r--   0        0        0     1439 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/events.py
--rw-r--r--   0        0        0      513 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/exceptions.py
--rw-r--r--   0        0        0      290 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/logs.py
--rw-r--r--   0        0        0     1124 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/module_loading.py
--rw-r--r--   0        0        0      156 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/__init__.py
--rw-r--r--   0        0        0      774 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/enums.py
--rw-r--r--   0        0        0      149 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/errors.py
--rw-r--r--   0        0        0     5943 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/node.py
--rw-r--r--   0        0        0      124 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/__init__.py
--rw-r--r--   0        0        0     1883 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/basic.py
--rw-r--r--   0        0        0     1945 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/processes.py
--rw-r--r--   0        0        0      619 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/threads.py
--rw-r--r--   0        0        0    11573 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/types.py
--rw-r--r--   0        0        0        0 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/__init__.py
--rw-r--r--   0        0        0     5385 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/dag.py
--rw-r--r--   0        0        0     2651 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/sample.py
--rw-r--r--   0        0        0     1214 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/schema.py
--rw-r--r--   0        0        0      597 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/utils.py
--rw-r--r--   0        0        0      524 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/favicon.ico
--rw-r--r--   0        0        0      571 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/index.html
--rw-r--r--   0        0        0      366 2024-03-28 14:15:00.404857 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/manifest.json
--rw-r--r--   0        0        0   693682 2024-03-28 14:15:00.408856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css
--rw-r--r--   0        0        0  1073488 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map
--rw-r--r--   0        0        0     4531 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js
--rw-r--r--   0        0        0    10597 2024-03-28 14:15:00.412856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map
--rw-r--r--   0        0        0   750045 2024-03-28 14:15:00.416856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js
--rw-r--r--   0        0        0     1629 2024-03-28 14:15:00.416856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt
--rw-r--r--   0        0        0  3506105 2024-03-28 14:15:00.428856 ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map
--rw-r--r--   0        0        0     1247 2024-03-28 14:15:00.432856 ml_pipeline_engine-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     8640 1970-01-01 00:00:00.000000 ml_pipeline_engine-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      410 2024-04-01 12:15:40.882996 ml_pipeline_engine-1.7.0/AUTHORS
+-rw-r--r--   0        0        0     2570 2024-04-01 12:15:40.882996 ml_pipeline_engine-1.7.0/LICENSE
+-rw-r--r--   0        0        0     7578 2024-04-01 12:15:40.882996 ml_pipeline_engine-1.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.882996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.882996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/enums.py
+-rw-r--r--   0        0        0      165 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/errors.py
+-rw-r--r--   0        0        0     1726 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/__init__.py
+-rw-r--r--   0        0        0      808 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/base.py
+-rw-r--r--   0        0        0     2394 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/filesystem.py
+-rw-r--r--   0        0        0      437 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/no_op.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/datasources.py
+-rw-r--r--   0        0        0      359 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/feature.py
+-rw-r--r--   0        0        0      354 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/ml_model.py
+-rw-r--r--   0        0        0      779 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/processors.py
+-rw-r--r--   0        0        0      381 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/vectorizer.py
+-rw-r--r--   0        0        0      585 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/cache.py
+-rw-r--r--   0        0        0     2781 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/chart.py
+-rw-r--r--   0        0        0     1403 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/cli.py
+-rw-r--r--   0        0        0       34 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/const.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/context/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/context/dag.py
+-rw-r--r--   0        0        0      207 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/__init__.py
+-rw-r--r--   0        0        0     2242 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/dag.py
+-rw-r--r--   0        0        0      444 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/enums.py
+-rw-r--r--   0        0        0      945 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/graph.py
+-rw-r--r--   0        0        0    23741 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/manager.py
+-rw-r--r--   0        0        0      588 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/retrying.py
+-rw-r--r--   0        0        0     3553 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/storage.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/__init__.py
+-rw-r--r--   0        0        0    14609 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/builder.py
+-rw-r--r--   0        0        0      531 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/errors.py
+-rw-r--r--   0        0        0     5765 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/marks.py
+-rw-r--r--   0        0        0     1796 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/decorators.py
+-rw-r--r--   0        0        0     1439 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/events.py
+-rw-r--r--   0        0        0      513 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/exceptions.py
+-rw-r--r--   0        0        0      290 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/logs.py
+-rw-r--r--   0        0        0     1124 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/module_loading.py
+-rw-r--r--   0        0        0      156 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/__init__.py
+-rw-r--r--   0        0        0      774 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/enums.py
+-rw-r--r--   0        0        0      149 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/errors.py
+-rw-r--r--   0        0        0     5943 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/node.py
+-rw-r--r--   0        0        0      124 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/__init__.py
+-rw-r--r--   0        0        0     1883 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/basic.py
+-rw-r--r--   0        0        0     1945 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/processes.py
+-rw-r--r--   0        0        0      619 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/threads.py
+-rw-r--r--   0        0        0    11612 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/types.py
+-rw-r--r--   0        0        0        0 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/__init__.py
+-rw-r--r--   0        0        0     5385 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/dag.py
+-rw-r--r--   0        0        0     2651 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/sample.py
+-rw-r--r--   0        0        0     1214 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/schema.py
+-rw-r--r--   0        0        0      597 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/utils.py
+-rw-r--r--   0        0        0      524 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/favicon.ico
+-rw-r--r--   0        0        0      571 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/index.html
+-rw-r--r--   0        0        0      366 2024-04-01 12:15:40.886996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/manifest.json
+-rw-r--r--   0        0        0   693682 2024-04-01 12:15:40.890996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css
+-rw-r--r--   0        0        0  1073488 2024-04-01 12:15:40.894996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map
+-rw-r--r--   0        0        0     4531 2024-04-01 12:15:40.894996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js
+-rw-r--r--   0        0        0    10597 2024-04-01 12:15:40.894996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map
+-rw-r--r--   0        0        0   750045 2024-04-01 12:15:40.898996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js
+-rw-r--r--   0        0        0     1629 2024-04-01 12:15:40.898996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt
+-rw-r--r--   0        0        0  3506105 2024-04-01 12:15:40.910996 ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map
+-rw-r--r--   0        0        0     1247 2024-04-01 12:15:40.914996 ml_pipeline_engine-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8640 1970-01-01 00:00:00.000000 ml_pipeline_engine-1.7.0/PKG-INFO
```

### Comparing `ml_pipeline_engine-1.6.0/LICENSE` & `ml_pipeline_engine-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/README.md` & `ml_pipeline_engine-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/serializers.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/serializers.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/base.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/base.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/artifact_store/store/filesystem.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/artifact_store/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/base_nodes/processors.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/base_nodes/processors.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/cache.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/cache.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/chart.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/chart.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/cli.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/cli.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/context/dag.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/context/dag.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/dag.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/dag.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,33 +40,26 @@
 
         if self.is_process_pool_needed:
             process_pool_registry.is_ready()
 
     async def run(self, ctx: PipelineContextLike) -> NodeResultT:
         self._start_runtime_validation()
 
-        run_manager = self.run_manager(
-            lock_manager=DAGConcurrentManagerLock(
-                self.node_map.keys(),
-            ),
-            dag=self,
-            ctx=ctx,
-        )
-
+        run_manager = self.run_manager(dag=self, ctx=ctx)
         return await run_manager.run()
 
     def visualize(  # noqa
         self,
         name: str,
         verbose_name: Optional[str] = None,
         target_dir: Optional[Union[pathlib.Path, str]] = None,
         **kwargs,
     ) -> None:
         """
-        Create a static for graph visualization
+        Create static files for graph visualization
 
         Args:
             name: Tech name for the dag
             verbose_name: Dag title
             target_dir: Target dir for static
             **kwargs: Graph config kwargs
         """
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/manager.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,64 +6,80 @@
 from dataclasses import dataclass, field
 
 import networkx as nx
 
 from ml_pipeline_engine.dag.enums import EdgeField, NodeField
 from ml_pipeline_engine.dag.graph import DiGraph
 from ml_pipeline_engine.dag.retrying import DagRetryPolicy
-from ml_pipeline_engine.dag.utils import get_connected_subgraph
+from ml_pipeline_engine.dag.graph import get_connected_subgraph
 from ml_pipeline_engine.exceptions import NodeErrorType
 from ml_pipeline_engine.dag.storage import DAGNodeStorage
 from ml_pipeline_engine.node import run_node, run_node_default
 from ml_pipeline_engine.types import (
     CaseResult,
     DAGLike,
     DAGRunManagerLike,
     NodeId,
     NodeResultT,
     PipelineContextLike,
     Recurrent,
-    DAGRunLockManagerLike,
     DAGNodeStorageLike,
 )
 
 from ml_pipeline_engine.logs import logger_manager as logger
 from cachetools import cachedmethod
 from cachetools.keys import hashkey
+from collections import defaultdict
 
 
-class DAGConcurrentManagerLock(DAGRunLockManagerLike):
+_EventDictT = t.Dict[NodeId, asyncio.Event]
+_EventConditionT = t.Dict[NodeId, asyncio.Condition]
 
-    def __init__(self, node_ids: t.Iterable[NodeId]):
-        self.lock_store = {node_id: asyncio.Event() for node_id in node_ids}
 
-    def get_lock(self, node_id: NodeId) -> asyncio.Event:
-        self.lock_store.setdefault(node_id, asyncio.Event())
-        return self.lock_store[node_id]
+@dataclass
+class DAGConcurrentManagerLock:
+    node_ids: t.Iterable[NodeId]
+    event_lock_store: _EventDictT = field(
+        default_factory=functools.partial(defaultdict, asyncio.Event),
+    )
+    condition_lock_store: _EventConditionT = field(
+        default_factory=functools.partial(defaultdict, asyncio.Condition),
+    )
+
+    @property
+    def conditions(self) -> _EventConditionT:
+        return self.condition_lock_store
+
+    @property
+    def events(self) -> _EventDictT:
+        return self.event_lock_store
 
 
 def cache_key(prefix, _, *args, **kwargs) -> t.Type[tuple]:
     """Custom func key generation excluding 'self'."""
     return hashkey(*args, prefix, **kwargs)
 
 
 @dataclass
 class DAGRunConcurrentManager(DAGRunManagerLike):
     """
     Дефолтный менеджер запуска графов.
     Производит конкурентное исполнение узлов.
     """
 
-    lock_manager: DAGRunLockManagerLike
     ctx: PipelineContextLike
     dag: DAGLike
     node_storage: DAGNodeStorageLike = field(default_factory=DAGNodeStorage)
 
+    _lock_manager: DAGConcurrentManagerLock = field(init=False)
     _memorization_store: t.Dict[t.Any, t.Any] = field(default_factory=dict)
 
+    def __post_init__(self):
+        self._lock_manager = DAGConcurrentManagerLock(self.dag.node_map.keys())
+
     async def run(self) -> NodeResultT:
         return await self._run_dag(self._get_reduced_dag(self.dag.input_node, self.dag.output_node))
 
     def _get_node_kwargs(self, node_id: NodeId) -> t.Dict[str, t.Any]:
         """
         Получить входные kwarg-и для узла графа перед его запуском
         """
@@ -146,20 +162,20 @@
             """
             return not self.dag.graph.nodes[u].get(NodeField.is_first_success_pool)
 
         return get_connected_subgraph(
             nx.subgraph_view(self.dag.graph, filter_edge=_filter, filter_node=_filter_node), source, dest
         )
 
-    def _get_reduced_dag_input_one_of(self, source: NodeId, dest: NodeId) -> DiGraph:
+    def _get_reduced_dag_input_one_of(self, source: NodeId, dest: NodeId, is_oneof: bool) -> DiGraph:
         """
         Получить связный подграф между двумя заданными узлами графа InputOneOf
         """
 
-        return get_connected_subgraph(nx.subgraph_view(self.dag.graph), source, dest)
+        return get_connected_subgraph(nx.subgraph_view(self.dag.graph), source, dest, is_oneof=is_oneof)
 
     def _add_case_result(self, switch_node_id: NodeId) -> None:
         """
         Записать выбор, сделанный оператором выбора Switch-Case, в контекст
         """
         selected_branch_label = None
         branch_nodes = {}
@@ -189,15 +205,15 @@
 
         # Due to concurrent nature, we have to check if the node is running concurrently in another subgraph.
         # In general, we have two checks: before execution and here. This check prevents a double run.
         # when the deep-nested node in the subgraph has been executed.
         if self.node_storage.exists_processed_node(node_id):
             logger.debug('Node %s has been executed. Stop new execution', node_id)
 
-            event_lock = self.lock_manager.get_lock(node_id)
+            event_lock = self._lock_manager.events[node_id]
             await event_lock.wait()
 
             return self.node_storage.get_node_result(node_id)
 
         self.node_storage.set_node_as_processed(node_id)
         await self.ctx.emit_on_node_start(node_id=node_id)
 
@@ -327,31 +343,50 @@
 
             if self._is_switch(dag, node_id):
                 with suppress(KeyError):
                     predecessors[idx] = self.node_storage.get_switch_result(node_id).node_id
 
         return predecessors
 
-    async def _is_ready_to_run(self, dag: DiGraph, node_id: NodeId) -> bool:
+    async def _is_ready_to_execute(self, dag: DiGraph, node_id: NodeId) -> bool:
         """
-        Метод проверяет возможность запуска узла
+        Check if the node is read to be executed
         """
 
+        logger.debug('Checking if the node can be executed node_id=%s', node_id)
+
+        def exist_predecessor_results() -> bool:
+            """
+            Check if the node's predecessors have executed and the have results
+            """
+
+            for pred_node_id in self._get_predecessors(dag, node_id):
+
+                if not self.node_storage.exists_node_result(pred_node_id):
+                    return False
+
+            return True
+
         # Switch context to collect any predecessors' results to approve the function for running.
         await asyncio.sleep(0)
 
-        if self.node_storage.exists_processed_node(node_id):
-            return False
+        # FIXME: It has to be different way to check oneof subgraph's nodes. PE-22
+        if not dag.is_oneof and self.node_storage.exists_node_in_waiting_list(node_id):
+            condition = self._lock_manager.conditions[node_id]
+
+            async with condition:
+                await condition.wait_for(exist_predecessor_results)
 
-        for pred_node_id in self._get_predecessors(dag, node_id):
+        else:
+            self.node_storage.set_node_in_waiting_list(node_id)
 
-            if not self.node_storage.exists_node_result(pred_node_id):
-                return False
+        if self.node_storage.exists_processed_node(node_id):
+            return False
 
-        return True
+        return exist_predecessor_results()
 
     async def _run_dag(self, dag: DiGraph) -> t.Union[NodeResultT, t.Any]:
         """
         Запустить граф / подграф
         """
 
         logger.debug('Начало запуска DAG, dag=%s', str(dag))
@@ -376,15 +411,15 @@
             # In that case, we simply skip the node because:
             #   1. If it's a recurrent subgraph, the result would be deleted for each node in the subgraph
             #      and this if-statement won't be executed.
             #   2. If it's a non-recurrent execution, we just assume that the node's done before in any other graphs.
             if self.node_storage.exists_processed_node(node_id):
                 continue
 
-            elif await self._is_ready_to_run(dag, node_id):
+            elif await self._is_ready_to_execute(dag, node_id):
                 logger.debug('Узел готов к обработке node_id=%s', node_id)
 
                 if self._is_switch(dag, node_id):
                     logger.debug('Узел является switch-кейсом node_id=%s', node_id)
                     self._add_case_result(node_id)
 
                     coro_to_run = asyncio.create_task(
@@ -393,22 +428,23 @@
                                 self.dag.input_node,
                                 (self.node_storage.get_switch_result(node_id)).node_id,
                             ),
                         ),
                         name=node_id,
                     )
 
-                elif dag.nodes[node_id].get(NodeField.is_first_success):
+                elif self._is_head_of_oneof(dag, node_id):
                     logger.debug('Узел является InputOneOf node_id=%s', node_id)
 
                     coro_to_run = asyncio.create_task(
                         self._run_dag(
                             dag=self._get_reduced_dag_input_one_of(
                                 self.dag.input_node,
                                 node_id,
+                                is_oneof=True,
                             ),
                         ),
                         name=node_id,
                     )
 
                 else:
                     logger.debug('Узел может быть обработан, отправляем его в обработку node_id=%s', node_id)
@@ -507,16 +543,20 @@
                             not isinstance(node_result, NodeErrorType)
                             and self._is_node_in_oneof(dag, node_result_id)
                         ):
                             self.node_storage.set_node_result(dag_output_node, node_result)
                             # Для искусственной остановки пайплайна помечаем текущий узел как выходной
                             node_result_id = dag_output_node
 
-                        self.node_storage.set_node_result(node_result_id, node_result)
-                        self.lock_manager.get_lock(node_result_id).set()
+                        condition = self._lock_manager.conditions[node_id]
+
+                        async with condition:
+                            self.node_storage.set_node_result(node_result_id, node_result)
+                            self._lock_manager.events[node_id].set()
+                            condition.notify_all()
 
                         # FIXME: Set new abstractions for event managers
                         await self.ctx.save_node_result(node_result_id, node_result)
 
                         if node_result_id == dag_output_node:
                             return self.node_storage.get_node_result(node_result_id, with_hidden=True)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/retrying.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/retrying.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag/storage.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag/storage.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 @dataclass
 class DAGNodeStorage(DAGNodeStorageLike):
     node_results: HiddenDict = field(default_factory=HiddenDict)
     processed_nodes: HiddenDict = field(default_factory=HiddenDict)
     switch_results: HiddenDict = field(default_factory=HiddenDict)
     recurrent_subgraph: HiddenDict = field(default_factory=HiddenDict)
+    waiting_list: HiddenDict = field(default_factory=HiddenDict)
 
     def set_node_result(self, node_id: NodeId, data: t.Any) -> None:
         self.node_results.set(node_id, data)
 
     def get_node_result(self, node_id: NodeId, with_hidden: bool = False) -> t.Any:
         return self.node_results.get(node_id, with_hidden)
 
@@ -76,11 +77,21 @@
 
     def delete_active_rec_subgraph(self, source: NodeId, dest: NodeId) -> None:
         self.processed_nodes.delete((source, dest))
 
     def exists_active_rec_subgraph(self, source: NodeId, dest: NodeId) -> bool:
         return self.processed_nodes.exists((source, dest))
 
+    def set_node_in_waiting_list(self, node_id: NodeId) -> None:
+        self.waiting_list.set(node_id, 1)
+
+    def exists_node_in_waiting_list(self, node_id: NodeId, with_hidden: bool = False) -> bool:
+        return self.waiting_list.exists(node_id, with_hidden)
+
+    def hide_node_in_waiting_list(self, node_id: NodeId) -> None:
+        self.waiting_list.hide(node_id)
+
     def hide_last_execution(self, *node_ids: NodeId) -> None:
         for node_id in node_ids:
             self.hide_processed_node(node_id)
             self.hide_node_result(node_id)
+            self.hide_node_in_waiting_list(node_id)
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/builder.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 import inspect
 import typing as t
 from collections import deque
 
 from ml_pipeline_engine.dag import DAG, EdgeField, NodeField
 from ml_pipeline_engine.dag.graph import DiGraph
-from ml_pipeline_engine.dag.utils import get_connected_subgraph
+from ml_pipeline_engine.dag.graph import get_connected_subgraph
 from ml_pipeline_engine.dag_builders.annotation import errors
 from ml_pipeline_engine.dag_builders.annotation.marks import (
     InputGenericMark,
     InputMark,
     InputOneOfMark,
     RecurrentSubGraphMark,
     SwitchCaseMark,
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/errors.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/errors.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/dag_builders/annotation/marks.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/dag_builders/annotation/marks.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/decorators.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/decorators.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/events.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/events.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/exceptions.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/module_loading.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/module_loading.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/enums.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/enums.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/node/node.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/node/node.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/basic.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/basic.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/processes.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/processes.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/parallelism/threads.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/parallelism/threads.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/types.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,26 +301,14 @@
 
     @property
     @abc.abstractmethod
     def exceptions(self) -> t.Tuple[t.Type[Exception]]:
         ...
 
 
-class DAGRunLockManagerLike(t.Protocol):
-    """
-    A manager object to store and manage locks related to NodeIds
-    """
-
-    lock_store: t.Dict[str, asyncio.Event] = {}
-
-    @abc.abstractmethod
-    def get_lock(self, node_id: NodeId) -> asyncio.Event:
-        ...
-
-
 class HiddenDictLike(t.Protocol):
     """
     Dict object that can hide some keys until they are set again
     """
 
     @abc.abstractmethod
     def get(self, key: t.Any, with_hidden: bool = True) -> t.Any:
@@ -351,14 +339,15 @@
     # FIXME: If we want to show these methods and structures, we have to declare switch in types.py,
     #        as well as recurrent subgraph
 
     processed_nodes: HiddenDictLike
     node_results: HiddenDictLike
     switch_results: HiddenDictLike
     recurrent_subgraph: HiddenDictLike
+    waiting_list: HiddenDictLike
 
     @abc.abstractmethod
     def set_node_result(self, node_id: NodeId, data: t.Any) -> None:
         ...
 
     @abc.abstractmethod
     def get_node_result(self, node_id: NodeId, with_hidden: bool = False) -> t.Any:
@@ -404,21 +393,32 @@
     def exists_active_rec_subgraph(self, source: NodeId, dest: NodeId) -> bool:
         ...
 
     @abc.abstractmethod
     def hide_last_execution(self, *node_ids: NodeId) -> None:
         ...
 
+    @abc.abstractmethod
+    def set_node_in_waiting_list(self, node_id: NodeId) -> None:
+        ...
+
+    @abc.abstractmethod
+    def exists_node_in_waiting_list(self, node_id: NodeId, with_hidden: bool = False) -> bool:
+        ...
+
+    @abc.abstractmethod
+    def hide_node_in_waiting_list(self, node_id: NodeId) -> None:
+        ...
+
 
 class DAGRunManagerLike(t.Protocol):
     """
     Менеджер управлением запуска графа
     """
 
-    lock_manager: DAGRunLockManagerLike
     node_storage: DAGNodeStorageLike
     ctx: PipelineContextLike
     dag: 'DAGLike'
 
     _memorization_store: t.Dict[t.Any, t.Any]
 
     @abc.abstractmethod
@@ -427,15 +427,15 @@
 
 
 class DAGLike(t.Protocol[NodeResultT]):
     """
     Граф
     """
 
-    graph: [t.Type[nx.DiGraph], nx.DiGraph]
+    graph: nx.DiGraph
     input_node: NodeId
     output_node: NodeId
     node_map: t.Dict[NodeId, NodeLike]
     run_manager: DAGRunManagerLike
     retry_policy: RetryPolicyLike
     is_process_pool_needed: bool
     is_thread_pool_needed: bool
```

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/dag.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/dag.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/sample.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/sample.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/schema.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/schema.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/utils.py` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/favicon.ico` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/index.html` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/index.html`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/css/main.fdcc84c5.css.map`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/453.ae999f12.chunk.js.map`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map` & `ml_pipeline_engine-1.7.0/ml_pipeline_engine/visualization/viewer/static/js/main.4827d1c7.js.map`

 * *Files identical despite different names*

### Comparing `ml_pipeline_engine-1.6.0/pyproject.toml` & `ml_pipeline_engine-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "ml-pipeline-engine"
 readme = "README.md"
-version = "1.6.0"
+version = "1.7.0"
 authors = [
   "Konyaev Matvey",
   "Vasiliy Pankov",
 ]
 repository = "https://github.com/tochka-public/ml-pipeline-engine"
 homepage = "https://github.com/tochka-public/ml-pipeline-engine"
 description = "Фреймворк для работы с пайплайном ML моделей"
```

### Comparing `ml_pipeline_engine-1.6.0/PKG-INFO` & `ml_pipeline_engine-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pipeline-engine
-Version: 1.6.0
+Version: 1.7.0
 Summary: Фреймворк для работы с пайплайном ML моделей
 Home-page: https://github.com/tochka-public/ml-pipeline-engine
 License: MIT
 Author: Konyaev Matvey
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

