# Comparing `tmp/cognite_sdk-6.5.0.tar.gz` & `tmp/cognite_sdk-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.5.0.tar", max compression
+gzip compressed data, was "cognite_sdk-6.5.1.tar", max compression
```

## Comparing `cognite_sdk-6.5.0.tar` & `cognite_sdk-6.5.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    11349 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/README.md
--rw-r--r--   0        0        0      574 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     7558 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49210 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8429 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    37786 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6503 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7897 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41584 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4087 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5065 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7395 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6593 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    30982 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2582 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    15081 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-27 12:38:07.746689 cognite_sdk-6.5.0/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/README.md
+-rw-r--r--   0        0        0      574 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8429 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    37850 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6503 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7897 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-06-27 13:00:13.127439 cognite_sdk-6.5.1/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41584 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-06-27 13:00:13.131439 cognite_sdk-6.5.1/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4087 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-06-27 13:00:13.135439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7395 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6593 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    30982 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2582 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    15081 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-27 13:00:13.139439 cognite_sdk-6.5.1/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-27 13:00:13.143439 cognite_sdk-6.5.1/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-27 13:00:13.143439 cognite_sdk-6.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.1/PKG-INFO
```

### Comparing `cognite_sdk-6.5.0/LICENSE` & `cognite_sdk-6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/README.md` & `cognite_sdk-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/__init__.py` & `cognite_sdk-6.5.1/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/annotations.py` & `cognite_sdk-6.5.1/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/assets.py` & `cognite_sdk-6.5.1/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 import json
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Sequence, Type, Union, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import INSTANCES_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes._base import CogniteResourceList
-from cognite.client.data_classes.data_modeling.aggregations import Aggregation, Histogram, HistogramValue
+from cognite.client.data_classes.data_modeling.aggregations import (
+    Aggregation,
+    Histogram,
+    HistogramValue,
+    MetricAggregation,
+)
 from cognite.client.data_classes.data_modeling.filters import Filter
 from cognite.client.data_classes.data_modeling.ids import (
     EdgeId,
     NodeId,
     ViewId,
     ViewIdentifier,
     _load_identifier,
@@ -571,27 +576,27 @@
 
         res = self._post(url_path=self._RESOURCE_PATH + "/search", json=body)
         return list_cls._load(res.json()["items"], cognite_client=None)
 
     def aggregate(
         self,
         view: ViewId,
-        aggregates: Aggregation | dict | Sequence[Aggregation | dict],
+        aggregates: MetricAggregation | dict | Sequence[MetricAggregation | dict],
         instance_type: Literal["node", "edge"] = "node",
         group_by: Sequence[str] | None = None,
         query: str | None = None,
         properties: Sequence[str] | None = None,
         filter: Filter | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
     ) -> InstanceAggregationResultList:
         """`Aggregate data across nodes/edges <https://developer.cognite.com/api/v1/#tag/Instances/operation/aggregateInstances>`_
 
         Args:
             view (ViewId): View to to aggregate over.
-            aggregates (Aggregation | dict | Sequence[Aggregation | dict]):  The properties to aggregate over.
+            aggregates (MetricAggregation | dict | Sequence[MetricAggregation | dict]):  The properties to aggregate over.
             instance_type (Literal["node", "edge"]): Whether to search for nodes or edges.
             group_by (Optional[Sequence[str]]): The selection of fields to group the results by when doing aggregations.
                                   You can specify up to 5 items to group by.
             query (Optional[str]): Query string that will be parsed and used for search.
             properties (Optional[Sequence[str]]): Optional array of properties you want to search through.
                                     If you do not specify one or more properties, the service will
                                     search all text fields within the view.
```

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/data_sets.py` & `cognite_sdk-6.5.1/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.5.1/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/datapoints.py` & `cognite_sdk-6.5.1/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/diagrams.py` & `cognite_sdk-6.5.1/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.5.1/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/events.py` & `cognite_sdk-6.5.1/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.5.1/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/files.py` & `cognite_sdk-6.5.1/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/functions.py` & `cognite_sdk-6.5.1/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/geospatial.py` & `cognite_sdk-6.5.1/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/iam.py` & `cognite_sdk-6.5.1/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/labels.py` & `cognite_sdk-6.5.1/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/raw.py` & `cognite_sdk-6.5.1/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/relationships.py` & `cognite_sdk-6.5.1/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/sequences.py` & `cognite_sdk-6.5.1/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.5.1/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/templates.py` & `cognite_sdk-6.5.1/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/three_d.py` & `cognite_sdk-6.5.1/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/time_series.py` & `cognite_sdk-6.5.1/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.5.1/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.5.1/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.5.1/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.5.1/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.5.1/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api/vision.py` & `cognite_sdk-6.5.1/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_api_client.py` & `cognite_sdk-6.5.1/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_cognite_client.py` & `cognite_sdk-6.5.1/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_http_client.py` & `cognite_sdk-6.5.1/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.1/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.5.1/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.5.1/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.5.1/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.5.1/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/config.py` & `cognite_sdk-6.5.1/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/credentials.py` & `cognite_sdk-6.5.1/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/_base.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/assets.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,41 +35,46 @@
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output = {self._aggregation_name: {"property": self.property}}
         if camel_case:
             output = convert_all_keys_recursive(output)
         return output
 
 
+@dataclass
+class MetricAggregation(Aggregation):
+    ...
+
+
 @final
 @dataclass
-class Avg(Aggregation):
+class Avg(MetricAggregation):
     _aggregation_name = "avg"
 
 
 @final
 @dataclass
-class Count(Aggregation):
+class Count(MetricAggregation):
     _aggregation_name = "count"
 
 
 @final
 @dataclass
-class Max(Aggregation):
+class Max(MetricAggregation):
     _aggregation_name = "max"
 
 
 @final
 @dataclass
-class Min(Aggregation):
+class Min(MetricAggregation):
     _aggregation_name = "min"
 
 
 @final
 @dataclass
-class Sum(Aggregation):
+class Sum(MetricAggregation):
     _aggregation_name = "sum"
 
 
 @final
 @dataclass
 class Histogram(Aggregation):
     _aggregation_name = "histogram"
```

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/events.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/files.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/functions.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/iam.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/labels.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/raw.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/shared.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/templates.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.5.1/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/exceptions.py` & `cognite_sdk-6.5.1/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/testing.py` & `cognite_sdk-6.5.1/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/__init__.py` & `cognite_sdk-6.5.1/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.5.1/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.5.1/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_graph.py` & `cognite_sdk-6.5.1/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_identifier.py` & `cognite_sdk-6.5.1/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_logging.py` & `cognite_sdk-6.5.1/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.5.1/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.5.1/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.5.1/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_text.py` & `cognite_sdk-6.5.1/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_time.py` & `cognite_sdk-6.5.1/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_validation.py` & `cognite_sdk-6.5.1/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.5.1/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.5.0/pyproject.toml` & `cognite_sdk-6.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.5.0"
+version = "6.5.1"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.5.0/PKG-INFO` & `cognite_sdk-6.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.5.0
+Version: 6.5.1
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.0 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.1 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

