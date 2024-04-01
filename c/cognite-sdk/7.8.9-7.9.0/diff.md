# Comparing `tmp/cognite_sdk-7.8.9.tar.gz` & `tmp/cognite_sdk-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-7.8.9.tar", max compression
+gzip compressed data, was "cognite_sdk-7.9.0.tar", max compression
```

## Comparing `cognite_sdk-7.8.9.tar` & `cognite_sdk-7.9.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0    11349 2024-01-04 07:39:04.049508 cognite_sdk-7.8.9/LICENSE
--rw-r--r--   0        0        0     4073 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/README.md
--rw-r--r--   0        0        0      539 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/__init__.py
--rw-r--r--   0        0        0       35 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     9124 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    64667 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1304 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0    11098 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0    10158 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     6408 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/graphql.py
--rw-r--r--   0        0        0    49894 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     7226 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     9651 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11304 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    51407 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    88539 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    13839 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/datapoints_subscriptions.py
--rw-r--r--   0        0        0    15467 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    31844 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/documents.py
--rw-r--r--   0        0        0    16048 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    37114 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/events.py
--rw-r--r--   0        0        0    18578 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    47408 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/files.py
--rw-r--r--   0        0        0    46978 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    46212 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0    19397 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6191 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24880 2024-01-04 07:39:04.053508 cognite_sdk-7.8.9/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    25732 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    58575 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7715 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32822 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    29236 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    40372 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    23074 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5100 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4718 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9551 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1867 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     3544 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/units.py
--rw-r--r--   0        0        0     5273 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/user_profiles.py
--rw-r--r--   0        0        0     6363 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    25504 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api/workflows.py
--rw-r--r--   0        0        0    51105 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_api_client.py
--rw-r--r--   0        0        0    10033 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      342 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_constants.py
--rw-r--r--   0        0        0     6972 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_http_client.py
--rw-r--r--   0        0        0      585 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     2117 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3524 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2681 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0    10018 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3524 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/beta.py
--rw-r--r--   0        0        0     6830 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/config.py
--rw-r--r--   0        0        0    22868 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/credentials.py
--rw-r--r--   0        0        0    10783 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    30830 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0    10462 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/aggregations.py
--rw-r--r--   0        0        0       35 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     6150 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     4950 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     9716 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    38940 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    32167 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/capabilities.py
--rw-r--r--   0        0        0    42085 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3926 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1239 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    14805 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     5387 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/core.py
--rw-r--r--   0        0        0     9643 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     5927 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     1428 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/graphql.py
--rw-r--r--   0        0        0     8548 2024-01-04 07:39:04.057508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    39356 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0    18475 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/query.py
--rw-r--r--   0        0        0     4392 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    30827 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6848 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    36595 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    16380 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/datapoints_subscriptions.py
--rw-r--r--   0        0        0    12803 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/documents.py
--rw-r--r--   0        0        0    13248 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    15610 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    14495 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    22081 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/filters.py
--rw-r--r--   0        0        0    18483 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    15487 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     9987 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5899 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4907 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    13988 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    28261 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     7298 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    17872 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    14298 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    14851 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    27522 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    15210 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    12178 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2565 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2804 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     3121 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     5356 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/units.py
--rw-r--r--   0        0        0     3514 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/user_profiles.py
--rw-r--r--   0        0        0    44085 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/data_classes/workflows.py
--rw-r--r--   0        0        0    12787 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/py.typed
--rw-r--r--   0        0        0    10226 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7808 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0    11756 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1482 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_experimental.py
--rw-r--r--   0        0        0     1202 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0    11375 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     1812 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_importing.py
--rw-r--r--   0        0        0     2506 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3698 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     4155 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     1140 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_retry.py
--rw-r--r--   0        0        0      908 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_session.py
--rw-r--r--   0        0        0     3064 2024-01-04 07:39:04.061508 cognite_sdk-7.8.9/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    25291 2024-01-04 07:39:04.065508 cognite_sdk-7.8.9/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     3229 2024-01-04 07:39:04.065508 cognite_sdk-7.8.9/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3339 2024-01-04 07:39:04.065508 cognite_sdk-7.8.9/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0      932 2024-01-04 07:39:04.065508 cognite_sdk-7.8.9/cognite/client/utils/useful_types.py
--rw-r--r--   0        0        0     2415 2024-01-04 07:39:04.065508 cognite_sdk-7.8.9/pyproject.toml
--rw-r--r--   0        0        0     5872 1970-01-01 00:00:00.000000 cognite_sdk-7.8.9/PKG-INFO
+-rw-r--r--   0        0        0    11349 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/LICENSE
+-rw-r--r--   0        0        0     4073 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/README.md
+-rw-r--r--   0        0        0      539 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0       35 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     9124 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    64667 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1304 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0    11098 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0    10158 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     6408 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/graphql.py
+-rw-r--r--   0        0        0    49894 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     7226 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     9651 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11304 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    51407 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    88539 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    13839 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/datapoints_subscriptions.py
+-rw-r--r--   0        0        0    15467 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    31844 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/documents.py
+-rw-r--r--   0        0        0    16048 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    37114 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    18578 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    47408 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    46978 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    46212 2024-01-05 07:59:55.416775 cognite_sdk-7.9.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0    19397 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6191 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24880 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    25732 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    58575 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7715 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32822 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    29236 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    40372 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    23074 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5100 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4718 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9551 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1867 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     3585 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/units.py
+-rw-r--r--   0        0        0     5804 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/user_profiles.py
+-rw-r--r--   0        0        0     6363 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    25504 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api/workflows.py
+-rw-r--r--   0        0        0    51105 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0    10033 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      342 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6972 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      585 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     2117 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3524 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2681 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0    10018 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3524 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     6830 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/config.py
+-rw-r--r--   0        0        0    22868 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0    10783 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    30830 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0    10462 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/aggregations.py
+-rw-r--r--   0        0        0       35 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     6150 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     4950 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     9716 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    38940 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    32167 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/capabilities.py
+-rw-r--r--   0        0        0    42085 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3926 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1239 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    14805 2024-01-05 07:59:55.420775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     5387 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/core.py
+-rw-r--r--   0        0        0     9643 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     5927 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     1428 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/graphql.py
+-rw-r--r--   0        0        0     8548 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    39356 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    18475 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     4392 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    30827 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6848 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    36595 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    16380 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/datapoints_subscriptions.py
+-rw-r--r--   0        0        0    12803 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/documents.py
+-rw-r--r--   0        0        0    13248 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    15610 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    14495 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    22081 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/filters.py
+-rw-r--r--   0        0        0    18483 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    15487 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     9987 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5899 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4907 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    13988 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    28261 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     7298 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    17872 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    14298 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    14851 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    27522 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    15174 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    12178 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2565 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2804 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     3121 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     5356 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/units.py
+-rw-r--r--   0        0        0     3835 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/user_profiles.py
+-rw-r--r--   0        0        0    44085 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/data_classes/workflows.py
+-rw-r--r--   0        0        0    12787 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/py.typed
+-rw-r--r--   0        0        0    10226 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7808 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0    11756 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1482 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_experimental.py
+-rw-r--r--   0        0        0     1202 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0    11381 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     1812 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_importing.py
+-rw-r--r--   0        0        0     2506 2024-01-05 07:59:55.424775 cognite_sdk-7.9.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3698 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     4155 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     1140 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_retry.py
+-rw-r--r--   0        0        0      908 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_session.py
+-rw-r--r--   0        0        0     3064 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    25291 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     3229 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3339 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0      932 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/cognite/client/utils/useful_types.py
+-rw-r--r--   0        0        0     2415 2024-01-05 07:59:55.428775 cognite_sdk-7.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5872 1970-01-01 00:00:00.000000 cognite_sdk-7.9.0/PKG-INFO
```

### Comparing `cognite_sdk-7.8.9/LICENSE` & `cognite_sdk-7.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/README.md` & `cognite_sdk-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/__init__.py` & `cognite_sdk-7.9.0/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/annotations.py` & `cognite_sdk-7.9.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/assets.py` & `cognite_sdk-7.9.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/graphql.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/data_sets.py` & `cognite_sdk-7.9.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-7.9.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/datapoints.py` & `cognite_sdk-7.9.0/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/datapoints_subscriptions.py` & `cognite_sdk-7.9.0/cognite/client/_api/datapoints_subscriptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/diagrams.py` & `cognite_sdk-7.9.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/documents.py` & `cognite_sdk-7.9.0/cognite/client/_api/documents.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/entity_matching.py` & `cognite_sdk-7.9.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/events.py` & `cognite_sdk-7.9.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-7.9.0/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/files.py` & `cognite_sdk-7.9.0/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/functions.py` & `cognite_sdk-7.9.0/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/geospatial.py` & `cognite_sdk-7.9.0/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/iam.py` & `cognite_sdk-7.9.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/labels.py` & `cognite_sdk-7.9.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/raw.py` & `cognite_sdk-7.9.0/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/relationships.py` & `cognite_sdk-7.9.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/sequences.py` & `cognite_sdk-7.9.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-7.9.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/templates.py` & `cognite_sdk-7.9.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/three_d.py` & `cognite_sdk-7.9.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/time_series.py` & `cognite_sdk-7.9.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-7.9.0/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-7.9.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-7.9.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-7.9.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/transformations/schema.py` & `cognite_sdk-7.9.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/units.py` & `cognite_sdk-7.9.0/cognite/client/_api/units.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, MutableSequence, overload
+from typing import TYPE_CHECKING, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client.data_classes.units import (
     Unit,
     UnitList,
     UnitSystem,
     UnitSystemList,
 )
 from cognite.client.utils._identifier import IdentifierSequence
+from cognite.client.utils.useful_types import SequenceNotStr
 
 if TYPE_CHECKING:
     from cognite.client import ClientConfig, CogniteClient
 
 
 class UnitAPI(APIClient):
     _RESOURCE_PATH = "/units"
@@ -28,24 +29,24 @@
         self.systems = UnitSystemAPI(config, api_version, cognite_client)
 
     @overload
     def retrieve(self, external_id: str, ignore_unknown_ids: bool = False) -> None | Unit:
         ...
 
     @overload
-    def retrieve(self, external_id: MutableSequence[str], ignore_unknown_ids: bool = False) -> UnitList:
+    def retrieve(self, external_id: SequenceNotStr[str], ignore_unknown_ids: bool = False) -> UnitList:
         ...
 
     def retrieve(
-        self, external_id: str | MutableSequence[str], ignore_unknown_ids: bool = False
+        self, external_id: str | SequenceNotStr[str], ignore_unknown_ids: bool = False
     ) -> Unit | UnitList | None:
         """`Retrieve one or more unit <https://developer.cognite.com/api#tag/Units/operation/byIdsUnits>`_
 
         Args:
-            external_id (str | MutableSequence[str]): External ID or list of external IDs
+            external_id (str | SequenceNotStr[str]): External ID or list of external IDs
             ignore_unknown_ids (bool): Ignore external IDs that are not found rather than throw an exception.
 
         Returns:
             Unit | UnitList | None: If a single external ID is specified: the requested unit, or None if it does not exist. If several external IDs are specified: the requested units.
 
         Examples:
```

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/user_profiles.py` & `cognite_sdk-7.9.0/cognite/client/_api/user_profiles.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 from __future__ import annotations
 
-from typing import List, MutableSequence, cast, overload
+from typing import List, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DEFAULT_LIMIT_READ
-from cognite.client.data_classes.user_profiles import UserProfile, UserProfileList
+from cognite.client.data_classes.user_profiles import UserProfile, UserProfileList, UserProfilesConfiguration
 from cognite.client.utils._identifier import UserIdentifierSequence
+from cognite.client.utils.useful_types import SequenceNotStr
 
 
 class UserProfilesAPI(APIClient):
     _RESOURCE_PATH = "/profiles"
 
+    def enable(self) -> UserProfilesConfiguration:
+        """Enable user profiles for the project"""
+        res = self._post("/update", json={"update": {"userProfilesConfiguration": {"set": {"enabled": True}}}})
+        return UserProfilesConfiguration.load(res.json()["userProfilesConfiguration"])
+
+    def disable(self) -> UserProfilesConfiguration:
+        """Disable user profiles for the project"""
+        res = self._post("/update", json={"update": {"userProfilesConfiguration": {"set": {"enabled": False}}}})
+        return UserProfilesConfiguration.load(res.json()["userProfilesConfiguration"])
+
     def me(self) -> UserProfile:
         """`Retrieve your own user profile <https://developer.cognite.com/api#tag/User-profiles/operation/getRequesterUserProfile>`_
 
         Retrieves the user profile of the principal issuing the request, i.e. the principal *this* CogniteClient was instantiated with.
 
         Returns:
             UserProfile: Your own user profile.
@@ -32,27 +43,25 @@
         """
         return UserProfile.load(self._get(self._RESOURCE_PATH + "/me").json())
 
     @overload
     def retrieve(self, user_identifier: str) -> UserProfile | None:
         ...
 
-    @overload  # Note, can't use Sequence[str], as str itself matches this requirement...
-    def retrieve(self, user_identifier: MutableSequence[str] | tuple[str, ...]) -> UserProfileList:
+    @overload
+    def retrieve(self, user_identifier: SequenceNotStr[str]) -> UserProfileList:
         ...
 
-    def retrieve(
-        self, user_identifier: str | MutableSequence[str] | tuple[str, ...]
-    ) -> UserProfile | UserProfileList | None:
+    def retrieve(self, user_identifier: str | SequenceNotStr[str]) -> UserProfile | UserProfileList | None:
         """`Retrieve user profiles by user identifier. <https://developer.cognite.com/api#tag/User-profiles/operation/getUserProfilesByIds>`_
 
         Retrieves one or more user profiles indexed by the user identifier in the same CDF project.
 
         Args:
-            user_identifier (str | MutableSequence[str] | tuple[str, ...]): The single user identifier (or sequence of) to retrieve profile(s) for.
+            user_identifier (str | SequenceNotStr[str]): The single user identifier (or sequence of) to retrieve profile(s) for.
 
         Returns:
             UserProfile | UserProfileList | None: UserProfileList if a sequence of user identifier were requested, else UserProfile. If a single user identifier is requested and it is not found, None is returned.
 
         Raises:
             CogniteNotFoundError: A sequences of user identifiers were requested, but one or more does not exist.
```

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/vision.py` & `cognite_sdk-7.9.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api/workflows.py` & `cognite_sdk-7.9.0/cognite/client/_api/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_api_client.py` & `cognite_sdk-7.9.0/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_cognite_client.py` & `cognite_sdk-7.9.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_http_client.py` & `cognite_sdk-7.9.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-7.9.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_points.proto` & `cognite_sdk-7.9.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-7.9.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-7.9.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-7.9.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/config.py` & `cognite_sdk-7.9.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/credentials.py` & `cognite_sdk-7.9.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/__init__.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/_base.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/aggregations.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/annotations.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/assets.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/capabilities.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/capabilities.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/contextualization.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/core.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/graphql.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/query.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/query.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/data_sets.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/datapoints.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/datapoints_subscriptions.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/datapoints_subscriptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/documents.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/documents.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/events.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/files.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/filters.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/functions.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/geospatial.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/iam.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/labels.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/raw.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/relationships.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/sequences.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/shared.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/templates.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/three_d.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/time_series.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,26 +286,26 @@
         destination_oidc_credentials.
 
     Args:
         client_id (str): Your application's client id.
         client_secret (str): Your application's client secret
         scopes (str | list[str]): A list of scopes or a comma-separated string (for backwards compatibility).
         token_uri (str): OAuth token url
+        cdf_project_name (str): Name of CDF project
         audience (str | None): Audience (optional)
-        cdf_project_name (str | None): Name of CDF project (optional)
     """
 
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         scopes: str | list[str],
         token_uri: str,
+        cdf_project_name: str,
         audience: str | None = None,
-        cdf_project_name: str | None = None,
     ) -> None:
         self.client_id = client_id
         self.client_secret = client_secret
         self.token_uri = token_uri
         self.audience = audience
         self.cdf_project_name = cdf_project_name
         self.scopes = self._verify_scopes(scopes)
@@ -351,16 +351,16 @@
             Self: No description.
         """
         return cls(
             client_id=data["clientId"],
             client_secret=data["clientSecret"],
             scopes=data["scopes"],
             token_uri=data["tokenUri"],
+            cdf_project_name=data["cdfProjectName"],
             audience=data.get("audience"),
-            cdf_project_name=data.get("cdfProjectName"),
         )
 
 
 class NonceCredentials:
     def __init__(
         self,
         session_id: int,
```

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/units.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/units.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/user_profiles.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/user_profiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Sequence, cast
 
+from typing_extensions import Self
+
 from cognite.client.data_classes._base import CogniteResource, CogniteResourceList
 from cognite.client.utils._text import to_camel_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
@@ -69,7 +71,16 @@
         """Get an item from this list by user_identifier.
         Args:
             user_identifier (str): The user_identifier of the item to get.
         Returns:
             UserProfile | None: The requested item or None if not found.
         """
         return self._user_identifier_to_item.get(user_identifier)
+
+
+class UserProfilesConfiguration(CogniteResource):
+    def __init__(self, enabled: bool) -> None:
+        self.enabled = enabled
+
+    @classmethod
+    def _load(cls, resource: dict, cognite_client: CogniteClient | None = None) -> Self:
+        return cls(enabled=resource["enabled"])
```

### Comparing `cognite_sdk-7.8.9/cognite/client/data_classes/workflows.py` & `cognite_sdk-7.9.0/cognite/client/data_classes/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/exceptions.py` & `cognite_sdk-7.9.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/testing.py` & `cognite_sdk-7.9.0/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/__init__.py` & `cognite_sdk-7.9.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_auxiliary.py` & `cognite_sdk-7.9.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_concurrency.py` & `cognite_sdk-7.9.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_experimental.py` & `cognite_sdk-7.9.0/cognite/client/utils/_experimental.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_graph.py` & `cognite_sdk-7.9.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_identifier.py` & `cognite_sdk-7.9.0/cognite/client/utils/_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 class DataModelingIdentifierSequence(IdentifierSequenceCore[DataModelingIdentifier]):
     ...
 
 
 class UserIdentifierSequence(IdentifierSequenceCore[UserIdentifier]):
     # TODO: Inferred type from inherited methods 'as_dicts' and 'as_primitives' wrongly include 'int'
     @classmethod
-    def load(cls, user_identifiers: str | Sequence[str]) -> UserIdentifierSequence:
+    def load(cls, user_identifiers: str | SequenceNotStr[str]) -> UserIdentifierSequence:
         if isinstance(user_identifiers, str):
             return cls([UserIdentifier(user_identifiers)], is_singleton=True)
 
         elif isinstance(user_identifiers, Sequence):
             return cls(list(map(UserIdentifier, map(str, user_identifiers))), is_singleton=False)
 
         raise TypeError(f"user_identifiers must be of type str or Sequence[str]. Found {type(user_identifiers)}")
```

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_importing.py` & `cognite_sdk-7.9.0/cognite/client/utils/_importing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_logging.py` & `cognite_sdk-7.9.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-7.9.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-7.9.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_retry.py` & `cognite_sdk-7.9.0/cognite/client/utils/_retry.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_session.py` & `cognite_sdk-7.9.0/cognite/client/utils/_session.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_text.py` & `cognite_sdk-7.9.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_time.py` & `cognite_sdk-7.9.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_validation.py` & `cognite_sdk-7.9.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/_version_checker.py` & `cognite_sdk-7.9.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/cognite/client/utils/useful_types.py` & `cognite_sdk-7.9.0/cognite/client/utils/useful_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-7.8.9/pyproject.toml` & `cognite_sdk-7.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "7.8.9"
+version = "7.9.0"
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = [
     "Erlend Vollset <erlend.vollset@cognite.com>",
     "Håkon Treider <hakon.treider@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>"
```

### Comparing `cognite_sdk-7.8.9/PKG-INFO` & `cognite_sdk-7.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 7.8.9
+Version: 7.9.0
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 7.8.9 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 7.9.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: all Provides-Extra:
```

